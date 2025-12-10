---
title: "EN AWBusiness LogisticsOptimizer 2.01"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["EN_AWBusiness_LogisticsOptimizer_2.01"]
version: "1.0"
last_updated: "2025-12-10"
description: "Logistic Optimizer             J                                    English                          A+W Business                                                                                                            Introduction                                             Introduction                                         This part of the documentation contains editorial notes.                                           Revision Overview                                         Part"
source_file: "EN_AWBusiness_LogisticsOptimizer_2.01.pdf"
---


# EN AWBusiness LogisticsOptimizer 2.01

Logistic Optimizer             J




                               English




                     A+W Business
                                                                                                           Introduction




                                        Introduction
                                        This part of the documentation contains editorial notes.


                                        Revision Overview
                                        Part                Description
                                        Version/Date

                                        1.00/05-2014        Original Version.

                                        2.00/05-2016        Complete Revision.

                                        2.01/01-2017        Product and company names adjusted.



                                        Editorial
                                        The editorial provides information on the following topics:
                                        •   Notes on this document
                                        •   Copyrights
                                        •   Trademarks
                                        •   Contacts

                                        Notes on this document
                                        This document is intended for end users of A+W Business.
                                        The documentation and software described are licenses that must only be
                                        used or copied in accordance with the conditions of our license agreement.
                                        The contents of the documentation are only informative and are subject to
                                        changes without prior notice. The text and illustrations were compiled with the
                                        utmost care. Still, errors cannot be totally excluded. A+W Software
                                        GmbHcannot be held liable for errors or inaccuracies, unless they can be at-
                                        tributed to wilful or grossly negligent action.
                                        This document describes the full scope of OTR.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-3
                 Introduction




                                Copyrights
                                © 2017, A+W Software GmbH, all rights reserved, including the right of reprint,
                                the production of copies and of the translation.
                                The documentation may be copied, completely or in part, saved in an archiving
                                system or transferred in any other form only in accordance with our license
                                agreement. Transmission of the documentation is not allowed, neither elec-
                                tronically, nor mechanically, nor by recording or in any other way, without A+W
                                Software GmbH's prior written approval.

                                Trademarks
                                All hardware and software names mentioned in this documentation can also
                                be registered trademarks or other property rights of third parties. Third-party
                                copyrights must therefore be observed.

                                Contacts
                                A+W Software GmbH

                                Am Pfahlgraben 4-10

                                D-35415 Pohlheim

                                   +49 6404 2051 0

                                   +49 6404 2051 877

                                Zentrale@a-w.com

                                http://www.a-w.com
2.01 / 01-2017




                 J-4                                                        A+W Business Logistic Optimizer
                                                                                                                                                        Contents




                                        Contents
                                           Revision Overview ............................................................................................... J-3
                                           Editorial ............................................................................................................... J-3

                                        Tutorial                                                                                                               J-9
                                        Overview ............................................................................................................... J-11
                                          Documentation .................................................................................................. J-12
                                            Tutorial Structure ........................................................................................... J-12
                                            Display conventions ....................................................................................... J-13
                                        Basic Principles of the OTR .................................................................................. J-14
                                          Database Connections ...................................................................................... J-15
                                              Connection to the OTR database ............................................................... J-15
                                              Connection to the ERP database ............................................................... J-16
                                          Dynamic Mode .................................................................................................. J-17
                                          User Interface .................................................................................................... J-21
                                            The Menu and Tool Bars ............................................................................... J-24
                                            Field help ....................................................................................................... J-30
                                        Administration ....................................................................................................... J-31
                                          Parameters ........................................................................................................ J-32
                                          Master Data ....................................................................................................... J-33
                                            User ............................................................................................................... J-34
                                            Status ............................................................................................................. J-35
                                              Managing Status Types .............................................................................. J-36
                                            Customers ...................................................................................................... J-37
                                              Managing Customers ................................................................................. J-38
                                            Departments .................................................................................................. J-40
                                              Managing Departments .............................................................................. J-40
                                            Vehicles ......................................................................................................... J-42
                                              Managing Vehicles ..................................................................................... J-43
                                            Driver ............................................................................................................. J-46
                                              Managing Drivers ....................................................................................... J-47
                                            Reports .......................................................................................................... J-49
                                              Managing Reports ...................................................................................... J-50
                                            Packaging Types ........................................................................................... J-51
                                              Managing Packaging Types ....................................................................... J-52
                                            Data Import .................................................................................................... J-54
                                        Planning Routes ................................................................................................... J-55
                                          Routes and Destinations ................................................................................... J-56
                                            General .......................................................................................................... J-57
                                            Import ............................................................................................................. J-58
                                            Routes ............................................................................................................ J-59
                                              Load a Saved Route ................................................................................... J-60
                                              Copy a Saved Route .................................................................................. J-61
                                            Working with Routes ...................................................................................... J-62
                                            Destinations ................................................................................................... J-69
                                              Display Documents ..................................................................................... J-70
                                              Deletion of Documents ............................................................................... J-70
                                              Show Items ................................................................................................. J-71
                                              Show Information ........................................................................................ J-72
                                              The Detailed View ...................................................................................... J-73
                                              Edit Customer Address ............................................................................... J-75
2.01 / 01-2017




                                              Working with Destinations .......................................................................... J-76




                 A+W Business Logistic Optimizer                                                                                                                 J-5
                 Contents




                              Costs ................................................................................................................. J-79
                                Expenses ....................................................................................................... J-80
                                Variable Costs ................................................................................................ J-80
                                Fixed Costs .................................................................................................... J-81
                                Route Costs ................................................................................................... J-81
                            Optimizing Routes ................................................................................................ J-82
                              Overview ........................................................................................................... J-83
                                Optimizing Routes .......................................................................................... J-84
                                  Different Map Modes .................................................................................. J-87
                                Changing Routes ........................................................................................... J-88
                            Check Results ....................................................................................................... J-91
                              Overview ........................................................................................................... J-92
                                The Result of the Optimization ....................................................................... J-93
                                  Routes ........................................................................................................ J-93
                                  Route Plan .................................................................................................. J-94
                                  Destination .................................................................................................. J-94
                                Change Route Status ..................................................................................... J-95
                                Real Route Costs ........................................................................................... J-96
                            Driving and Tracking Routes ................................................................................ J-97
                              Overview ........................................................................................................... J-98
                                Preparations ................................................................................................... J-99
                                  Respective Route Status ............................................................................ J-99
                                  Loading Documents in the Cloud ............................................................... J-99
                                  Install App or use Browser ........................................................................ J-100
                                Driving Routes ............................................................................................. J-101
                                  Enter Password ........................................................................................ J-101
                                  Operation of App or Browser .................................................................... J-102
                                  Booking Data ............................................................................................ J-103
                                Tracking Routes ........................................................................................... J-109
                            Queries ............................................................................................................... J-112
                              Overview ......................................................................................................... J-113
                                Different Queries .......................................................................................... J-114
                                Routes .......................................................................................................... J-114
                                  Filter .......................................................................................................... J-114
                                  Change and Status ................................................................................... J-115
                                  Clear ......................................................................................................... J-115
                                Export ........................................................................................................... J-116
                                  Export to Navigation Systems .................................................................. J-116
                                History .......................................................................................................... J-119
                                Reports ........................................................................................................ J-120
                                  Selected Route ......................................................................................... J-120
                                  Print Lists .................................................................................................. J-121
                                  Report Launcher ....................................................................................... J-121
                                  Statistics ................................................................................................... J-121
                                  Create a Statistic ...................................................................................... J-123
                                View ............................................................................................................. J-125
                                  Route ........................................................................................................ J-125
                                  Destination ................................................................................................ J-125
                                  Calendar ................................................................................................... J-125
2.01 / 01-2017




                 J-6                                                                              A+W Business Logistic Optimizer
                                                                                                                                                        Contents




                                        Software Reference                                                                                              J-127
                                        Configuration ...................................................................................................... J-129
                                          OTR Connection .............................................................................................. J-130
                                          ERP Connection .............................................................................................. J-131
                                          Parameters ...................................................................................................... J-132
                                        Administration ..................................................................................................... J-141
                                          User ................................................................................................................. J-142
                                          Status .............................................................................................................. J-143
                                          Customers ....................................................................................................... J-145
                                          Departments .................................................................................................... J-147
                                          Vehicles ........................................................................................................... J-148
                                          Driver ............................................................................................................... J-151
                                          Reports ............................................................................................................ J-154
                                          Packaging ........................................................................................................ J-155
                                          Data Import ...................................................................................................... J-157
                                        Planning .............................................................................................................. J-159
                                          Copy a Saved Route ....................................................................................... J-161
                                          Load a Saved Route ........................................................................................ J-163
                                          Import Destinations ......................................................................................... J-164
                                          Creating a New Route – General .................................................................... J-165
                                          Geolocate ........................................................................................................ J-168
                                          Creating a New Route - Vehicle ...................................................................... J-169
                                          Select Vehicle .................................................................................................. J-172
                                          Add Driver ....................................................................................................... J-173
                                          Creating a New Route – Parameters .............................................................. J-174
                                          Route Factors .................................................................................................. J-178
                                          Creating a New Route – Costs ........................................................................ J-180
                                          Groups ............................................................................................................. J-182
                                          Vehicles ........................................................................................................... J-183
                                          Edit Destination ............................................................................................... J-184
                                          Time Range ..................................................................................................... J-186
                                          Documents ...................................................................................................... J-187
                                          Show Items ...................................................................................................... J-188
                                          Show Information ............................................................................................ J-189
                                          Customers ....................................................................................................... J-190
                                          Detailed View .................................................................................................. J-191
                                        Optimization ........................................................................................................ J-192
                                          Optimize Route ................................................................................................ J-193
                                        Result .................................................................................................................. J-195
                                          Result of the Optimization ............................................................................... J-196
                                          Route Information ............................................................................................ J-198
                                        Query .................................................................................................................. J-200
                                          Filter Routes .................................................................................................... J-201
                                          Export .............................................................................................................. J-202
                                          Change Status ................................................................................................. J-203
                                          History ............................................................................................................ J-204
                                          Confirmation and Delivery List ....................................................................... J-206
                                          Report .............................................................................................................. J-209
                                          Statistics ......................................................................................................... J-210
                                            General Tab ................................................................................................. J-210
                                            General Graphic Tab ................................................................................... J-211
                                            Vehicles Tab ................................................................................................ J-212
                                            Drivers Tab .................................................................................................. J-213
2.01 / 01-2017




                                            Department Tab ........................................................................................... J-214
                                            Customers Tab ............................................................................................ J-215




                 A+W Business Logistic Optimizer                                                                                                                J-7
                 Contents




                               Calendar .......................................................................................................... J-216
                               Attach Files ...................................................................................................... J-217
                               Attach File ....................................................................................................... J-219

                            Partindex                                                                                                       J-221
                            Index ................................................................................................................... J-224
2.01 / 01-2017




                 J-8                                                                              A+W Business Logistic Optimizer
Logistic Optimizer               J

                            Tutorial




                     A+W Business
                 Tutorial                                                                                        Overview




                                        Overview
                                        The A+W Logistic Optimizer (also called OTR - Optimizer of Transport Rou-tes)
                                        deals with the basics of route planning. This tutorial is based on the under-
                                        standing of the master data and the number manager.

                                            The functions depend on the enabled modules
                                            Please note that the various functions are only available if the associated
                                            modules and interfaces are installed and enabled.

                                            If you detect functions in this description that are not available in your ver-
                                            sion, please contact A+W Software GmbH.

                                        Subjects
                                        This tutorial offers the following subjects:
                                        •   Basic Principles of the OTR
                                        •   Administration
                                        •   Planning Routes
                                        •   Optimizing Routes
                                        •   Check Results
                                        •   Driving and Tracking Routes
                                        •   Queries

                                        Required knowledge
                                        This tutorial is meant for those who prepare orders for delivery and monitor de-
                                        livery using different trucks in OTR. Participants must be familiar with the mas-
                                        ter data and number manager concept.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                     J-11
                 Overview                                                                                   Tutorial




                            Documentation
                            The following documents are available for the OTR module:

                            Handout                      Printout of tutorial for training session

                            PDF                          Complete documentation
                                                         • Tutorial
                                                         • Software Reference
                                                         • Index

                            Online help <F1>             Context-sensitive dialog help for the OTR software
                                                         references and tutorials on the basic version


                            Tutorial Structure
                            This tutorial consists of subjects with several training modules each. Each
                            module consists of the following elements:

                            Overview                     Each training module starts with an overview of the
                                                         major topics:
                                                         • Objectives: What shall be conveyed?
                                                         • Benefit: What can this knowledge be used for?
                                                         • Maxims: Which correlations are to be remembered?

                            Concepts                     First, the concepts and terms of the corresponding
                                                         training module will be explained. This is followed by
                                                         examples and instructions.

                            Exercises                    For some of the training modules, exercises with certain
                                                         tasks and suggested solutions are available.

                            Cross-references             At the end of each training module there is a section
                                                         with cross references pointing to additional information
                                                         in the software reference and in other sections.
                                                         This will help you to extend your newly acquired
                                                         knowledge.


                            Reading tip
                            The contents of a training module are based on the knowledge conveyed in the
                            previous module. We therefore recommend you do not skip any modules.
                            If you are already familiar with a subject you should at least read the summary at the
                            start of a training module in order to bring the main details to mind.
2.01 / 01-2017




                 J-12                                                         A+W Business Logistic Optimizer
                 Tutorial                                                                                      Overview




                                        Display conventions
                                        Certain parts of sentences are specially marked. These have the following
                                        meanings:

                                        Italics                  marks character strings describing the software
                                                                 elements, e.g. the Number Manager dialog.

                                        Bold                     Marks character strings to be entered via the keyboard,
                                                                 e.g.: Enter the value 0.

                                        >                        The so-called breadcrumb trail shows how to open a
                                                                 dialog, e. g. Production > Production > Transfer to
                                                                 production.

                                        []                       Square brackets mark buttons in a dialog, e.g. [OK] to
                                                                 save the data.

                                        <>                       Angle brackets refer to keys or shortcuts on the
                                                                 keyboard, e.g. <F1> is used to open the online help.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                    J-13
                 Basic Principles of the OTR                                                                         Tutorial




                                          Basic Principles of the OTR
                                          The objective of meaningful route optimization and routing planning in the
                                          transport field is to reduce transportation times and routes and thus reduce
                                          fuel consumption significantly. As a result, the environmental impact is re-
                                          duced, vehicles are subject to less wear and drivers are not burdened with un-
                                          necessary mileage.
                                          Routing planning as well as route optimization therefore save costs and in-
                                          crease productivity.
                                          The Optimizer for Transport Routes (OTR) organizes your destinations, cus-
                                          tomer addresses or stopping points into a useful and efficient order.
                                          In addition to your individual fleet of vehicles, this order also takes the defined
                                          route requirements, e. g. tunnels or toll roads, into consideration. The technol-
                                          ogy is based on Nokia Maps in combination with a mathematical algorithm.
                                          The driver can book and report deliveries directly via mobile App. In addition,
                                          all necessary information regarding the total route and individual loading sta-
                                          tions are provided.
                                          The office can monitor the deliveries via GPS.
                                          The procedure is as follows:


                                               Planning       Optimization   Result



                                          Fig. J-1        Standard process for the delivery sequence


                                          The process is divided into four phases:
                                          •    In this phase you create the route(s). You can create new routes, edit ex-
                                               isting ones or also delete them. Within the routes, you can add destination
                                               locations (stopping points), and also edit or delete individual locations. Dur-
                                               ing this phase, you also have access to the individual items in order to ob-
                                               tain an overview.
                                          •    Optimization: Optimization of the route takes place in this phase. On the
                                               overview map, you will see the routing and, on the right side, a list of the
                                               individual stations (waypoints). You can exchange individual stations and
                                               you have access to the optimization factors.
                                               The optimizations considers settings and modifications of the planning
                                               phase - for example certain unloading times or priorities of customers
                                               (loading stations).
                                          •    Result:
                                               This phase provides the total result of the route, divided into the individual
                                               routes, the graphical route plan and the list of the destination locations.
2.01 / 01-2017




                 J-14                                                                     A+W Business Logistic Optimizer
                 Tutorial                                                                   Basic Principles of the OTR




                                        Database Connections
                                        To work with the module, the following two database connections have to be
                                        in place:
                                        •   OTR
                                        •   ERP

                                        Connection to the OTR database
                                        The connection to the OTR is necessary to plan the routes.




                                        Fig. J-2      Database settings OTR


                                        A dialog appears when you call the database for the first time. In the field Data
                                        Source enter the path to the OTR database server. You can obtain this infor-
                                        mation from your contact at our A+W Support or Qualified Service.
                                        Enter the standard database in the field Start Catalog. This is OTR. You can
                                        also obtain the User ID and Password from your contact at A+W Support or
                                        Qualified Service.
                                        After you have made the settings, you can establish a test connection to the
                                        database with the [Test] button.

                                            Database connection
                                            Please note that these settings have to be made for each user.


                                        Additional information
                                         Software Reference, “OTR Connection” on page J-130
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                    J-15
                 Basic Principles of the OTR                                                                     Tutorial




                                          Connection to the ERP database
                                          The connection to the ERP database server is necessary for the module to ac-
                                          cess the data from A+W Business.




                                          Fig. J-3       Database Settings ERP


                                          A dialog with the tab OTR appears when you call the database for the first
                                          time. Switch to the tab ERP Connection.
                                          Enter the standard database in the field Start Catalog. You can also obtain the
                                          User ID and Password from your contact at A+W Support or Qualified Service.
                                          After you have made the settings, you can establish a test connection to the
                                          database with the [Test] button.

                                               Database connection
                                               Please note that these settings have to be made for each user.


                                          Additional information
                                           Software Reference, “OTR Connection” on page J-130
2.01 / 01-2017




                 J-16                                                                 A+W Business Logistic Optimizer
                 Tutorial                                                                  Basic Principles of the OTR




                                        Dynamic Mode
                                        When working with the dynamic mode, the following dialog opens after clicking
                                        the icon button in number manager:




                                        Fig. J-4      Dynamic mode, delivery areas


                                        This is where OTR groups destinations based on coordinates and under con-
                                        sideration of weight and the geolocation takes place.
                                        Field Number of delivery areas shows in how many groups OTR combined the
                                        individual destinations.
                                        You can either accept or change the value. In case you change it, a recalcula-
                                        tion based on the new value takes place in background .

                                           Geolocation in Dynamic Mode
                                           If geolocation was successful for all addresses, the Geolocation phase will
                                           be skipped in OTR.

                                        After pressing the [OK] button, dialog Select Vehicle appears.




                                        Fig. J-5     Dynamic mode, select vehicle


                                        The dialog gives an overview of the individual vehicles defined in the system.
2.01 / 01-2017




                                        You can either choose certain vehicles (own trucks or transport companies) or
                                        all vehicles. By selecting all vehicles, the system has the freedom to distribute
                                        the orders optimally on the trucks. If you enable the checkbox Maximum vehi-



                 A+W Business Logistic Optimizer                                                                   J-17
                 Basic Principles of the OTR                                                                         Tutorial




                                            cle weight and visiting time, the maximum load defined in the master data as
                                            well as the time defined for the customer are taken into consideration.
                                            Click on [OK], the following display opens:




                 Fig. J-6    User interface after start


                                            OTR uses the above mentioned entries for calculation. On the left-hand side
                                            you see the map containing the inidividual groups that are visited. The top right
                                            shows the routes and the destinations below.
                                            The number in field Groups is identical with the number on the map (s.a.).
                                            The [Groups] button contains the menu entries:
                                            •   Hierarchical
                                            •   EM
                                            These are two types of calculation leading to different results. The appropriate
                                            mode depends on how many groups and how many destinations are visited.
                                            To make this clear, we split 94 destinations into different numbers of groups
                                            and show the result of both modes:
2.01 / 01-2017




                 J-18                                                                     A+W Business Logistic Optimizer
                 Tutorial                                                                    Basic Principles of the OTR




                                        If these destinations are split into three groups, the result is as follows:




                                        Hierarchical mode                        EM mode (recommended)


                                        If these destinations are split into four groups, the result is as follows:




                                        Hierarchical mode                        EM mode (recommended)
2.01 / 01-2017




                                        If these destinations are split into six groups, the result is as follows:




                 A+W Business Logistic Optimizer                                                                       J-19
                 Basic Principles of the OTR                                                                            Tutorial




                                          Hierarchical mode (recommended)          EM mode


                                          If these destinations are split into nine groups, the result is as follows:




                                          Hierarchical mode (recommended)          EM mode


                                          According to our experience, the EM mode has a more efficient splitting of
                                          destinations for just a few groups. If you have a large amount of groups, the
                                          hierarchical mode has a more efficient splitting.
                                          Use the menu entries Hierarchical and EM to simulate the splitting and to
                                          choose the best result.

                                               Calculation of Groups
                                               The splitting always takes place under consideration of the vehicle values
                                               defined in the master data.

                                          Tab Route Information provides an overview of the truck load, weight, and the
                                          route time.
                                          The progress bar in column Status shows the percentage of the truck load.
                                          Next step:
                                           Optimization, Page J-84


                                          Additional information
                                           Software Reference, “Groups” on page J-182
2.01 / 01-2017




                 J-20                                                                   A+W Business Logistic Optimizer
                 Tutorial                                                                       Basic Principles of the OTR




                                            User Interface
                                            Open the module OTR by pressing the [OTR] button in the number manager.
                                            Once you have started OTR, the module appears as follows:


                 A
                 B
                 C

                                                                                                                            R




                                                                                                                            G




                 D




                 E
                                                                                                                            H

                 A Menu bar                               D Map                           G Overview of the destinations
                 B Tool bar                               E Map tools                     H Button
                 C Process presentation                   F Overview of the routes
                 Fig. J-7    User interface after start


                                            The upper area contains, from left to right, the menu bar (A), the tool bar (B)
                                            and presentation of the whole process (C) from planning up to data transfer.
                                            With the wizard, you can complete the entire process (planning, geolocation,
                                            etc,) in just a few steps.
                                            The [Next] button takes you one step further in the process. Please note that
                                            you can only continue if no errors have occurred in the respective process. For
                                            instance: in the Geolocation area you can only continue to the next step if all
                                            destinations could be located.
                                            The [Back] button takes you one step back in the process.
                                            The optimization results are displayed at the end of this process and you can
                                            decide whether you are going to accept (save) the route and the optimization
                                            results or repeat the optimization with other settings to achieve a better result.
                                            The map (D) shows the destinations combined to groups. The area below
                                            shows the tools to edit routes on the map (E). The Routes (F) section contains
2.01 / 01-2017




                                            all upcoming routes and the Destinations (G) section shows you the individual
                                            stations of the route. The (H) button takes you to the next step in the process.




                 A+W Business Logistic Optimizer                                                                        J-21
                 Basic Principles of the OTR                                                                           Tutorial




                                          Below the map you will find the following tools:




                                          Description of the individual icons
                                          At the end you will find a list of buttons/icons and their meaning.

                                          Icon                 Description

                                                               Menu
                                                               If you enable this icon button you can use the <Ctrl> key to
                                                               select one or more destinations. These are displayed in red. A
                                                               popup menu opens with actions that can be made at this point.

                                                               Destinations
                                                               If you enable this icon button the map shows the last two digits
                                                               of the route ID.
                                                               If the icon button is disabled the numbers of the destinations
                                                               are displayed.

                                                               Groups
                                                               With this icon button the outward destinations are connected
                                                               by lines.

                                                               Groups
                                                               With this icon button the delivery areas are displayed circular.

                                                               Information
                                                               With this icon button you turn the route information (Nokia
                                                               Maps) on or off.

                                                               Optimized route
                                                               After the optimization you can use this icon button to show or
                                                               hide the route.

                                                               Destinations
                                                               With this button you can show or hide destinations.

                                                               Zoom
                                                               This icon button lets you zoom in and out (map). The sections
                                                               Routes and Destinations are hidden. Click the icon button
                                                               again to show the sections Routes and Destinations and to
                                                               reduce the map.
2.01 / 01-2017




                 J-22                                                                    A+W Business Logistic Optimizer
                 Tutorial                                                                     Basic Principles of the OTR




                                        Enable the Menu button, keep the <Ctrl> key pressed and click on a destina-
                                        tion. The following menu opens:




                                        Use this menu to combine groups. Thus, keep the <Ctrl> key pressed and click
                                        on the destination you want to move. The menu opens and you click in the
                                        menu on the group, the destination shall be moved to. The menu closes and
                                        the destination is now in the requested group.
                                        It is very easy to delete a destination, keep the <Ctrl> key pressed and select
                                        the destination. The menu opens and section Delete Destinaton contains the
                                        selected one. Click it and it will be deleted.

                                            Delete Destination
                                            Presently, after deleting a destination the status for the order (orders) is not
                                            changed in the ERP. Only for the other orders (planned, optimized, re-
                                            leased, etc.)

                                        In section Destination you can mark a destination as priority or assign a differ-
                                        ent point. The following points are possible:
                                        •   Starting point
                                        •   Intermediate point
                                        •   End point


                                        Additional information
                                         “The Menu and Tool Bars” on page J-24
                                         “Field help” on page J-30
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                       J-23
                 Basic Principles of the OTR                                                                             Tutorial




                                          The Menu and Tool Bars
                                          The menu bar contains the most important functions for the user. The individ-
                                          ual menus can be opened with the click of a mouse. Some menu items can be
                                          directly opened with the aid of key combinations (e.g. Ctrl+S = Start).




                                          The Start area contains the following buttons:




                                          Description of the individual icons
                                          At the end you will find a list of buttons/icons and their meaning.

                                          Icon                 Description

                                                               Close
                                                               This is used to close the module.

                                                               Check Service
                                                               This button is used to check connection to the service.

                                                               Logbook
                                                               This button is used to open the logbook, in which daily events
                                                               are recorded.

                                                               Help
                                                               This button opens the A+W Business Help.


                                                               About OTR
                                                               This button opens a dialog containing information about the
                                                               version and the license key.


                                          The View area contains the following entries:




                                          The individual entries are used to adjust the appearance of OTR.
2.01 / 01-2017




                 J-24                                                                   A+W Business Logistic Optimizer
                 Tutorial                                                                    Basic Principles of the OTR




                                        The Configuration area contains the following buttons:




                                        Description of the individual icons
                                        At the end you will find a list of buttons/icons and their meaning.

                                        Icon                 Description

                                                             Settings
                                                             This button lets you access the database settings. It opens the
                                                             Settings dialog.

                                                             Parameters
                                                             This button takes you to the parameters. It opens the
                                                             Parameters dialog.

                                                             Import/Export
                                                             Use this icon button to backup the parameter in XML format.


                                                             Language
                                                             You can select the program language for OTR with this button.



                                        The Settings area contains the following buttons:




                                        Description of the individual icons
                                        At the end you will find a list of buttons/icons and their meaning.

                                        Icon                 Description

                                                             User
                                                             This button takes you to the users. The User dialog opens.

                                                             Status
                                                             This button lets you access the status. The Status dialog
                                                             opens.

                                                             Customers
                                                             This button takes you to the customers. The Customer dialog
                                                             opens.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                         J-25
                 Basic Principles of the OTR                                                                             Tutorial




                                          Icon                 Description

                                                               Departments
                                                               This button takes you to the departments. The Department
                                                               dialog opens.

                                                               Vehicles
                                                               You can access the fleet park by pressing this button. It
                                                               opens the Vehicles dialog.

                                                               Drivers
                                                               With this button, you have access to your drivers. The
                                                               Drivers dialog opens.

                                                               Reports
                                                               This button takes you to the reports. The Report dialog opens

                                                               Packaging types
                                                               This icon button allows you to access the packaging types.
                                                               The Packaging Types dialog opens.

                                                               Data import
                                                               With this button you can import data in CSV format. The Data
                                                               import dialog opens

                                          The Query area contains the following buttons:




                                          Description of the individual icons
                                          At the end you will find a list of buttons/icons and their meaning.

                                          Icon                 Description

                                                               Filter
                                                               This button is used to filter individual routes. It opens the
                                                               dialog Filter routes.

                                                               Edit route
                                                               This button is used to change the route status and the real
                                                               costs. The Edit Route dialog opens.

                                                               Delete route
                                                               This button is used to delete a previously selected route.


                                                               Export route
                                                               With this button, you can export data to a navigation system.
                                                               This opens the Export dialog.

                                                               Edit status
2.01 / 01-2017




                                                               This button is used to change the route status. The Change
                                                               status dialog opens.




                 J-26                                                                    A+W Business Logistic Optimizer
                 Tutorial                                                                     Basic Principles of the OTR




                                        Icon                 Description

                                                             History
                                                             This button is used to view the document history. It opens the
                                                             History dialog.

                                                             Selected route
                                                             This button opens the Crystal Report Confirmation and
                                                             Delivery List for the selected route.

                                                             Report launcher
                                                             This button opens the Report launcher dialog for the selected
                                                             route.

                                                             Statistics
                                                             This button opens the Statistics dialog for the selected route.

                                                             View route
                                                             This button opens the Route dialog.

                                                             View destination
                                                             This button opens the Destination dialog.

                                                             Calendar
                                                             This button opens the Calendar dialog. The calendars shows
                                                             the routes traveled by vehicles and drivers.

                                                             Route administrator
                                                             This button serves for online tracking of the currently
                                                             traveling routes.

                                                             Attach files
                                                             This button is used to add a document to a destination.



                                        The tool bar in the planning phase
                                        The tool bar in the planning phase enables access to all functions and dialogs
                                        that are relevant to this phase.




                                        Description of the individual icons
                                        At the end you will find a list of buttons/icons and their meaning.

                                        Icon                 Description

                                                             Copy saved route.
2.01 / 01-2017




                                                             With this button, you can add a saved route. The dialog
                                                             Saved Routes opens..




                 A+W Business Logistic Optimizer                                                                        J-27
                 Basic Principles of the OTR                                                                Tutorial




                                          Icon   Description

                                                 Load saved route.
                                                 With this button, you can add a new route to a saved route.
                                                 The dialog Saved Route List opens.

                                                 Import destinations
                                                 With this button, you can import destinations. The Data
                                                 Import dialog opens..

                                                 New route
                                                 This button is used to create a new route. The Route dialog
                                                 opens.

                                                 Edit route
                                                 This button is used to edit a previously selected route.


                                                 Delete route
                                                 This button is used to delete a previously selected route.


                                                 Groups
                                                 With this button, you can split routes in groups.

                                                 Vehicles
                                                 Use this button to assign a different vehicle to the route. The
                                                 Vehicles dialog opens..

                                                 New destination
                                                 This button is used to add a new destination to a route. The
                                                 Destination dialog opens.

                                                 Edit destination
                                                 By pressing this button, you can edit a previously selected
                                                 destination. The dialog Edit destination opens.

                                                 Delete destination
                                                 By pressing this button, you can delete a previously selected
                                                 destination.

                                                 Packaging
                                                 This button opens the Packaging tab.

                                                 Detailed view
                                                 This button gives you a detailed view of the destinations of a
                                                 route.

                                                 Initialize
                                                 This button takes you back to the starting situation. If, e.g.
                                                 you have grouped records, which you wish to undo, click this
                                                 button.
2.01 / 01-2017




                 J-28                                                      A+W Business Logistic Optimizer
                 Tutorial                                                                     Basic Principles of the OTR




                                        The tool bar in the optimization phase
                                        The tool bar in the realization phase enables access to all functions and dia-
                                        logs that are relevant to this phase.




                                        Description of the individual icons
                                        At the end you will find a list of buttons/icons and their meaning.

                                        Icon                 Description

                                                             Optimize route
                                                             This button optimizes the route again.


                                                             Stop optimization
                                                             This button is used to stop the optimization.


                                                             Traffic
                                                             This button is used to determine the traffic based on
                                                             statistical values (Nokia Maps).

                                                             Stop traffic
                                                             Use this button to abort traffic determination.

                                                             Edit route
                                                             This button is used to edit a route. The Route dialog opens.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                      J-29
                 Basic Principles of the OTR                                                                           Tutorial




                                          The tool bar in the result phase
                                          The tool bar in the result phase enables access to all functions and dialogs that
                                          are relevant to this phase.




                                          Description of the individual icons
                                          At the end you will find a list of buttons/icons and their meaning.

                                          Icon                  Description

                                                                View route
                                                                This button opens the Route dialog.

                                                                View destination
                                                                This button opens the Destination dialog.

                                                                Edit route
                                                                This button is used to change the route status and the real
                                                                costs. The Edit Route dialog opens.



                                          Field help
                                          If the [Help] icon is located next to a field, hover your mouse on it and it shows
                                          you information about the field.




                                          Fig. J-8     Field help


                                          Additional information
                                           “User Interface” on page J-21
2.01 / 01-2017




                 J-30                                                                    A+W Business Logistic Optimizer
                 Tutorial                                                                 Administration




                                        Administration
                                        This section introduces the master data in OTR.
                                        This includes the following training modules:
                                        •   “Parameters” on page J-32
                                        •   “User” on page J-34
                                        •   “Status” on page J-35
                                        •   “Customers” on page J-37
                                        •   “Departments” on page J-40
                                        •   “Vehicles” on page J-42
                                        •   “Driver” on page J-46
                                        •   “Reports” on page J-49
                                        •   “Packaging Types” on page J-51
                                        •   “Data Import” on page J-54
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                   J-31
                 Administration                                                                           Tutorial




                                  Parameters
                                  In this area you define standard settings to work with OTR.
                                  The parameters are first divided into two groups:
                                  •   Parameters for the configuration of the application
                                      These parameters are used for general configuration, such as text format,
                                      unit systems, currency, etc.
                                  •   Parameters for routes
                                      Routes are created and optimized on this basis of these values. Via the Edit
                                      Route dialog you can always access these values and make temporary
                                      changes.
                                  The software reference provides a detailed description on this.


                                  Additional information
                                   Software Reference, “Parameters” on page J-132
2.01 / 01-2017




                 J-32                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                                     Administration




                                        Master Data
                                        Objectives

                                        •   Getting to know the parameters
                                        •   Learning and understanding how to work with the vehicles fleet
                                        •   Learning and understanding how to work with users and departments
                                        •   Learning and understanding how to work with drivers


                                        Benefits

                                        • Fleet park data has to be maintained accurately in order to determine route costs.
                                          This is the only way to obtain accurate values. As it may be necessary to contact
                                          your driver by phone, we recommend keeping their data up to date.


                                        Definition

                                        Fixed costs                 Costs that remain unchanged when changing a variable
                                                                    (total distance, fuel costs).


                                        Please note

                                        Creating a new vehicle      When creating a new vehicle, we recommend having the
                                                                    vehicle registration at hand.

                                        Maintenance date            You have the opportunity to enter the next maintenance
                                                                    date for your vehicle. The module reminds you of this
                                                                    date in due time.

                                        Assigning a driver          You can assign the vehicle to a fixed driver.

                                        Costs                       Costs can be set up per driver based on time or distance.

                                        Personnel                   OTR differentiates between own personnel (employees)
                                                                    and external personnel (hired drivers).
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                       J-33
                 Administration                                                                           Tutorial




                                  User
                                  This section is used to control user profiles, that are registered under Windows
                                  or in a domain. The data is automatically generated at program (OTR) start.




                                  Fig. J-9     User


                                  The table above shows which profiles have already been created. As admin-
                                  istrator you can define e.g. users with default profile (language, presentation
                                  of user interface, etc.) that can be copied later on.
                                  The software reference provides a detailed description of the individual fields.

                                     Rights
                                     To edit, the user must be a member of the administrator group. The users
                                     are registered, after starting OTR from A+W Business. Otherwise, the us-
                                     ers are registered by the operating system.


                                  Additional information
                                   Software Reference, “User” on page J-142
2.01 / 01-2017




                 J-34                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                                Administration




                                        Status
                                        Depending on the route condition, it has a certain status.




                                        Fig. J-10    Status


                                        The table above shows which status types have already been created. You
                                        can define a new status or change an existing one. The field Editable shows
                                        the status that can be changed. A green checkmark indicates that the status
                                        can be changed. All status types without green checkmaks cannot be
                                        changed.
                                        To load data into the cloud, a manual change of status may be necessary for
                                        those routes, manually released for the driver.
                                        The individual status are grouped. The group (650) for example deals with var-
                                        ious behaviors concerning destinations. It contains the following status:
                                        •   Destination problem: The truck could not reach the destination.
                                        •   Destination not found: The destination was simply not found.
                                        The software reference provides a detailed description of the individual fields.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-35
                 Administration                                                                          Tutorial




                                  Managing Status Types
                                  Here you will learn how to create, edit or delete new status types.
                                  The following instructions exist for this training module:
                                  •   “How to create a new status” on page J-36
                                  •   “How to delete an existing status” on page J-36
                                  •   “How to make changes to a certain status” on page J-36


                                   How to create a new status
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Status] button.
                                      The Status dialog opens.
                                  3 Press the icon button [New].
                                      The lower part of the dialog is now available for editing.
                                  4 Click on the icon button. The Status Type dialog opens. From the list select
                                    the type the status belongs to. Click [OK]. The dialog closes. The informa-
                                    tion will be adopted.
                                  5 Field Status is prepopulated with the next free number.
                                  6 In the Status name field, enter the name.
                                  7 Whether the checkboxes Routes and Destinations are enabled or not de-
                                    pends on the groups, they are allocated to.
                                  8 You can enter a detailed description of the status in the Description field.


                                   How to delete an existing status
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Status] button.
                                      The Status dialog opens.
                                  3 Select the status from the table that is to be deleted.
                                  4 Press the icon button [Delete].
                                      The entry is deleted.


                                   How to make changes to a certain status
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Status] button.
                                      The Status dialog opens.
                                  3 Select the status from the table that is to be changed. The checkmark in
                                    field Editable indicates that the status can be changed.
2.01 / 01-2017




                 J-36                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                                Administration




                                        4 Press the [Edit] button.
                                        5 Carry out the required changes.
                                        6 Press the [Save] button.
                                           The data is saved.


                                        Additional information
                                         Software Reference, “Status” on page J-143


                                        Customers
                                        In OTR you can manage individual, additional customer data (addresses).
                                        This may be helpful to manage loading and unloading addresses without cre-
                                        ating them in the ERP system (A+W Business Customer Master Data). To ac-
                                        tivate this property, set the value USE_CUSTOMERS_OTR to Yes in the
                                        parameters.




                                        Fig. J-11    Customers


                                        If the parameter is enabled, OTR checks during import whether the customer
                                        is already saved. If not it is saved and can be used immediately.
                                        The software reference provides a detailed description of the individual fields.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-37
                 Administration                                                                               Tutorial




                                  Managing Customers
                                  Here you will learn how to create, edit or delete new customers manually.
                                  The following instructions exist for this training module:
                                  •   “How to create a new customer manually” on page J-38
                                  •   “How to delete an existing customer” on page J-38
                                  •   “How to make changes to a certain customer” on page J-39


                                   How to create a new customer manually
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Customer] button.
                                      The Customer dialog opens.
                                  3 Press the icon button [New].
                                      The lower part of the dialog is now available for editing.
                                  4 Enter the required number in field Customer. Note: Each number can only
                                    be assigned once.
                                  5 Enter the name of the customer in the Name field.
                                  6 Enter the telephone number in the Telephone Number field.
                                  7 In the field Address you can enter the customer address.
                                      Please enter the name of the street and the name of the city separated by
                                      comma.
                                  8 If the longitude and latitude fields are not filled, click [Geolocate].
                                  9 In field Time (Minutes) you can enter the time that the driver has on site.
                                  10 In field Time Range you can enter the unloading time on-site for the driver.
                                  11 In field Contact Person you can enter a contact person for the customer.
                                  12 In field E-Mail Address Contact you can enter the email address of the con-
                                     tact.


                                   How to delete an existing customer
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Customer] button.
                                      The Customer dialog opens.
                                  3 Select the customer from the table that is to be deleted.
                                  4 Press the icon button [Delete].
                                      The entry is deleted.
2.01 / 01-2017




                 J-38                                                           A+W Business Logistic Optimizer
                 Tutorial                                                                             Administration




                                         How to make changes to a certain customer
                                        1 Go to the menu bar to Administration.
                                        2 Press the [Customer] button.
                                           The Customer dialog opens.
                                        3 Select the customer from the table that is to be changed.
                                        4 Press the [Edit] button.
                                        5 Carry out the required changes.
                                        6 Press the [Save] button.
                                           The data is saved.


                                        Additional information
                                         Software Reference, “Customers” on page J-145
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                               J-39
                 Administration                                                                           Tutorial




                                  Departments
                                  Use this dialog to add, change or delete individual departments. This serves
                                  for statistical evaluations. On this basis individual evaluations can be imple-
                                  mented. Thus, external companies (transport companies) can be defined as
                                  Department.




                                  Fig. J-12    Departments


                                  The table above shows which departments have already been created.
                                  The software reference provides a detailed description of the individual fields.

                                  Managing Departments
                                  Here you will learn how to create, edit or delete departments.
                                  The following instructions exist for this training module:
                                  •   “How to define a new department” on page J-40
                                  •   “How to delete an existing department” on page J-41
                                  •   “How to make changes to a certain department” on page J-41


                                   How to define a new department
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Department] button.
                                      The Department dialog opens.
                                  3 Enter the number of the department in the Department field.
                                  4 Enter the name of the department in the Name field.
                                  5 You can enter a description of the department in the Description field.
2.01 / 01-2017




                 J-40                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                               Administration




                                         How to delete an existing department
                                        1 Go to the menu bar to Administration.
                                        2 Press the [Department] button.
                                           The Department dialog opens.
                                        3 Select the department from the table that is to be deleted.
                                        4 Press the icon button [Delete].
                                           The entry is deleted.


                                         How to make changes to a certain department
                                        1 Go to the menu bar to Administration.
                                        2 Press the [Department] button.
                                           The Department dialog opens.
                                        3 Select the department from the table that is to be changed.
                                        4 Press the [Edit] button.
                                        5 Carry out the required changes.
                                        6 Press the [Save] button.
                                           The data is saved.


                                        Additional information
                                         Software Reference, “Departments” on page J-147
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                 J-41
                 Administration                                                                             Tutorial




                                  Vehicles
                                  In this area you find all vehicles that are available for the delivery of goods.
                                  This includes:
                                  •   Truck
                                  •   Automobile
                                  •   Trailer




                                  Fig. J-13    Vehicles


                                  The table above shows you which vehicles have already been created. You
                                  can create new vehicles and also make changes to existing vehicles.
                                  The software reference provides a detailed description of the individual fields.

                                      Vehicle data
                                      When creating a new vehicle, we recommend having the vehicle registra-
                                      tion at hand. Data will be requested by the system that you can find here,
                                      such as empty weight.


                                  Additional information
                                   Software Reference, “Vehicles” on page J-148
2.01 / 01-2017




                 J-42                                                           A+W Business Logistic Optimizer
                 Tutorial                                                                                   Administration




                                        Managing Vehicles
                                        Here you will learn how to create, edit or delete new vehicles.
                                        The following instructions exist for this training module:
                                        •   “How to create a new vehicle” on page J-43
                                        •   “How to delete an existing vehicle” on page J-44
                                        •   “How to make changes to a certain vehicle” on page J-44
                                        •   “How to assign a vehicle to a fixed driver” on page J-45
                                        •   “How to remove a fixed driver” on page J-45


                                         How to create a new vehicle
                                        1 Go to the menu bar to Administration.
                                        2 Press the [Vehicles] button.
                                            It opens the Vehicles dialog.
                                        3 Press the icon button [New].
                                            The lower part of the dialog is now available for editing. For the entries that
                                            follow, we recommend having the vehicle registration at hand.
                                        4 Fill the fields License Plate, Brand, Model and Chassis Number on the ba-
                                          sis of the vehicle registration documents.
                                        5 Fill the field Purchase Date.
                                        6 In the field Next Maintenance, you can enter the date for the next mainte-
                                          nance.
                                            If the entry New maintenance date for vehicles is enabled in the parame-
                                            ters, the field here is evaluated accordingly.
                                        7 Field Department allows to assign a department to the vehicle. This serves
                                          for statistical evaluations. The button opens the dialog Select Department,
                                          containing all defined departments.
                                        8 Fill the fields Maximum Width, Maximum Height, Maximum Length, Maxi-
                                          mum Load and Empty Weight on the basis of the information in the vehicle
                                          documentation.
                                        9 Enter the average fuel consumption of the vehicle in the Consumption field
                                          in liters, e.g. 18.5.
                                        10 Enter the average price for a liter of fuel in the Fuel Costs field, e.g. 1.43.
                                           You can set up the currency unit in the parameters.
                                            You can set up the currency unit in the parameters.
                                        11 Enter the average price for a liter of fuel in the Fixed Costs field, e.g. 1.43.
                                            You can set up the currency unit in the parameters.
                                        12 Select the vehicle type from the combo box Vehicle Type.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                      J-43
                 Administration                                                                           Tutorial




                                  13 The fields Driver ID, First Name and Surname are linked to the [Add driver]
                                     button.
                                     If you press the button, the Driver dialog opens. You can select a driver
                                     here. This is recommended if employees have a fixed assignment to a ve-
                                     hicle.
                                  14 The route numbers shown here are transferred from AWBusiness and
                                     serves to assign trucks to certain route numbers.
                                  15 The Sequence field is in direct connection with the Routes field. If the same
                                     route number is allowed for two or more trucks, this field allows to deter-
                                     mine the sequence. The field will be evaluated if the value
                                     ROUTE_ORIGIN has been set to Yes in the parameters.
                                  16 The checkbox Vehicle Available is used to define whether the vehicle is
                                     generally available for all routes.
                                  17 If your vehicle is equipped with a trailer hitch, enable the checkbox Truck
                                     with trailer.


                                   How to delete an existing vehicle
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Vehicles] button.
                                     It opens the Vehicles dialog.
                                  3 Select the vehicle that is to be deleted from the table.
                                  4 Press the icon button [Delete].
                                     The entry is deleted.


                                   How to make changes to a certain vehicle
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Vehicles] button.
                                     It opens the Vehicles dialog.
                                  3 Select the vehicle in the table that is to be changed.
                                  4 Press the [Edit] button.
                                  5 Carry out the required changes.
                                  6 Press the [Save] button.
                                     The data is saved.
2.01 / 01-2017




                 J-44                                                         A+W Business Logistic Optimizer
                 Tutorial                                                                                Administration




                                         How to assign a vehicle to a fixed driver
                                        1 Go to the menu bar to Administration.
                                        2 Press the [Vehicles] button.
                                           It opens the Vehicles dialog.
                                        3 Select the vehicle in the table that is to be assigned to a driver.
                                        4 Press the [Edit] button.
                                        5 Press the [Add Driver] button.
                                           The Drivers dialog opens.
                                        6 Select the desired driver.
                                        7 Press the [OK] button.
                                           The dialog is closed and you are now back in the Vehicles dialog.
                                        8 Press the [Save] button.
                                           The data is saved.


                                         How to remove a fixed driver
                                        1 Go to the menu bar to Administration.
                                        2 Press the [Vehicles] button.
                                           It opens the Vehicles dialog.
                                        3 Select the vehicle in the table, from which the driver is to be removed.
                                        4 Press the [Edit] button.
                                        5 Press the [Delete Driver] button.
                                           The driver is deleted.
                                        6 Press the [Save] button.
                                           The data is saved.


                                        Additional information
                                         Software Reference, “Vehicles” on page J-148
                                         Software Reference, “Driver” on page J-151
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-45
                 Administration                                                                             Tutorial




                                  Driver
                                  In this area, you can administer data for your drivers. In this area you find all
                                  drivers that are available for the delivery of goods. This includes:
                                  •   Company drivers
                                  •   Drivers from other companies (hired drivers)




                                  Fig. J-14    Driver


                                  The table above shows you which drivers have already been created. You can
                                  create new drivers and also make changes to existing drivers.
                                  The software reference provides a detailed description of the individual fields.


                                  Additional information
                                   Software Reference, “Driver” on page J-151
2.01 / 01-2017




                 J-46                                                            A+W Business Logistic Optimizer
                 Tutorial                                                                                   Administration




                                        Managing Drivers
                                        Here you will learn how to create, edit or delete new drivers.
                                        The following instructions exist for this training module:
                                        •   “How to create a new driver” on page J-47
                                        •   “How to delete an existing driver” on page J-48
                                        •   “How to make changes to a certain driver” on page J-48


                                         How to create a new driver
                                        1 Go to the menu bar to Administration.
                                        2 Press the [Driver] button.
                                            The Drivers dialog opens.
                                        3 Press the icon button [New].
                                            The lower part of the dialog is now available for editing.
                                        4 Enter a short description of the driver in the Driver ID field.
                                        5 Fill the fields Name, Surname and Surname 2.
                                        6 Enter the tax number of the employee in the field Tax ID.
                                        7 Enter the e-mail address of the employee in the E-Mail field.
                                        8 In the Costs field you can enter an amount attributed to the route that is
                                          caused by the employee.
                                            Costs are differentiated by time and by distance. Please enable the under-
                                            lying radio buttons (By time / By distance). The value entered here is includ-
                                            ed in the evaluation in the Costs tab.
                                        9 In the Address field, enter the address of the employee and enter the re-
                                          spective telephone numbers in the fields Telephone and Telephone 2.
                                        10 In the Contact field, you can enter the name of a contact person if the driver
                                           is not employed with your company.
                                            Example: You book a driver from a transport company for a route.
                                        11 In the field Contact Address you can enter the address of your contact.
                                        12 Enter the respective telephone number in the Telephone-Contact field.
                                        13 You can enter a description of the driver or the contact in the Description
                                           field and the e-mail in the respective E-mail Address Contact field.
                                        14 Field Department allows to assign a department to the driver. This serves
                                           for statistical evaluations.
                                            The button opens the dialog Select Department, containing all defined de-
                                            partments.
                                        15 Via the checkbox Company Driver you can indicate whether the driver is
                                           employed with your company and via the checkbox Available, whether the
2.01 / 01-2017




                                           driver is always available.
                                        16 The checkbox Reset Password is used to reset the password necessary at
                                           start of the GDC App (mobil App for drivers).


                 A+W Business Logistic Optimizer                                                                     J-47
                 Administration                                                                          Tutorial




                                   How to delete an existing driver
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Driver] button.
                                     The Drivers dialog opens.
                                  3 Select the driver from the table that is to be deleted.
                                  4 Press the icon button [Delete].
                                     The entry is deleted.


                                   How to make changes to a certain driver
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Driver] button.
                                     The Drivers dialog opens.
                                  3 Select the driver from the table that is to be changed.
                                  4 Press the [Edit] button.
                                  5 Carry out the required changes.
                                  6 Press the [Save] button.
                                     The data is saved.


                                  Additional information
                                   Software Reference, “Driver” on page J-151
2.01 / 01-2017




                 J-48                                                            A+W Business Logistic Optimizer
                 Tutorial                                                                                Administration




                                        Reports
                                        In this area, you can administer data for your reports. The dialog contains all
                                        reports defined. OTR works with reports on basis of SAP Crystal Reports.




                                        Fig. J-15    Reports


                                        The table above shows which reports have already been created. You can cre-
                                        ate new reports and also make changes to existing reports.
                                        The software reference provides a detailed description of the individual fields.


                                        Additional information
                                         Software Reference, “Reports” on page J-154
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-49
                 Administration                                                                          Tutorial




                                  Managing Reports
                                  Here you will learn how to create, edit or delete new reports.
                                  The following instructions exist for this training module:
                                  •   “How to create a new report” on page J-50
                                  •   “How to delete an existing report” on page J-50
                                  •   “How to make changes to a certain report” on page J-50


                                   How to create a new report
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Report] button.
                                      The Report dialog opens.
                                  3 Press the icon button [New].
                                      The lower part of the dialog is now available for editing.
                                  4 Enter the name of the report in the Name field, e.g. Short.
                                  5 Field Report Path allows to enter where the report is to be saved.
                                  6 The Description field allows you to enter information about the report.
                                  7 Use the checkboxes in section Parameter to select the information to be
                                    printed on the report.


                                   How to delete an existing report
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Report] button.
                                      The Report dialog opens.
                                  3 Select the report from the table that is to be deleted.
                                  4 Press the icon button [Delete].
                                      The entry is deleted.


                                   How to make changes to a certain report
                                  1 Go to the menu bar to Administration.
                                  2 Press the [Report] button.
                                      The Report dialog opens.
                                  3 Select the reports from the table that is to be changed.
                                  4 Press the [Edit] button.
                                  5 Carry out the required changes.
                                  6 Press the [Save] button.
2.01 / 01-2017




                                      The data is saved.




                 J-50                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                                Administration




                                        Additional information
                                         Software Reference, “Reports” on page J-154


                                        Packaging Types
                                        In this area, you can administer data for your packaging types. The dialog con-
                                        tains all packing types defined. A packaging might be a rack but also a box.




                                        Fig. J-16    Packaging


                                        The table above shows which packaging types have already been created.
                                        You can create new packaging types and also make changes to existing types.
                                        The software reference provides a detailed description of the individual fields.

                                           Loading Space Optimization
                                           The current version does not support a loading space optimization for
                                           trucks. Use the defined packaging types for booking purposes like unload-
                                           ing or collecting (tracking of packaging types).


                                        Additional information
                                         Software Reference, “Packaging” on page J-155
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-51
                 Administration                                                                            Tutorial




                                  Managing Packaging Types
                                  Here you will learn how to create, edit or delete new packaging types.
                                  The following instructions exist for this training module:
                                  •   “How you create one new packaging type” on page J-52
                                  •   “How to delete an existing packaging type” on page J-52
                                  •   “How to make changes to a certain packaging type” on page J-53


                                   How you create one new packaging type
                                  1 Go to the menu bar to Administration.
                                  2 Press the icon button [Packaging Types].
                                      The Packaging Types dialog opens.
                                  3 Press the icon button [New].
                                      The lower part of the dialog is now available for editing.
                                  4 Enter the packaging ID in field Packaging ID, e.g. 1000100.
                                  5 Enter the type in field Packaging Type, e.g. A rack, L rack, box.
                                  6 Field Department allows to assign a department to the packaging type. This
                                    serves for statistical evaluations. The icon button opens the dialog Select
                                    Department, containing all defined departments.
                                  7 Enter the specific values in the fields Width, Height, Length, and Empty
                                    Weight.
                                  8 In field Costs, you have the opportunity to set up purchase costs for the
                                    packaging type.
                                  9 Enable the checkbox Do no collect if the customer shall keep the packag-
                                    ing.
                                  10 The Description field allows you to enter information about the packaging
                                     type.


                                   How to delete an existing packaging type
                                  1 Go to the menu bar to Administration.
                                  2 Press the icon button [Packaging Type].
                                      The Packaging Types dialog opens.
                                  3 Select the packaging type that is to be deleted from the table.
                                  4 Press the icon button [Delete].
                                      The entry is deleted.
2.01 / 01-2017




                 J-52                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                             Administration




                                         How to make changes to a certain packaging type
                                        1 Go to the menu bar to Administration.
                                        2 Press the icon button [Packaging Type].
                                           The Packaging Types dialog opens.
                                        3 Select the packaging type in the table that is to be changed.
                                        4 Press the [Edit] button.
                                        5 Carry out the required changes.
                                        6 Press the [Save] button.
                                           The data is saved.


                                        Additional information
                                         Software Reference, “Packaging” on page J-155
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                               J-53
                 Administration                                                                           Tutorial




                                  Data Import
                                  Use this dialog to import data in CSV format (MS Excel).




                                  Fig. J-17    Data import


                                  Please select the data to be imported from the combo box. The following op-
                                  tions are available:
                                  •   Customers
                                  •   Departments
                                  •   Driver
                                  •   Vehicles
                                  The software reference provides a detailed description of the individual fields.


                                  Additional information
                                   Software Reference, “Data Import” on page J-157
2.01 / 01-2017




                 J-54                                                         A+W Business Logistic Optimizer
                 Tutorial                                                                         Planning Routes




                                        Planning Routes
                                        This section shows you how to plan routes and create new destinations.
                                        This includes the following training modules:
                                        •   “General” on page J-57
                                        •   “Import” on page J-58
                                        •   “Routes” on page J-59
                                        •   “Destinations” on page J-69
                                        •   “The Detailed View” on page J-73
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                 J-55
                 Planning Routes                                                                                 Tutorial




                                   Routes and Destinations
                                   Objectives

                                   •   Getting to know both working methods
                                   •   Getting to know and understanding the import
                                   •   Getting to know and understanding the planning phase
                                   •   Getting to know and understanding routes
                                   •   Getting to know and understanding destinations


                                   Benefits

                                   • Route planning determines the most efficient route from A to D via B and C. This
                                     saves time and money.


                                   Definition

                                   Route                       The route describes the exact way between several
                                                               waypoints.

                                   Route                       The route is adopted from A+W Business customer data.


                                   Please note

                                   Delivery Date               Delivery date that was transferred from A+W Business.

                                   Original Route              This number is a route number from A+W Business.

                                   Route ID                    The route ID assigned by OTR.

                                   Sequence                    The sequence of the waypoints within the route.

                                   Dynamic mode                Groups and routes are created automatically.
2.01 / 01-2017




                 J-56                                                             A+W Business Logistic Optimizer
                 Tutorial                                                                               Planning Routes




                                        General
                                        OTR can work in two different mode. Which one to use depends on your work
                                        process. The settings are made in the parameters.
                                        •   Mode 1: The routes are used that are created and transferred by A+W
                                            Business. OTR uses these routes for planning and optimization of routes
                                            (distance, sequence of stops).
                                        •   Mode 2: This is the Dynamic Mode. OTR creates the routes itself. No work
                                            is necessary in A+W Business. After the import OTR groups the routes au-
                                            tomatically based on the addresses. In this step Geolocation of addresses
                                            takes place. Grouping is made by the following criteria:
                                            – Addresses
                                            – Weight per address (orders are grouped by customers)
                                            The assignment is based on target time, additional stops, e.g. for collecting
                                            racks and statistical determination of traffic (Nokia maps).
                                            To print delivery notes in correct sequence, the data can be reported to
                                            A+W Business in this mode, too.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                    J-57
                 Planning Routes                                                                                  Tutorial




                                          Import
                                          Data import is made via number manager. During the import OTR checks the
                                          addresses and either uses the address from the order header, an alternate de-
                                          livery address or the address from the OTR master data.
                                          In this step Geolocation of addresses and grouping take place. Based on lon-
                                          gitude and latitude the system calculates the distance between the individual
                                          destinations and combines the orders into areas and routes under consider-
                                          ation of weight and available trucks.




                 Fig. J-18   Sections and table overview


                                          The table shows in the Routes section the number of route to be travelled.
                                          The graphic below contains on the left side the groups in different colors. So
                                          you can see at a glance how many destinations are grouped. Adjacent to the
                                          right are the respective routes and destinations.
                                          A selected destination on the map is highlighted in the table. Thus, identifica-
                                          tion is simple and stops can easily be assigend to a different group.
2.01 / 01-2017




                 J-58                                                                 A+W Business Logistic Optimizer
                 Tutorial                                                                             Planning Routes




                                        Routes
                                        This area shows you all routes that are current routes for delivery.




                                        Fig. J-19    Route Information


                                        The content of the field Name of the Route (ROUTE NORD) is obtained from
                                        the A+W Business master data. The route ID (8) is assigned by OTR and in-
                                        creased by 1 for each route. The delivery date (21.03.2014) is from A+W Busi-
                                        ness, as is the content of the field Original Route (21).
                                        Assign the Truck Driver, the License Plate as well as the Brand and Model. The
                                        content of the fields Fuel Costs and Fuel Consumption are obtained from the
                                        OTR master data (parameter: Fuel costs, Average Fuel Consumption).
                                        Double-clicking a route opens the Route dialog.
                                        The software reference provides a detailed description of the individual fields.
                                        In case the number manager contains orders with various delivery dates, the
                                        system creates or splits automatically different routes. You can override this
                                        manually in Planning step.


                                        Additional information
                                         Software Reference, “Creating a New Route – General” on page J-165
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-59
                 Planning Routes                                                                           Tutorial




                                   Load a Saved Route
                                   OTR automatically saves the routes after the last process step (Result).
                                   You can access a route at any time in order to optimize it with new parameters.
                                   The ID is not changed during this process. Only routes with the following sta-
                                   tus can be loaded:
                                   •   Roughly scheduled (planned)
                                   •   Scheduled in detail (optimized)




                                   Fig. J-20     Saved route list


                                   The software reference provides a detailed description of the individual fields.


                                   Additional information
                                    Software Reference, “Creating a New Route – General” on page J-165>
2.01 / 01-2017




                 J-60                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                                Planning Routes




                                        Copy a Saved Route
                                        With this function, you can copy a route to perform various simulations so that
                                        you can make the best possible decision.
                                        Copying the route changes the ID. For this, the route status is insignificant, i.e.
                                        you can copy routes with any route status.




                                        Fig. J-21    Copy saved route


                                        The software reference provides a detailed description of the individual fields.


                                        Additional information
                                         Software Reference, “Copy a Saved Route” on page J-161>
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                      J-61
                 Planning Routes                                                                               Tutorial




                                   Working with Routes
                                   Here you will learn how to create, edit or delete new routes.
                                   The following instructions exist for this training module:
                                   •   “How to create a new route” on page J-62
                                   •   “How to load a saved route” on page J-66
                                   •   “How to copy a saved route” on page J-67
                                   •   “How to delete a current route” on page J-67
                                   •   “How to combine routes” on page J-68


                                    How to create a new route
                                   1 Press the [New Route] button.
                                       This opens the Route dialog, tab General.




                                   2 In the Delivery Date field, define the day on which the route is to take place.
                                       Clicking on the arrow at the end of the field opens the calendar from which
                                       you can easily select the respective date.
                                   3 In the field Start Time, enter the time at which the route is to start.
                                       You can set the time with the arrows at the end of the field.
2.01 / 01-2017




                 J-62                                                           A+W Business Logistic Optimizer
                 Tutorial                                                                                Planning Routes




                                        4 Assign a name to the route in the field Route Name.
                                        5 You can enter a detailed description of the route in the Description field.
                                        6 The content of the fields Name, Address, in the Starting Point are values
                                          that you have set up in the parameters (fields: Start-Company Name, Start-
                                          Address).
                                           If your route hasn't started yet, you can overwrite the entries.
                                        7 If the address specified under point 6 should also serve as starting point,
                                          enable the checkbox Use Starting Point.
                                           If the address and starting point do not correspond, it may be attributed to
                                           the fact that you have a headquarters with several subsidiaries. In this
                                           case, the headquarters is not the starting point of the route.
                                        8 If the longitude and latitude fields are not filled, click [Geolocate].
                                           This opens the Simple Geolocation dialog.




                                           The map view shows you the address with a red dot. If the address is cor-
                                           rect, the Latitude and Longitude fields are filled automatically.
                                        9 You can accept the data by pressing the [Accept] button.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                    J-63
                 Planning Routes                                                                        Tutorial




                                   10 Then go to the Vehicles tab.




                                   11 Click on the [Select Vehicle] button.
                                      The Select Vehicle dialog opens.




                                   12 Select the vehicle that is to be used for the route.
                                   13 Press the [OK] button.
                                      The vehicle will adopted.
2.01 / 01-2017




                 J-64                                                           A+W Business Logistic Optimizer
                 Tutorial                                                                             Planning Routes




                                        14 Switch to the tab Parameter tab.




                                        15 Make the desired selection for Toll, Highway and Tunnel Mode.
                                        16 Select the Route mode.
                                        17 If desired, change the route factors in the Optimization area.




                                        18 Press the [OK] button.
                                           The settings will be transferred. You are now back in the Planning area.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                J-65
                 Planning Routes                                                                       Tutorial




                                    How to load a saved route
                                   1 Press the [Load Saved Route] button.
                                      The dialog Saved Route List opens.




                                   2 Select the required route.
                                   3 Press the [OK] button.
                                      You will be asked whether you want to add the saved route to the current
                                      route.
                                   4 Press the [Yes] button.
                                      The selected route is adopted. You are now back in the Planning area.


                                    How to delete a saved route
                                   1 Press the [Load Saved Route] button.
                                      The dialog Saved Route List opens.
                                   2 Select the route that you would like to copy.
                                   3 Press the [Delete Route] button.
                                      You will be asked whether you really want to delete the route.
                                   4 Press the [Yes] button.
                                      The selected route will be deleted.
2.01 / 01-2017




                 J-66                                                         A+W Business Logistic Optimizer
                 Tutorial                                                                              Planning Routes




                                         How to copy a saved route
                                        1 Press the [Copy Route] button.
                                           The dialog Saved Routes opens.




                                        2 Select the required route.
                                        3 Press the [Route] button.
                                           You will be asked whether you want to add the saved route to the current
                                           route.
                                        4 Press the [Yes] button.
                                           The selected route is adopted. You are now back in the Planning area.


                                         How to delete a current route
                                        1 In the Route area, select the route that is to be deleted.
                                        2 Press the [Delete Route] button.
                                           You will be asked whether you really want to delete the route.
                                        3 Press the [Yes] button.
                                           The selected route will be deleted.
                                        4 Press the [Delete Route] button.
                                           You will be asked whether you really want to delete the route.
                                        5 Press the [Yes] button.
2.01 / 01-2017




                                           The selected route will be deleted.




                 A+W Business Logistic Optimizer                                                                 J-67
                 Planning Routes                                                                          Tutorial




                                    How to combine routes
                                      Sometimes it might make sense to combine a route. To do so, proceed as
                                      follows:
                                   1 In the Destinations area, select the data records that you would like to com-
                                     bine.




                                   2 Open the context menu with the right mouse key. It is imported where (on
                                     which route) you open the context menu. Additional stops are assigned to
                                     this route.
                                      The following message appears:




                                   3 Point your cursor at the message and click it.
                                   4 Both routes are combined into one.




                                   Additional information
                                    Tutorial, “Routes and Destinations” on page J-56
                                    Tutorial, “Vehicles” on page J-42
                                    Software Reference, “Load a Saved Route” on page J-163
                                    Software Reference, “Creating a New Route – General” on page J-165
                                    Software Reference, “Creating a New Route - Vehicle” on page J-169
2.01 / 01-2017




                                    Software Reference, “Creating a New Route – Parameters” on page J-174
                                    Software Reference, “Vehicles” on page J-148




                 J-68                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                              Planning Routes




                                        Destinations
                                        This area contains information about the individual destinations that are driven
                                        to on the route. Either goods are unloaded or racks are collected at certain
                                        destinations.

                                           Number of waypoints
                                           Please note that a route may not have more than 37 waypoints (destina-
                                           tions). This is the maximum number that Nokia can work with in a route.




                                        Fig. J-22    Destinations


                                        The content of the field Name of the Route (ROUTE NORD) is obtained from
                                        the master data. The route ID (8) is assigned by and increased by 1 for each
                                        route. The sequence of the waypoints comes from , whereby 0 represents the
                                        starting point. The order number is shown in the Order field, the customer
                                        number in the Customer field, the customer name in the Name field and the
                                        customer address in the Address field.
                                        The Delivery Weight field contains the weight of the delivered goods. The Col-
                                        lected Weight field shows you how heavy the collected goods are. This could
                                        involve, e.g. racks that you collect on the way.
                                        The checkboxes Delivery and Collection indicate whether the waypoint is a de-
                                        livery point, a collection point or both.
                                        Double-clicking a destination opens the Edit Destination dialog
                                        The software reference provides a detailed description of the individual fields.


                                        Additional information
                                         Software Reference, “Edit Destination” on page J-184
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-69
                 Planning Routes                                                                           Tutorial




                                   Display Documents
                                   If you would like to know what a customer has ordered, you can view the indi-
                                   vidual orders.
                                   Open Documents tab




                                   Fig. J-23    Documents


                                   The software reference provides a detailed description of the individual fields.


                                   Additional information
                                    Software Reference, “Show Information” on page J-189

                                   Deletion of Documents
                                   The context menu permits to delete documents. This might be necessary for
                                   documents with content that can not be deliverred.




                                   Fig. J-24    Documents
2.01 / 01-2017




                 J-70                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                             Planning Routes




                                        Show Items
                                        If you would like to know which customer has ordered what, you can view the
                                        individual items of an order by destination.
                                        Open Items tab




                                        Fig. J-25    Items


                                        The software reference provides a detailed description of the individual fields.


                                        Additional information
                                         Software Reference, “Show Items” on page J-188
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-71
                 Planning Routes                                                                           Tutorial




                                   Show Information
                                   If you would like to know which information are defined for a customer, you can
                                   view these.
                                   Open Information tab




                                   Fig. J-26    Information


                                   The software reference provides a detailed description of the individual fields.


                                   Additional information
                                    Software Reference, “Show Information” on page J-189
2.01 / 01-2017




                 J-72                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                             Planning Routes




                                        The Detailed View
                                        If you have a large vehicle fleet and a large shipping area, the content of the
                                        areas Routes and Destinations may become very cluttered.
                                        The Detailed View gives you the opportunity to restrict the displayed data. If
                                        the Detailed View button is enabled, only the destinations of the route are
                                        shown that you have selected in the Routes area.




                                        Fig. J-27    Detailed view turned off
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-73
                 Planning Routes                                                                           Tutorial




                                   The Detailed View gives you the opportunity to restrict the displayed data. If
                                   the Detailed View button is enabled, only the destinations of the route are
                                   shown that you have selected in the Routes area.




                                   Fig. J-28    Detailed view turned on


                                   If you select a route in section Routes Detailed View you can use the Group
                                   icon button to split the route into several groups.
                                   The software reference provides a detailed description of the individual fields.


                                   Additional information
                                    Software Reference, “Detailed View” on page J-191
2.01 / 01-2017




                 J-74                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                               Planning Routes




                                        Edit Customer Address
                                        OTR offers the possibility to save customer data. For this purpose, the respec-
                                        tive value has to be enabled in the parameters (parameter: OTR Customer Ad-
                                        dresses).
                                        Then, the button as well as the respective dialog is enabled.




                                        Fig. J-29     Customers


                                        Double-clicking an entry opens the Edit Destination dialog. Changes that are
                                        made in this dialog are saved in the OTR database and are available the next
                                        time. The following values are saved:
                                        •   Geolocation
                                        •   Address
                                        •   Delivery times (from / to)
                                        •   Unloading time
                                        The software reference provides a detailed description of the individual fields.

                                            Changes to customer addresses
                                            Please note that the changes to customer addresses that you make here
                                            are not written back to A+W Business. The changes are saved in the OTR
                                            database.


                                        Additional information
                                         Software Reference, “Customers” on page J-190
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-75
                 Planning Routes                                                                            Tutorial




                                   Working with Destinations
                                   Here you will learn how to add destinations to a route, to change them and to
                                   delete them.
                                   The following instructions exist for this training module:
                                   •   “How to add a new destination to a route” on page J-76
                                   •   “How to delete a destination from a route” on page J-77
                                   •   “How to edit a destination” on page J-78


                                    How to add a new destination to a route
                                   1 In the Routes area select the route to which you would like to add a new
                                     destination.
                                   2 Press the [New Destination] button.
                                       The New Destination dialog opens.




                                       This field Customer No. is preset with number 9999.
                                   3 Enter the respective name in the Customer field and open the dialog of the
                                     same name by pressing the [Customer] button.
                                       This is where all customers saved in the OTR database are listed.
                                   4 In the Type field, specify whether the destination is a starting point, the end
                                     point or an intermediate point.
                                   5 In the fields From and To, you can enter the times at which the driver is to
2.01 / 01-2017




                                     be at a destination.
                                       This can be used e.g. if a company has fixed delivery times.
                                   6 You can set up the duration of stay in the field Time (minutes).


                 J-76                                                           A+W Business Logistic Optimizer
                 Tutorial                                                                               Planning Routes




                                        7 The field Selected Route contains all of your routes currently in planning.
                                           This way you can simply assign the new destination to the desired route.
                                        8 You can enter the weight of the delivery in the Delivery Weight field.
                                        9 If you collect empty racks at a destination, you can enter this weight in the
                                          Collected Weight field.
                                           These values are required for the concrete determination of costs but are
                                           not absolutely necessary.
                                        10 You can enter a detailed description about the driver in the Description
                                           field.
                                        11 In the field Address you can enter the customer address.
                                           Please enter the name of the street and the name of the city separated by
                                           comma.
                                        12 Then, press the [Suggestions] button.
                                           A list with suggestions as well as a map view appears beneath the address.
                                           You can transfer an entry from the list to the address field by marking it. You
                                           can also click the red marking point in the map view and, while keeping the
                                           mouse key pressed, pull it to another position on the map.
                                        13 Close the dialog by pressing the [OK] button.


                                         How to delete a destination from a route
                                        1 Tag the location you would like to delete in the Destinations area.
                                        2 Press the [Delete Destination] button.
                                           The message Delete Destination appears.
                                        3 Close the message by pressing the [Yes] button.
                                           The entry is deleted.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                     J-77
                 Planning Routes                                                                         Tutorial




                                    How to edit a destination
                                   1 Tag the location you would like to edit in the Destinations area.
                                   2 Press the [Edit Destination] button.
                                      The dialog Edit destination opens.
                                   3 Make the required changes.
                                   4 Close the dialog by pressing the [OK] button.


                                   Additional information
                                    Software Reference, “Edit Destination” on page J-184
                                    Software Reference, “Customers” on page J-190
                                    “Working with Routes” on page J-62
2.01 / 01-2017




                 J-78                                                           A+W Business Logistic Optimizer
                 Tutorial                                                                                  Planning Routes




                                        Costs
                                        Objectives

                                        • Working with the Costs dialog
                                        • Learning and understanding how to work with various costs
                                        • Creating and editing costs


                                        Benefits

                                        • Fleet park data has to be maintained accurately in order to determine route costs.
                                          This is the only way to obtain accurate values.


                                        Definition

                                        Variable costs              Costs that also change when changing a variable (total
                                                                    distance, fuel costs).

                                        Fixed costs                 Costs that remain unchanged when changing a variable
                                                                    (total distance, fuel costs).

                                        Route costs                 What the route actually costs.


                                        Please note

                                        Real costs                  Costs that are entered when the driver has returned from
                                                                    the route.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                       J-79
                 Planning Routes                                                                           Tutorial




                                   Expenses
                                   This area shows you which expenses you have to reckon with.




                                   Fig. J-30     Costs


                                   The fields are automatically filled after optimization. Based on these values,
                                   you can create various kinds of reports which you can present to the customer
                                   as cost analyses.
                                   The tab is divided into three sections:
                                   •   Variable costs / Real variable costs
                                   •   Fixed costs / Real fixed costs
                                   •   Rote costs / Real route costs


                                   Variable Costs
                                   This area contains the costs that are variable and that also change when
                                   changing a variable (total distance, fuel costs). This may involve costs such as
                                   average fuel price and average consumption. The values are obtained from
                                   the respective parameters (Configuration > Parameter > Vehicles).
                                   The values in the area Real Variable Costs can only be entered once your driv-
                                   er has returned with the route report. Then you know how high the actual costs
                                   were. You can enter these costs in the dialog Edit Route in the tab Route In-
                                   formation.
                                   The software reference provides a detailed description of the individual fields.
2.01 / 01-2017




                 J-80                                                          A+W Business Logistic Optimizer
                 Tutorial                                                                              Planning Routes




                                        Fixed Costs
                                        This area contains the fixed costs, which remain unchanged when changing a
                                        variable (total distance, fuel costs). This involves costs such as insurance, tax
                                        and repairs.

                                        Example

                                        Cost type                  Costs/Year

                                        Insurance per year         1,200.00 €

                                        Tax per year               800.00 €

                                        Maintenance per year       300.00 €


                                        In total: 2,300.00 €. Based on an estimated number of routes of approx. 220
                                        per year, the resulting fixed costs is 10.45 € per route. This value should be
                                        included in the vehicle master data. If the vehicle is assigned to a route, the
                                        fixed costs of the route will be increased by 10.45 €.
                                        The software reference provides a detailed description of the individual fields.


                                        Route Costs
                                        This area contains the total costs of the route. The route costs consist of vari-
                                        able and fixed costs. They cannot be changed manually.
                                        The software reference provides a detailed description of the individual fields.


                                        Additional information
                                         Software Reference, “Creating a New Route – Costs” on page J-180
                                         Software Reference, “Route Information” on page J-198
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                    J-81
                 Optimizing Routes                                                                       Tutorial




                                     Optimizing Routes
                                     This section deals with the optimization of the route.
                                     This includes the following training modules:
                                     •   “Optimizing Routes” on page J-84
                                     •   “Changing Routes” on page J-88
2.01 / 01-2017




                 J-82                                                            A+W Business Logistic Optimizer
                 Tutorial                                                                                 Optimizing Routes




                                        Overview
                                        Objectives

                                        • Getting to know and understanding route optimization


                                        Benefits

                                        • The more efficient the route is, the lower the costs are. Routes are optimally
                                          calculated and drivers are less burdened.


                                        Please note

                                        Optimized route              Sequence of the waypoints after optimization.

                                        Original Route               Sequence of the waypoints before optimization.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                           J-83
                 Optimizing Routes                                                                            Tutorial




                                     Optimizing Routes
                                     Once all waypoints have been localized, the next step in optimizing the route
                                     is performed. This means, OTR puts the individual waypoints in an optimum
                                     sequence based on the defined factors.




                                     Fig. J-31    Optimization of the route


                                     This dialog shows you the result of the optimization in a chart and in a table.
                                     The map with the route is located on the left side. The route width and opacity
                                     can be set in the parameters (parameter: Optimized_Route_Opacity,
                                     Optimized_Route_Width). At the right, you see the route as a list.
                                     The combo box in the upper right contains all routes that you have optimized.
                                     If you have optimized more than one route, you can select the respective route
                                     from the combo box.




                                     The two tabs beneath it (Optimized Route/Original Route) show you the order
                                     of the individual stations after optimization (Optimized Route tab) and before
                                     optimization (Original Route tab).




                                     The list below this provides a summary of the route in the upper area.
2.01 / 01-2017




                 J-84                                                            A+W Business Logistic Optimizer
                 Tutorial                                                                                 Optimizing Routes




                                        In the example above, the route consists of four stations, whereby the starting
                                        point of the route is always regarded as a station.
                                        With the help of the symbols next to it, you can show and hide the route in the
                                        map view. Possible settings are:

                                        Icon         Description

                                                     Traffic
                                                     This symbol indicates that traffic is turned on.

                                                     Show route
                                                     If this symbol is activated, the route is shown in the map view.

                                                     Hide route
                                                     If this symbol is activated, the route is hidden in the map view.


                                        The color symbol allows you to temporarily change the route color in the map
                                        view. Click the symbol twice to open the Color dialog. Here you can assign a
                                        different color to the route. The default value of the color is based on the pa-
                                        rameter settings (Optimized_Route_Color).
                                        The small white arrows in the route indicate the direction of the route.
                                        The route has a total distance of 152.13 km and the driving time amounts to 2
                                        hours and 2 minutes. The costs of the route are € 15.44. This value calculates
                                        the vehicle's fuel consumption, the fuel costs and the total distance.

                                           Costs of Route
                                           The costs of the route are calculated on the basis of the values that you
                                           have defined for the vehicles. The more accurate these values are, the
                                           more accurate the route costs will be. This primarily applies to fuel costs,
                                           which tend to fluctuate to a great extent.

                                        The neighboring field Toll tells you whether the route contains toll roads.




                                        The starting point is indicated by a green dot. You declared this waypoint as
                                        such during planning. You can neither move it nor change it. To make such
                                        changes, you have to go back to Planning.
                                        All of the following waypoints have a red dot. In addition, the following informa-
                                        tion icons are available:
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                         J-85
                 Optimizing Routes                                                                               Tutorial




                                     Icon         Description

                                                  Delivery
                                                  This icon shows you that goods are to be unloaded at this address.

                                                  Collection
                                                  This icon shows you that goods are to be collected (generally racks)
                                                  at this address.

                                                  On-time
                                                  This icon shows you that the address has a fixed time at which goods
                                                  can be unloaded or collected. This can be the case if the customer
                                                  has fixed times for goods acceptance or goods can only be unloaded
                                                  at a construction site at certain times.

                                                  Priority
                                                  This icon shows you that the address has a priority.


                                     Waypoints in the list can be shifted to another position by drag & drop. After a
                                     waypoint was shifted re-optimization is made automatically.
                                     Double-clicking a waypoint in the list opens a field with respective detailed in-
                                     formation in the map view. This field also appears if you double-click the way-
                                     point in the map view.




                                     Double-clicking a route section in the map view opens a field with respective
                                     route information, e.g. distance from A to B.
2.01 / 01-2017




                 J-86                                                               A+W Business Logistic Optimizer
                 Tutorial                                                                          Optimizing Routes




                                        Different Map Modes
                                        Here you can select from various map views.




                                        In the terrain view you can see topography and height. The satellite view pro-
                                        vides 2D images and the map view shows you the map.
                                        Next step:
                                         Result of the optimization, Page J-93


                                        Additional information
                                         Software Reference, “Optimize Route” on page J-193
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                J-87
                 Optimizing Routes                                                                          Tutorial




                                     Changing Routes
                                     This section shows you how you can change route criteria.
                                     The following instructions exist for this training module:
                                     •   “How to assign a priority to a waypoint” on page J-88
                                     •   “How to remove a priority from a way point” on page J-88
                                     •   “How to chang the sequence manually” on page J-88
                                     •   “How to stop an optimization” on page J-89
                                     •   “How to edit the route” on page J-89
                                     •   “How to change factors” on page J-90


                                      How to assign a priority to a waypoint
                                     1 Select the waypoint from the list.
                                     2 Click on the flag.
                                         The flag is shown in green and symbolizes that the address has priority.
                                         After new optimization, this waypoint is located at the uppermost position
                                         (priority).


                                      How to remove a priority from a way point
                                     1 Select the waypoint with the priority.
                                     2 Click on the flag.
                                         The flag is shown in gray and symbolizes that the address no longer has
                                         priority.
                                     3 After new optimization, this waypoint is located at any position in the se-
                                       quence.


                                      How to chang the sequence manually
                                     1 Select the waypoint from the list and keep the mouse key pressed.
                                     2 Drag the waypoint to the desired location within the list.
                                     3 Release the mouse key once you have reached the position at which you
                                       would like to drop the waypoint.
                                         The waypoint is now moved to this position

                                         Do not forget to perform a new optimization
                                         If you change the sequence of the waypoints manually, you have to perform
                                         a new optimization in order to update the values.
2.01 / 01-2017




                 J-88                                                             A+W Business Logistic Optimizer
                 Tutorial                                                                         Optimizing Routes




                                         How to stop an optimization
                                           If for whatever reason you need to stop an optimization, proceed as fol-
                                           lows.
                                        1 Press the [Stop Optimization] button.
                                           The optimization is stopped.
                                           The data from the previous optimization remain unchanged and are shown.


                                         How to edit the route
                                        1 Press the [Edit Route] button.
                                           The Route dialog opens for the selected route. In this tab you can change
                                           the delivery date, the starting time and the name of the route.




                                        2 In the Vehicles tab, you can change the vehicle and the driver.
                                        3 In the Parameter tab, you can change the Route Mode and the Optimiza-
                                          tion Factors.
                                        4 In the Costs tab, you can change the Toll Costs and the Extra Costs.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                 J-89
                 Optimizing Routes                                                                           Tutorial




                                      How to change factors
                                     1 Press the [Optimization Factors] button.
                                        The Optimization Factor dialog opens for the selected route.




                                     2 Now you can move individual factors back and forth.
                                        As the total always amounts to 100%,changes made to factors always af-
                                        fect the other factors.
                                     3 If you want to fix a value, press the [Lock] button.
                                        This locks the value and it can no longer be changed.
                                     4 To reset the factors to the default settings, press the [Default Values] but-
                                       ton.
                                        The values are then changed in line with the parameter settings.


                                     Additional information
                                      Software Reference, “Route Factors” on page J-178
2.01 / 01-2017




                 J-90                                                             A+W Business Logistic Optimizer
                 Tutorial                                                                         Check Results




                                        Check Results
                                        This section deals with the result of the optimization.
                                        This includes the following training modules:
                                        •   “The Result of the Optimization” on page J-93
                                        •   “Change Route Status” on page J-95
                                        •   “Real Route Costs” on page J-96
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                          J-91
                 Check Results                                                                                  Tutorial




                                 Overview
                                 Objectives

                                 •   Changing the route status
                                 •   Exporting data for a navigation system
                                 •   Printing delivery lists for your drivers
                                 •   Created subsequent real route costs


                                 Benefits

                                 • By entering real route costs, your estimated route costs become more accurate.
                                   This gives you a more solid foundation in planning in terms of costs.


                                 Definition

                                 Polylines                     Lines are portrayed on the map with the aid of polylines,
                                                               which represent a sorted sequence of locations.

                                 Locations                     Are objects on a card that are bound to longitude and
                                                               latitude coordinates.


                                 Please note

                                 White fields                  The white fields in the dialogs Route and Destination are
                                                               used to copy field content. No changes can be made to
                                                               the content.

                                 Real costs                    The real costs can only be determined once the driver
                                                               has returned from the route and has submitted the route
                                                               report.
2.01 / 01-2017




                 J-92                                                             A+W Business Logistic Optimizer
                 Tutorial                                                                                      Check Results




                                           The Result of the Optimization
                                           Once optimization has been run, the last step takes place - the presentation of
                                           the result.




                 Fig. J-32   Result of the optimization


                                           This dialog shows you the result of the optimization in detail. It consists of three
                                           sections:
                                           •   Routes
                                           •   Route Plan
                                           •   Destination

                                           Routes
                                           This area contains the current optimization of the routes.




                 Fig. J-33   Result of the optimization, Route area
2.01 / 01-2017




                                           The Route Status field show the status of the route. After optimization, the sta-
                                           tus is Roughly scheduled. Then the delivery date is shown.



                 A+W Business Logistic Optimizer                                                                         J-93
                 Check Results                                                                          Tutorial




                                 The Original Route field shows you the route number assigned by A+W Busi-
                                 ness. The Route ID shows you the route ID assigned by OTR. The field Name
                                 of the Route contains the name that you have assigned or selected in the Plan-
                                 ning. The Costs involve the costs for a liter of fuel and the field Consumption
                                 contains the fuel consumption of a vehicle for 100 km. The field Kilometers
                                 Driven shows you the entire route and the field Route Time how much time this
                                 route takes. The Route Costs are calculated on the basis of the route, vehicle
                                 fuel consumption as well as the fuel price. In the field Weight you see how
                                 heavy the load is, where returned racks are portrayed with a minus sign. The
                                 field Vehicles shows you which vehicles are used on the route and the field
                                 Truck Driver shows you the name of the driver.
                                 Double-clicking a route opens the Route dialog, which has been described in
                                 detail in a previous section.

                                 Route Plan




                                 Fig. J-34    Route plan


                                 This area shows you the route with its destinations.
                                 The [Zoom In/Zoom Out] button lets you zoom in and out of the view.

                                 Destination
                                 This area shows you the individual destinations.
                                 Double-clicking a destination opens the View Destination dialog, which has
                                 also been described in detail in a previous section.


                                 Additional information
                                  Tutorial, “Destinations” on page J-69
                                  Software Reference, “Edit Destination” on page J-184
2.01 / 01-2017




                 J-94                                                         A+W Business Logistic Optimizer
                 Tutorial                                                                               Check Results




                                        Change Route Status
                                        Once the optimization has been run, you can change the status of the route in
                                        this area.
                                        The following values are then available:
                                        •   Roughly scheduled: This is the status of the route after optimization.
                                        •   Detailed schedule: This status is not analyzed at present.
                                        •   Released: Once you have changed the status to released, the Delivery
                                            Date, the Sequence and the Route are returned to A+W Business. Addi-
                                            tionally, the data are loaded in the Cloud. You can only change the status
                                            to released once.
                                        Beside the route status, you can change the department and Edit the route.


                                         How to change the status of a route
                                        1 Select the route from the list.
                                        2 Use the mouse to click the [Edit Route] button.
                                            The Edit Route dialog opens.




                                        3 Choose the required status from the combo box Route Status.
                                        4 Exit the dialog by pressing [OK].


                                        Additional information
2.01 / 01-2017




                                         Software Reference, “Route Status” on page J-196




                 A+W Business Logistic Optimizer                                                                 J-95
                 Check Results                                                                          Tutorial




                                 Real Route Costs
                                 Only once your driver has returned from their route, are you able to ascertain
                                 how high the actual costs were. For instance, the planned free route might
                                 have been blocked and the driver may have had to revert to a section with a
                                 toll road. This could not have been foreseen at the time the route was planned.
                                 The real costs therefore differ from the planned costs of the route.
                                 In OTR you have the possibility to enter the real costs retroactively. They are
                                 then available for future route plans.


                                  How to enter the real costs
                                 1 Open the Query item in the menu bar.
                                 2 In the Route area, select the respective route.
                                 3 Use the mouse to click the [Edit Route] button.
                                    The Edit Route dialog opens.
                                 4 Switch to the tab Route Information.
                                    The Real Costs fields initially have the same values as the cost fields on
                                    the right side.




                                 5 Correct the Real Costs fields.
                                    You can overwrite the values or set them all to 0 beforehand with the button
                                    [Clear costs].
                                 6 When you are done with your entries, you see how much the route really
                                   cost in the field Real Route Costs.
2.01 / 01-2017




                                 Additional information
                                  Software Reference, “Route Information” on page J-198



                 J-96                                                        A+W Business Logistic Optimizer
                 Tutorial                                                                 Driving and Tracking Routes




                                        Driving and Tracking Routes
                                        This sections deals with the driver tasks on the route and the possibilities of
                                        the employee in the company regarding the tracking.
                                        This includes the following training modules:
                                        •   “Preparations” on page J-99
                                        •   “Driving Routes” on page J-101
                                        •   “Tracking Routes” on page J-109
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-97
                 Driving and Tracking Routes                                                                          Tutorial




                                         Overview
                                         Objectives

                                         •   Load documents in the Cloud.
                                         •   Getting to know and understanding the GDC app for the drivers.
                                         •   Getting to know and understanding booking via Browser.
                                         •   Getting to know and understanding the tracking function.


                                         Benefits

                                         • The tracking function always provides the employees in the company with
                                           information regarding the route. Many situations are promptly dealt with. E.g. a
                                           damaged lite can be reproduced while the truck is still on the route.


                                         Definition

                                         GDC app                     App for Android, to be downloaded in Google Playstore
                                                                     free of charge.


                                         Please note

                                         Android                     The GDC app available for Android in Googly Playstore.

                                         and others                  The users of non-Android systems can use the Browser
                                                                     for direct login.

                                         Update                      Don't forget to press the [Update] button in Route
                                                                     Administrator from time to time to synchronize the data.
2.01 / 01-2017




                 J-98                                                                    A+W Business Logistic Optimizer
                 Tutorial                                                                  Driving and Tracking Routes




                                        Preparations
                                        To make sure that both the App and the GPS tracking work correctly, the fol-
                                        lowing preliminary work is necessary:

                                        Respective Route Status
                                        To load the route data in the Cloud, it is necessary to set the route status to
                                        Released.
                                        Thus, mark the corresponding route in section Result, click on the Edit Route
                                        button and select the status Released from the combobox Route Status.
                                        For a detailed description on how to edit the route status, please see:
                                         “How to change the status of a route” on page J-95

                                           Route Status Released
                                           As soon as you change the route status to Released, it is not possible to
                                           transfer these orders again from A+W Business to OTR. If this should be
                                           necessary, you have to copy the number manager first to get new order
                                           numbers. Make sure that the new order status is in the correct status range
                                           (generally 01 to 800).

                                        Loading Documents in the Cloud
                                        To provide documents for the driver in digital form, they have to be loaded in
                                        the Cloud, too.




                                        To do so, proceed as follows:
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-99
                 Driving and Tracking Routes                                                                         Tutorial




                                          How to load documents in the Cloud and reference them
                                         1 Open the Query menu.
                                         2 Click on the[Attach Files] button. The dialog with the same name opens.
                                         3 Field Route ID contains the route selected before. Use fields Customer and
                                           Order to enter information for the driver.
                                         4 The Destination area, shows the destinations that are driven to on the
                                           route. Choose the destination for which the document shall be entered.
                                               •   Click on [Plus] icon button. The Attach Files dialog opens.
                                               •   Field File Name allows to enter a name, e.g. Delivery Note.
                                               •   Field File Path allows to enter the corresponding path for the Cloud, e.g.
                                                   https://drive.google.com/file/d/....
                                               •   Use field Description for further information.
                                               •   Exit the dialog by pressing [OK].
                                               •   Section Files contains all corresponding documents.

                                         Install App or use Browser
                                         Booking of data can be based on two different types:
                                         •     Via app (for Android devices)
                                         •     Via Browser (for non-Android devices)


                                          How to install the App (Android)
                                         1 Open Google Play Store.
                                         2 Load the Android app GDC: Goods Delivery Control.
                                         3 Install the app.


                                          How to work with a Browser (non-Android device)
                                         1 Start the Browser (Safari).
                                         2 Enter the URL. You find the respective address in OTR in Start > About
                                           A+W Logistics Optimizer, section GDC Web App. In our example: http://
                                           gdcapp.onerbox.com
2.01 / 01-2017




                 J-100                                                                   A+W Business Logistic Optimizer
                 Tutorial                                                                  Driving and Tracking Routes




                                        Driving Routes
                                        This section contains the information for the driver.
                                        •   Enter Password
                                        •   Operation of App or Browser
                                        •   Booking Data

                                        Enter Password
                                        On the first login with ID (via app or Browser), the driver is asked to enter the
                                        following.




                                        1 Enter the corresponding ID from the license information (Start > About
                                          A+W Logistics Optimizer, button [License Information], field CompanyId).
                                        2 Enter the Driver ID (Administration > Driver, field Driver ID) in field User.
                                        3 Enter the password in field Password.
                                        4 In field Repeat Password you have to enter the password again.
                                        5 Click on [Login], to register.

                                            Forgot password
                                            In case you forgot the password, it can be reset in the Driver dialog, check-
                                            box Reset Password.
2.01 / 01-2017




                                        Additional information
                                         Software Reference, “Driver” on page J-151




                 A+W Business Logistic Optimizer                                                                  J-101
                 Driving and Tracking Routes                                                                       Tutorial




                                         Operation of App or Browser
                                         After the driver logged in routes are shown that are assigned to the driver ID.
                                         A click on the route opens the overview with three tabs.
                                         •     Destinations
                                         •     Information
                                         •     Map

                                         Destinations Tab
                                         Tab Destinations contains all destinations that are driven to on the route.




                                         Press the [Start] icon and you will be asked whether you location shall be
                                         transferred vie GPS. In order to transfer the position coordinates of the book-
                                         ing back and to access these data from the company, please confirm.
                                         After confirmation the first entry (start point, example above: A+W) is set to Ac-
                                         cepted.
2.01 / 01-2017




                 J-102                                                                A+W Business Logistic Optimizer
                 Tutorial                                                                Driving and Tracking Routes




                                        Booking Data
                                        Arriving at the first destination (example above Becker Glasbau) the driver
                                        clicks it in the list and the following window opens:




                                        Use the combobox Status to assign the respective status. The options are:
                                        •   Accepted
                                        •   Partially accepted
                                        •   Rejected
                                        •   Rejected (breakage)
                                        •   In route
                                        Select the corresponding status.
                                        Use section Comment to enter information. You can enter e.g. a broken lite.
                                        Since the data are reported to the Cloud, the company can access these data,
                                        too. Thus, breakage can be reproduced immediately.
                                        The section Documents shows the order numbers. Depending on the status,
                                        you can select or deselect them. Example: If you select status Accepted, all
                                        documents are automatically selected. If you select status Paritally accepted,
                                        single documents can be choosen. Then, you can select just the documents,
                                        for which the delivery was accepted.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                J-103
                 Driving and Tracking Routes                                                                    Tutorial




                                         Section Company
                                         A click in the section Company opens a new window. The employee who ac-
                                         cepted the delivery can sign in the yellow area.




                                         Click on [Accepted], the window is closed and the signature is displayed at the
                                         right side of the screen.




                                         Now, the word Yes is shown below the entry Company. This means a signature
                                         exists. If the signature is wrong or must be repeated, click on the trash icon,
                                         top right. The signature is deleted and can be repeated.
2.01 / 01-2017




                 J-104                                                               A+W Business Logistic Optimizer
                 Tutorial                                                                 Driving and Tracking Routes




                                        Section Packaging
                                        In section Packaging click on [Add], the Packaging window opens.




                                        Enter the respective ID below the Barcode entry. In field Action you can
                                        choose whether the packaging is a delivery or a collection. Use section Com-
                                        ment for further information regarding the packaging type.
                                        Click on [Add], a new window opens:




                                        Enter the batch, the order number, and the line item. Click on [Add] to save the
                                        data and you are back in window Packaging.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                 J-105
                 Driving and Tracking Routes                                                                   Tutorial




                                         Click on [Save] to close the window.




                                         Booked Destinations
                                         Depending on the status, the overview shows the destinations in different col-
                                         ors. Accepted deliveries are marked in green. Partially accepted or rejected
                                         deliveries are marked in yellow.
2.01 / 01-2017




                 J-106                                                              A+W Business Logistic Optimizer
                 Tutorial                                                                Driving and Tracking Routes




                                        Information Tab
                                        This tab contains information regarding the route.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                              J-107
                 Driving and Tracking Routes                                                               Tutorial




                                         Map Tab
                                         This tab shows the map with the routes to be driven.
2.01 / 01-2017




                 J-108                                                             A+W Business Logistic Optimizer
                 Tutorial                                                                 Driving and Tracking Routes




                                        Tracking Routes
                                        The Route administrator provides a permanent online tracking of the vehicles
                                        and the drivers. Every time the driver books via App or Safari, the data is up-
                                        dated via cloud.

                                        Example for a partially accepted delivery
                                        In the App:




                                        In OTR:
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                J-109
                 Driving and Tracking Routes                                                                    Tutorial




                                         Destinations Tab
                                         The different colors show the current status. Destinations in gree color were
                                         completely delivered. Destinations in yellow color were either partly delivered
                                         or rejected.
                                         Double clicking the destination to the right of the map, shows this on the map
                                         together with a box that contains all relevant information.

                                         Tab Logbook
                                         Tab Logbook shows an overview of the route in table form.




                                         Field Date shows the date of the route and field Route the number. Field Cus-
                                         tomer shows the customer number and field Name the corresponding name.
                                         Field Status shows the status of the respective destination. The field remains
                                         on Initiate until the driver selects and books the correponding status via App
                                         or Safari. Then, the data is copied via Cloud. Possible values are:
                                         •     Accepted
                                         •     Partially accepted
                                         •     Rejected
                                         •     Rejected (breakage)
                                         •     In route
                                         Field Comment shows the information defined by the driver. Field User shows
                                         the name of the driver.
                                         If you click on a destination, a point appears at the place where the driver
                                         made the booking. This way, you are always informed about the real booking
                                         place.
2.01 / 01-2017




                 J-110                                                               A+W Business Logistic Optimizer
                 Tutorial                                                                  Driving and Tracking Routes




                                        Documents Tab
                                        Tab Documents gives an overview on the orders of the respective customer
                                        (destination) in table form.




                                        Field Order No. contains the order number. Field Customer shows the custom-
                                        er number and field Name the respective customer name. Field Status shows
                                        the order status. The field remains on Initiate until the driver selects and books
                                        the correponding status via App or Safari. Field Delivery Weight shows the
                                        weight of the order in kg. The weight of collected racks is shown in field Col-
                                        lected Weight.

                                           Update Display
                                           Don't forget to press the [Update] button from time to time to synchronize
                                           the data.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-111
                 Queries                                                                      Tutorial




                           Queries
                           This section deals with the query tools.
                           This includes the following training modules:
                           •   “Routes” on page J-114
                           •   “Reports” on page J-120
                           •   “View” on page J-125
2.01 / 01-2017




                 J-112                                                A+W Business Logistic Optimizer
                 Tutorial                                                                                                Queries




                                        Overview
                                        Objectives

                                        • Knowing and understanding the different queries.
                                        • Getting to know and understanding statistics.
                                        • Getting to know and understanding the calendar.


                                        Benefits

                                        • The statistic function is a flexible and powerful control and analysis tool.


                                        Please note

                                        ITN format                   Export format, e.g. for TomTom navigation systems

                                        GPX format                   Export format, e.g. for Garmin navigation systems
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                          J-113
                 Queries                                                                          Tutorial




                           Different Queries
                           Use this section to query all relevant information depending on the route sta-
                           tus. The tab is divided into the following groups:.
                           •   Routes
                           •   Reports
                           •   View
                           •   Update


                           Routes
                           This area contains information that are connected to routes. You will find the
                           following entries:
                           •   Filter
                           •   Change
                           •   Clear
                           •   Export
                           •   Status
                           •   History

                           Filter
                           You can filter the routes by date, route ID, route name, etc.




                           Fig. J-35     Filter routes
2.01 / 01-2017




                 J-114                                                 A+W Business Logistic Optimizer
                 Tutorial                                                                                          Queries




                                         How to Filter
                                        1 If you want to filter display by a certain period, enable the checkbox Date
                                          and enter the requested date in the fields from to.
                                        2 If you want to filter display by a certain route, enter the corresponding route
                                          ID in field Route ID.
                                        3 If you want to filter display by a certain route name, enter the corresponding
                                          name in field Route Name.
                                        4 If you want to filter display by a certain status, select the corresponding sta-
                                          tus from the combobox Route Status.
                                        5 If you want to filter display by a certain driver, select the corresponding driv-
                                          er from the combo box in field Driver ID.
                                        6 If you want to filter display by a certain department, select the correspond-
                                          ing department from the combo box in field Department.
                                        7 Use field Customer to filter by a customer.

                                        Change and Status
                                        Depending on the route status, you can change this or modify the real values
                                        (real distance and real costs) of the route.
                                        The fields of this dialog are identical with the fields of dialog Route Information.
                                         Software Reference, “Route Information” on page J-198
                                         Tutorial, “Change Route Status” on page J-95

                                        Clear
                                        Use this entry to delete selected routes. There will be a security query. The
                                        route will be deleted if you confirm this by [Yes].
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                     J-115
                 Queries                                                                            Tutorial




                           Export
                           The system contains the following export functions:
                           •   Export to navigation systems
                           •   Load data to mobile devices (via cloud)

                           Export to Navigation Systems
                           With this function you can export the route to a navigation system.
                           The data can be exported in the following file formats:
                           •   ITN format (e.g. TomTom)
                           •   GPX format (e.g. Garmin)
                           Please refer to the instruction manual of your navigation system for further in-
                           formation on the file format your device works with.

                           Locations
                           When exporting you have the possibility to choose whether individual loca-
                           tions are to be exported or not.
                           The differences are shown in the following example. A route is exported with
                           three destinations.
                           If locations are not exported, the folder in the Explorer looks like this:




                           If the file is opened in an editor, the content looks like this:




                           Only the coordinates of the individual waypoints are listed, however they direc-
                           tions on how to get there are not.
                           If locations are exported, the folder in the Explorer looks like this:
2.01 / 01-2017




                 J-116                                                    A+W Business Logistic Optimizer
                 Tutorial                                                                                          Queries




                                        If one of the files is opened in an editor, the content looks like this:




                                        The values mark the coordinates.
                                        In the example above, the longitudinal coordinates of the address are 7.82888
                                        and latitudinal coordinates are 50,43582. Then the individual markings follow
                                        up to the target address at longitude 6,95058 and latitude 50,92786.


                                         How to export data
                                        1 Click the [Export] button.
                                           This opens the Export dialog.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                    J-117
                 Queries                                                                          Tutorial




                           2 Depending on the navigation system you have, enable the radio button ITN
                             (e.g. for TomTom) or GPX (e.g. for Garmin).
                           3 Enable the checkbox Insert location, when the individual locations are to be
                             exported.
                           4 Enable the checkbox Create new folder for this route if a new folder is to be
                             created for each route to be exported.
                           5 In the Export path field specify whether the file is to be saved.

                              Standard Path for Export Files
                              You define the standard path for exporting data in the parameters (Param-
                              eter: Path_Export_ITN_GPS_File).


                           Additional information
                            Software Reference, “Export” on page J-202
2.01 / 01-2017




                 J-118                                                 A+W Business Logistic Optimizer
                 Tutorial                                                                                Queries




                                        History
                                        The history provides information on who made changes to the documents and
                                        when.
                                        In the history, you can filter by the following criteria:
                                        •   Route ID
                                        •   Order number
                                        •   Customer


                                         How to create a history for an order number
                                        1 Open the Query item in the menu bar.
                                        2 Use the mouse to click the [History] button.
                                            The History dialog opens.




                                        3 Enter the order number in field Document.
                                        4 Use the mouse to click the [OK] button.
                                            This data is displayed.


                                        Additional information
                                         Software Reference, “Filter Routes” on page J-201
                                         Software Reference, “Route Information” on page J-198
                                         Software Reference, “Export” on page J-202
                                         Software Reference, “History” on page J-204
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                           J-119
                 Queries                                                                               Tutorial




                           Reports
                           This section contains all queries related to reports and statistics. You will find
                           the following entries:
                           •   Selected Route
                           •   Report Launcher
                           •   Statistics

                           Selected Route
                           You can open the confirmation and delivery lists with the button either for one
                           or for all optimization routes.




                           Fig. J-36     Confirmation and delivery list


                           You can print the list and give it to the driver. The list contains all relevant in-
                           formation for the route.
2.01 / 01-2017




                           Additional information
                            Software Reference, “Confirmation and Delivery List” on page J-206



                 J-120                                                    A+W Business Logistic Optimizer
                 Tutorial                                                                                        Queries




                                        Print Lists
                                        This session shows you how to print lists.


                                         How to print the list for a certain route of the optimization
                                        1 In the Route area, select the route for which the list is to be printed.
                                        2 Use the mouse to click the [Selected Route] button. This opens the list.




                                        3 Using the tree structure on the left side, you can view and print a list of the
                                          individual destinations.


                                        Additional information
                                         Software Reference, “Confirmation and Delivery List” on page J-206

                                        Report Launcher
                                        Use the Report Launcher entry to open the dialog of that name. It contains all
                                        reports, defined in the systems. Select the desired report format and click on
                                        [Print Report]. The respective Crystal Report opens.

                                        Statistics
2.01 / 01-2017




                                        With the Statistics entry you have access to powerful statistics covering the en-
                                        tire OTR field. Click the entry, the Statistics dialog opens.



                 A+W Business Logistic Optimizer                                                                     J-121
                 Queries                                                                               Tutorial




                           •   General
                           •   General graphic
                           •   Vehicles
                           •   Driver
                           •   Departments
                           •   Customers

                           General Tab
                           This area contains information on routes. The real costs are compared with the
                           planned costs. In addition, the deviation is shown in currency as well as in per-
                           cent.




                           Fig. J-37     Statistics, Tab general


                           The dialog is divided into two sections. The left side contains the filter functions
                           that are the basis for the results on the right side.
2.01 / 01-2017




                 J-122                                                    A+W Business Logistic Optimizer
                 Tutorial                                                                                         Queries




                                        Fig. J-38    Filter function


                                        After activating the checkbox Date, you can enter the date in the fields below
                                        from and ton, the values are to be displayed for.
                                        Choose the required status from the checkbox Route Status. By pressing the
                                        icon buttons below you can enable or disable all.
                                        Choose the required status from the combo box Route Status. Via combo box
                                        Department you can filter by a certain department. Use combo box Vehicles to
                                        filter routes by the vehicles the route was driven with. The combo box Driver
                                        ID filters certain drivers and in field Route Name you can enter the name of a
                                        route to be filtered.
                                        In addition, you can select a customer number from the combo box in the Cus-
                                        tomer section.
                                        The fields and combo boxes mentioned above can be combined freely. If noth-
                                        ing is selected or entered, all available data is displayed.

                                        Create a Statistic
                                        This session shows you how to create statistics.
                                        The following instructions exist for this training module:
2.01 / 01-2017




                                        •   “How to create statistics for a customer” on page J-124
                                        •   “How to create statistics for a vehicle” on page J-124
                                        •   “How to create statistics for a driver and a vehicle” on page J-124

                 A+W Business Logistic Optimizer                                                                   J-123
                 Queries                                                                          Tutorial




                            How to create statistics for a customer
                              You would like to know the route costs for a customer in a certain period.
                           1 Activate the checkbox Date and choose the requested date from the fields
                             below, e.g. 01.07.2015 to 31.08.2015.
                           2 Enter the customer number in section Customer or select the customer
                             from the list via Customer button.
                           3 Choose the required status from the combo box Route Status, e.g. Com-
                             pleted.
                           4 Enter the customer number in the section Customer from to.
                           5 Click [OK]. The data on the right side is updated.
                           6 Tab Customer shows the data in graphic form.


                            How to create statistics for a vehicle
                              You would like to know the route costs for a vehicle.
                           1 Select the required vehicle from the Vehicles combo box.
                           2 Click [OK]. The data on the right side is updated.
                           3 Tab Vehicles shows the data in graphic form.


                            How to create statistics for a driver and a vehicle
                              You would like to know the route costs for a driver and a certain vehicle.
                           1 Select the required driver from the Drivers combo box.
                           2 Select the required vehicle from the Vehicles combo box.
                           3 Click [OK]. The data on the right side is updated.
                           4 Tabs Vehicles and Drivers shows the data in graphic form.


                           Additional information
                            Software Reference, “Statistics” on page J-210
2.01 / 01-2017




                 J-124                                                  A+W Business Logistic Optimizer
                 Tutorial                                                                                          Queries




                                        View
                                        This section contains all view. You will find the following entries:
                                        •   Route
                                        •   Destination
                                        •   Calendar

                                        Route
                                        This dialog shows general information, vehicles, parameters, and the costs for
                                        the selected route.
                                        The fields of this dialog are identical with the fields of dialog Route.
                                         Software Reference, “Creating a New Route – General” on page J-165
                                         Software Reference, “Creating a New Route - Vehicle” on page J-169
                                         Software Reference, “Creating a New Route – Parameters” on page J-174
                                         Software Reference, “Creating a New Route – Costs” on page J-180

                                        Destination
                                        This dialog shows general information on the destinations of the selected
                                        route.
                                        The fields of this dialog are identical with the fields of dialog Destinations.
                                         Software Reference, “Edit Destination” on page J-184

                                        Calendar
                                        The calendar provides an overview of the routes to be driven and routes that
                                        have been driven.
2.01 / 01-2017




                                        Fig. J-39    Calendar




                 A+W Business Logistic Optimizer                                                                    J-125
                 Queries                                                                           Tutorial




                           The calendar is divided into two types:
                           •   Vehicles
                           •   Driver
                           The entries of the lower section change, after changing the calendar type in
                           the upper section. If you selected the calendar type Vehicles, the lower sec-
                           tions shows the vehicles. If you selected the type Drivers, the drivers are dis-
                           played.
                           Use the icons Month and Day to switch between the periods to be displayed.
                           Double-clicking a day in the monthly view opens the respective view. The left
                           side shows a timeline in half hour intervals. The header depends on the select-
                           ed calendar type.




                           Fig. J-40      Calendar in day layout


                           Double-clicking an entry on this level opens the Query dialog. It shows an
                           overview in table form of the routes including all destinations.
                           Red entries always signal an overlapping. Either in connection with the driver
                           or the vehicle. Double-clicking an entry opens the Edit Route dialog. It serves
                           to assign a different driver or a different vehicle easily and quickly.
                           Use the combo box Route Status to limit the contents. You can display the
                           routes depending on their status.
2.01 / 01-2017




                 J-126                                                 A+W Business Logistic Optimizer
Logistic Optimizer                  J

                     Software Reference




                      A+W Business
                 Software Reference                                                                           Configuration




                                        Configuration
                                        Configuration menu
                                        All data required to work properly is configured and administered in this area.
                                        The area contains:
                                        •   Database settings:
                                            Here you can make settings for the database connections (OTR and ERP).
                                             “OTR Connection” on page J-130
                                        •   Parameters:
                                            This area is for general settings such as consideration of traffic, priority fac-
                                            tors, time factors, etc.
                                             “Parameters” on page J-132
                                        •   Language:
                                            Use this combobox to change the language during operation. Presently,
                                            the program is available in the following languages:
                                            – Spanish
                                            – English (US)
                                            – German
                                            – Portuguese
                                            – Catalan

                                            Dialog buttons
                                            The standard buttons and menus are described in detail in the section
                                            Overview and in the tutorials. We are therefore not going to describe them
                                            in connection with the dialogs.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                      J-129
                 Configuration                                                            Software Reference




                                 OTR Connection
                                 Configuration > Settings




                                 Fig. J-41    OTR connection


                                 The dialog is divided into two tabs:
                                 •   OTR Connection
                                 •   ERP Connection
                                 This tab applies to the settings for the OTR database server.

                                 Description of fields

                                 Data Source Here you enter the path to the OTR database.

                                 Initial Catalog In this field you enter the standard database. This is OTR.

                                 User ID Enter the user ID in this field.

                                 Password Enter the password in this field.

                                 Test With this symbol you can test the connection to the OTR database.

                                     Database Connection
                                     Please note that these settings have to be made for each user.


                                 Additional information
                                  Tutorial, “Database Connections” on page J-15
2.01 / 01-2017




                 J-130                                                       A+W Business Logistic Optimizer
                 Software Reference                                                                     Configuration




                                        ERP Connection
                                        Configuration > Database Configuration > ERP Connection tab




                                        Fig. J-42    ERP connection


                                        This tab applies to the settings for the ERP database server.

                                        Use SQL ERP Connection Use this checkbox to control whether a connec-
                                        tion to the A+W Business database exists or not.
                                         OTR is not connected to A+W Business database.
                                         OTR uses the following settings to connect to A+W Business database.

                                        Data Source Here you enter the path to the A+W Business database.

                                        Initial Catalog In this field you enter the A+W Business standard database.

                                        User ID Enter the user ID here.

                                        Password Enter the password in this field.

                                        Test With this symbol you can test the connection to the A+W Business data-
                                        base.

                                           Database Connection
                                           Please note that these settings have to be made for each user.


                                        Additional information
                                         Tutorial, “Database Connections” on page J-15
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                              J-131
                 Configuration                                                              Software Reference




                                 Parameters
                                 Configuration > Parameters




                                 Fig. J-43    Parameters


                                 Here you find all parameters including their description and their specific set-
                                 ting.

                                 Description of the Parameters

                                 Delivery_Date/Route_Origin This entry is used to define how the routes are
                                 formed. Possible values are:
                                 • Yes: So-called mulit-routes are created. Multi-routes means that the origi-
                                    nal routes from the A+W Business remain.
                                 • No: No multi-routes are created. One single route is created on the basis
                                    of the delivery datet
                                 Technical information: Parameter name: Mulit-routes

                                 Delivery Date This field only applies if the entry for the field Delivery_Date/
                                 Route_Origin has been enabled with YES. Possible values are:
                                 • Yes: The route is created on the basis of the original route.
                                 • No: The route is created on the basis of the delivery date.
2.01 / 01-2017




                                 Technical information: Parameter name: Delivery_Date




                 J-132                                                       A+W Business Logistic Optimizer
                 Software Reference                                                                        Configuration




                                        Generate one Route for each Origin Route This field is used to define
                                        whether an own route is to be generated for each route from the A+W Busi-
                                        ness. Possible values are:
                                        • Yes: A route for each origin route of the A+W Business is created.
                                        • No: One route for each delivery date will be created.
                                        Technical information: Parameter name: Route_Origin

                                        Dynamic vehicle Assignment This field is used to define whether vehicles
                                        are assigned dynamically for each route. Possible values are:
                                        • Yes: The vehicle will be assigned dynamically for each route.
                                        • No. The vehicles will be permanently assigned to the routes.
                                        Technical information: Parameter name: Dynamic_Vehicle_Assignment

                                        Trucks not Allowed This field is used to define whether roads are permitted
                                        for routes that do not allow trucks. Possible values are:
                                        • Yes: Even those roads can be used that are not permitted for trucks.
                                        • No: Only those roads can be used that are permitted for trucks.
                                        Technical information: Parameter name: Allow_Routes_Without_Trucks

                                        Toll Mode This field is used to define whether toll roads are permitted for the
                                        route. Possible values are:
                                        • Always avoid toll roads: Optimization ensures that route sections that con-
                                           tain toll roads are entirely avoided (completely excluded). If the condition
                                           cannot be met, no route is created.
                                        • Avoid toll roads partially: Optimization does not include route sections that
                                           contain toll roads. If this restriction prevents the system from defining a
                                           route, the condition is relaxed.
                                        • Penalty for toll roads: Optimization penalizes the use of toll roads.
                                        • Normal: Optimization retains the sequence of the route sections that con-
                                           tain toll roads.
                                        • Preferred: Optimization prefers connections that contain toll roads.
                                        Technical information: Parameter name: Nokia_Avoid_Tolls

                                        Train Mode This field is used to define whether trains are permitted on the
                                        route. Possible values are:
                                        • Always avoid trains: Optimization ensures that route sections that contain
                                           trains are entirely avoided (completely excluded). If the condition cannot be
                                           met, no route is created.
                                        • Avoid trans partially: Optimization does not include route sections that con-
                                           tain trains. If this restriction prevents the system from defining a route, the
                                           condition is relaxed.
                                        • Penalty for trains: Optimization penalizes the use of connections with
                                           trains.
                                        • Normal: Optimization retains the sequence of the connections that contain
                                           trains.
2.01 / 01-2017




                                        • Preferred: Optimization prefers connections that contain trains.
                                        Technical information: Parameter name: Nokia_Avoid_Trains



                 A+W Business Logistic Optimizer                                                                   J-133
                 Configuration                                                               Software Reference




                                 Ferry Mode This field is used to define whether ferries are permitted on the
                                 route.
                                 • Always avoid ferries: Optimization ensures that route sections that contain
                                    ferries are entirely avoided (completely excluded).
                                 • Avoid ferries partially: Optimization does not include route sections that
                                    contain ferries. If this resriction prevents the system from defining a route,
                                    the condition is relaxed.
                                 • Penalty for ferries: Optimization penalizes the use of connections with fer-
                                    ries.
                                 • Normal: Optimization retains the sequence of the connections that contain
                                    ferries.
                                 • Preferred: Optimization prefers connections that contain ferries.
                                 Technical information: Parameter name: Nokia_Avoid_Ferrys

                                 Highway Mode This field is used to define whether highways are permitted
                                 on the route. Possible values are:
                                 • Always avoid highways: Optimization ensures that route sections that con-
                                    tain highways are entirely avoided (completely excluded). For instance, this
                                    is the case with HOV lanes in the USA and Canada. If the condition cannot
                                    be met, no route is created.
                                 • Avoid highways partially: Optimization does not include route sections that
                                    contain highways. If this restriction prevents the system from defining a
                                    route, the condition is relaxed. If this restriction prevents the system from
                                    defining a route, the condition is relaxed.
                                 • Penalty for highways: Optimization penalizes the use of highways.
                                 • Normal: Optimization retains the sequence of the connections that contain
                                    highways.
                                 • Preferred: Optimization prefers connections that contain highways.
                                 Technical information: Parameter name: Nokia_Avoid_Motorways
2.01 / 01-2017




                 J-134                                                        A+W Business Logistic Optimizer
                 Software Reference                                                                        Configuration




                                        Tunnel Mode This field is used to define whether roads with tunnels are per-
                                        mitted on the route. Possible values are:
                                        • Always avoid tunnels: Optimization ensures that route sections that contain
                                           tunnels are entirely avoided (completely excluded). If the condition cannot
                                           be met, no route is created.
                                        • Avoid tunnels partially: Optimization does not include route sections that
                                           contain tunnels. If this restriction prevents the system from defining a route,
                                           the condition is relaxed.
                                        • Penalty for highways: Optimization penalizes the use of connections with
                                           tunnels.
                                        • Normal: Optimization retains the sequence of the connections that contain
                                           highways.
                                        • Preferred: Optimization prefers connections that contain highways.
                                        Technical information: Parameter name: Nokia_Avoid_Tunnels

                                        Vehicle Type Here you can set the vehicle type. Possible values are:
                                        • Truck
                                        • Automobile
                                        Technical information: Parameter name: Nokia_Vehicles

                                        Route Type Here you can define the desired mode of the route. Possible val-
                                        ues are:
                                        • Fastest: This setting determines the fastest connection between departure
                                           and arrival point. Optimization is based on the driving time.
                                        • Shortest: This setting determines the shortest connection between depar-
                                           ture and arrival point. Optimization is based on the distance.
                                        • Economic: This setting determines the most economic route. Optimization
                                           is based on fuel consumption.
                                        Technical information: Parameter name: Nokia_Mode

                                        Costs Average price per liter fuel. This is used if no vehicle has been select-
                                        ed.
                                        Technical information: Parameter name: Average_Cost_Fuel

                                        Average Fuel Consumption Average fuel consumption in liters for 100 km.
                                        This is used if no vehicle has been selected.
                                        Technical information: Parameter name: Average_Consumption_Fuel

                                        Distance Factor The distance factor is based on the length of the route. It
                                        searches for the shortest distances.
                                        Technical information: Parameter name: Ga_Distance_Proportion
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-135
                 Configuration                                                                  Software Reference




                                 Weight Factor This factor assesses the relationship of weight and the dis-
                                 tance of the route. It multiplies the weight of the load with the distance of each
                                 point of the route and takes unloading and collection processes at each point
                                 into consideration.
                                 Technical information: Parameter name: Ga_Weight_Proportion

                                 On-Time Factor This factor counts the number of destinations to be reached
                                 within the delivery/pickup time defined. It searches for the route with the larg-
                                 est number of on-time delivery destinations.
                                 Technical information: Parameter name: Ga_OnTime_Proportion

                                 Priority Factor This factor evaluates the route according to the number of
                                 destinations marked as priority that make up the first destinations on the route.
                                 It searches for routes with a larger number of priority destinations as the first
                                 stops.
                                 Technical information: Parameter name: Ga_Priority_Proportion

                                 Time factor This factor is based on the length of the route. It searches for the
                                 fastest route.
                                 Technical information: Parameter name: Ga_Time_Proportion

                                 General route With this parameter you define the name of the routes, manu-
                                 ally created in OTR.
                                 Technical information: Parameter name: Default_Route_Name

                                 Initial Department This parameter defines the entry the field Department will
                                 be filled with. The value can be changed in the corresponding dialogs.
                                 Technical information: Parameter name: Initial_Department

                                 License WebService This field contains the WebService address.
                                 Technical information: Parameter name: Ort_License_Web_Service

                                 Start Time of Route This parameter defines the start time of routes. The re-
                                 spective fields will be filled later on in the dialogs with this entry. The value can
                                 be changed.
                                 Technical information: Parameter name: Default_Route_Init_Time

                                 Duration of Route This parameter defines the maximum duration of the
                                 routes, e.g. 8 hours. The respective fields will be filled later on in the dialogs.
                                 The value can be changed. Please consider statutory regulations of the indi-
                                 vidual countries.
                                 Technical information: Parameter name: Initial_Max_Route_Time
2.01 / 01-2017




                 J-136                                                          A+W Business Logistic Optimizer
                 Software Reference                                                                         Configuration




                                        Use Default Initial Address In this field you enter the name of the company
                                        at which the route is to start, e.g. A+W Software GmbH. Possible values are:
                                        • Yes: The default address is used as starting point for the route.
                                        • No: The default address is not used as starting point for the route.
                                        Technical information: Parameter name: Use_Initial_Point

                                        Start Company Name In this field you enter the name of the company at
                                        which the route is to start, e.g. A+W Software GmbH.
                                        Technical information: Parameter name: Initial_Companyname

                                        Initial Address In this field, you enter the initial address for the routes, e.g.
                                        Konrad-Adenauer-Str. 15, 35440 Linden.
                                        Technical information: Parameter name: Initial_Address

                                        Time On-Site With this parameter you define the time in minutes on-site to
                                        load or unload, e.g. 12 minutes. The respective fields will be filled later on in
                                        the dialogs. The value can be changed.
                                        Technical information: Parameter name: Default_Visiting_Time

                                        Show Original Route With this entry you define whether the original routes
                                        are also shown. Possible values are:
                                        • Yes: The original route is shown in addition to the optimized route.
                                        • No: The original route is not shown.
                                        Technical information: Parameter name: Show_Original_Route

                                        Show Optimized Route with Straight Lines With this entry, you define
                                        whether the route is only shown with a straight line. Possible values are:
                                        • Yes: The individual waypoints are connected by a straight line
                                        • No: The route is portrayed along the road
                                        Technical information: Parameter name: Straight_Optimized_Routes

                                        Opacity of Optimized Route (Map) Here you enter the value for the opacity
                                        of the optimized route, e.g. 0.5.
                                        Technical information: Parameter name: Optimized_Route_Opacity

                                        Optimized Route Width Here you can enter the width of the optimized route
                                        in the map, e.g. 10 = 10 Pixel.
                                        Technical information: Parameter name: Optimized_Route_Width

                                        Opacity of the Original Route (Map) Here you enter the value for the opac-
                                        ity of the original route, e.g. 0.5.
                                        Technical information: Parameter name: Original_Route_Opacity

                                        Original Route Width Here you can enter the width of the original route in the
2.01 / 01-2017




                                        map, e.g. 10 = 10 Pixel.
                                        Technical information: Parameter name: Show_Route_Width



                 A+W Business Logistic Optimizer                                                                   J-137
                 Configuration                                                           Software Reference




                                 Optimized Route Color in Map Here you enter the color value for the opti-
                                 mized route, e.g. #0000FF. The fields Color of optimized route and Original
                                 route color should clearly differ. This is how a differentiation is made.
                                 Technical information: Parameter name: Optimized_Route_Color

                                 Original Route Color in Map Here you enter the color value for the original
                                 route, e.g. #585858.
                                 Technical information: Parameter name: Original_Route_Color

                                 More than One Route With this entry, you can define whether the WebServ-
                                 er calculates several routes. Possible values are:
                                 • Yes: The WebServer calculates several routes
                                 • No: The WebServer calculates just one route
                                 Technical information: Parameter name: Alternatives

                                 Unit System for Distances Here you define the length unit with which the
                                 module should work. Possible values are:
                                 • Metric: Kilometers and meters
                                 • Imperial: Miles and feet
                                 Technical information: Parameter name: Units

                                 Country-Code Here you can enter the ISO country code for the country in
                                 which the OTR is installed. Possible values are:
                                 • de: Germany
                                 • es: Spain
                                 • uk: England
                                 • fr: France
                                 • us: USA
                                 • it: Italy
                                 • sv: Sweden
                                 • pl: Poland
                                 • mx: Mexico
                                 Technical information: Parameter name: Region

                                 Uppercase Letters Here you can define whether the contents of the fields
                                 are to be displayed in uppercase letters. Possible values:
                                 • Yes: The content is displayed in only uppercase letters (e.g.: ROUTE
                                    NORTH)
                                 • No: The content is not displayed in only uppercase letters (e.g.: Route
                                    Nord)
                                 Technical information: Parameter name: Upper_Case
2.01 / 01-2017




                 J-138                                                     A+W Business Logistic Optimizer
                 Software Reference                                                                  Configuration




                                        Vehicle Assignment Here you can define whether the vehicles are automat-
                                        ically assigned during order import A+W Business. Possible values:
                                        • Yes: The vehicles are automatically assigned.
                                        • No: The vehicles are not automatically assigned.
                                        Technical information: Parameter name: Automatic_Vehicle_Assignment

                                        Images for Reports Here you can define whether to create images for the in-
                                        dividual route sections. Possible values:
                                        • Yes: Images are created
                                        • No: Images are not created.
                                        Technical information: Parameter name: Generate_Destinations_Image

                                        Overall Appearance of the Application Here you can define the design of
                                        the application. Possible settings are:
                                        • Office 2007 or 2010 Blue
                                        • Office 2008 or 2010 Black
                                        • Office 2007 or 2010 Silver
                                        • Sparkle Blue
                                        • Professional System
                                        • Sparkle Orange
                                        • Sparkle Purple
                                        After you have changed the settings, you must restart the module.
                                        Technical information: Parameter name: Overall_Appearance_Application

                                        Enable Login Here you can define whether to enable the login module. Pos-
                                        sible values:
                                        • Yes: Login is necessary.
                                        • No: Login is not necessary
                                        Technical information: Parameter name: Enable_Login

                                        Password not Necessary Here you can define, whether to use the App with
                                        our without password. Possible values:
                                        • Yes: Can be used without password.
                                        • No: Can only be used with possword.
                                        Technical information: Parameter name: Allow_No_Password

                                        ERP Master Data Here you can define whether the master data of the ERP
                                        system are used. Yes means, the OTR master data are not considered. Pos-
                                        sible values:
                                        • Yes: The ERP master data are used.
                                        • No: The ERP master data are not used.
                                        Technical information: Parameter name: Use_ERP_Masterdata
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                            J-139
                 Configuration                                                              Software Reference




                                 Use Delivery Address With this entry, you can define which address is used
                                 as delivery address. Possible values:
                                 • Yes: The delivery address can be changed in the module. The changed de-
                                    livery address is then considered to be the destination and the address
                                    from the order is overwritten.
                                 • No: Addresses from the A+W Business cannot be changed.
                                 Technical information: Parameter name: Use_Delivery_Address

                                 Currency Here you can define the local currency unit. For example, € for eu-
                                 ros or $ for dollars.
                                 Technical information: Parameter name: Currency

                                 OTR Customer Address With this entry, you can define whether customer
                                 addresses in OTR can be changed and saved. Possible values:
                                 • Yes: The customer address can be changed and saved in the module. If
                                    the parameter is set to Yes, the neighboring icon in the dialog Edit destina-
                                    tion is active. This takes you to the Customer dialog.
                                 • No: Addresses from the A+W Business cannot be changed.
                                 Technical information: Parameter name: Use_Customers_OTR

                                 Next Maintenance Date With this date you can define whether you would
                                 like to work with the maintenance dates of the individual vehicles. Possible val-
                                 ues:
                                 • Yes: You want the next maintenance data to be taken into consideration for
                                     your fleet.
                                 • No: The next maintenance date will not be taken into consideration.
                                 Technical information: Parameter name: Use_Vehicle_Maintenance

                                 Number of Days Here you can enter the desired number of days after which
                                 the next maintenance is due. Once this date has been reached, a message
                                 indicating this will be output.
                                 Technical information: Parameter name: Days_Before_Vehicles_Maintenance

                                 Export Path Here you define where the export files for the navigation system
                                 are saved.
                                 Technical information: Parameter name: Path_Export_ITN_GPX_File

                                 Export With this entry, you can define whether export files for navigation sys-
                                 tems are created or not. Possible values:
                                 • Yes: The export function can be used.
                                 • No: No files for navigation systems can be exported.
                                 Technical information: Parameter name: Use_Export_To_GPS_Systems


                                 Additional information
2.01 / 01-2017




                                  Tutorial, “Parameters” on page J-32




                 J-140                                                        A+W Business Logistic Optimizer
                 Software Reference                                                                     Administration




                                        Administration
                                        Menu Administration
                                        All data required to work properly is configured and administered in this area.
                                        The area contains:
                                        •   User:
                                            You can change, delete or edit users.
                                             “User” on page J-142
                                        •   Status:
                                            You can change, delete or edit status.
                                             “Status” on page J-143
                                        •   Customer:
                                            You can change, delete or edit customers.
                                             “Customers” on page J-145
                                        •   Departments:
                                            You can change, delete or edit departments.
                                             “Departments” on page J-147
                                        •   Vehicles:
                                            You can change, delete or edit vehicles.
                                             “Vehicles” on page J-148
                                        •   Drivers:
                                            You can change, delete or edit drivers.
                                             “Driver” on page J-151
                                        •   Reports:
                                            You can access reports.
                                             “Reports” on page J-154
                                        •   Data import:
                                            You can import data.
                                             “Data Import” on page J-157

                                            Dialog buttons
                                            The standard buttons and menus are described in detail in the section
                                            Overview and in the tutorials. We are therefore not going to describe them
                                            in connection with the dialogs.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                J-141
                 Administration                                                             Software Reference




                                  User
                                  Administration > User




                                  Fig. J-44    User


                                  This dialog is used to control user profiles, that are registered under Windows
                                  or in a domain.

                                  Description of fields in the section Detail

                                  User ID This field contains the user ID, e.g. Windows authentification. The
                                  data are automatically generated at program start.

                                  Name This field contains the name of the user. The field can be changed.

                                  Copy from As administrator you can copy an exisiting user. Open the com-
                                  bobox and select the user to be copied.


                                  Additional information
                                   Tutorial, “User” on page J-34
2.01 / 01-2017




                 J-142                                                        A+W Business Logistic Optimizer
                 Software Reference                                                                       Administration




                                        Status
                                        Administration > Status




                                        Fig. J-45    Status


                                        This dialog shows you all defined status. You can define a new status or
                                        change an existing one. The field Editable shows the status that can be
                                        changed. A green checkmark indicates that the status can be changed. All sta-
                                        tus without green checkmaks cannot be changed.

                                        Description of fields

                                        Status Type This field contains the status type. The types are split into the fol-
                                        lowing:
                                        • 1: Created:
                                           The A+W Business system provides this information automatically when
                                           the wizard function is used but not saved.
                                        • 50: In editon:
                                           The route has this mode after a saved route was loaded.
                                        • 100: Planned:
                                           After saving, the route gets this status.
                                        • 150: Organized:
2.01 / 01-2017




                                           This is a free status, that can be used for a company organization.




                 A+W Business Logistic Optimizer                                                                   J-143
                 Administration                                                              Software Reference




                                  •   200: Released:
                                      In this status, routes can be transferred to the GDC App and are available
                                      on mobile devices.
                                  •   250: Initiate:
                                      In the GDC App, the user can start tracking by clicking on Start Route.
                                  •   860: Completion deleted:
                                      In the GDC App, the user can cancel the route.
                                  •   870: Total completion:
                                      In the GDC App, the user can close the route, after finishing all destina-
                                      tions.
                                  •   880: Completion unfinished:
                                      In the GDC App, the user can close the route. In this case at least one des-
                                      tination was rejected or partially accepted.
                                  •   890: Deleted:
                                      In the GDC App, the user can cancel the route.
                                  •   900: Partially completed:
                                      All documents were rejected from the GDC App.
                                  •   1000: Archived:
                                      The OTR user can set the status manually to Archived. The route vanishes
                                      from the GDC App and will be saved to the OTR database.

                                  Status This field contains the status. If the fields Status Type and Status are
                                  identical, no modifications are possible.

                                  Name This field contains the status name..

                                  Editable This field shows whether the status can be edited or not. The status
                                  can be edited when the field has a green tick.


                                  Additional information
                                   Tutorial, “Status” on page J-35
                                   Tutorial, “Managing Status Types” on page J-36
2.01 / 01-2017




                 J-144                                                        A+W Business Logistic Optimizer
                 Software Reference                                                                    Administration




                                        Customers
                                        Administration > Customer




                                        Fig. J-46   Customers


                                        Use this dialog to add, change or delete basic customer data. Customers are
                                        saved automatically if the value USE_CUSTOMERS_OTR has been set to
                                        Yes in the parameters.

                                        Description of fields in tab Main

                                        Customer No. This field contains the customer number.

                                        Name This field contains the customer name.

                                        Telephone This field contains the phone number

                                        Address This field contains the customer address.

                                        Priority This checkbox is active for addresses that are priority addresses.

                                        Latitude This field contains the latitude of the company address.
2.01 / 01-2017




                                        Longitude This field contains the longitude of the company address.




                 A+W Business Logistic Optimizer                                                               J-145
                 Administration                                                                  Software Reference




                                  Time In this field you can enter the time in minutes that the driver has for un-
                                  loading and loading (empty racks).

                                  Clock Use this button to open a dialog in which you can enter a time range
                                  for the driver on-site. If you enter such a range, it will be displayed in field Time
                                  Range.

                                  Contact Person This field allows to enter a contact person at customer.

                                  E-Mail-Address Contact This field allows to enter the email address of the
                                  contact.

                                  Description of fields in tab Information

                                  Name2 This field allows to enter a further name.

                                  Name3 This field allows to enter a further name.

                                  Telephone 2 This field allows to enter a further phone number.

                                  Fax This field allows to enter a fax number.

                                  Web If the customer has a website, you can enter the respective address.

                                  Description This field allows to enter a further description for the customer.


                                  Additional information
                                   Tutorial, “Customers” on page J-37
                                   Tutorial, “Managing Customers” on page J-38
2.01 / 01-2017




                 J-146                                                           A+W Business Logistic Optimizer
                 Software Reference                                                                     Administration




                                        Departments
                                        Administration > Department




                                        Fig. J-47    Departments


                                        Use this dialog to add, change or delete departments. This serves for statisti-
                                        cal evaluations.

                                        Description of fields

                                        Department This field allows to enter the department, e.g. dispatch.

                                        Name This field allows to enter the name of the department, e.g. dispatch
                                        north.

                                        Description This field allows to enter a further description.


                                        Additional information
                                         Tutorial, “Departments” on page J-40
                                         Tutorial, “Managing Departments” on page J-40
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                J-147
                 Administration                                                                Software Reference




                                  Vehicles
                                  Administration > Vehicles




                                  Fig. J-48    Vehicles


                                  This dialog contains all created vehicles that OTR can work with. A vehicle
                                  may be a truck, a trailer as well as a larger transporter.
                                  The dialog is divided into two sections. The upper area provides an overview
                                  of all vehicles that have been set up. If you click on a vehicle in the upper area,
                                  the lower area will show you Detailed Information about the selected vehicle.

                                  Description of fields in the section Detail

                                  License Plate Enter the license plate number of the vehicle in this field, e.g.
                                  HH-XY-123. If you do not know the license plate number, please refer to the
                                  vehicle documents (vehicle registration).

                                  Brand In this field, enter the brand of the vehicle, e.g. Iveco. If you do not
                                  know this information, please refer to the vehicle documents (vehicle registra-
                                  tion).

                                  Model Enter the vehicle model in this field, e.g. Daily 50 C 14. If you do not
                                  know the vehicle model, please refer to the vehicle documents (vehicle regis-
2.01 / 01-2017




                                  tration).




                 J-148                                                          A+W Business Logistic Optimizer
                 Software Reference                                                                         Administration




                                        Chassis Number Enter the chassis number in this field, e.g.
                                        WWW1256425DERE. If you do not know the chassis model, please refer to
                                        the vehicle documents (vehicle registration).

                                        Purchase Date Enter the date on which you purchased the vehicle in this
                                        field. This gives you an overview of how many kilometers the vehicle has driv-
                                        en.

                                        Next Maintenance In this field you can enter the next maintenance date for
                                        the respective vehicle. In the parameter (The program shows the number of
                                        days after which the next maintenance is due), you can define the number of
                                        desired days.

                                        Department This field allows to assign a department to the vehicle. The value
                                        is loaded from Administration > Department.

                                        Maximum Width Enter the maximum width of the vehicle in meters, e.g.
                                        2.85, in this field. If you do not know the width, please refer to the vehicle doc-
                                        uments (vehicle registration).

                                        Maximum Height Enter the maximum height of the vehicle in meters, e.g.
                                        3.85, in this field. If you do not know the height, please refer to the vehicle doc-
                                        uments (vehicle registration).

                                        Maximum Length Enter the maximum length of the vehicle in meters, e.g.
                                        7.6, in this field. If you do not know the length, please refer to the vehicle doc-
                                        uments (vehicle registration).

                                        Maximum Load Enter the maximum width of the vehicle in meters, e.g.
                                        25650, in this field. If you do not know the width, please refer to the vehicle
                                        documents (vehicle registration). Please note that transport racks are also part
                                        of the load.

                                        Empty Weight Enter the empty weight of the vehicle in this field, e.g. 7800. If
                                        you do not know the empty weight, please refer to the vehicle documents (ve-
                                        hicle registration).

                                        Consumption Enter the average fuel consumption in this field in liters per
                                        100 km, e.g. 18.5. This means that the vehicle consumes 18.5 liters of fuel on
                                        100 km. If you do not enter a value here, the default value from the parameters
                                        is used to calculate the route costs.

                                        Costs Enter the average price for a liter of fuel here, e.g. 1.43. You can set
                                        up the currency unit in the parameters. If you do not enter a value here, the
                                        default value from the parameters is used to calculate the route costs.

                                        Vehicle Type Choose the corresponding vehicle from combo box. e.g. truck
                                        or automobile.
2.01 / 01-2017




                                        From / to Timeframe of the vehicle. In case the start or end time of the route
                                        is not in the frame, a warning icon appears in column Status (in the planning
                                        views).



                 A+W Business Logistic Optimizer                                                                     J-149
                 Administration                                                               Software Reference




                                  Driver This field contains the driver ID. The value comes from Configuration
                                  > Driver > Driver ID.

                                  Name This field contains the first name of the driver. The value comes from
                                  Configuration > Driver > Name.

                                  Surname This field contains the surname of the driver. The value comes from
                                  Configuration > Driver > Surname.

                                  Driver If you press this button, the Driver dialog opens. You can select the re-
                                  spective driver here.

                                  Routes The route numbers shown here are transferred from AWBusiness
                                  and serves to assign trucks to certain route numbers.

                                  Sequence If the same route number is allowed for two or more trucks, this
                                  field allows to determine the sequence. The field will be evaluated if the value
                                  ROUTE_ORIGIN has been set to Yes in the parameters.

                                  With Trailer This checkbox is used to define whether the vehicle can accom-
                                  modate a trailer.
                                  Trailers are not permitted for this vehicle.
                                   Trailers are permitted for this vehicle.

                                  Vehicle Available This checkbox is used to define whether the vehicle is
                                  generally available.
                                   The vehicle is not generally available.
                                   The vehicle is generally available and can be scheduled.

                                  GPS Type Select the respective GPS type from the combo box, e.g. GDC (in-
                                  dividual delivery App), Atlantis (spanish GPS provider for trucks) or SkyeEye
                                  (US GPS provider for trucks).

                                  Code Enter the code of the respective GPS system.

                                  Description Here you can enter a description of the vehicle.


                                  Additional information
                                   Tutorial, “Vehicles” on page J-42
                                   Tutorial, “Managing Vehicles” on page J-43
2.01 / 01-2017




                 J-150                                                           A+W Business Logistic Optimizer
                 Software Reference                                                                     Administration




                                        Driver
                                        Administration > Driver




                                        Fig. J-49    Driver


                                        This dialog contains all created drivers that you have access to. This involves
                                        permanent as well as temporary staff.

                                        Description of fields in the section Detail

                                        Driver ID Enter the code of the driver here.

                                        Name Enter the first name of the driver here.

                                        Surname Enter the surname of the driver here.

                                        Surname 2 Here you have the opportunity to enter a second surname of the
                                        driver.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                 J-151
                 Administration                                                             Software Reference




                                  Tax ID Enter the tax ID of the driver here. You can request this ID from the
                                  driver.

                                  E-Mail Enter the email address of the driver here.

                                   Costs In this field, you have the opportunity to set up various driver costs.
                                  This field is linked with the underlying radio buttons By Time and By Distance.
                                  The value you enter here is based on the respective radio button that you have
                                  enabled.

                                  By Time With this radio button you define whether the costs that you have en-
                                  tered in the field Costs per driver are based on the route time.

                                  By Distance With this radio button you define whether the costs that you
                                  have entered in the field Costs per driver are based on the route distance.

                                  Address You can enter the address of the driver in this field.

                                  Telephone You can enter the telephone number of the driver in this field, e.g.
                                  the land line number.

                                  Telephone 2 You can enter the telephone number of the driver in this field,
                                  e.g. the mobile phone number.

                                  Contact Person In this field, you can enter the name of a contact person if
                                  the driver is not employed with your company but with another company.

                                  Contact Address In this field, you can enter the contact address if the driver
                                  is not employed with your company but with another company.

                                  Telepone Contact In this field, you can enter the phone number if the driver
                                  is not employed with your company but with another company.

                                  Description In this field, you can enter a description about the driver or the
                                  contact person.

                                  E-Mail-Address-Contact In this field, you can enter the email address of the
                                  contact person.

                                  Department This field allows to assign a department to the vehicle. The value
                                  is loaded from Administration > Department.

                                  Company Driver In this field you define whether the driver is an employee in
                                  your company or not.
                                   The driver is not employed with your company.
                                   The driver is employed with your company.
2.01 / 01-2017




                 J-152                                                        A+W Business Logistic Optimizer
                 Software Reference                                                                   Administration




                                        Available This checkbox is used to define whether the driver is generally
                                        available.
                                         The driver is not generally available.
                                         The driver is generally available and can be scheduled.

                                        Reset Password This checkbox is used to reset the password necessary at
                                        start of the GDC App.


                                        Additional information
                                         Tutorial, “Driver” on page J-46
                                         Tutorial, “Managing Drivers” on page J-47
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                              J-153
                 Administration                                                              Software Reference




                                  Reports
                                  Administration > Reports




                                  Fig. J-50    Reports


                                  This dialog is used to define new report, or change existing ones. The table
                                  above shows which reports have already been created.

                                  Description of fields

                                  Report Name This field allows to enter the report name.

                                  Report Path This field allows to enter where the report is to be saved.

                                  Description This field allows to enter a further description.

                                  Parameters Use the checkboxes to select the parameters to be printed on
                                  the report.


                                  Additional information
                                   Tutorial, “Reports” on page J-49
                                   Tutorial, “Managing Reports” on page J-50
2.01 / 01-2017




                 J-154                                                          A+W Business Logistic Optimizer
                 Software Reference                                                                      Administration




                                        Packaging
                                        Administration > Packaging Types




                                        Fig. J-51    Packaging


                                        This dialog is used to define new packaging types, or change existing ones.
                                        The table above shows which packaging types have already been created.

                                           Loading Space Optimization
                                           The current version does not support a loading space optimization for
                                           trucks. Use the defined packaging types for booking purposes like unload-
                                           ing or collecting (tracking of packaging types).

                                        Description of fields

                                        Packaging ID Enter the packaging ID in this field.

                                        Packaging Type This field allows to enter the packaging type, e.g. A rack, L
                                        rack, box.

                                        Department This field allows to assign a department to the packaging type.
                                        The value is loaded from Administration > Department. The underlying button
                                        opens the dialog Select Department.

                                        Width This field allows to enter the width of the packaging in meter, e.g. 2,50.
2.01 / 01-2017




                                        It will be used for program extension (loading space optimization).




                 A+W Business Logistic Optimizer                                                                 J-155
                 Administration                                                              Software Reference




                                  Height This field allows to enter the height of the packaging in meter, e.g.
                                  1,98. It will be used for program extension (loading space optimization).

                                  Length This field allows to enter the length of the packaging in meter, e.g.
                                  0,95. It will be used for program extension (loading space optimization).

                                  Empty Weight This field allows to enter the empty weight of the packaging in
                                  kilogram, e.g. 250,00. This value is necessary to use the available total weight
                                  of the vehicle efficiently.

                                   Costs This field allows to enter the purchase costs of the packaging type,
                                  e.g. 300,00. This value serves for statistical avaluations later on.

                                  No Collection Enable this checkbox if the packaging type shall not be re-
                                  turned. This may be the case for wooden boxes. They remain at the customer.

                                  Description This field allows to enter a further description.


                                  Additional information
                                   Tutorial, “Packaging Types” on page J-51
2.01 / 01-2017




                 J-156                                                         A+W Business Logistic Optimizer
                 Software Reference                                                                        Administration




                                        Data Import
                                        Administration > Data Import




                                        Fig. J-52    Data import


                                        Use this dialog to import data in CSV format.

                                        Description of fields

                                        Import Please select the data type from the combo box. Possible values are:
                                        • Customers
                                        • Departments
                                        • Driver
                                        • Vehicles

                                        Options If the first line shall be ignored, activate the checkbox Ignore First
                                        Line. Enter the separator of the file to be imported in the line below, e.g. semi-
                                        colon, comma, etc.

                                        Import Use the radio buttons to control the import. If the radio button Import
                                        is enabled, import will be executed and the imported data (csv file) will be kept.
                                        If the radio button Delete and Import is enabled, the data will be deleted after
                                        import.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-157
                 Administration                                                            Software Reference




                                  Import Path Select where the file to be imported can be found.

                                  Table The table below shows the fields to be imported.


                                  Additional information
                                   Tutorial, “Data Import” on page J-54
2.01 / 01-2017




                 J-158                                                     A+W Business Logistic Optimizer
                 Software Reference                                                                              Planning




                                        Planning
                                        Planning menu
                                        All data required for planning a route is configured and administered in this ar-
                                        ea.
                                        The area contains:
                                        •   Copy route:
                                            This dialog is used to copy a saved route.
                                             “Copy a Saved Route” on page J-161
                                        •   Load saved routes:
                                            This dialog is used to load a saved route.
                                             “Load a Saved Route” on page J-163
                                        •   New route:
                                            This dialog is used to create a new route.
                                             “Creating a New Route – General” on page J-165
                                             “Creating a New Route - Vehicle” on page J-169
                                             “Creating a New Route – Parameters” on page J-174
                                             “Creating a New Route – Costs” on page J-180
                                        •   Edit route:
                                            The fields of this dialog are identical with the fields of dialog Create a new
                                            route.
                                             “Creating a New Route – General” on page J-165
                                        •   Delete route:
                                            With this button you can delete the current route.
                                        •   Groups:
                                            In this dialog, you can enter the number of groups.
                                             “Groups” on page J-182
                                        •   Vehicles:
                                            In this dialog, you can assign a vehicle to a route.
                                             “Select Vehicle” on page J-172
                                        •   New destination:
                                            In this dialog, you can enter a new destination.
                                             “Creating a New Route – General” on page J-165
                                        •   Edit destination:
                                            In this dialog, you can change an existing destination.
                                             “Edit Destination” on page J-184
                                        •   Delete destination:
                                            You can delete a selected destination with this button.
                                        •   Positions:
                                            Here you see the individual positions of the route.
                                             “Show Items” on page J-188
                                        •   Detailed view:
                                            The detail view provides an overview of the individual destinations of a
                                            route.
2.01 / 01-2017




                                             “Detailed View” on page J-191




                 A+W Business Logistic Optimizer                                                                   J-159
                 Planning                                                               Software Reference




                            •   Initialize:
                                This button takes you back to the starting situation. If, e.g. you have
                                grouped records, which you wish to undo, click this button.
2.01 / 01-2017




                 J-160                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                            Planning




                                        Copy a Saved Route
                                        Planning > Copy Route




                                        Fig. J-53   Copy saved route


                                        This dialog contains all routes saved in the system. You can copy routes and
                                        perform various simulations. To do so, mark the route you want to copy and
                                        press the [Route] button.

                                        Description of fields in the section Routes

                                        Route Status This field contains the route status.

                                        Delivery Date Here the delivery date of the original route is shown.

                                        Original Route The original route number is shown here. This route number
                                        comes from A+W Business.

                                        Route ID The field contains the route ID assigned by OTR.

                                        Route Name Here the name of the route that you have assigned to it is
                                        shown.

                                        Distance Here you can see the number of kilometers the original route had.

                                        Route Time Here you can see how long the original route took.
2.01 / 01-2017




                                        Route Costs Here you can see what the original route cost.




                 A+W Business Logistic Optimizer                                                                 J-161
                 Planning                                                               Software Reference




                            Allocated Weight Here you can see the weight of the original route.

                            License Plate The license plate number is shown here. Based on this num-
                            ber, you can determine which vehicle was driven on the original route.

                            Brand and Model Here you can see the brand and the model of the vehicle
                            that was driven on the original route.

                            Truck Load This field shows you the weight of the truck load.

                            Department This field contains the department that initiated the route.

                            Traffic This field shows whether the route contained traffic information.

                            Tolls This field shows whether the route contained tolls.

                            Description of fields in the section Destinations

                            Route Name This fields shows the name of the route.

                            Route ID This field contains the route ID.

                            Sequence These fields show the sequence of the individual destinations.

                            Customer This field contains the customer number.

                            Customer This field contains the customer name.

                            Address This field contains the customer address.

                            Order This field contains the order number.

                            Delivery Weight This field contains the weight per destination.

                            Collected Weight This field contains the collected weight per destination.

                            Expected Arrival This field contains the scheduled delivery date.

                            Priority This field shows whether the address is a priority address.

                            On Time This field shows wehther the adress has been reached in time.

                            Type This field contains the destination type (start type, intermediate type,
                            etc.).

                            Description of buttons

                            Filter If you press this button, the Filter Routes dialog opens.
2.01 / 01-2017




                            Copy After pressing this button, you will be asked whether you want to add
                            the saved route to the current routes.




                 J-162                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                            Planning




                                        Additional information
                                         Tutorial, “Copy a Saved Route” on page J-61
                                         Tutorial, “How to copy a saved route” on page J-67



                                        Load a Saved Route
                                        Planning > Load a Saved Route




                                        Fig. J-54     Saved route list


                                        This dialog contains all routes saved in the system. Routes are automatically
                                        saved if you press the button [End] in the Result. You can add a saved route
                                        from this list to a route your are currently planning. To do so, mark the route
                                        you want to add and press the [OK] button. You can also delete individual
                                        routes from the list by selecting the route and the clicking the button [Delete
                                        route].

                                        Description of fields
                                        The fields of this dialog are identical with the fields of dialog Copy a Saved
                                        Route.
                                         “Copy a Saved Route” on page J-161


                                        Additional information
                                         Tutorial, “Load a Saved Route” on page J-60
                                         Tutorial, “How to load a saved route” on page J-66
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-163
                 Planning                                                               Software Reference




                            Import Destinations
                            Planning > Import Destinations




                            Fig. J-55    Import destinations


                            Use this dialog to import destinations in CSV format.

                            Description of fields

                            Options If the first line shall be ignored, activate the checkbox Ignore First
                            Line. Enter the separator of the file to be imported in the line below, e.g. semi-
                            colon, comma, etc.

                            Import Path Select where the file to be imported can be found.

                            Table The table below shows the fields to be imported.
2.01 / 01-2017




                 J-164                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                               Planning




                                        Creating a New Route – General
                                        Planning > Add Route




                                        Fig. J-56     New route, General tab


                                        In this dialog you can define all the settings you need to plan a route. It is di-
                                        vided into three tabs:
                                        •   Creating a New Route – General
                                        •   Creating a New Route - Vehicle
                                        •   Creating a New Route – Parameters

                                        Description of fields in the section Information

                                        Delivery Date Open the combo box and select a delivery date.

                                        Start Time In this field, enter the time the route is to start. You can set the time
                                        with the keyboard or the arrow keys.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                     J-165
                 Planning                                                               Software Reference




                            Route Status The route status is shown here. The value can no longer be
                            changed at this point. Only once optimization has been run can you change
                            the status in the Result area. The following values are then available:
                            • Roughly scheduled: This is the status of the route after optimization.
                            • Detailed schedule: This status is not analyzed at present.
                            • Released: Once you have changed the status to released, the Delivery
                               Date, the Sequence and the Route are returned to A+W Business. You can
                               only change the status to released once.

                            Route ID The field contains the route ID assigned by OTR. The value cannot
                            be changed.

                            Route Name Enter the name of the route in this field. The entry is prepopu-
                            lated with the content of the field lblGeneralRoute, the current date and the
                            original route.

                            Original Route The original route number is shown here. This route number
                            comes from A+W Business. As you are creating a new route, the field is filled
                            with 0. The value cannot be changed.

                            Route Name The original route name is shown here. This name comes from
                            A+W Business and cannot be changed.

                            Department This field contains the department. The prepopulation can be
                            changed by pressing the icon buttons below.

                            Description You can enter a detailed description of the route in this field.

                            Description of fields in the Starting Point section

                            Company Name This field contains the company name at which the route
                            starts. The value comes from the parameters (Initial_Companyname).

                            Address This field contains the company address at which the route starts.
                            The value comes from the parameters (Initial_Address). Street, city and coun-
                            try have to be separated by comma. For instance: Konrad-Adenauer-Str. 15,
                            35440 Linden, Germany.

                            Latitude This field contains the latitude of the company address. If the field is
                            empty, you can determine the location by pressing the [Geolocate] button. This
                            opens the Simple Geolocation dialog.

                            Longitude This field contains the longitude of the company address. If the
                            field is empty, you can determine the location by pressing the [Geolocate] but-
                            ton. This opens the Simple geolocation dialog.
2.01 / 01-2017




                 J-166                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                        Planning




                                        Use Starting Point With this checkbox you can specify whether the company
                                        address is to be used as starting point.
                                         The company address is not used as starting point
                                         The company address is used as starting point

                                        Geolocate If you press the button [Geolocate], the Simple Geolocation dialog
                                        opens.


                                        Additional information
                                         “Geolocate” on page J-168
                                         Tutorial, “How to create a new route” on page J-62
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                              J-167
                 Planning                                                               Software Reference




                            Geolocate
                            Planning > New Route > General > [Geolocate]




                            Fig. J-57    Simple Geolocation


                            This dialog is used to geolocate your address.

                            Description of fields

                            Address This field contains the company address. The content of the field
                            comes from the Address field in the General Route dialog. You can change the
                            address if necessary. Please make sure that the street, the city and the coun-
                            try are separated by commas.

                            Latitude This field contains the latitude of the company address.

                            Longitude This field contains the longitude of the company address.

                            Suggestions If you press the [Suggestions] button, a small table opens con-
                            taining suggestions for the respective address. If there are several entries, you
                            can choose one. Pressing [Accept] transfers the data to the Route dialog.


                            Additional information
                             “Creating a New Route – General” on page J-165
2.01 / 01-2017




                 J-168                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                              Planning




                                        Creating a New Route - Vehicle
                                        Planning > New Route > Vehicle




                                        Fig. J-58      New route, Vehicles tab


                                        In this tab, you can make all settings that apply to the vehicle that will be used
                                        for the route. The tab is divided into the following sections:
                                        •   Vehicles
                                        •   Driver

                                        Description of fields in the section Vehicles

                                        License Plate Enter the license plate number of the vehicle in this field, e.g.
                                        HH-XY-123. If you do not know the license plate number, please refer to the
                                        vehicle documents (vehicle registration).

                                        Brand and Model In this field, enter the brand and model of the vehicle, e.g.
                                        Iveco. If you do not know this information, please refer to the vehicle docu-
                                        ments (vehicle registration).
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-169
                 Planning                                                                 Software Reference




                            Fuel Costs Enter the average price for a liter of fuel here, e.g. 1.43. You can
                            set up the currency unit in the parameters.

                            Fuel Consumption Enter the average fuel consumption in this field in liters,
                            e.g. 18.5.

                            Maximum Width Enter the maximum width of the vehicle in meters, e.g.
                            2.85, in this field. If you do not know the width, please refer to the vehicle doc-
                            uments (vehicle registration).

                            Maximum Height Enter the maximum height of the vehicle in meters, e.g.
                            3.85, in this field. If you do not know the height, please refer to the vehicle doc-
                            uments (vehicle registration).

                            Maximum Length Enter the maximum length of the vehicle in meters, e.g.
                            7.6, in this field. If you do not know the length, please refer to the vehicle doc-
                            uments (vehicle registration).

                            Truck Load Enter the total permissible weight of the vehicle in this field. If you
                            do not know this information, please refer to the vehicle documents (vehicle
                            registration).

                            Vehicle Type Choose the required vehicle type from the combo box.
                            • Truck
                            • Automobile

                            Truck with Trailer This checkbox is used to define whether the truck can ac-
                            commodate a trailer. This is important to calculate the correct route. OTR con-
                            siders hard curves, too.
                            Trailers are not permitted for this truck or car.
                             Trailers are permitted for this truck or car.

                            Select Vehicle Pressing the [Select vehicle] button opens the dialog Select
                            Vehicle.

                            Description of fields in the section Driver

                            Driver ID This field contains the driver ID. The value comes from Configura-
                            tion > Driver > Driver ID.

                            Name This field contains the first name of the driver. The value comes from
                            Configuration > Driver > Name.

                            Surname This field contains the surname of the driver. The value comes from
                            Configuration > Driver > Surname.
2.01 / 01-2017




                 J-170                                                    A+W Business Logistic Optimizer
                 Software Reference                                                                        Planning




                                        Driver Costs This field contains the costs per driver. The value comes from
                                        Configuration > Driver > Costs.

                                        By Time If this checkbox is enabled, the costs per driver are based on route
                                        time.

                                        By Distance If this checkbox is enabled, the costs per driver are based on
                                        distance.


                                        Additional information
                                         Tutorial, “Vehicles” on page J-42
                                         Tutorial, “Managing Vehicles” on page J-43
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                              J-171
                 Planning                                                               Software Reference




                            Select Vehicle
                            Planning > New Route > Vehicle > [Select Vehicle]




                            Fig. J-59     Select Vehicle


                            In this dialog you can select the vehicle that is to be used for the route. The
                            data is obtained from the parameters.

                            Description of fields

                            License Plate The license plate number of the vehicle is shown in this field.

                            Brand This field contains the vehicle brand.

                            Model This field contains the vehicle model.

                            Maximum Load The maximum load of the vehicle in kg is shown in this field.

                            Fuel Consumption This field contains the average fuel consumption in liters.

                            Fuel Costs This field contains the average cost of a liter fuel.

                            From / to The timeframe of the vehicle.

                            Department This field contains the department.


                            Additional information
                             “Vehicles” on page J-148
                             Tutorial, “Vehicles” on page J-42
2.01 / 01-2017




                 J-172                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                               Planning




                                        Add Driver
                                        Planning > New Route > Vehicles > [Add Driver]




                                        Fig. J-60     Driver overview


                                        This dialog shows you all saved drivers.

                                        Description of fields

                                        Find text This field is used to filter the displayed data. It is directly connected
                                        to the Filter Type field. First select the filter type (driver ID, surname, name, or
                                        address) and enter the information that is to be used for filtering in the Find
                                        Text field.

                                        Filter Type With this combo box you specify which entries are to be used for
                                        filtering, Driver ID, Name, Surname or Address. Then enter the filter criteria in
                                        the field Find text.

                                        Filter Once you have entered the respective criteria int he fields Find Text and
                                        Filter Type, press this button. This updates the lists of entries.

                                        Clear Press the button to delete the entered filter criteria. This updates the
                                        lists of entries and all entries are shown again.

                                        Driver ID This field contains the driver ID. The value comes from Configura-
                                        tion > Driver > Driver ID.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                     J-173
                 Planning                                                              Software Reference




                            Name This field contains the first name of the driver. The value comes from
                            Configuration > Driver > Name.

                            Surname This field contains the surname of the driver. The value comes from
                            Configuration > Driver > Surname.

                            Address This field contains the customer address. The value comes from
                            Configuration > Driver > Address.


                            Additional information
                             Tutorial, “Managing Drivers” on page J-47



                            Creating a New Route – Parameters
                            Planning > New Route > Parameters




                            Fig. J-61     New route, Parameters tab


                            This tab is used to define the criteria for the route.

                            Description of fields in the section Parameters
2.01 / 01-2017




                 J-174                                                    A+W Business Logistic Optimizer
                 Software Reference                                                                            Planning




                                        Route Mode Here you can define the desired mode of the route. Possible val-
                                        ues are:
                                        • Fastest: This setting determines the fastest connection between departure
                                           and arrival point. Optimization is based on the driving time.
                                        • Shortest: This setting determines the shortest connection between depar-
                                           ture and arrival point. Optimization is based on the distance.
                                        • Economic: This setting determines the most economic route. Optimization
                                           is based on fuel consumption.
                                        The default value for this field comes from the parameters and can be change
                                        there (parameter: Nokia_Mode).

                                        Multi Route This checkbox is not enabled for routes that you create manual-
                                        ly.

                                        Delivery Date This checkbox is not enabled for routes that you create manu-
                                        ally.

                                        Start Route This checkbox is not enabled for routes that you create manually.

                                        Traffic If this checkbox is not enabled, traffic is not determined. You can call
                                        this option later on in dialog Optimization via Traffic button.

                                        Skip Optimization If this checkbox is enabled, optimization is skipped at first.
                                        You can call this option later on in dialog Optimization via Optimize Route but-
                                        ton.

                                        Toll Mode This field is used to define whether toll roads are permitted for the
                                        route. Possible values are:
                                        • Always avoid toll roads: Optimization ensures that route sections that con-
                                           tain toll roads are entirely avoided (completely excluded). If the condition
                                           cannot be met, no route is created.
                                        • Avoid toll roads partially: Optimization does not include route sections that
                                           contain toll roads. If this restriction prevents the system from defining a
                                           route, the condition is relaxed.
                                        • Penalty for toll roads: Optimization penalizes the use of toll roads.
                                        • Normal: Optimization retains the sequence of the route sections that con-
                                           tain toll roads.
                                        • Preferred: Optimization prefers connections that contain toll roads.
                                        The default value for this field comes from the parameters and can be change
                                        there (parameter: Nokia_Avoid_Tolls).

                                        Highway Mode This field is used to define whether highways are permitted
                                        on the route. Possible values are:
                                        • Always avoid highways: Optimization ensures that route sections that con-
                                           tain highways are entirely avoided (completely excluded). For instance, this
                                           is the case with HOV lanes in the USA and Canada. If the condition cannot
                                           be met, no route is created.
2.01 / 01-2017




                                        • Avoid highways partially: Optimization does not include route sections that
                                           contain highways.If this resriction prevents the system from defining a
                                           route, the condition is relaxed. If this restriction prevents the system from
                                           defining a route, the condition is relaxed.


                 A+W Business Logistic Optimizer                                                                  J-175
                 Planning                                                               Software Reference




                            •  Penalty for highways: Optimization penalizes the use of highways.
                            •  Normal: Optimization retains the sequence of the connections that contain
                               highways.
                            • Preferred: Optimization prefers connections that contain highways.
                            The default value for this field comes from the parameters and can be change
                            there (parameter: Nokia_Avoid_Motorways).

                            Tunnel Mode This field is used to define whether roads with tunnels are per-
                            mitted on the route. Possible values are:
                            • Always avoid tunnels: Optimization ensures that route sections that contain
                               tunnels are entirely avoided (completely excluded). If the condition cannot
                               be met, no route is created.
                            • Avoid tunnels partially: Optimization does not include route sections that
                               contain tunnels. If this restriction prevents the system from defining a route,
                               the condition is relaxed.
                            • Penalty for tunnels: Optimization penalizes the use of connections with tun-
                               nels.
                            • Normal: Optimization retains the sequence of the connections that contain
                               tunnels.
                            • Preferred: Optimization prefers connections that contain tunnels.
                            The default value for this field comes from the parameters and can be change
                            there (parameter: Nokia_Avoid_Tunnels).

                            Ferry Mode This field is used to define whether ferries are permitted on the
                            route. Possible values are:
                            • Always avoid ferries: Optimization ensures that route sections that contain
                               ferries are entirely avoided (completely excluded). If the condition cannot
                               be met, no route is created.
                            • Avoid ferries partially: Optimization does not include route sections that
                               contain ferries. If this restriction prevents the system from defining a route,
                               the condition is relaxed. If this restriction prevents the system from defining
                               a route, the condition is relaxed.
                            • Penalty for ferries: Optimization penalizes the use of connections with fer-
                               ries.
                            • Normal: Optimization retains the sequence of the connections that contain
                               ferries.
                            • Preferred: Optimization prefers connections that contain ferries.
                            The default value for this field comes from the parameters and can be change
                            there (parameter: Nokia_Avoid_Ferrys).
2.01 / 01-2017




                 J-176                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                             Planning




                                        Train Mode This field is used to define whether trains are permitted on the
                                        route. Possible values are:
                                        • Always avoid trains: Optimization ensures that route sections that contain
                                           trains are entirely avoided (completely excluded). If the condition cannot be
                                           met, no route is created.
                                        • Avoid trans partially: Optimization does not include route sections that con-
                                           tain trains. If this restriction prevents the system from defining a route, the
                                           condition is relaxed. If this restriction prevents the system from defining a
                                           route, the condition is relaxed.
                                        • Penalty for trains: Optimization penalizes the use of connections with
                                           trains.
                                        • Normal: Optimization retains the sequence of the connections that contain
                                           trains.
                                        • Preferred: Optimization prefers connections that contain trains.
                                        The default value for this field comes from the parameters and can be change
                                        there (parameter: Nokia_Avoid_Trains).

                                        Description of the fields in section Optimization

                                        Distance Factor This section shows you the distance factor.

                                        Weight Factor This section shows you the weight factor.

                                        On-time Factor This section shows you the on-time factor.

                                        Priority Factor This section shows you the priority factor.

                                        Time Factor This section shows you the time factor.

                                        Route Factors Pressing the button [Route Factors] opens the dialog Route
                                        factors. This is where you can change individual factors.


                                        Additional information
                                         Tutorial, “Working with Routes” on page J-62
                                         Tutorial, “How to create a new route” on page J-62
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-177
                 Planning                                                                Software Reference




                            Route Factors
                            Planning > New Route > Parameters > [Route Factors]




                            Fig. J-62     Route factors


                            In this dialog you define the factors that influence the individual features.
                            Please note that the individual percentages add up to a total of 100%. In order
                            to change the values, click the slider and move it in the respective direction.
                            With the [Lock] button, you can lock individual values that should no longer be
                            changed.
                            The following factors are available:
                            •   Distance factor:
                                The distance factor is based on the length of the route. It searches for the
                                shortest route.
                            •   Weight factor:
                                The weight factor assesses the relation between the weight with regard to
                                the length of the route. It multiplies the weight of the goods to be transport-
                                ed with the length of each route section, taking into account the goods de-
                                livered and collected at each destination. The factor searches for a lower
                                weight-route relation.
                            •   On-time factor:
                                The on-time factor counts the number of destinations to be reached within
                                the defined delivery and pickup times. It searches for the route with the
                                largest number of on-time delivery destinations.
2.01 / 01-2017




                 J-178                                                    A+W Business Logistic Optimizer
                 Software Reference                                                                             Planning




                                        •   Priority factor:
                                            The priority factor evaluates the route according to the number of destina-
                                            tions marked as priority that make up the first destinations on the route. It
                                            searches for routes with a larger number of priority destinations as the first
                                            stops.
                                        •   Time factor:
                                            The time factor is simply based on the duration of the route. It searches for
                                            the route with the shortest duration.

                                        Default Values If you press the button [Default values] the settings made are
                                        rejected and reset to the default parameter settings (Ga_Distance_Proportion,
                                        Ga_Weight_Proportion, Ga_OnTime_Proportion, Ga_Priority_Proportion,
                                        Ga_Time_Proportion). This also applies to blocked values!


                                        Additional information
                                         Tutorial, “How to edit the route” on page J-89
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-179
                 Planning                                                             Software Reference




                            Creating a New Route – Costs
                            Planning > New Route > Costs




                            Fig. J-63    New Route, Costs tab


                            This tab provides an overview of all costs that are incurred during a route. A
                            difference is made between estimated costs and real costs. The fields in the
                            right section (Real costs) are supplemented once the driver has returned from
                            his route and submitted his report to you, based on which you can then enter
                            the real values.

                            Description of fields in the section Variable Costs

                            Total Distance This field contains the total distance of the route.

                            Time Here you can see how long the route takes.

                            Fuel Costs This field contains the fuel costs for the route, you entered in tab
                            General in field Fuel Costs.

                            Fuel Consumption This field contains the consumption for the route, you en-
                            tered in tab General in field Fuel Consumption.

                            Driver Costs This field contains the costs that have accrued per driver.

                            Toll Costs If the route contains toll roads, you can enter the estimated costs
2.01 / 01-2017




                            here.

                            Fuel Costs This field contains the fuel costs for the route.


                 J-180                                                  A+W Business Logistic Optimizer
                 Software Reference                                                                          Planning




                                        Extra Costs This field shows you the extra costs for the route.

                                        Description of fields in the section Real Variable Costs

                                        Real Driver Costs This field contains the costs that have accrued per driver.

                                        Real Toll Costs If the route contains toll roads, the respective costs are
                                        shown to you here.

                                        Real Fuel Costs This field contains the fuel costs for the route.

                                        Real Distance This field contains the total distance of the route.

                                        Real Time Here you can see how long the route takes.

                                        Real Extra Costs This field shows you the extra costs for the route.

                                        Description of fields in the section Fixed Costs

                                        Fixed Costs This field shows you how large the portion of fixed costs is.

                                        Description of fields in the section Real Fixed Costs

                                        Real Fixed Costs This field shows you how large the portion of fixed costs is.

                                        Description of fields in the section Route Costs

                                        Route Costs This field shows you how much the entire route is going to cost.

                                        Description of fields in the section Real Route Costs

                                        Real Route Costs This field shows you how much the entire route is going to
                                        cost.


                                        Additional information
                                         Tutorial, “Vehicles” on page J-42
                                         Tutorial, “Driver” on page J-46
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                J-181
                 Planning                                                               Software Reference




                            Groups
                            Planning > Groups




                            Fig. J-64    Groups


                            You can use this dialog to define the number of groups the item shall be split in.
                            Enter the number and close the dialog. The groups will be adapted automati-
                            cally.


                            Additional information
                             Tutorial, “Dynamic Mode” on page J-17
2.01 / 01-2017




                 J-182                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                                Planning




                                        Vehicles
                                        Planning > Vehicles




                                        Fig. J-65     Select vehicle


                                        Use this dialog to assign a different vehicle to a route. Select the requested
                                        vehicle and press [OK] to quit the dialog.
                                        The requested vehicle will be assigned to the route.
                                        The checkbox Maximum vehicle weight and visiting time is enabled by default.
                                        This is to avoid overloading a vehicle and that both the driving time and the
                                        visiting time will be kept. If this is not the case, a different vehicle will be used
                                        automatically.


                                        Additional information
                                         Tutorial, “Vehicles” on page J-42
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                      J-183
                 Planning                                                                Software Reference




                            Edit Destination
                            Planning > Edit Destination




                            Fig. J-66    Edit destination


                            In this dialog, you can edit a destination within a route.

                               Change Address
                               The changes you make here have no effect on the actual master data from
                               A+W Business. The changes are saved in the OTR database and are avail-
                               able there.

                            Description of fields

                            Customer No. This field contains the customer number.

                            Customers This field contains the name of the customer.

                            Icon Button This button is only enabled if the value OTR Customer Address
                            has been enabled in the parameters. If you press this button, the Customer di-
                            alog opens. It contains all customers saved in the OTR database.

                            Type Choose the required route type from the combo box. Possible values
                            are:
                            • Intermediate point: The intermediate point is a random waypoint within the
                               route.
                            • Starting point: This is the starting point of the route.
                            • End point: This is the end point of the route.
2.01 / 01-2017




                            Time In this field you can enter the time in minutes that the driver has for un-
                            loading and loading (empty racks).



                 J-184                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                             Planning




                                        Selected Route The routes contained in the Routes table in the Planning
                                        section are shown here. You can open the combo box and select another
                                        route.

                                        Delivery Date This field contains the delivery date. You cannot change the
                                        value here as delivery dates can only be changed for entire routes and not in-
                                        dividual destinations. To change the date, open the Routes dialog by clicking
                                        on a route twice.

                                        Route Here you see the original route number. This value cannot be
                                        changed.

                                        Sequence If the same route number is allowed for two or more trucks, this
                                        field allows to determine the sequence. The field will be evaluated if the value
                                        ROUTE_ORIGIN has been set to Yes in the parameters.

                                        Delivery Weight This field shows you the weight of the delivery of the respec-
                                        tive customer. You can change this value.

                                        Collected Weight If the driver collected racks at a destination for return de-
                                        livery, you can enter the respective weight in this field. This gives you an over-
                                        view of the total weight of the route at all times.

                                        Priority Enable this checkbox, if the adress is a priority address.

                                        On Time Enable this checkbox if you would like to visit the adress on-time..

                                        Time Range Press the icon button behind to open the Destinations dialog.
                                        Enter the time the customer can be visited.

                                        Description You can enter a detailed description in this field.

                                        Address This field contains the customer address.

                                        Latitude This field contains the latitude of the company address.

                                        Longitude This field contains the longitude of the company address.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-185
                 Planning                                                               Software Reference




                            Suggestions If you press the [Suggestions] button, a small table opens con-
                            taining suggestions for the respective address. If there are several entries, you
                            can choose one. Pressing [Accept] transfers the data to the Route dialog.


                            Additional information
                             Tutorial, “Destinations” on page J-69
                             Tutorial, “How to edit a destination” on page J-78



                            Time Range
                            Planning > Edit Destination > From ...To ...




                            Fig. J-67     Time range


                            You can enter a time range for a customer in this dialog.

                            Description of fields

                            From/to If your customers have fixed unloading times, you can set this up
                            here. For instance from 11:30 a.m. to 1 p.m. In the field From enter 11:30 and
                            13:00 in the field To.
2.01 / 01-2017




                 J-186                                                     A+W Business Logistic Optimizer
                 Software Reference                                                                            Planning




                                        Documents
                                        Planning > Edit Destination > Tab Documents




                                        Fig. J-68    Edit destination, Tab documents


                                        This field contains the documents for the selected destination. These fields are
                                        display fields only. Changes can not be made.

                                        Description of fields

                                        Status This field contains the status of the waypoint.

                                        Order No. This field contains the order number of the customer order.

                                        Customer This field contains the customer number.

                                        Name This field contains the name of the customer.

                                        Delivery Weight This field shows you the weight of the delivery of the respec-
                                        tive customer.

                                        Collected Weight If the driver collected racks at a destination for return de-
                                        livery, the respective weight of these racks is shown in this field.


                                        Additional information
                                         Tutorial, “Display Documents” on page J-70
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                 J-187
                 Planning                                                              Software Reference




                            Show Items
                            Planning > Edit Destination > tab Items




                            Fig. J-69    Edit destination, Tab items


                            This dialog shows you the individual positions of the route(s) in a table.

                            Description of fields

                            Order This field contains the order number.

                            Item This field contains the item number of the order.

                            Product This field contains the article number.

                            Description 1-3 This field contains the description 1-3 of the product.

                            Date This field contains the order date of the order.

                            Quantity This field contains the ordered quantity per item.

                            Width This field contains the width of the unit.

                            Height This field contains the height of the unit.

                            Thickness This field contains the thickness of the unit.

                            Total Weight This field contains the total weight of the item. This value is ob-
                            tained by multiplying the weight of the unit with the quantity.
2.01 / 01-2017




                            M2 This field contains the square meter value of the item. This value is ob-
                            tained on the basis of the dimensions and is transferred from A+W Business.



                 J-188                                                  A+W Business Logistic Optimizer
                 Software Reference                                                                            Planning




                                        Additional information
                                         Tutorial, “Show Items” on page J-71



                                        Show Information
                                        Planning > Edit Destination > tab Information




                                        Fig. J-70    Edit destination, Tab information


                                        In this dialog you can view information on the destination.

                                        Description of fields

                                        Contact Person This field allows to enter a contact person for the customer.

                                        Telephone In this field, you can enter the phone number of the contact per-
                                        son.

                                        E-Mail-Address In this field, you can enter the In this field, you can enter the
                                        email address of the contact person.

                                        Description This field allows to enter a further description for the customer.

                                        Address This field contains the customer address. Entries can be changed.

                                        Longitude This field contains the longitude of the company address. Entries
                                        can be changed.

                                        Latitude This field contains the latitude of the company address. Entries can
2.01 / 01-2017




                                        be changed.




                 A+W Business Logistic Optimizer                                                                 J-189
                 Planning                                                                Software Reference




                            Additional information
                             Tutorial, “Show Information” on page J-72



                            Customers
                            Planning > Edit Destination > [Customer] button




                            Fig. J-71    Customer overview


                            This dialog shows you all saved customer addresses.

                            Description of fields

                            Filter This field is used to filter the displayed data. It is directly connected to
                            the Filter Type field. First select the filter type (customer or address) and enter
                            the information that is to be used for filtering in the Find Text field.

                            Filter Type With this combo box you specify which entries are to be used for
                            filtering, Customer or Address. Then enter the filter criteria in the field Filter.

                            Filter Once you have entered the respective criteria int he fields Filter and Fil-
                            ter Type, press this button. This updates the lists of entries.

                            Delete Filter Press the button to delete the entered filter criteria. This up-
                            dates the lists of entries and all entries are shown again.

                            Customer No. This field contains the customer number.

                            Customer This field contains the name of the customer.
2.01 / 01-2017




                            Address This field contains the customer address.




                 J-190                                                    A+W Business Logistic Optimizer
                 Software Reference                                                                           Planning




                                        Longitude This field contains the longitude of the company address.

                                        Latitude This field contains the latitude of the company address.

                                           Parameter Settings
                                           The dialog and the respective buttons are only enabled of the respective
                                           parameter entry (parameter: OTR Customer Address) has been enabled.


                                        Additional information
                                         Tutorial, “Edit Customer Address” on page J-75



                                        Detailed View
                                        Planning > Detailed View




                                        Fig. J-72    Show detailed view


                                        The Detailed View gives you the opportunity to restrict the displayed data. If
                                        the Detailed View is disabled, all destinations of all routes are shown in the
                                        Destinations area.
                                        If the button is enabled, only the Destinations of the route are shown that you
                                        have selected in the Routes area. The example above makes use of the des-
                                        tinations for Route 60.


                                        Additional information
2.01 / 01-2017




                                         Tutorial, “The Detailed View” on page J-73




                 A+W Business Logistic Optimizer                                                                 J-191
                 Optimization                                                              Software Reference




                                Optimization
                                The optimization of the route is performed in this area.
                                The area contains:
                                •   Optimize the paths between the destinations:
                                     “Optimize Route” on page J-193
2.01 / 01-2017




                 J-192                                                      A+W Business Logistic Optimizer
                 Software Reference                                                                        Optimization




                                        Optimize Route
                                        Planning > [Continue]




                                        Fig. J-73    Optimize route


                                        In this dialog, the route(s) are optimized in line with the predefined specifica-
                                        tions. The map provides a graphic overview of the current route. The right side
                                        shows a combo box containing the optimized routes. The two tabs beneath it
                                        (Optimized Route / Original Route) also refer to the current route. The Opti-
                                        mized Route tab shows you the waypoints to be driven to in the respective se-
                                        quence (after optimization). The Original Route tab shows you the original
                                        sequence (before optimization).

                                        Description of buttons

                                        Optimize Route You have to press this button if you have make changes to
                                        the route. For instance, you can change the sequence of the waypoints with
                                        the mouse. To do so, click the waypoint, keep the mouse button pressed and
                                        pull the waypoint to the new position within the sequence. Such an action af-
                                        fects the entire route, the time and the costs. You have to press the Optimize
                                        route button to update these fields and to perform a new optimization. Optimi-
                                        zation can be done by the following criteria:
                                        • Start route: Optimization is based on the start route.
                                        • Fastest: Optimization is based on the fastest route.
                                        • Shortest: Optimization is based on the shortest route. This option is just for
                                           cars (with or without trailer), not for trucks.

                                        All Routes Enable this checkbox to re-optimize all routes. The new results or
                                        optimized routes are displayed additionally and you can choose the preferred
2.01 / 01-2017




                                        result.




                 A+W Business Logistic Optimizer                                                                  J-193
                 Optimization                                                               Software Reference




                                Stop Optimization You can press this button if you want to stop an ongoing
                                optimization.

                                Optimization Factors You can press this button if you want to change the
                                optimization factors. A dialog containing the individual factors opens:
                                • Distance factor
                                • Weight factor
                                • On-time factor
                                • Priority factor
                                • Time factor
                                If you have changed one of these values, you have to optimize the route again.


                                Additional information
                                 Tutorial, “Optimizing Routes” on page J-84
                                 “Route Factors” on page J-178
2.01 / 01-2017




                 J-194                                                         A+W Business Logistic Optimizer
                 Software Reference                                                                             Result




                                        Result
                                        This area shows the result of the optimization including all necessary informa-
                                        tion.
                                        The area contains:
                                        •   The result is shown either in a chart or a table:
                                             “Result of the Optimization” on page J-196
                                        •   Enter the actual costs of the route:
                                             “Route Information” on page J-198
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                J-195
                 Result                                                                               Software Reference




                                           Result of the Optimization
                                           Planning > Optimization > [Continue]




                 Fig. J-74   Result of the optimization


                                           This dialog shows you the result of the optimization. It contains all necessary
                                           information, presented in a chart or table.
                                           The dialogue consists of three sections:
                                           •   Routes
                                           •   Route plan
                                           •   Destinations

                                           Description of fields in the section Routes

                                           Route Status This field contains the route status. The following values are
                                           possible:
                                           • Created: This is the part of the status the route is in from the wizard to the
                                              point at which the route is saved. The status then changes to Roughly
                                              scheduled. If saved routes are loaded, they also have the status Created.
                                           • Roughly scheduled: This is the status of the route after optimization.
                                           • Detailed schedule: This status is not analyzed at present.
2.01 / 01-2017




                                           • Released: Once you have changed the status to released, the Delivery
                                              Date, the Sequence and the Route are returned to A+W Business. You can
                                              only change the status to released once.



                 J-196                                                                 A+W Business Logistic Optimizer
                 Software Reference                                                                             Result




                                        The remaining fields are located at the top and have already been explained.

                                        Description of fields in the section Route Plan
                                        A map of the routes is shown here. If the result contains more than one route,
                                        select the route you would like to view in the Routes section.

                                        Description of fields in the section Destinations
                                        This is where the individual destinations are listed.
                                        The individual fields have already been explained.
                                         “Edit Destination” on page J-184

                                        Description of buttons

                                        Route If you press this button, the Route dialog opens with the tabs General,
                                        Vehicles, Parameters and Costs. You have access to a number of values in
                                        the individual tabs. Access is used to copy the values and not to change them!

                                        Destination If you press this button, the Destination dialog opens. Here you
                                        have access to the following values:
                                        • Delivery weight
                                        • Collected weight
                                        • Address
                                        Access is used to copy the values and not to change them!

                                        Edit Route If you press this button, the Route dialog opens with the tabs Sta-
                                        tus and Route Information. Here you can change the following value:
                                        • Route status


                                        Additional information
                                         “Confirmation and Delivery List” on page J-206
                                         Tutorial, “The Result of the Optimization” on page J-93
                                         Tutorial, “How to export data” on page J-117
                                         Tutorial, “Export” on page J-116
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                J-197
                 Result                                                               Software Reference




                          Route Information
                          Planning > Optimization > Result > [Edit Route]




                          Fig. J-75    Route information


                          This dialog provides an overview of route costs. The costs defined for the route
                          are located on the left side. On the right, you have the possibility to enter the
                          actual costs that have accrued during the route. This data is saved and taken
                          into account for the next route. Please note that the actual costs can only be
                          entered once the driver has returned from the route and submitted his route
                          report.

                          Description of fields in the right section

                          Real Distance In this field you specify how many kilometers the route actually
                          had.

                          Real Driver Costs In this field, you enter the actual costs per driver that ac-
                          crued during the route.

                          Real Time In this field, you define how long the route actually took.

                          Days In this field, you define how many days the route actually took.
2.01 / 01-2017




                 J-198                                                 A+W Business Logistic Optimizer
                 Software Reference                                                                                Result




                                        Hours In this field, you define how many hours the route actually took.

                                        Minutes In this field, you define how many minutes the route actually took.

                                        Real Toll Costs In this field, you enter the actual toll costs that accrued during
                                        the route.

                                        Real Fuel Costs In this field, you enter the actual fuel costs that accrued dur-
                                        ing the route.

                                        Real Extra Costs In this field, you enter the actual extra costs that accrued
                                        during the route.

                                        Real Fixed Costs In this field, you enter the actual fixed costs that accrued
                                        during the route.

                                        Description of buttons

                                        Transfer Costs If you press this button, the costs in the left section are trans-
                                        ferred to the costs in the Real Costs section.

                                        Remove Costs If you press this button, the values in the Real Costs section
                                        are deleted.

                                        Description of fields in the section Total Costs

                                        Real Route Costs This field shows you how much the route really costs. It is
                                        the total of all Real Costs.


                                        Additional information
                                         Tutorial, “Real Route Costs” on page J-96
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-199
                 Query                                                               Software Reference




                         Query
                         Use this section to query all relevant information. Depending on the route sta-
                         tus (initiate, planned, in edition, etc.) the menu bar offers different funtions.
                         Thus, it is not possible to change the status for a Planned route, which means,
                         the button Change of Status is disabled.
                         The area contains:
                         •   Filter routes:
                              “Filter Routes” on page J-201
                         •   Print lists for your drivers:
                              “Confirmation and Delivery List” on page J-206
                         •   Print reports:
                              “Confirmation and Delivery List” on page J-206
                         •   Create statistics:
                              “Statistics” on page J-210
                         •   Show calendar:
                              “Calendar” on page J-216
                         •   Export the route for navigation systems:
                              “Export” on page J-202
                         •   View the history:
                              “History” on page J-204
2.01 / 01-2017




                 J-200                                                 A+W Business Logistic Optimizer
                 Software Reference                                                                               Query




                                        Filter Routes
                                        Query> [Filter]




                                        Fig. J-76    Filter routes


                                        This dialog allows to filter routes. Thus, the number of displayed routes is lim-
                                        ited.

                                        Description of fields

                                        Date from In this field you enter the start date for the filter.

                                        Date to In this field you enter the end date for the filter.

                                        Route ID If you want to filter display by route ID., enter the corresponding
                                        route ID.

                                        Route Name If you want to filter display by route name, enter the correspond-
                                        ing route name.

                                        Route Status If you want to filter display by route status, choose the corre-
                                        sponding status from the checkbox Route Status. By pressing the icon buttons
                                        below you can enable or disable all.

                                        Vehicles If you want to filter display by vehicles, choose the corresponding
                                        vehicle from combo box.

                                        Driver ID If you want to filter display by driver ID, choose the corresponding
2.01 / 01-2017




                                        ID from combo box.

                                        Department If you want to filter display by departments, choose the corre-
                                        sponding department from combo box.


                 A+W Business Logistic Optimizer                                                                  J-201
                 Query                                                             Software Reference




                         Customer Enter a customer by which you intend to filter.

                         Description of buttons

                         Clear Use this button to reset the entries. Dialog is empty.


                         Additional information
                          Tutorial, “Routes” on page J-114



                         Export
                         Query > Route > [Export Route]




                         Fig. J-77    Export


                         In this dialog you can export the route data for a navigation system.

                            File Format
                            Please refer to the instruction manual of your navigation system for further
                            information on the file format your device works with.

                         Description of fields

                         ITN Format Press the radio button to export data in ITN format (e.g. Tom-
                         Tom).

                         GPX Format Press the radio button to export data in GPX format (e.g. Gar-
2.01 / 01-2017




                         min).




                 J-202                                               A+W Business Logistic Optimizer
                 Software Reference                                                                              Query




                                        Insert Locations Activate this checkbox if you also want to export the desti-
                                        nations in addition to the route.

                                        Create New Folder for this Route Enable this checkbox if you would like to
                                        create a new folder for the export.

                                        Export Path In this field you specify where the file is to be exported to.

                                           Standard Path for Export Files
                                           You define the standard path for exporting data in the parameters (Param-
                                           eter: Path_Export_ITN_GPS_File).

                                        Copy Click on this button to copy and to send the route via Mail to the Android
                                        URL. The user can call the corresponding URL on his Android device via Here
                                        maps.


                                        Additional information
                                         Tutorial, “Export” on page J-116



                                        Change Status
                                        Query > [Change of Status]




                                        Fig. J-78    Change of status


                                        Use this dialog to change the status of a route manually. This may be neces-
                                        sary when the process has been closed prior to tab Result. In this case, the
                                        route status is Created or in Edition. Then, it is necessary to change status
                                        manually to Planned or Organized.

                                        Description of fields

                                        Current Status This field contains the current route status. It can not be
                                        changed.

                                        Date Modified This field contains the date of last modification. It can not be
                                        changed.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                 J-203
                 Query                                                                Software Reference




                         Route Status The combo box contains all valid status for routes. Select the
                         desired status.

                         User This field contains the current user. It can not be changed.


                         History
                         Query > [History]




                         Fig. J-79    History


                         In this dialog, you have the opportunity to view a history. In the upper area (Fil-
                         ter), you make a selection and in the lower area (Result) you see the respec-
                         tive data.

                         Description of fields in the section Fields

                         Route ID If you want to filter display by route ID., enter the corresponding
                         route ID.

                         Document If you want to filter display by order number, enter the corre-
                         sponding order number. Alternatively you can also enter the delivery note
                         number.

                         Customer If you want to filter display by customer, enter the corresponding
                         customer number.

                         Display Archived Routes If you want to display also archived routes, enable
                         this checkbox.
2.01 / 01-2017




                 J-204                                                 A+W Business Logistic Optimizer
                 Software Reference                                                                            Query




                                        Description of buttons

                                        OK This button is used to start the filter function.

                                        Description of fields in tab Route

                                        Date This fields shows the date of the route.

                                        Customer This field contains the customer number.

                                        Name This field contains the name of the customer.

                                        Status This field contains the route status.

                                        Comment This field contains the defined comment.

                                        Order This field contains the order number. If you entered a delivery note
                                        number, it is shown here.

                                        User In this field, you can see who made changes to the document.

                                        Description of fields in tab Documents

                                        Order This field contains the order number. If you entered a delivery note
                                        number, it is shown here.

                                        Route ID This field contains the route ID.

                                        Customer This field contains the customer number.

                                        Name This field contains the name of the customer.

                                        State This field contains the route status.

                                        Delivery Weight This field contains the weight for the selected destination.

                                        Collected Weight If you collected empty racks from a customer, you can see
                                        their weight here.


                                        Additional information
                                         Tutorial, “History” on page J-119
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                               J-205
                 Query                                                                Software Reference




                         Confirmation and Delivery List
                         Query > Reports > [Selected Route]
                         The displayed confirmation and delivery list is just a sample. It is based on
                         SAP crystal reports and may look different or show different data on your sys-
                         tem.




                         Fig. J-80    Confirmation and delivery list


                         This list provides a detailed overview of the optimization result. It contains all
                         necessary information, presented in a chart or table. The list can be printed
                         and given to the driver.
2.01 / 01-2017




                 J-206                                                 A+W Business Logistic Optimizer
                 Software Reference                                                                                 Query




                                        Description of fields

                                        Route This field contains the route number.

                                        Name Here the name of the route that you have assigned to it or selected is
                                        shown.

                                        Date Shows the date on which the route is to take place.

                                        Driver Name This field contains the name of the driver.

                                        Vehicle This field contains the vehicle that is to be used for the route.

                                        KM Total This field shows you the total number of kilometers of the route.

                                        Total Weight This field shows you how many kilograms are to be transported
                                        on the entire route. The weight also includes return deliveries.

                                        Total Time This field shows you how many kilograms are to be transported
                                        on the entire route. The weight also includes return deliveries.

                                        Start Time This field contains the time at which the route is started.

                                        Available If you have set up fixed unloading times for your customer, they are
                                        shown here.

                                        Address This field shows the starting address for the next route section. For
                                        instance, from A to B. So here you see the address A and in the Destination
                                        field, you see address B.

                                        Target This field show the destination address of the next route segment. For
                                        instance, from A to B. So here you see address B and address A in the Ad-
                                        dress field.

                                        KM from Starting Point to Destination This field shows you the distance to
                                        the next destination.

                                        Delivery Weight This field contains the weight for the selected destination.

                                        Collected Weight If you collect empty racks from a customer, you can see
                                        their weight here.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                    J-207
                 Query                                                             Software Reference




                         Travel Time Here you can see the travel time to the next destination.

                         Unloading Time If unloading and loading times (for racks) were set up for
                         your driver, they are shown here.

                         Remark Your driver can enter a comment here.

                         Signature This is where your customer places their signature after delivery.


                         Additional information
                          Tutorial, “Selected Route” on page J-120
2.01 / 01-2017




                 J-208                                                A+W Business Logistic Optimizer
                 Software Reference                                                                           Query




                                        Report
                                        Query > [Report Launcher]




                                        Fig. J-81    Report launcher


                                        Use this dialog to print reports, previously defined.

                                        Description of fields

                                        Report Name This field contains the name of the report you have defined
                                        when creating the report.

                                        Report Path This field contains the path of the report you have defined when
                                        creating the report.

                                        Parameters This section contains the parameter you have selected when
                                        creating the report.

                                        Description of buttons

                                        Print Report Use this button to start printing.


                                        Additional information
                                         “Reports” on page J-120
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                              J-209
                 Query                                                                  Software Reference




                         Statistics
                         Query > [Statistics]




                         Fig. J-82     Statistics, Tab general


                         Use this dialog to create global statistics. The dialog is split into the following
                         tabs:
                         Use this dialog to create global statistics.
                         The dialog is split into the following tabs:
                         •   General
                         •   General graphic
                         •   Vehicles
                         •   Driver
                         •   Departments
                         •   Customers


                         General Tab
                         This tab provides an overview of the route costs. The real costs are compared
                         with the planned costs. In addition, the deviation is shown in currency as well
                         as in percent.
                         Information regarding weights, consumption, distance, etc. is displayed.
                         The section Filter is located on the left side of the dialog. It serves to adjust the
                         data to be displayed to individual needs. After the selection is made, click on
2.01 / 01-2017




                         [OK]. The display will be updated.




                 J-210                                                  A+W Business Logistic Optimizer
                 Software Reference                                                                                Query




                                        General Graphic Tab
                                        Query > [Statistics] > General Graphic Tab




                                        Fig. J-83    Statistics, general graphic tab


                                        According to the filter criteria you made on the left side, this tab shows the re-
                                        sult in a chart.


                                        Additional information
                                         Tutorial, “Reports” on page J-120
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-211
                 Query                                                                   Software Reference




                         Vehicles Tab
                         Query > [Statistics] > Vehicles Tab




                         Fig. J-84     Statistics, vehicles tab


                         According to the filter criteria you made on the left side, this tab shows the ve-
                         hicles in a chart.
                         In addition to the filter criteria the view offers the further criteria:
                         •   Distance
                         •   Time
                         •   Allocated weight
                         •   Fuel costs
                         •   Estimated costs
                         •   Real costs


                         Additional information
                          Tutorial, “Reports” on page J-120
2.01 / 01-2017




                 J-212                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                                  Query




                                        Drivers Tab
                                        Query > [Statistics] > Drivers Tab




                                        Fig. J-85     Statistics, drivers tab


                                        According to the filter criteria you made on the left side, this tab shows the driv-
                                        ers in a chart.
                                        In addition to the filter criteria the view offers the further criteria:
                                        •   Distance
                                        •   Time
                                        •   Allocated weight
                                        •   Costs per driver
                                        •   Estimated costs
                                        •   Real costs


                                        Additional information
                                         Tutorial, “Reports” on page J-120
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                     J-213
                 Query                                                                   Software Reference




                         Department Tab
                         Query > [Statistics] > Department Tab




                         Fig. J-86     Statistics, department tab


                         According to the filter criteria you made on the left side, this tab shows the de-
                         partments in a chart.
                         In addition to the filter criteria the view offers the further criteria:
                         •   Distance
                         •   Time
                         •   Allocated weight
                         •   Department
                         •   Estimated costs
                         •   Real costs


                         Additional information
                          Tutorial, “Reports” on page J-120
2.01 / 01-2017




                 J-214                                                   A+W Business Logistic Optimizer
                 Software Reference                                                                                 Query




                                        Customers Tab
                                        Query > [Statistics] > Customers Tab




                                        Fig. J-87     Statistics, customers tab


                                        According to the filter criteria you made on the left side, this tab shows the cus-
                                        tomers in a chart.
                                        In addition to the filter criteria the view offers the further criteria:
                                        •   Quantity
                                        •   Distance
                                        •   Objective distance
                                        •   Time
                                        •   Allocated weight


                                        Additional information
                                         Tutorial, “Reports” on page J-120
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                    J-215
                 Query                                                               Software Reference




                         Calendar
                         Query > [Calendar]




                         Fig. J-88    Calendar


                         The calendar provides an overview of drivers and vehicles. You can have the
                         result displayed by day or month. Clicking an entry twice opens the dialog
                         Query with a table view of routes and destinations. You can limit the view to a
                         certain route status (planned, released, ar-chived, etc.). Use the button [Clear]
                         to reset selection of route status and to update display.
                         If you assigned a driver or truck to more routes (simultaneously or unknowing-
                         ly) the conflict can be resolved by assigning a new driver or truck. This way, it
                         is not necessary to plan and to optimize again.


                         Additional information
                          Tutorial, “Calendar” on page J-125
2.01 / 01-2017




                 J-216                                                A+W Business Logistic Optimizer
                 Software Reference                                                                                Query




                                        Attach Files
                                        Query > [Attach Files]




                                        Fig. J-89    Attach files


                                        Use this dialog to provide the driver with digital documents.
                                        The dialog is divided into the following sections.
                                        •   Filter
                                        •   Destinations
                                        •   Files

                                        Description of fields in the section Filter

                                        Route ID In this field you specify the route ID for which you want to load the
                                        documents in the Cloud. If you do not know the route ID but the name, you can
                                        select the corresponding route name with a double-click in section Routes.
                                        The field is filled automatically with the selected route ID. Now, the Destination
                                        area shows only the destinations for the selected route ID.

                                        Customer In this field you specify the customer number for which you want
                                        to load the documents in the Cloud. The Destination area, field Customer
                                        shows all customers that are driven to on the route.

                                        Order In case a customer receives several order numbers, you can specify in
                                        this field the order number for which you want to load the documents in the
                                        Cloud.
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                   J-217
                 Query                                                             Software Reference




                         Description of fields in the section Documents

                         Route ID This field contains the route ID of the order, for which you want to
                         load the documents in the Cloud.

                         Route name This field contains the route name of the order, for which you
                         want to load the documents in the Cloud.

                         Customer No. This field contains the customer number of the order, for which
                         you want to load the documents in the Cloud.

                         Customer This field contains the customer name of the order, for which you
                         want to load the documents in the Cloud.

                         Order This field contains the order number, for which you want to load the
                         documents in the Cloud.

                         Description of fields in the section Files
                         This section contains only data after you loaded documents in the Cloud.

                         Name This fields shows the name of the document you entered.

                         Description This fields shows the description you entered.

                         File path This field shows the path of the file.

                         Description of buttons

                         Attach Document If you press this button, the Attach File dialog opens.
                         Specify the document you want to load in the Cloud.

                         Edit Document If you press this button, the Attach File dialog opens for the
                         selected document.This way, you can edit the attached document.

                         Delete Document If you press this button, the selected document will be de-
                         leted.


                         Additional information
                          “Loading Documents in the Cloud” on page J-99
2.01 / 01-2017




                 J-218                                               A+W Business Logistic Optimizer
                 Software Reference                                                                               Query




                                        Attach File
                                        Query > [Attach Files] > Icon Button




                                        Fig. J-90    Attach file


                                        Use this button to load documents in the Cloud.

                                        Description of fields

                                        File Name This field allows to enter a name, e.g. Delivery Note.

                                        File Path In this field you enter the corresponding path for the Cloud, e.g.
                                        https://drive.google.com/file/d/....

                                        Description This field allows to enter a further description.


                                        Additional information
                                         Tutorial, “How to load documents in the Cloud and reference them” on page J-100
2.01 / 01-2017




                 A+W Business Logistic Optimizer                                                                  J-219
                 Query                Software Reference
2.01 / 01-2017




                 J-220   A+W Business Logistic Optimizer
Logistic Optimizer                J

                        Section Index




                     A+W Business
                 Index                                                              Section Index




                 Index
                 A                                    – Costs of route J-161
                 Attach file J-219                    – Customer name J-162
                 – Description J-219                  – Customer number J-162
                 – File name J-219                    – Delivery date J-161
                 – File path J-219                    – Delivery weight J-162
                 Attach files J-217                   – Department J-162
                 – Attach document button J-218       – Distance J-161
                 – Customer no. J-217, J-218          – Estim. delivery J-162
                 – Delete document button J-218       – Filter button J-162
                 – Description J-218                  – In time J-162
                 – Edit document button J-218         – License plate J-162
                 – File path J-218                    – Name of route J-161
                 – Name J-218                         – Order J-162
                 – Order J-217                        – Original number J-161
                 – Route ID J-217, J-218              – Priority J-162
                                                      – Route ID J-161, J-162
                                                      – Route name J-162
                 C
                                                      – Route time J-161
                 Calendar J-216
                                                      – Sequence J-162
                 Change status
                                                      – Status J-161
                 – Current status J-203
                                                      – Tolls J-162
                 – Modification date J-203
                                                      – Traffic J-162
                 – Route status J-204
                                                      – Type J-162
                 – User J-204
                                                      – Weight J-162
                 Confirmation and delivery list
                                                      Copy saved route J-161
                 – Comment J-208
                                                      Create new route J-165
                 – Date of route J-207
                                                      Customer
                 – Delivery weight J-207
                                                      – Address J-145
                 – Destination J-207
                                                      – Contact person J-146
                 – Driving time J-208
                                                      – Description J-146
                 – KM from starting point to target
                                                      – Email address J-146
                   destination J-207
                                                      – Fax J-146
                 – Name of driver J-207
                                                      – Latitude J-145
                 – Name of route J-207
                                                      – Longitude J-145
                 – Route J-207
                                                      – Name 2 J-146
                 – Signature J-208
                                                      – Name 3 J-146
                 – Total distance J-207
                                                      – Number J-145
                 – Total time J-207
                                                      – Phone J-145, J-146
                 – Total weight J-207
                                                      – Priority J-145, J-146
                 – Unloading time J-208
                                                      – Time J-146
                 – Vehicle J-207
                                                      – Time range J-146
                 Connection
                                                      Customers J-37, J-145
                 – Database J-130
                 Copy
                 – Saved route J-161                  D
                 Copy route                           Data import J-157
                                                      Database
2.01 / 01-2017




                 – Address J-162
                 – Brand and model J-162              – Connection (OTR) J-130
                 – Collected weight J-162             – Source J-130, J-131
                 – Copy button J-162


                 J-223                                                  A+W Business Master Data
                 Section Index                                                                        Index




                 Departments J-147                           – In time J-185
                 – Department J-147                          – Priority J-185
                 – Description J-147                         – Returned weight J-185, J-187
                 – Name J-147                                – Route no. J-185
                 Display conventions J-13                    – Selected route J-185
                 Document                                    – Time range J-185
                 – Customer name J-187                       – Unloading time J-184
                 – Customer number J-187                     – Unloading time from ... to ... J-186
                 – Order no. J-187                           Edit driver
                 – Status J-187                              – Find text J-173
                 Documentation                               ERP connection
                 – Types J-12                                – Use SQL ERP connection J-131
                 Driver J-151                                Export
                 – Address J-152                             – Copy J-203
                 – Contact J-152                             – Export path J-203
                 – Contact address J-152                     – GPX format J-202
                 – Contact phone J-152                       – Insert locations J-203
                 – Costs J-152                               – ITN format J-202
                 – Costs per driver acc. to distance J-152   – New folder for route J-203
                 – Costs per driver acc. to time J-152
                 – Department J-152                          F
                 – Description J-152                         Filter
                 – Driver ID J-151                           – Clear J-202
                 – E-mail J-152                              – Customer J-202
                 – Email contact J-152                       – Date from J-201
                 – Employee J-152                            – Date to J-201
                 – Name J-151                                – Department J-201
                 – Reset password J-153                      – Driver ID J-201
                 – Surname J-151                             – Route ID J-201
                 – Surname 2 J-151                           – Route name J-201
                 – Tax ID J-152                              – Route status J-201
                 – Telephone number J-152                    – Vehicles J-201
                 – Telephone number 2 J-152
                                                             G
                 E                                           Groups   J-182
                 Edit customer
                 – Address J-174, J-189, J-190
                 – Customer name J-190                       H
                 – Customer no. J-190                        History
                 – Delete filter J-173, J-190                – Collected weight (documents) J-205
                 – Filter J-173, J-190                       – Comment (route) J-205
                 – Filter type J-173, J-190                  – Customer J-204
                 – Latitude J-189, J-191                     – Customer (documents) J-205
                 – Longitude J-189, J-191                    – Customer (route) J-205
                 Edit destination                            – Customer name (documents) J-205
                 – Address J-185                             – Customer name (route) J-205
                 – Customer name J-184                       – Delivery weight (documents) J-205
                 – Customer no. J-184                        – Document J-204
                 – Delivery date J-185                       – Filter J-205
2.01 / 01-2017




                 – Delivery weight J-185, J-187              – Order no. (documents) J-205
                 – Description J-185                         – Order no. (route) J-205
                 – Destination type J-184                    – Route date (route) J-205



                 A+W Business Master Data                                                             J-224
                 Index                                                                          Section Index




                 – Route ID J-204                            – Fuel consumption general J-180
                 – Route ID (documents) J-205                – Fuel costs general J-180
                 – Route status (documents) J-205            – Geolocate J-167
                 – Route status (route) J-205                – Geolocate suggestions J-168, J-186
                 – Show routes J-204                         – Highway mode J-175
                 – User (route) J-205                        – Latitude of starting point J-166, J-168, J-185
                                                             – Longitude of starting point J-166, J-168, J-185
                 I                                           – Maximum height J-170
                 Icons                                       – Maximum length J-170
                 – Open J-85                                 – Maximum width J-170
                 Import                                      – Multi-Tour J-175
                 – Data Import path J-158                    – Name of starting point J-166
                 – Data, Import CSV J-157                    – On-time factor J-177
                 – Data, Options J-157                       – Original number J-166
                 – Data, Table J-158                         – Priority factor J-177
                 – Data, what to import J-157                – Real costs per driver J-181
                 – Destination, import path J-164            – Real extra costs J-181
                 – Destination, options J-164                – Real fixed costs J-181
                 – Destination, table J-164                  – Real fuel costs J-181
                 Import data J-164                           – Real route costs J-181
                 Information                                 – Real time J-181
                 – Contact person J-189                      – Real toll costs J-181
                 – Description J-189                         – Real total distance J-181
                 – Email address J-189                       – Route costs J-181
                                                             – Route factors J-177
                                                             – Route ID J-166
                 L                                           – Route mode J-175
                 Load                                        – Route name J-166
                 – Saved route J-163                         – Route name (original) J-166
                 Load saved route J-163                      – Route status J-166
                                                             – Select vehicle J-170
                 M                                           – Skip optimization J-175
                 Module                                      – Standard route factors J-179
                 – function   J-11                           – Start of tour J-175
                                                             – Start time J-165, J-169
                 N                                           – Street of starting point J-166, J-168
                 New route                                   – Surname J-170
                 – Costs per driver J-171, J-180             – Time J-180
                 – Costs per driver acc. to distance J-171   – Time factor J-177
                 – Costs per driver acc. to time J-171       – Toll costs J-180
                 – Delivery date J-165, J-175                – Toll mode J-175
                 – Department J-166                          – Total distance J-180
                 – Description J-166                         – Traffic J-175
                 – Distance factor J-177                     – Train mode J-177
                 – Driver ID J-170                           – Truck load J-170
                 – Extra costs J-181                         – Truck with trailer J-170
                 – Ferry mode J-176                          – Tunnel mode J-176
                 – First name J-170                          – Use starting point J-167
                 – Fixed costs J-181                         – Vehicle type J-170
2.01 / 01-2017




                 – Fuel J-170                                – Weight factor J-177
                 – Fuel consumption J-170




                 J-225                                                            A+W Business Master Data
                 Section Index                                                                      Index




                 O                                               – Portrayal of application J-139
                 Optimization                                    – Portrayal of route width J-137
                 – Factors J-194                                 – Priority factor J-136
                 – Optimize route J-193                          – Route type J-135
                 – Stop J-193, J-194                             – Several routes J-138
                 OTR Database connection                         – Show original route J-137
                 – Password J-130, J-131                         – Start address J-137
                 – User ID J-130, J-131                          – Start company name J-137
                 OTR Database source (OTR) J-130, J-131          – Start time of route J-136
                 OTR Test database connection J-130, J-131       – Time factor J-136
                                                                 – Time on-site J-137
                                                                 – Toll mode J-133
                 P
                                                                 – Train mode J-133
                 Packaging J-155
                                                                 – Transparency of route J-137
                 – Costs J-156
                                                                 – Truck not allowed J-133
                 – Department J-155
                                                                 – Tunnel mode J-135
                 – Description J-156
                                                                 – Unit system J-138
                 – Empty weight J-156
                                                                 – Uppercase letters J-138
                 – Height J-156
                                                                 – Use ERP master data J-139
                 – ID J-155
                                                                 – Use OTR customer address J-140
                 – Length J-156
                                                                 – Vehicle type J-135
                 – No collection J-156
                                                                 – Vehicles assignment J-139
                 – Type J-155
                                                                 – Weight factor J-136
                 – Width J-155
                                                                 Parameters J-132
                 Parameter
                                                                 Password J-130, J-131
                 – Activate export J-140
                 – Average fuel consumption J-135
                 – Costs J-135                                   R
                 – Country code J-138                            Report
                 – Currency J-140                                – Description J-154
                 – Default initial address J-137                 – Name J-154
                 – Delivery address instead of order             – Parameter J-154
                   address J-140                                 – Path J-154
                 – Delivery date J-132                           Report launcher J-209
                 – Distance factor J-135                         – Parameter J-209
                 – Duration of route J-136                       – Print report J-209
                 – Dynamic vehicle assignment J-133              – Report name J-209
                 – Export path for navigation systems J-140      – Report path J-209
                 – Ferry mode J-134                              Reports J-154
                 – General route J-136                           Result
                 – Highway mode J-134                            – Destination J-197
                 – License WebService J-136                      – Edit route J-197
                 – Next maintenance date J-140                   – Route J-197
                 – Next maintenance date in ... days J-140       Route information
                 – No password J-139                             – Real costs J-199
                 – One route for every original route J-133      – Real costs/driver J-198
                 – On-time factor J-136                          – Real days J-198
                 – Opacity of original route J-137               – Real distance J-198
                 – Optimized route through straight line J-137   – Real extra costs J-199
                 – Optimized route width J-137                   – Real fixed costs J-199
2.01 / 01-2017




                 – Original department J-136                     – Real fuel costs J-199
                 – Original route color J-138                    – Real hours J-199
                 – Picture for route report J-139                – Real minutes J-199



                 A+W Business Master Data                                                           J-226
                 Index                                                                   Section Index




                 – Real time J-198                    – Department J-149
                 – Remove costs J-199                 – Description J-150
                 – Toll costs J-199                   – Driver ID J-150, J-173
                 – Transfer costs J-199               – First name J-150, J-174
                 Route status J-143                   – From/to J-149
                                                      – Last name J-150, J-174
                 S                                    – License plate J-148
                 Saved route                          – Maximum height J-149
                 – Load J-162                         – Maximum length J-149
                 Select vehicle                       – Maximum load J-149
                 – Brand J-172                        – Maximum width J-149
                 – Department J-172                   – Model J-148
                 – From/to J-172                      – Next maintenance J-149
                 – Fuel consumption J-172             – Purchase date J-149
                 – Fuel costs J-172                   – Routes J-150
                 – Maximum load J-172                 – Sequence J-150, J-185
                 – Model J-172                        – Vehicle available J-150, J-153
                 Show items                           – Weight empty J-149
                 – Description 1-3 J-188              – With trailer J-150
                 – Height of unit J-188               Vehicles J-148
                 – Item number J-188
                 – M2 J-188
                 – Order date J-188
                 – Order number J-188
                 – Ordered quantity J-188
                 – Thickness of unit J-188
                 – Weight of position J-188
                 – Width of unit J-188
                 Statistics J-210
                 Status
                 – Editable J-144
                 – Name J-144
                 – Status J-144, J-145
                 – Type J-143
                 Status change J-203

                 U
                 Use SQL ERP connection       J-131
                 User J-142
                 – Copy from J-142
                 – ID J-142
                 – Name J-142
                 UserID J-130, J-131

                 V
                 Vehicle
                 – Average consumption J-149
                 – Average costs J-149
2.01 / 01-2017




                 – Brand J-148
                 – Button driver J-150
                 – Chassis number J-149
                 – Code J-150


                 J-227                                                    A+W Business Master Data
                 Index                     Section Index
2.01 / 01-2017




                 J-228   A+W Business Logistic Optimizer

