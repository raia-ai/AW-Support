---
description: "EN AWProduction Rough Scheduling 2.50"
---



# EN AWProduction Rough Scheduling 2.50

Rough Scheduling          C




                           English




               A+W Production
                                                                                                            Introduction




                                       Introduction
                                       This part of the documentation contains editorial notes.


                                       Revision Overview
                                       Part                       Processing
                                       Version / Date

                                       2.50 / 01-2023             Search for document added.

                                       2.01 / 01-2017             Product and company names adjusted.

                                       2.00 / 05-2014             New tutorial and software reference.

                                       1.50 / 08-2013             Complete revision of the ALCIM documentation and
                                                                  adjustment to A+W Production.

                                       1.00 / 03-2006             Original version.



                                       Editorial
                                       This editorial provides information on the following topics:
                                       •   Notes on this document
                                       •   Copyrights
                                       •   Trademarks
                                       •   Contact

                                       Notes on this document
                                       This publication is written exclusively with end users of the A+W Production in
                                       mind.
                                       The documentation and software described are licensed only and must be
                                       used or copied only in accordance with the terms of our license agreement.
                                       The contents of the documentation are for information purposes only and are
                                       subject to changes without prior notice. The text and illustrations were com-
                                       piled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W
                                       Software GmbH cannot be held liable for errors or inaccuracies, unless they
                                       can be attributed to intentional or grossly negligent behavior.
                                       This document describes the full scope of the master data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                     C-3
                 Introduction




                                Copyrights
                                © 2023, A+W Software GmbH, all rights, including the right of reprint, produc-
                                tion of copies and translation, are reserved.
                                The documentation may be copied, completely or in part, saved in an archiving
                                system, or transferred in any other form only in accordance with our license
                                agreement. This documentation may not be transmitted, neither electronically,
                                nor mechanically, nor by recording or in any other way, without the prior written
                                permission from A+W Software GmbH.

                                Trademarks
                                All hardware and software names mentioned in this documentation might also
                                be registered trademarks or other property rights of third parties. Copyrights of
                                third parties must be complied with.

                                Contact
                                A+W Software GmbH
                                Am Pfahlgraben 4 - 10
                                D-35415 Pohlheim
                                Germany
                                    +49 6404 2051 0
                                    +6404 2051 877
                                Zentrale@a-w.com
                                http://www.a-w.com
2.50 / 01-2023




                 C-4                                                       A+W Production Rough Scheduling
                                                                                                                                                       Contents




                                       Contents
                                       Introduction ............................................................................................................. C-3
                                         Revision Overview ............................................................................................... C-3
                                         Editorial ............................................................................................................... C-3
                                       Contents ................................................................................................................. C-5

                                       Tutorial                                                                                                              C-7
                                       Overview ................................................................................................................. C-9
                                        Documentation .................................................................................................. C-10
                                           Tutorial Structure ........................................................................................... C-10
                                           Display Conventions ...................................................................................... C-11
                                       Rough Scheduling ................................................................................................ C-12
                                        Production Preparation Process ........................................................................ C-13
                                        Views ................................................................................................................. C-16
                                           Views in Rough Scheduling ........................................................................... C-17
                                           Configure views, work with views .................................................................. C-19
                                              Create and configure tabs .......................................................................... C-19
                                              Create and configure columns .................................................................... C-21
                                              Create and configure totals row .................................................................. C-24
                                              Define new column or totals row ................................................................ C-26
                                              Create and configure filters ........................................................................ C-28
                                           Exercises: Configure views, work with views ................................................. C-33
                                        Orders / Pool ..................................................................................................... C-34
                                           Orders in Rough Scheduling .......................................................................... C-35
                                        Buckets .............................................................................................................. C-37
                                           Buckets in Rough Scheduling ........................................................................ C-38
                                        Batches and Batch Strategies ........................................................................... C-43
                                           Batches in Rough Scheduling ........................................................................ C-44
                                        Items .................................................................................................................. C-50
                                           Items in Rough Scheduling ............................................................................ C-51
                                        Find Documents ................................................................................................ C-53

                                       Software Reference                                                                                                 C-55
                                       Rough Scheduling ................................................................................................ C-57
                                       Orders in Rough Scheduling ................................................................................. C-58
                                          Orders ............................................................................................................... C-59
                                          Order Overview ................................................................................................. C-62
                                          Filler Orders ....................................................................................................... C-65
                                          Surplus Editor .................................................................................................... C-68
                                          Modification of Procurement Type ..................................................................... C-70
                                       Buckets in Rough Scheduling ............................................................................... C-72
                                          Buckets .............................................................................................................. C-72
                                          Reservation Orders-Bucket ............................................................................... C-75
                                          Purchase Parts Bucket ...................................................................................... C-78
                                          Bucket Creation ................................................................................................. C-81
                                          Edit Bucket Description ..................................................................................... C-83
                                       Batches in Rough Scheduling ............................................................................... C-84
                                          Batches ............................................................................................................. C-84
                                          Batch creation ................................................................................................... C-88
                                          Create Special Glass Batch .............................................................................. C-90
2.50 / 01-2023




                                          Edit Batch Description ....................................................................................... C-91
                                       Items in Rough Scheduling ................................................................................... C-92
                                          Items .................................................................................................................. C-93
                                          Add Order to Items ............................................................................................ C-97



                 A+W Production Rough Scheduling                                                                                                               C-5
                 Contents




                              Split Items .......................................................................................................... C-98
                              Field Definition ................................................................................................. C-100
                              Export/Import Item View .................................................................................. C-102
                            Processings in Rough Scheduling ...................................................................... C-103
                              Processings ..................................................................................................... C-103
                              Change Default Times ..................................................................................... C-106
                            Glass types, Details, Barcoding and Lots ........................................................... C-107
                              Glass Types .................................................................................................... C-107
                              Details ............................................................................................................. C-110
                              Barcoding ........................................................................................................ C-114
                              Lots .................................................................................................................. C-118
                            Overlapping Dialogs ........................................................................................... C-121
                              Work Plan ........................................................................................................ C-122
                              Properties of (tab) ............................................................................................ C-125
                              Column Definition ............................................................................................ C-126
                              (Filter Name) ................................................................................................... C-127
                              Filter Definition ................................................................................................ C-128
                              Links to Documents ......................................................................................... C-130
                              Surface Deletion .............................................................................................. C-131
                            Overlapping Context Menus ............................................................................... C-133

                            Section index                                                                                                  C-137
                            Index ................................................................................................................... C-139
2.50 / 01-2023




                 C-6                                                                           A+W Production Rough Scheduling
Rough Scheduling           E

                       Tutorial




               A+W Production
                 Tutorial                                                                                      Overview




                                       Overview
                                       The tutorial on the Rough scheduling process addresses the batch creation in
                                       A+W Production. With the different views in Rough Scheduling, the persons
                                       responsible for the production preparation process obtain an overview and
                                       create batches with different strategies that allow an optimal production pro-
                                       cess.

                                          The functions depend on the enabled modules
                                          Note that the individual functions are available only if the corresponding
                                          modules and interfaces have been installed and enabled.
                                          If you detect functions in this description which are not available in your ver-
                                          sion, please contact A+W Software GmbH.

                                       Required knowledge
                                       This tutorial is meant for persons in charge of production preparation in A+W
                                       Production who are responsible for organizing the optimum production pro-
                                       cess. Participants must be familiar with the master data concept in A+W Pro-
                                       duction.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                     C-9
                 Overview                                                                                Tutorial




                            Documentation
                            The following documents are available for the Rough Scheduling module:

                            Handout                   Printout of tutorial for training session

                            PDF                       Complete documentation
                                                      • Tutorial
                                                      • Software Reference
                                                      • Index

                            Online help <F1>          Context-sensitive dialog help


                            Tutorial Structure
                            This tutorial consists of sets of topics with several training modules in each.
                            Each module consists of the following elements:

                            Overview                  Each training module starts with an overview of the
                                                      major topics:
                                                      • Objectives: What shall be conveyed?
                                                      • Benefit: What can this knowledge be used for?
                                                      • Maxims: Which correlations are to be remembered?

                            Concepts                  First, the concepts and terms of the corresponding
                                                      training module will be explained. This is followed by
                                                      examples and instructions.

                            Exercises                 There are exercises featuring special tasks for some of
                                                      the training sessions.

                            Cross-references          At the end of each training module there is a section
                                                      with cross references pointing to additional information
                                                      in the software reference and in other sections.
                                                      This will help you to extend your newly acquired
                                                      knowledge.
2.50 / 01-2023




                 C-10                                                   A+W Production Rough Scheduling
                 Tutorial                                                                                        Overview




                                       Display Conventions
                                       Certain parts of sentences are specially marked. The meanings are:

                                       Italics                    Marks character strings describing the software
                                                                  elements, e.g. the Buckets dialog.

                                       Bold                       Marks character strings to be entered via the keyboard,
                                                                  e.g.: Enter the value 0.

                                       >                          Shows the way to open a dialog, e.g. Display > Filler
                                                                  orders > Context menu - List > Order overview.

                                       []                         Square brackets mark buttons in a dialog, e.g. [OK] to
                                                                  save the data.

                                       <>                         Angle brackets refer to keys or shortcuts on the
                                                                  keyboard, e.g. <F1> is used to open the online help.


                                       Reading tip
                                       The content of a training module is based on the knowledge conveyed in the
                                       previous module. We therefore recommend that you do not skip any modules.
                                       If you are already familiar with a subject, read at least the summary at the start
                                       of the module to bring the main details to mind.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                     C-11
                 Rough Scheduling                                                                          Tutorial




                                    Rough Scheduling
                                    This tutorial will show you which sections of A+W Production are part of Rough
                                    Scheduling and how you execute the process.
                                    Different views (display dialogs) provide you with an overview and apply strat-
                                    egies to create batches.
                                    The following chapters are included in Rough Scheduling:
                                    •   “Production Preparation Process” on page C-13
                                    •   “Views” on page C-16
                                    •   “Orders / Pool” on page C-34
                                    •   “Buckets” on page C-37
                                    •   “Batches and Batch Strategies” on page C-43
                                    •   “Items” on page C-50
2.50 / 01-2023




                 C-12                                                        A+W Production Rough Scheduling
                 Tutorial                                                                               Rough Scheduling




                                       Production Preparation Process

                                           ERP System                     Orders / Pool




                                                                                              resolve
                                                                         Batch / Bucket
                                                                           Status: 100




                                                                                              reset
                                                                            Detailed
                                                                           Scheduling
                                                                           Status: 150




                                                                                                          reset
                                                                          Released for
                                                                           production
                                                                           Status: 200




                                                                           Production
                                                                           Status: 300


                                       Fig. C-1     Production Preparation Process


                                       The diagram above shows the production preparation process including rough
                                       scheduling. After scheduling from the ERP system, the orders and/or items are
                                       included in the Pool, i.e. the Orders dialog. You can get an overview by using
                                       the overview dialogs and you can apply strategies to create batches. If you
                                       have created batches you can carry out Detailed Scheduling (rack allocation
                                       and optimization) and subsequently release them for production. The orders
                                       are shown in the views of production preparation during the entire process.
                                       You can also track the statuses of individual orders.
                                       If you resolve batches and buckets, they are returned to the pool. You can re-
                                       set orders from a higher status and carry out new detailed scheduling or create
                                       new batches or buckets.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                   C-13
                 Rough Scheduling                                                                                      Tutorial




                                    Rough Scheduling and Capacity Planning
                                    Some functions of Rough Scheduling interact with Capacity Planning. The cor-
                                    responding points are referred to in this tutorial.
                                    Capacity Planning provides you with a direct access point to Rough Schedul-
                                    ing; from within the Production Monitor you can open the Workplan dialog.
                                    Here you can create and manage batches and order items by taking the re-
                                    sults of capacity planning into account. With active A+W Capacity Planner, we
                                    therefore recommend to start the steps of production preparation from within
                                    the Production Monitor.

                                    Set status
                                    If you are working with A+W Capacity Planner:
                                    If you set the status or orders to produced, ready for shipment, or delivered,
                                    A+W Capacity Planner releases the capacities again. The respective functions
                                    are described in the A+W Capacity Planner manual.

                                    Terms in Rough Scheduling
                                    The following terms are used in the description of Rough Scheduling:

                                    Term                     Description

                                    Orders / Pool            After the order data from the EPR system has been
                                                             scheduled, the orders are listed in the Orders view which is
                                                             also called Pool.

                                    Pool_tables              The database tables Pool_ are filled with data during
                                                             scheduling of the order data from the ERP system.
                                                             Pool_tables describe the BOM and order header of a product.

                                    Bill of material         The BOM shows the elements included in an order in a tree
                                    (BOM)                    structure. The BOM also describes the interdependencies of
                                                             the items.

                                    Item                     Items are parts of orders. An item includes different parts, e.g.
                                                             float 4 mm and therm 4 mm. The parts are subject to different
                                                             kinds of processing, e.g. cutting or polishing.

                                    Processing               Processing procedure with which the item is processed, e.g.
                                                             polishing or grinding.

                                    Work process             Work processes bring together the properties of processing,
                                                             e.g. polishing, with the properties of the work piece. An item
                                                             from the BOM, for example, includes the request to be
                                                             polished in a certain way. Based on this request, the work
                                                             process defines the special type of polishing.

                                    Release parts            Parts that are explicitly to be planned for production. Release
                                                             parts are shown in the views. Release parts are defined in the
                                                             master data.

                                    Non-release parts        Parts that are implicitly to be planned for production. Non-
2.50 / 01-2023




                                                             release parts are defined in the master data.

                                    Tab. C-1           Terms in Rough Scheduling



                 C-14                                                                 A+W Production Rough Scheduling
                 Tutorial                                                                               Rough Scheduling




                                       Term               Description

                                       Batch              Group of orders and/or items that you want to be produced
                                                          together.

                                       Bucket             Repository or buffer in which you manage orders for which the
                                                          further procedure is yet to be clarified.
                                                          For example, you can keep orders in a bucket until there are
                                                          enough items with the same glass type. Subsequently, you
                                                          create a batch from this bucket or buckets.

                                       Lot                Part of a batch that runs through the same production
                                                          processes as a group. A lot can be created simultaneously on
                                                          the same machine with the same tool.

                                       Start date         Date when the production of a batch starts.

                                       Production date    Assembly date of the header part.

                                       Tab. C-1     Terms in Rough Scheduling
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                   C-15
                 Rough Scheduling                                                                                  Tutorial




                                    Views
                                    Objectives

                                    • What are views?
                                    • How are views configured?
                                    • How to work with views.


                                    Benefits

                                    •   Views provide you with an overview of orders and/or items.
                                    •   Views help you decide on a batch strategy.
                                    •   With views you can see the status of orders or items.
                                    •   You edit the orders from within the views, e.g. by creating batches or buckets.


                                    Note

                                    Views                         Overview dialogs in which orders and/or items are
                                                                  displayed grouped by topic, e.g. by orders, processing,
                                                                  or buckets.
2.50 / 01-2023




                 C-16                                                              A+W Production Rough Scheduling
                 Tutorial                                                                            Rough Scheduling




                                       Views in Rough Scheduling




                 Fig. C-2   Orders


                                       The overview dialogs or views are predefined so that you can work with them
                                       directly. You can edit the orders and/or items from within the views, e.g. by cre-
                                       ating batches or buckets. You control the dialogs mainly via context menus.

                                       Configurable components
                                       Most dialogs can be configured so that you can have exactly the information
                                       displayed that you need for your production. In this chapter, you will learn how
                                       to work with overview dialogs and how to configure them.
                                       The following components of the overview dialogs can be configured:
                                       •   Tab
                                       •   Columns
                                       •   Totals row
                                       •   Filter
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                   C-17
                 Rough Scheduling                                                                                            Tutorial




                                             The following dialogs are overviews and described in detail in the Software
                                             Reference:


                 “Orders” on page C-59     The Orders dialog provides you with an overview of all orders that have been scheduled
                                           but not yet processed. From this view, you can further process the orders in the process
                                           of production preparation, e.g. create batches and buckets.

                 “Order Overview” on       The Order Overview dialog provides you with an overview of details in orders. You can
                 page C-62                 sort the order overview by items, parts, or processings. In addition, you can hide or
                                           show the frames or foils. From the Order Overview dialog, you cannot create batches or
                                           buckets.

                 “Filler Orders” on        The Filler Order dialog provides you with an overview of all filler orders. For example,
                 page C-65                 you can use it to display how many items of the filler orders have already been
                                           produced and how many still have to be produced.

                 “Buckets” on page C-72 The Buckets dialog provides you with an overview of buckets in A+W Production. You
                                        can sort the buckets by different criteria and edit them.

                 “Reservation Orders-      The Reservation Orders-Bucket dialog provides you with an overview of reservation
                 Bucket” on page C-75      orders. The dialog serves for overview purposes of scheduled capacities only; you
                                           cannot create any batches or buckets from the dialog.

                 “Purchase Parts Bucket” The Purchase Parts Bucket dialog provides you with an overview of buckets that have
                 on page C-78            been created with purchase parts.

                 “Batches” on page C-84 The Batches dialog provides you with an overview of the created batches.

                 “Items” on page C-93      The Items dialog provides you with an overview of items in the orders.

                 “Processings” on          The Processings dialog provides you with an overview of processings in the orders.
                 page C-103

                 “Glass Types” on          The Glass Types dialog provides you with an overview of the included glass types for
                 page C-107                selected orders or items. You can create a batch.

                 “Details” on page C-110 The Details dialog provides you with details on selected orders, items, parts, batches, or
                                         buckets.
                                           You can open the Details dialog from any view in Rough Scheduling; it is therefore
                                           recommended that you configure this view optimally.

                 “Barcoding” on            The Barcoding dialog provides you with an overview of information relating to
                 page C-114                production data collection.

                 “Lots” on page C-118      The Lots dialog provides you with an overview of the created lots of the selected
                                           batches.

                 “Work Plan” on            The Work Plan dialog provides you with an overview from within the production monitor
                 page C-122                view. The work plan shows you all the planned batches on a machine or in a shift.
2.50 / 01-2023




                 C-18                                                                       A+W Production Rough Scheduling
                 Tutorial                                                                              Rough Scheduling




                                         Configure views, work with views
                                         You can configure views to meet your demands. Compile the most important
                                         information on the first tab of a dialog and let other information follow on other
                                         tabs. Use the views to show as much information as required and as little as
                                         possible to keep dialogs clearly arranged. Add totals rows to obtain a faster
                                         overview. Use filters for specific applications.

                                         Create and configure tabs
                                         Please see the following instructions concerning inserting and configuring
                                         tabs:
                                         •   “How to insert a tab” on page C-19
                                         •   “Configuring a tab” on page C-20


                                          How to insert a tab
                                         1 Open the view in which you want to insert a tab, e.g.
                                           Display > Orders.
                                         2 Open the context menu of the tab next to which the new tab shall be insert-
                                           ed.
                                             Or open the context menu in the head section of the dialog if no tabs exist
                                             yet.




                 Fig. C-3   Orders - Tab context menu
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                     C-19
                 Rough Scheduling                                                                          Tutorial




                                    3 Click Insert in the context menu.




                                       Fig. C-4     Properties of (tab)


                                       The Properties of (tab) dialog opens in which you enter a tab text and a de-
                                       scription. With the System-wide Display checkbox, you can define whether
                                       the tab is displayed to all users or just to you.
                                       The new tab is inserted next to the tab whose context menu you have
                                       opened. You can move a tab by dragging it with the cursor to the required
                                       location.


                                     Configuring a tab
                                    1 Open the view which you want to configure, e.g.
                                      Display > Orders.
                                    2 Open the context menu of the tab you want to edit.
                                    3 The options are:
                                       •   Click Autosave to automatically save all changes to the respective tab.
                                           If you do not select Autosave, you must click Save after every change
                                           to the tab so that all the changes are adopted.




                                       Fig. C-5     Orders - Enabled Autosave


                                           The pound sign next to the name of the tab shows that Autosave has
                                           been enabled.
2.50 / 01-2023




                 C-20                                                           A+W Production Rough Scheduling
                 Tutorial                                                                             Rough Scheduling




                                            •   Click Properties in the context menu of the tab to edit the properties of
                                                a tab.
                                                The Properties of (tab) dialog opens. Here you can edit the tab text and
                                                description. With the System-wide Display checkbox, you can define
                                                whether the tab is displayed to all users or just to you.
                                            •   You can import or export the configured tab and thus use it as a tem-
                                                plate for other dialogs or users.

                                        Create and configure columns
                                        Please see the following instructions concerning inserting and configuring col-
                                        umns:
                                        •   “How to insert a column” on page C-21
                                        •   “Configuring a column” on page C-22


                                         How to insert a column
                                        1 Open the view in which you want to insert a column, e.g.
                                          Display > Orders.
                                        2 Open the context menu of the column next to which the new column shall
                                          be inserted.




                 Fig. C-6   Orders - Column context menu


                                        3 Click Insert in the context menu. Different categories are available for se-
2.50 / 01-2023




                                          lection.
                                            The new column is inserted next to the column whose context menu you
                                            have opened.


                 A+W Production Rough Scheduling                                                                   C-21
                 Rough Scheduling                                                                           Tutorial




                                     Configuring a column
                                    1 Open the view in which you want to configure a column, e.g.
                                      Display > Orders.
                                    2 Open the context menu of the column you want to edit.
                                    3 The options are:
                                       •   Click Resort to sort the respective columns in the reverse order, e.g. by
                                           ascending or descending date.
                                       •   Click Format in the context menu of a column to assign a unit to the col-
                                           umn, e.g. information in millimeters. Different categories are available
                                           for selection.
                                       •   Click Display Definition in the context menu of a column to show details
                                           concerning the column.




                                       Fig. C-7     Column Definition


                                           The Define Columns dialog opens.
                                       •   You can move a column by dragging it to the required location.

                                       Colors in columns
                                       Please contact the Customer Service of A+W Software GmbH if you want
                                       to assign colors to the columns in views.
                                       An entry in the database is required to show columns in different colors.
2.50 / 01-2023




                 C-22                                                         A+W Production Rough Scheduling
                 Tutorial                                                                        Rough Scheduling




                                          How to use the list
                                         1 Open the view with which you want to work, e.g. Display > Orders.
                                         2 Open the context menu of the list.




                 Fig. C-8   Orders - List context menu


                                         3 Select an option from the list.
                                             The context menus are described in the Software Reference.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                               C-23
                 Rough Scheduling                                                                                 Tutorial




                                         Create and configure totals row
                                         Please see the following instructions concerning inserting and configuring to-
                                         tals rows:
                                         •   “How to insert a totals row” on page C-24
                                         •   “Configuring a totals row” on page C-25


                                          How to insert a totals row
                                         1 Open the view in which you want to insert a totals row, e.g. Display > Or-
                                           ders.
                                         2 Open the context menu of the totals row next to which the new totals row
                                           shall be inserted.
                                             Or open the context menu in the field of the totals rows if no totals row ex-
                                             ists yet.




                 Fig. C-9   Orders - Totals row context menu
2.50 / 01-2023




                 C-24                                                               A+W Production Rough Scheduling
                 Tutorial                                                                            Rough Scheduling




                                       3 Select a filter criterion, e.g. Total sum pieces




                                          A



                                          A Inserted totals row
                                          Fig. C-10     Totals row


                                          The totals row is inserted. Any additional totals row is inserted after the to-
                                          tals row in the context menu which you have opened.


                                        Configuring a totals row
                                       1 Open the view in which you want to configure a totals row, e.g. Display >
                                         Orders.
                                       2 Open the context menu of the totals row you want to configure.
                                       3 The options are:
                                          •   Click Format to assign a unit to the totals row, e.g. information in milli-
                                              meters. Different categories are available for selection.
                                          •   Select Display Definition in the context menu to show settings for the to-
                                              tals row.
                                          The Define Columns dialog opens.




                                          Fig. C-11     Column Definition
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                   C-25
                 Rough Scheduling                                                                             Tutorial




                                         Define new column or totals row

                                          How to define columns or totals rows
                                         1 Open the view in which you want to insert a column or totals row, e.g.
                                           Display > Orders.
                                         2 Open the context menu or a column or totals row.




                 Fig. C-12   Orders - Column context menu


                                         3 Click Insert > Field Definitions > Edit in the context menu.




                                             Fig. C-13      Field definition
2.50 / 01-2023




                                             The Field Definition dialog opens.



                 C-26                                                             A+W Production Rough Scheduling
                 Tutorial                                                                           Rough Scheduling




                                       4 Select, in the Menu Group field, the group in the context menu to which you
                                         want to assign the column or totals row, e.g. Accumulated parts.
                                       5 Enter a name for the column or totals row in the Menu Entry field, e.g. Fin-
                                         ished parts.
                                       6 Enter, in the Column Title field, the name of the column or totals row. This
                                         name will be displayed in the dialog, e.g. Finished parts_all.
                                       7 Enter a description for the column or totals row in the Description line, e.g.
                                         Shows all finished parts.
                                       8 Select the format for the column or totals row with the button Format, e.g.
                                         Text.
                                       9 Select an SQL printout that is stored for the column or totals row with the
                                         button Open Selection.
                                          Select the entry SQL printout to enter an individual SQL printout.




                                          Fig. C-14    Field definition


                                       10 Select the display options for the column or totals row, e.g. whether the
                                          sorting of data is in ascending or descending order.
                                       11 Click [Save] to adopt the changes.
                                       12 Click [Close] to close the dialog.
                                          The new column or totals row Finished Parts is now available in the context
                                          menu.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                 C-27
                 Rough Scheduling                                                                           Tutorial




                                                                                        A


                                        A New column
                                        Fig. C-15    Define columns


                                    Create and configure filters
                                    Please see the following instructions concerning selecting, inserting, configur-
                                    ing and defining filters:
                                    •   “How to select a filter” on page C-29
                                    •   “How to add a filter” on page C-30
                                    •   “Configure filters or define new filters” on page C-30
2.50 / 01-2023




                 C-28                                                          A+W Production Rough Scheduling
                 Tutorial                                                                            Rough Scheduling




                                           How to select a filter
                                          1 Open the view in which you want to select a filter, e.g. Display > Orders.
                                          2 Open drop down of a filter to select a filter.




                 Fig. C-16   Orders - Filter drop down menu


                                          3 Select a filter.
                                              Now the view is filtered.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                  C-29
                 Rough Scheduling                                                                         Tutorial




                                     How to add a filter
                                    1 Open the view in which you want to add a filter, e.g. Display > Orders.
                                    2 Click [Add filter] to add a filter.




                                       Fig. C-17     Added filter


                                       A filter has been added.


                                     Configure filters or define new filters
                                    1 Open the view in which you want to configure or define filters, e.g. Display
                                      > Orders.
                                    2 Open the context menu of the filter you want to configure or after which you
                                      want to add a new filter.
                                       The (Filter Name) dialog opens.




                                       Fig. C-18     (Filter Name)


                                    3 Click [Manage].
                                       The Filter Definition dialog opens.
2.50 / 01-2023




                                       Fig. C-19     Filter Definition




                 C-30                                                        A+W Production Rough Scheduling
                 Tutorial                                                                              Rough Scheduling




                                       4 Select a filter from the list if you want to configure it or select New Filter from
                                         the list if you want to define a new filter.
                                          If you are configuring an existing filter, the fields on the right-hand side of
                                          the dialog are already filled and you can carry out the changes. If you define
                                          a new filter you must fill in these fields.
                                       5 Edit the name of the filter in the Name field, e.g. only IG.
                                       6 Enter a description for the filter in the Description field, e.g. Shows only IG
                                         orders.
                                       7 Define a default value in the Standard Parameters field, e.g. default date
                                         which is used when the corresponding database tables or fields do not de-
                                         termine a value.
                                       8 In the Valid for Display field, select the views in which the filter is shown,
                                         e.g. Pool view, Bucket view and Batch view.
                                          The visual appearance of the buttons for the selected dialogs changes.
                                       9 Click [Save] to save the changes for the new filter.
                                          Now you have configured or created the filter and it is available in the re-
                                          spective views.




                                          Fig. C-20     Configured or new filter


                                          You can export or import the filters with the buttons [Export] or
                                          [Import] and thus use them as templates for other dialogs or users.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                      C-31
                 Rough Scheduling                                                                               Tutorial




                                    White screen in a view
                                    If a view does not display any orders and/or items, then either there are none
                                    available or you have set the criteria of the view in a manner that no orders or
                                    items meet the criteria. Examples of possible reasons for blank lists:
                                    •   There is only one column in the view. A category has been defined for this
                                        column that is not included in the orders.
                                        For example, the column shows LAMI, but the orders do not include any
                                        LAMI.
                                        Remedy: Define a criterion in the column that corresponds to the orders.
                                    •   There are several columns in the view. The criteria of the columns restrict
                                        the orders so much that none are shown or the criteria are contradictory.
                                        You have two columns, for example, one of which shows a LAMI and the
                                        other one an IG. Orders that each only include LAMI or IG cannot meet both
                                        criteria at the same time.
                                        Remedy: Define criteria in the columns that correspond to the orders.
                                    •   You have activated a filter, of which the criterion does not correspond to any
                                        order.
                                        For example, the list is blank if the filter only IG is activated and no IG is
                                        included in the orders.
                                        Remedy: Remove the filter or select a different one.
                                    •   You have added a column that filters for batch-related information, for ex-
                                        ample. If you have not yet created a batch for the displayed orders or items,
                                        the column filters non-existing or unauthorized data and the result is a white
                                        screen.
                                        Remedy: Add columns for later work processes in production preparation
                                        only to those views that show later processes of production preparation,
                                        e.g. batch-related data in the Batch view.
2.50 / 01-2023




                 C-32                                                           A+W Production Rough Scheduling
                 Tutorial                                                                           Rough Scheduling




                                       Exercises: Configure views, work with views
                                       The following exercises shall help to strengthen your newly acquired knowl-
                                       edge.
                                       •   Open a view in Rough Scheduling.
                                       •   Enable autosave.
                                       •   Review which information is missing in this view.
                                       •   Create a corresponding tab.
                                       •   Create pertaining columns.
                                       •   Insert a totals row.
                                       •   Add a filter.
                                       •   Define an individual column and/or totals row and insert it into the view.


                                       Additional information
                                        Software Reference, “Rough Scheduling” on page C-57
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                  C-33
                 Rough Scheduling                                                                               Tutorial




                                    Orders / Pool
                                    Objectives

                                    • How to work with the Orders view.


                                    Benefits

                                    • The Orders view provides you with an overview of all the orders that have been
                                      scheduled from the ERP system.
                                    • From the Orders view, you can access other views.


                                    Note

                                    Orders                     After import from the ERP system, orders are shown in
                                                               the Orders dialog.

                                    Pool                       The Orders dialog is also called Pool.

                                    Order overview             The order overview shows the BOM.

                                    Items                      The Items dialog provides you with all details concerning
                                                               items in the orders.

                                    Filler orders              Filler orders are not assigned to any batch and are used
                                                               by Detailed Scheduling to optimize waste.

                                    Surplus                    Edit business- and production-related surpluses in the
                                                               Surplus Editor.
                                                                Software Reference, “Surplus Editor” on page C-68

                                    Change procurement type    In the Modification of Procurement Type dialog you can
                                                               change the procurement type from TG to LAMI.
                                                                Software Reference, “Modification of Procurement
                                                                 Type” on page C-70
2.50 / 01-2023




                 C-34                                                           A+W Production Rough Scheduling
                 Tutorial                                                                           Rough Scheduling




                                       Orders in Rough Scheduling




                 Fig. C-21   Orders


                                       The Orders dialog provides you with an overview of all orders that have been
                                       scheduled but not yet processed. From this view you can further process the
                                       orders in the process of production preparation, e.g. create batches and buck-
                                       ets. The Orders dialog is also called Pool.
                                       Resolved batches and buckets are automatically returned to the Pool. The Or-
                                       ders dialog can be configured.
                                       In the Pool you can open the Order Overview, in which the BOM is shown. You
                                       can open the Surplus Editor, in which you can edit production- and business
                                       related surpluses.
                                       In addition, you can access Rescheduling to Other Machines and Machine Al-
                                       location from the Pool.
                                       The Orders dialog is intended to provide you with an overview of the delivery
                                       data, products and processings that are included in the orders. Keep the Or-
                                       ders dialog as simple and clearly arranged as possible. If you have batched
                                       orders, they are no longer shown in the Pool. You will find these orders in other
                                       views, e.g. in the Batches dialog. Create a tab in the Orders dialog in which
                                       you will find the customer data, e.g. delivery names, delivery addresses and
                                       routes.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                  C-35
                 Rough Scheduling                                                                           Tutorial




                                       Rescheduling to other machines, machine allocation and capacity
                                       planning
                                       If you are working with capacity planning, you must take the following into
                                       account:
                                       A new rescheduling to another machine or machine allocation from within
                                       Rough Scheduling will affect the planned and calculated capacities.
                                       The respective functions are described in the Capacity Planning Manual.

                                    Orders with faulty information
                                    With respect to orders with missing or faulty information, you can either edit
                                    the faulty items or the entire order. Either you delete the respective orders or
                                    items or you move them back to the pool.
                                    Delete faulty items from batches to ensure that they do not remain in the sys-
                                    tem.
2.50 / 01-2023




                 C-36                                                         A+W Production Rough Scheduling
                 Tutorial                                                                              Rough Scheduling




                                       Buckets
                                       Objectives

                                       • What is a bucket?
                                       • How to work with the Buckets view.
                                       • How to create a bucket.


                                       Benefits

                                       • Buckets help you to keep an overview of orders that are not immediately further
                                         processed.
                                       • You can create buffers with buckets, e.g. by collecting orders of the same type.


                                       Note

                                       Bucket                      A bucket is a repository in which you manage orders for
                                                                   which the further procedure is yet to be clarified.

                                       Resolve bucket              Orders from resolved buckets are returned to the pool.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                      C-37
                 Rough Scheduling                                                                             Tutorial




                                       Buckets in Rough Scheduling




                 Fig. C-22   Buckets


                                       The Buckets dialog provides you with an overview of all buckets in Rough
                                       Scheduling. A bucket is a repository or buffer in which you manage orders for
                                       which the further procedure is yet to be clarified. This could be the case, for
                                       example, if you are waiting for order changes or additional panes made of
                                       high-cost glass type.
                                       You can create buckets from almost all overviews or assign orders to existing
                                       buckets. The created buckets are then moved to the Buckets dialog. From
                                       here, you can manage the buckets, e.g. by creating batches or resolving buck-
                                       ets. Orders from resolved buckets are returned to the Pool.
                                       For details on how to work with buckets, please see the following instructions:
                                       •   “How to create a bucket” on page C-39
                                       •   “How to add orders to an existing bucket” on page C-40
                                       •   “How to resolve a bucket” on page C-42
2.50 / 01-2023




                 C-38                                                            A+W Production Rough Scheduling
                 Tutorial                                                                          Rough Scheduling




                                           How to create a bucket
                                          1 Open the view in which you want to create a bucket, e.g. Display > Orders.




                 Fig. C-23   Orders - List context menu


                                          2 Open the context menu of the orders from which you want to create a buck-
                                            et and select Create bucket.
                                              The Create Bucket dialog opens.




                                              Fig. C-24   Create bucket


                                          3 Select the bucket type in the Bucket Type drop down menu.
                                          4 A+W Production creates a new bucket in the Bucket field. Adopt this name
                                            or rename it.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                C-39
                 Rough Scheduling                                                                                     Tutorial




                                          5 Select the production start in the Production Date calendar field.
                                              Please note that a modified production date affects capacity planning.
                                          6 In the Production Shift field, enter the shift in which production shall be
                                            started.
                                              Please note that a modified shift affects capacity planning.
                                          7 In the Article Type Filter field, select whether an article type filter is defined
                                            for the bucket.
                                          8 Select with the Keep Order Together checkbox whether you want the order
                                            to be kept together in production.
                                          9 Click [OK] to save the data.
                                              The bucket has been created and is listed in the Buckets view.


                                           How to add orders to an existing bucket
                                          1 Open the view in which you want to add orders to a bucket, e.g. Display >
                                            Orders.




                 Fig. C-25   Orders - List context menu
2.50 / 01-2023




                 C-40                                                                 A+W Production Rough Scheduling
                 Tutorial                                                                              Rough Scheduling




                                       2 Open the context menu of the orders that you want to add to a bucket and
                                         select Create Bucket.
                                          The Create Bucket dialog opens.




                                          Fig. C-26     Create bucket


                                       3 Select the bucket type in the Bucket Type drop down menu.
                                       4 Select an existing bucket in the Bucket field to add the orders to a bucket.
                                       5 Select the production start in the Production Date calendar field.
                                          Please note that a modified production date affects capacity planning.
                                       6 In the Production Shift field, enter the shift in which production shall be
                                         started.
                                          Please note that a modified shift affects capacity planning.
                                       7 Select in the Article Type Filter field, whether an article type filter is defined
                                         for the bucket.
                                       8 Select with the Keep Order Together checkbox whether you want the order
                                         to be kept together in production.
                                       9 Click [OK] to save the data.
                                          The orders have been added to the bucket.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                     C-41
                 Rough Scheduling                                                                          Tutorial




                                           How to resolve a bucket
                                          1 Select Master Data Display > Buckets.




                 Fig. C-27   Buckets - List context menu


                                          2 Open the context menu of the bucket or buckets you want to resolve and
                                            select Resolve Bucket.
                                              The orders have been returned to the Pool.
2.50 / 01-2023




                 C-42                                                             A+W Production Rough Scheduling
                 Tutorial                                                                                Rough Scheduling




                                       Batches and Batch Strategies
                                       Objectives

                                       •   What is a batch?
                                       •   How to work with the Batches view.
                                       •   How to create a batch.
                                       •   Which strategies are available to schedule a batch?


                                       Benefits

                                       • The Batches view provides you with an overview of all the created batches.
                                       • The Batches view displays the status of the batches.
                                       • In the Batches view you can manage batches e.g. by setting a status, resetting or
                                         resolving batches.
                                       • In the Batches view you can transfer batches to Detailed Scheduling.


                                       Note

                                       Batches                      Batches are a grouping of orders and/or items that are to
                                                                    be processed together in the process of production
                                                                    preparation and production release.

                                                                    Rough scheduling, detailed scheduling, optimization and
                                                                    batch release are executed on the basis of the batches.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                       C-43
                 Rough Scheduling                                                                            Tutorial




                                       Batches in Rough Scheduling




                 Fig. C-28   Batches


                                       The Batches dialog provides you with an overview of all created batches. From
                                       this view you can further process the batches in the process of production
                                       preparation, e.g. by linking or resolving batches or transferring them to De-
                                       tailed Scheduling.
                                       Batches are a grouping of orders and/or items that are to be processed togeth-
                                       er in the process of production preparation and production release. Detailed
                                       scheduling, optimization and batch release are executed on the basis of the
                                       batches.
                                       Resolved batches are automatically returned to the Pool. The Batches dialog
                                       can be configured. For example, you can access Rescheduling to Other Ma-
                                       chines from the Batches dialog.

                                          Rescheduling to other machines, machine allocation and capacity
                                          planning
                                          If you are working with capacity planning you must take the following into
                                          account:
                                          A new rescheduling to another machine or machine allocation from within
                                          Rough Scheduling will affect capacity planning.
                                          The respective functions are described in the Capacity Planning Manual.
2.50 / 01-2023




                 C-44                                                           A+W Production Rough Scheduling
                 Tutorial                                                                             Rough Scheduling




                                       Useful batches and batch strategies
                                       The following applies in general: A batch strategy is good if it works. If you mix
                                       different pane sizes into a batch, the yield is improved. Do not isolate special
                                       products, but include special products in the batches.
                                       You can pursue the following batch strategies:
                                       •   By glass type: You can create separate batches with thick glass panes.
                                           Thick glasses are usually larger in size and thus result in a worse yield; it
                                           may therefore be beneficial to create separate batches and produce thick
                                           glass when it fits best into production.
                                       •   By product type: In the case of more complex productions, e.g. IG, TG or
                                           LAMI, it may be beneficial to compile product types in batches. You will get
                                           a better overview of production and accept a lower yield.
                                       •   By processing: You can compile orders or items to batches on a process-
                                           ing-oriented basis, e.g. to minimize set-up costs and times.
                                       •   By production date: Capacity planning assigns production dates to the in-
                                           dividual processings. You can use those as a basis and create batches
                                           from the respective processings with the same date.
                                       •   By order and/or item: You can create batches from items or individual ele-
                                           ments of orders. In the case of multi-step productions, this strategy will help
                                           you to organize the individual departments. If you need space for changes
                                           you can distribute different product types of an order to several batches.
                                       •   Schedule in several stages: Here, you separate orders and/or items by
                                           your main criteria and check the result. Depending on the yield, quantity,
                                           residual plates and number of required racks, you separate parts into indi-
                                           vidual batches and add parts to the batches.
                                       •   Empty pool: With this strategy you pack new orders and/or items into buck-
                                           ets or batches as fast as possible. The advantage of this strategy is that
                                           you see new orders and/or items immediately when they are moved to the
                                           pool. The disadvantage is that it is more difficult to keep track of existing
                                           buckets and batches.
                                       •   Full pool: You keep orders and/or items in the pool as long as possible. The
                                           advantage of this strategy is that you completely keep track. The disadvan-
                                           tage is that it is more difficult for you to notice new orders and/or items.

                                           Careful with batch strategies
                                           A+W Production gives you complete freedom in planning your production
                                           and consequently full responsibility.
                                           For example, you can ignore results of capacity planning.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                    C-45
                 Rough Scheduling                                                                                  Tutorial




                                          You should not use the following batch strategies:
                                          •   Using today's small sizes to increase today's yield. This strategy results in
                                              problems on the following day.
                                          •   Mixing too many products or glass types into the batches without appropri-
                                              ate organization. This strategy results in an unclear production process and
                                              jams.
                                          •   Default glass quantity too small.
                                          •   Delete batches to accept order modifications. It is better to move items or
                                              batches back to the pool.
                                          For details on how to work with batches, please see the following instructions:
                                          •   “Creating a batch” on page C-46
                                          •   “How to add orders to an existing batch” on page C-48
                                          •   “How to manage batches or resolve batches” on page C-49


                                           Creating a batch
                                          1 Open the view in which you want to create a batch, e.g.
                                            Display > Orders.




                 Fig. C-29   Orders - List context menu
2.50 / 01-2023




                 C-46                                                                A+W Production Rough Scheduling
                 Tutorial                                                                              Rough Scheduling




                                       2 Open the context menu of the orders from which you want to create a batch
                                         and select Create batch.
                                          The Create Batch dialog opens.




                                          Fig. C-30     Create Batch


                                       3 A+W Production automatically creates a new batch number in the Batch
                                         field.
                                       4 Enter the description for the batch in the Description field.
                                       5 Select the production start in the Production Date calendar field.
                                          Please note that a modified production date affects capacity planning.
                                       6 In the Production Shift field, enter the shift in which production shall be
                                         started.
                                          Please note that a modified shift affects capacity planning.
                                       7 In the Article Type Filter field, select whether an article type filter is defined
                                         for the batch.
                                       8 Select with the Keep Order Together checkbox whether you want the order
                                         to be kept together in production.
                                       9 Click [OK] to save the data.
                                          The batch has been created and is listed in the Batches view.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                     C-47
                 Rough Scheduling                                                                            Tutorial




                                           How to add orders to an existing batch
                                          1 Open the view in which you want to add orders to a batch, e.g. Display >
                                            Orders.
                                          2 Open the context menu of the orders that you want to add to a batch and
                                            select Create Batch.




                 Fig. C-31   Orders - List context menu


                                              The Create Batch dialog opens.




                                              Fig. C-32   Create Batch


                                          3 Select an existing batch in the drop down menu to add the orders to a
2.50 / 01-2023




                                            batch.
                                          4 Enter the description for the batch in the Description field.



                 C-48                                                               A+W Production Rough Scheduling
                 Tutorial                                                                                 Rough Scheduling




                                          5 Select the production start in the Production Date calendar field.
                                              Please note that a modified production date affects capacity planning.
                                          6 In the Production Shift field, enter the shift in which production shall be
                                            started.
                                              Please note that a modified shift affects capacity planning.
                                          7 In the Article Type Filter field, select whether an article type filter is defined
                                            for the batch.
                                          8 Select with the Keep Order Together checkbox whether you want the order
                                            to be kept together in production.
                                          9 Click [OK] to save the data.
                                              The orders have been added to the batch.


                                           How to manage batches or resolve batches
                                          1 Select Display > Batches.




                 Fig. C-33   Batches - List context menu


                                          2 Open the context menu of the batch or batches you want to edit or resolve
                                            and select the corresponding option in the context menu.
                                              The batch or the orders can now be seen in the corresponding views.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                        C-49
                 Rough Scheduling                                                                                Tutorial




                                    Items
                                    Objectives

                                    • What are items?
                                    • How to work with the Items view.


                                    Benefits

                                    • The Items view provides you with an overview of all the items in orders.


                                    Note

                                    Items                       Items are parts of orders.
2.50 / 01-2023




                 C-50                                                            A+W Production Rough Scheduling
                 Tutorial                                                                             Rough Scheduling




                                       Items in Rough Scheduling




                 Fig. C-34   Items


                                       The Items dialog provides you with an overview of items of scheduled orders.
                                       The Items dialog can be configured. However, you cannot create batches or
                                       buckets from within the view.
                                       Items are parts of orders. An item includes different parts, e.g. float 4 mm and
                                       therm. 4 mm. The parts are subject to different kinds of processing, e.g. cutting
                                       or polishing.

                                       Split items
                                       The Split Items dialog is used for splitting order items by different criteria. You
                                       can divide items into additional items or create items that include a certain
                                       number of panes. You can furthermore divide items in accordance with pack-
                                       aging optimization.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                    C-51
                 Rough Scheduling                                                                            Tutorial




                                     How to split an item
                                    1 Select Display > Orders > Context menu on selected orders> Processings
                                      > Context menu > Split items.
                                    2 Select the items (A) you want to split in the list Selected Items.




                                       A




                                       B



                                       A Order items                                B Options
                                       Fig. C-35       Split items with selected option


                                    3 Select the option (B) with which you want to execute splitting.
                                    4 Click [Split].
                                       The items have been split and are listed in the New Items field.




                                       Fig. C-36       Split items with new items


                                    5 Click button [End] to close the dialog.
2.50 / 01-2023




                 C-52                                                               A+W Production Rough Scheduling
                 Tutorial                                                                          Rough Scheduling




                                       Find Documents
                                       Edit > Find document




                                       Fig. C-37    Find document


                                       Here, you can search the system for orders and/or quotations. When you open
                                       the dialog, it is empty. Content is only displayed after you have made the ap-
                                       propriate selections and pressed the [Display] button.
                                       In the first step, in the Search by document type area, you specify whether you
                                       want to search for an order, a quotation or both when searching.
                                       Then, in the Search for ... area, you must enter the appropriate document
                                       number (for order or quotation) or the desired customer number.
                                       In the Display by area, you can select whether the display should be sorted by
                                       document number and item or by batches.
                                       In the Display from ... area, you have another opportunity to subdivide the con-
                                       tent displayed. For example, you can use the Parts radio button to display the
                                       appropriate parts numbers. The Batch radio button shows you the entire
                                       batch.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                 C-53
                 Rough Scheduling                            Tutorial
2.50 / 01-2023




                 C-54               A+W Production Rough Scheduling
Rough Scheduling                  E

                   Software Reference




               A+W Production
                 Software Reference                                                                  Rough Scheduling




                                       Rough Scheduling
                                       In Rough Scheduling you create batches that you subsequently plan in detail
                                       and optimize in the process of production preparation. The size and composi-
                                       tion of the batch is decisive for the optimization results and production capacity
                                       utilization.
                                       After scheduling the orders, you will find them in the Orders dialog, also called
                                       Pool. From here you are able to presort the orders into buckets or create
                                       batches directly. The different views help you to obtain an overview of the or-
                                       der data and details. From the views you create batches and transfer these to
                                       the next process step in production preparation: detailed scheduling.
                                       You can adjust the views of Rough Scheduling to your demands so that they
                                       show exactly the information that you require.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                   C-57
                 Orders in Rough Scheduling                                                      Software Reference




                                        Orders in Rough Scheduling
                                        This chapter provides you with information on all the dialogs with which you
                                        can get an overview of orders or order data. You can manage filler orders and
                                        process surplus quantities.
2.50 / 01-2023




                 C-58                                                            A+W Production Rough Scheduling
                 Software Reference                                                        Orders in Rough Scheduling




                                          Orders
                                          Show > Orders




                 Fig. C-38   Orders – Totals (Example)


                                          The Orders dialog provides you with an overview of all orders that have been
                                          scheduled but not yet processed. From this view you can further process the
                                          orders in the process of production preparation, e.g. create batches and buck-
                                          ets and show order details from different perspectives. The Orders dialog is
                                          also called Pool.
                                          You can configure the following components of the Orders dialog as you like:
                                          •   Tab
                                          •   Columns
                                          •   Totals row
                                          •   Filter
                                          You control this dialog mainly via context menus.
                                          The Totals tab includes the following columns, for example:

                                          Delivery date Delivery date for the order.

                                          TG pc Number of TG included in the order.
2.50 / 01-2023




                                          Shp pc Number of shapes included in the order.

                                          Georgian bar pc Number of Georgian bars included in the order.


                 A+W Production Rough Scheduling                                                                  C-59
                 Orders in Rough Scheduling                                                         Software Reference




                                        Georgian bars produced Number of Georgian bars already produced for
                                        the order.

                                        Georgian bars purchased Number of Georgian bars already purchased for
                                        the order.

                                        Qty. triple Quantity of triple IG included in the order.

                                        Qty. stepped IG Quantity of stepped IG included in the order.

                                              Database information from columns
                                              You can open the Column definition dialog by right-clicking on a column
                                              and selecting the option Show definition. In the Column definition dialog
                                              you will find the respective database information of a column.

                                         “Column Definition” on page C-126

                                        Totals row

                                        Qty final product Quantity of selected final products, e.g. IG or LAMI.

                                        IG pc Quantity of selected IG in case of multiple selection.

                                        Only cutting Total of all lites that must be cut.

                                        Filter

                                        [Add filter] Adds a filter.

                                        Drop-down menu The following options are available in the drop-down
                                        menu of the filter:
                                        • Click: Opens the drop-down menu from which you select a filter.
                                        • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                          Filter Definition dialog in which you edit the respective filter.
                                         “Filter Definition” on page C-128

                                        Context menus
                                        Context menus are offered in the following sections of the Orders dialog:
                                        •     Tab
                                        •     Columns
                                        •     List
                                        •     Totals row
                                        •     Filter
                                        Context menus that appear in the entire area of production preparation are list-
                                        ed in the chapter Overlapping Context Menus.
                                         “Overlapping Context Menus” on page C-133
2.50 / 01-2023




                 C-60                                                               A+W Production Rough Scheduling
                 Software Reference                                                         Orders in Rough Scheduling




                                         Group       Path                 Remark

                                         List        Work plan >          Opens the Rescheduling dialog to reschedule to
                                                     Rescheduling to      other machines.
                                                     other machines
                                                                           Capacity Planning: Software Reference,
                                                                            “Machine Reallocation” on page K-183
                                                                          The results of the machine allocation within the
                                                                          scope of scheduling are overwritten.

                                                     Work plan >          Carries out the machine allocation for selected
                                                     Machine allocation   orders again.
                                                                          The results of the machine allocation within the
                                                                          scope of scheduling are overwritten.

                                                     Work plan >          Currently not being used.
                                                     Recalculate work
                                                     plan

                                                     Change               Opens the Change procurement type dialog.
                                                     procurement type
                                                                           “Modification of Procurement Type” on
                                                                            page C-70
                                                                          The option only works with TG and LAMI.

                 Tab. C-2   Orders, context menus

                                         Buttons

                                         [Batch] Creates a batch from selected orders, items or parts.

                                         [Glass types] Shows the glass types for the selected orders.

                                         [Details] Shows the details for the selected orders.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                      C-61
                 Orders in Rough Scheduling                                                          Software Reference




                                          Order Overview
                                          Display > Orders > Context menu – List > Processings > Context menu – List
                                          > Order Overview
                                          Display > Orders > Context menu – List > Glass types > Context menu – List
                                          > Order Overview
                                          Display > Orders > Context menu – List > Details > Context menu – List > Or-
                                          der Overview
                                          Display > Buckets > Context menu – List > Order Overview
                                          Display > Batches > Context menu – List > Order Overview
                                          Display > Filler orders > Context menu – List > Order Overview




                 Fig. C-39   Order Overview, sorted by processings (example)


                                          The Order Overview dialog provides you with an overview of details in orders.
                                          You can sort the order overview by items, parts or processings. In addition, you
                                          can hide or show the spacers or foils.
                                          From the Order Overview dialog you cannot create batches or buckets.
2.50 / 01-2023




                                          In the Order Overview dialog you can adapt tabs and columns to fit your needs
                                          so that exactly the required information is shown.
                                          You control this dialog mainly via context menus.

                 C-62                                                               A+W Production Rough Scheduling
                 Software Reference                                                     Orders in Rough Scheduling




                                       [Autosave] Activates automatic saving.

                                       [Save] Saves the current data.

                                       [System-wide display] Changes in the Order Overview dialog are saved
                                       system-wide.
                                       The Order Overview dialog includes the following information, for example:

                                       Order Order for which the details are shown.

                                       [Items] Sorts the view by items.

                                       [Parts] Sorts the view by parts.

                                       [Processings] Sorts the view by processings.

                                       Show frames, foils Checkbox with the following functions:
                                        Processings that include frames and foils are not shown.
                                        Processings that include frames and foils are shown.

                                       Item Item number of the order item.

                                       Name Article or order item.

                                       Size Size of the lites.

                                       Quantity Number of articles.

                                       Machine Machine used for this processing.

                                       Prod. Date Date when this processing will be executed.

                                       Prod. Quantity Number of lites already produced.

                                       Batch Batch allocated to the processing.

                                       Procurement type Procurement type allocated to the article.

                                       Shape number Shape number of the lite.

                                       Processing text Remarks about the processing.

                                          Database information from columns
                                          You can open the Column definition dialog by right-clicking on a column
                                          and selecting the option Show definition. In the Column definition dialog
                                          you will find the respective database information of a column.

                                        “Column Definition” on page C-126
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                               C-63
                 Orders in Rough Scheduling                                                               Software Reference




                                         Context menus
                                         Context menus are offered in the following sections of the Order Overview di-
                                         alog:
                                         •    Button bar
                                         •    Header
                                         •    Columns
                                         Context menus that appear in the entire area of production preparation are list-
                                         ed in the chapter Overlapping Context Menus.
                                          “Overlapping Context Menus” on page C-133


                                         Group         Path                  Remark

                                         Header        Formatting            Select format or unit for the columns in the
                                                                             header, e.g. date format or length unit.

                                                       Insert                Inserts a new column in the header. Different
                                                                             categories are available.

                                                       Delete                Deletes a selected column.

                                                       Display definition    Opens the Column Definition dialog.
                                                                              “Column Definition” on page C-126

                                         Columns       Formatting            Select format or unit for the columns in the list,
                                                                             e.g. date format or length unit.

                                                       Insert > Processing   Inserts a new column with processing data.
                                                       data                  Different categories are available.

                                                       Insert > BOM data     Inserts a new column with BOM data. Different
                                                                             categories are available.

                                                       Delete                Deletes a selected column.

                                                       Display definition    Opens the Column Definition dialog that shows
                                                                             details concerning the respective column.
                                                                              “Column Definition” on page C-126

                 Tab. C-3   Order overview, context menus
2.50 / 01-2023




                 C-64                                                                  A+W Production Rough Scheduling
                 Software Reference                                                         Orders in Rough Scheduling




                                           Filler Orders
                                           Display > Filler order




                 Fig. C-40   Filler orders (example)


                                           The Filler Order dialog provides you with an overview of all filler orders. For
                                           example, you can use it to display how many items of the filler orders have al-
                                           ready been produced and how many still have to be produced.
                                           You can configure the following components of the Filler Orders dialog as you
                                           like:
                                           •   Tab
                                           •   Columns
                                           •   Totals row
                                           •   Filter
                                           You control this dialog mainly via context menus.
                                           The Filler Order dialog includes the following columns, for example:

                                           Order Order number for the corresponding order.

                                           Itm (int Itm) Internal A+W Production sub-item, assigned, for example, after
                                           an item split.
2.50 / 01-2023




                                           Article description Name of the article included in the order.




                 A+W Production Rough Scheduling                                                                    C-65
                 Orders in Rough Scheduling                                                         Software Reference




                                        Produced quantity Number of already produced items in the corresponding
                                        order.

                                              Database information from columns
                                              You can open the Column definition dialog by right-clicking on a column
                                              and selecting the option Show definition. In the Column definition dialog
                                              you will find the respective database information of a column.

                                         “Column Definition” on page C-126

                                        Totals row

                                        Qty final product Quantity of selected final products, e.g. IG or LAMI.

                                        IG pc Quantity of selected IG.

                                        Only cutting Number of selected lites that must be cut.

                                        Filter

                                        [Add filter] Adds a filter.

                                        Drop-down menu The following options are available in the drop-down
                                        menu of the filter:
                                        • Click: Opens the drop-down menu from which you select a filter.
                                        • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                          Filter Definition dialog in which you edit the respective filter.
                                         “Filter Definition” on page C-128

                                        Context menus
                                        Context menus are offered in the following sections of the Filler Orders dialog:
                                        •     Tab
                                        •     Columns
                                        •     List
                                        •     Totals row
                                        •     Filter
                                        Context menus that appear in the entire area of production preparation are list-
                                        ed in the chapter Overlapping Context Menus.
                                         “Overlapping Context Menus” on page C-133
2.50 / 01-2023




                 C-66                                                               A+W Production Rough Scheduling
                 Software Reference                                                               Orders in Rough Scheduling




                                          Group            Path                 Remark

                                          List             Work plan >          Opens the Rescheduling dialog to reschedule to
                                                           Rescheduling to      other machines.
                                                           other machines
                                                                                The results of the machine allocation within the
                                                                                scope of scheduling are overwritten.

                                                           Work plan >          Carries out the machine allocation for selected
                                                           Machine allocation   orders or items again.
                                                                                The results of the machine allocation within the
                                                                                scope of scheduling are overwritten.

                                                           Work plan >          Currently not being used.
                                                           Recalculate work
                                                           plan

                                                           Change               Opens the Change procurement type dialog.
                                                           procurement type
                                                                                 “Modification of Procurement Type” on
                                                                                  page C-70
                                                                                The option only works with TG and LAMI.

                 Tab. C-4   Filler Orders, context menus

                                          Buttons

                                          [Batch] Creates a batch from selected orders, items or parts.

                                          [Glass types] Shows the glass types for the selected orders.

                                          [Details] Shows the details for the selected orders.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                            C-67
                 Orders in Rough Scheduling                                                            Software Reference




                                              Surplus Editor
                                              Display > Orders > Context menu – List > Reentry > Surplus




                 Fig. C-41   Surplus Editor


                                              Use the Surplus Editor to edit business- and production-related surpluses in
                                              orders.

                                              Order items

                                              Order Number of order.

                                              Itm Number of items included in the order.

                                              Product Product name from the product master data.

                                              Quantity according to order Quantity specified in the purchase order.

                                              Surplus Business-related surplus that can be changed if required.
2.50 / 01-2023




                 C-68                                                                  A+W Production Rough Scheduling
                 Software Reference                                                    Orders in Rough Scheduling




                                       Excess Quantity Production-related excess quantity that can be changed if
                                       required.

                                       Total quantity Total quantity of the items after you changed the surpluses
                                       and excess quantities.

                                       Overview
                                       Display of the lite structure.

                                       Shape
                                       Display of the selected product's shape.

                                       Buttons

                                       [Save] Saves the data.

                                       [Close] Closes the dialog without saving the data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                              C-69
                 Orders in Rough Scheduling                                                       Software Reference




                                          Modification of Procurement Type
                                          Display > Orders > Context menu – List > Modify procurement type
                                          Display > Filler ord. > Context menu – List > Modify procurement type




                 Fig. C-42   Modification of procurement type


                                          In the Modification of Procurement Type dialog you can change the procure-
                                          ment type of TG and LAMI.

                                          Modifiable parts

                                          List of parts for which you can change the procurement type.

                                          Details

                                          Order number Order number of the selected part.

                                          Item number Item number of the selected part.
2.50 / 01-2023




                                          Article description Description of the selected part.




                 C-70                                                             A+W Production Rough Scheduling
                 Software Reference                                                      Orders in Rough Scheduling




                                       Pcs Number of parts included.

                                       Production date Production start date of parts.

                                       Current procurement type Currently defined procurement type.

                                       Structure Lites included for which you can change the procurement type.

                                       [Arrow down] Moves selected parts to the Selected Parts field.

                                       [Arrow up] Moves selected parts back to the Modifiable Parts field.

                                       Selected parts
                                       List of selected parts.

                                       Selection of new procurement type
                                       Selection of new procurement type. Select from Cutting, Production, P.O. or
                                       Stock Withdrawal.

                                       [Execute] Executes the change of the procurement type.

                                       [Close] Closes the dialog without saving the data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                             C-71
                 Buckets in Rough Scheduling                                                      Software Reference




                                          Buckets in Rough Scheduling
                                          This chapter provides you with information on all the dialogs with which you
                                          can get an overview of buckets. You can create and edit buckets and manage
                                          reserved orders.


                                          Buckets
                                          Display > Buckets




                 Fig. C-43   Buckets – Buckets (example)


                                          The Bucket dialog provides you with an overview of buckets in A+W Produc-
                                          tion. You can sort the buckets by different criteria and edit them.
                                          You can configure the following components of the Buckets dialog as you like:
                                          •   Tab
                                          •   Columns
                                          •   Totals row
                                          •   Filter
                                          You control this dialog mainly via context menus.
                                          The Buckets tab includes the following columns, for example:

                                          Bucket Name of bucket.
2.50 / 01-2023




                                          Description Description of the bucket.

                                          Orders Number of orders included in the respective bucket.


                 C-72                                                              A+W Production Rough Scheduling
                 Software Reference                                                     Buckets in Rough Scheduling




                                       Items Number of items included in the respective bucket.

                                       IG Number of IG included in the respective bucket.

                                       LAMI Number of LAMI included in the respective bucket.

                                       TG Number of TG included in the respective bucket.

                                       Shapes Number of shapes included in the respective bucket.

                                           Database information from columns
                                           You can open the Column definition dialog by right-clicking on a column
                                           and selecting the option Show definition. In the Column definition dialog
                                           you will find the respective database information of a column.

                                        “Column Definition” on page C-126

                                       Totals row

                                       Total area Total area of all items.

                                       IG total Number of IG included.

                                       TG pcs Number of TG included.

                                       Filter

                                       [Add filter] Adds a filter.

                                       Drop-down menu The following options are available in the drop-down
                                       menu of the filter:
                                       • Click: Opens the drop-down menu from which you select a filter.
                                       • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                         Filter Definition dialog in which you edit the respective filter.
                                        “Filter Definition” on page C-128

                                       Context menus
                                       Context menus are offered in the following sections of the Buckets dialog:
                                       •   Tab
                                       •   Columns
                                       •   List
                                       •   Totals row
                                       •   Filter
                                       Context menus that appear in the entire area of production preparation are list-
                                       ed in the chapter Overlapping Context Menus.
                                        “Overlapping Context Menus” on page C-133
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                 C-73
                 Buckets in Rough Scheduling                                                      Software Reference




                                         Group       Path                Remark

                                         List        Resolve bucket      Resolves the selected buckets and moves the
                                                                         included orders back to the Orders dialog



                 Tab. C-5   Buckets, context menus

                                         Buttons

                                         [Batch] Creates a batch from selected orders, items or parts.

                                         [Glass types] Shows the glass types for the selected buckets.

                                         [Details] Shows the details for the selected buckets.
2.50 / 01-2023




                 C-74                                                             A+W Production Rough Scheduling
                 Software Reference                                                       Buckets in Rough Scheduling




                                          Reservation Orders-Bucket
                                          Display > Reservation orders




                 Fig. C-44   Reservation Orders-Bucket (example)


                                          Use the Reservation Orders-Bucket to display reservation orders. The dialog
                                          serves for overview purposes of scheduled capacities only; you cannot create
                                          any batches or buckets from the dialog.
                                          The Reservation Orders-Bucket dialog is not activated by default in A+W Pro-
                                          duction. You must activate the dialog view before you can use it.
                                          In the Reservation Orders-Bucket dialog you can adapt tabs and columns to
                                          fit your needs so that exactly the information that you require is shown.
                                          The Reservation Orders-Bucket dialog includes the following columns, for ex-
                                          ample:

                                          Order number Specifies the order number.

                                          Batch number Specifies the batch number.

                                          Delivery date Specifies the delivery date.

                                             Database information from columns
                                             You can open the Column definition dialog by right-clicking on a column
                                             and selecting the option Show definition. In the Column definition dialog
                                             you will find the respective database information of a column.

                                           “Column Definition” on page C-126
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                  C-75
                 Buckets in Rough Scheduling                                                           Software Reference




                                         Totals row

                                         Pcs Number of items of the orders shown in the dialog.

                                         Filter

                                         [Add filter] Adds a filter.

                                         Drop-down menu The following options are available in the drop-down
                                         menu of the filter:
                                         • Click: Opens the drop-down menu from which you select a filter.
                                         • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                           Filter Definition dialog in which you edit the respective filter.
                                          “Filter Definition” on page C-128

                                         Context menus
                                         Context menus are offered in the following sections of the Glass Types dialog:
                                         •   Columns
                                         •   List
                                         •   Totals row
                                         •   Filter
                                         Context menus that appear in the entire area of production preparation are list-
                                         ed in the chapter Overlapping Context Menus.
                                          “Overlapping Context Menus” on page C-133


                                         Group        Path                 Remark

                                         Columns      Re-sorting           Sort column in ascending or descending order.
                                                                           Affects the first three columns in the dialog.

                                                      Formatting           Select format or unit for the columns, e.g. date
                                                                           format or length unit.

                                                      Insert               Inserts a new column. Different categories are
                                                                           available.

                                                      Insert > Field       Opens the Field Definition dialog in which you
                                                      definitions > Edit   can formulate queries in database tables and
                                                                           fields. These queries can then be inserted, e.g.
                                                                           part-, item- or order-related as a column.
                                                                            “Field Definition” on page C-100

                                                      Insert > Field       Opens the Import Field Definitions dialog.
                                                      definitions > Import

                                                      Insert > Field       Opens the Export Field Definitions dialog with
                                                      definitions > Export which you can export field definitions.
2.50 / 01-2023




                                                      Delete               Deletes the selected column.

                 Tab. C-6   Reservation Orders-Bucket, context menus




                 C-76                                                                A+W Production Rough Scheduling
                 Software Reference                                                          Buckets in Rough Scheduling




                                         Group        Path                 Remark

                                                      Change               Currently not being used.

                                                      Display definition   Opens the Column Definition dialog that shows
                                                                           details concerning the respective column.
                                                                            “Column Definition” on page C-126

                                         List         Order overview       Opens the Order Overview dialog
                                                                            “Order Overview” on page C-62


                                                      Items                Opens the Items dialog.
                                                                            “Items” on page C-93

                                         Totals row   Re-sorting           Currently not being used.

                                                      Formatting           Select format or unit for the columns, e.g. date
                                                                           format or length unit.

                                                      Insert               Inserts a new field in the totals row. Different
                                                                           categories are available.

                                                      Insert > Field       Opens the Field Definition dialog in which you
                                                      definitions > Edit   can formulate queries in database tables and
                                                                           fields. These queries can then be inserted, e.g.
                                                                           part-, item- or order-related.
                                                                            “Field Definition” on page C-100

                                                      Insert > Field       Opens the Import Field Definitions dialog.
                                                      definitions > Import

                                                      Insert > Field       Opens the Export Field Definitions dialog with
                                                      definitions > Export which you can export field definitions.

                                         Filter                            Opens the dialog (Filter Name). The [Manage]
                                                                           button opens the Filter Definition dialog in which
                                                                           you can edit filters.
                                                                            “Filter Definition” on page C-128

                 Tab. C-6   Reservation Orders-Bucket, context menus

                                         Buttons

                                         [Batch creation] Currently not active.

                                         [Glass types] Currently not active.

                                         [Details] Currently not active.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                          C-77
                 Buckets in Rough Scheduling                                                        Software Reference




                                          Purchase Parts Bucket
                                          Display > Purchase Parts Bucket




                 Fig. C-45   Purchase Parts Bucket (example)


                                          The Purchase Parts Bucket dialog provides you with an overview of buckets
                                          that have been created with purchase parts.
                                          In the Purchase Parts Bucket dialog you can adapt tabs and columns to fit your
                                          needs so that exactly the information that you require is shown.
                                          You control this dialog mainly via context menus.
                                          The Purchase Parts Bucket dialog includes the following columns, for exam-
                                          ple:

                                          Order Number of order.

                                          Article Article number.

                                          Delivery date Date of the delivery.

                                          Article description Article name.
2.50 / 01-2023




                 C-78                                                              A+W Production Rough Scheduling
                 Software Reference                                                     Buckets in Rough Scheduling




                                           Database information from columns
                                           You can open the Column definition dialog by right-clicking on a column
                                           and selecting the option Show definition. In the Column definition dialog
                                           you will find the respective database information of a column.

                                        “Column Definition” on page C-126

                                       Totals row

                                       Total pcs Total of all parts in the selected orders or items.

                                       Total duration Total processing duration of the selected orders or items. Unit:
                                       hours.

                                       Filter

                                       [Add filter] Adds a filter.

                                       Drop-down menu The following options are available in the drop-down
                                       menu of the filter:
                                       • Click: Opens the drop-down menu from which you select a filter.
                                       • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                         Filter Definition dialog in which you edit the respective filter.
                                        “Filter Definition” on page C-128

                                       Context menus
                                       Context menus are offered in the following sections of the Purchase Parts
                                       Bucket dialog:
                                       •   Tab
                                       •   Columns
                                       •   List
                                       •   Totals row
                                       •   Filter
                                       Context menus that appear in the entire area of production preparation are list-
                                       ed in the chapter Overlapping Context Menus.
                                        “Overlapping Context Menus” on page C-133
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                 C-79
                 Buckets in Rough Scheduling                                                           Software Reference




                                         Group        Path                 Remark

                                         List         Move to pool         Moves the selected orders back to the Orders
                                                                           dialog and thus into the status prior to Rough
                                                                           Scheduling.
                                                                            “Orders” on page C-59

                                                      Work plan >          Carries out the machine allocation for selected
                                                      Machine allocation   orders again.
                                                                           The results of the machine allocation within the
                                                                           scope of scheduling are overwritten.

                                                      Work plan >          Currently not active.
                                                      Recalculate work
                                                      plan

                                                      Purchase orders      Currently not active.
                                                      for subsequent
                                                      parts > Trigger

                                                      Purchase orders      Currently not active.
                                                      for subsequent
                                                      parts > Do not
                                                      trigger



                 Tab. C-7   Purchase Parts Bucket, context menus

                                         Buttons

                                         [Batch] Creates a batch from selected purchase parts.

                                         [Glass types] Currently not active.

                                         [Details] Currently not active.
2.50 / 01-2023




                 C-80                                                                A+W Production Rough Scheduling
                 Software Reference                                                     Buckets in Rough Scheduling




                                       Bucket Creation
                                       Display > Orders > Context menu – List > Create bucket
                                       Display > Buckets > Context menu – List > Create bucket
                                       Display > Batches > Context menu – List > Create bucket
                                       Display > Filler orders > Context menu – List > Create bucket
                                       Glass types > Context menu – List > Create bucket
                                       Processing > Context menu – List > Create bucket
                                       Details > Context menu – List > Create bucket




                                       Fig. C-46    Bucket creation


                                       Use the Create Bucket dialog to create a bucket. It is shown in the Buckets di-
                                       alog. You can use buckets as intermediate storage, e.g. if there isn't a suffi-
                                       cient number or orders of the same type available.

                                       Bucket type Selection of the bucket type:
                                       • Normal
                                       • Purchase part bucket

                                       Bucket You can create a new bucket or add the order to an existing bucket.
                                       • If you do not change anything, a new bucket is created.
                                       • If you select a bucket from the selection list, the order is added to an exist-
                                         ing bucket.

                                       Description Name of bucket.

                                       Production date Selection of production date for the batch.

                                       Production shift Specifies the shift in which the batch should be started.
2.50 / 01-2023




                                       Article type filter Selection of the parts for which you are creating a bucket.
                                       The following ones are available: Georgian bars, Foil, Frame or Other Non-
                                       Glass Articles.


                 A+W Production Rough Scheduling                                                                  C-81
                 Buckets in Rough Scheduling                                                       Software Reference




                                        For further processing, the parts must have been created in the article master
                                        data as release parts.

                                        Keep order together You can keep the order items together. This means, all
                                        items (including those that have not specifically been selected) are run through
                                        the production together. This ensures that no items of the order are forgotten.
                                        The order items are not kept together.
                                        The order items are kept together.

                                        [OK] Saves the data.

                                        [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 C-82                                                             A+W Production Rough Scheduling
                 Software Reference                                                   Buckets in Rough Scheduling




                                       Edit Bucket Description
                                       Display > Buckets > Context menu – List > Change text




                                       Fig. C-47   Edit bucket description


                                       Use the Edit Bucket Description dialog to change the description, production
                                       date and production shift of a bucket.

                                       Bucket Name of bucket.

                                       Description Name of bucket.

                                       Production date Selection of the production start for the bucket.

                                       Production shift Specifies the shift in which the bucket should be started.

                                       [OK] Saves the data.

                                       [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                              C-83
                 Batches in Rough Scheduling                                                        Software Reference




                                         Batches in Rough Scheduling
                                         This chapter provides you with information on all the dialogs with which you
                                         can get an overview of batches. You can create and edit batches, create spe-
                                         cial glass batches and release batches that are thus released for production.


                                         Batches
                                         Display > Batches




                 Fig. C-48   Batches (example)


                                         The Batches dialog provides you with an overview of the created batches.
                                         Batches are a grouping of orders or items that are to be processed together in
                                         the process of production preparation and production release. Rough sched-
                                         uling, detailed scheduling, optimization and batch release are executed on the
                                         basis of the batches.
                                         You can sort the batches by different criteria and edit them. You control this
                                         Batches dialog mainly via context menus. You can configure the following
                                         components of the Batches dialog as you like:
                                         •   Tab
                                         •   Columns
2.50 / 01-2023




                                         •   Totals row
                                         •   Filter



                 C-84                                                              A+W Production Rough Scheduling
                 Software Reference                                                       Batches in Rough Scheduling




                                       The Batches tab includes the following columns, for example:

                                       Batch Name of batch.

                                       Status Batch status.

                                       Number Number of orders included in the respective batch.

                                       Shapes Number of shapes included in the respective batch.

                                       Description Description of the batch.

                                          Database information from columns
                                          You can open the Column definition dialog by right-clicking on a column
                                          and selecting the option Show definition. In the Column definition dialog
                                          you will find the respective database information of a column.

                                        “Column Definition” on page C-126

                                       Totals row
                                       You can display different totals in the totals row, e.g. the following information:

                                       Shapes Total of all shapes in the orders or items.

                                       Total duration Total processing duration of the selected orders or items. Unit:
                                       hours.

                                       Total pcs Total of all parts in the selected orders or items.

                                       Filter

                                       [Add filter] Adds a filter.

                                       Drop-down menu The following options are available in the drop-down
                                       menu of the filter:
                                       • Click: Opens the drop-down menu from which you select a filter.
                                       • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                         Filter Definition dialog in which you edit the respective filter.
                                        “Filter Definition” on page C-128
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                    C-85
                 Batches in Rough Scheduling                                                           Software Reference




                                         Context menus
                                         Context menus are offered in the following sections of the Batches dialog:
                                         •   Tab
                                         •   Columns
                                         •   List
                                         •   Totals row
                                         •   Filter
                                         Context menus that appear in the entire area of production preparation are list-
                                         ed in the chapter Overlapping Context Menus.
                                          “Overlapping Context Menus” on page C-133


                                         Group        Path                 Remark

                                         List         Release batch        Release selected batches for production.




                                                      Manage batch >       Batch status is reset.
                                                      Reset batch

                                                      Manage batch >       The batch is resolved. The order data is
                                                      Resolve batch        returned to the pool.

                                                      Manage batch >       The batch is archived.
                                                      Archive batch
                                                                           The archive view is created by a service from
                                                                           A+W Software GmbH

                                                      Manage batch >       Opens the Set status dialog where you can
                                                      Set status           select the status of the batch.
                                                                           •   in production
                                                                           •   produced
                                                                           •   ready for shipment
                                                                           •   delivered

                                                      Detailed             Transfers the batch to Detailed Scheduling and
                                                      scheduling           opens the Detailed Scheduling for Batch (name)
                                                                           dialog

                                                      Georgian bars print Starts printing of production papers for Georgian
                                                                          bars.

                                                      Georgian bars        Transfers production data for Georgian bars to
                                                      machine control      the respective machines.

                                                      Rescheduling to      Opens the Rescheduling dialog to reschedule to
                                                      other machines       other machines.
                                                                           
                                                                           The results of the machine allocation within the
                                                                           scope of scheduling are overwritten.
2.50 / 01-2023




                 Tab. C-8   Batches, context menus




                 C-86                                                                A+W Production Rough Scheduling
                 Software Reference                                                   Batches in Rough Scheduling




                                       Buttons

                                       [Release] Releases the selected batches for production.

                                       [Detailed Sched.] Transfers the selected batch to Detailed Scheduling and
                                       opens the Detailed Scheduling for Batch (name) dialog.

                                       [Glass types] Shows the glass types for the selected batches.

                                       [Details] Shows the details for the selected batches.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                           C-87
                 Batches in Rough Scheduling                                                         Software Reference




                                        Batch creation
                                        Display > Orders > [Batch]
                                        Display > Buckets > [Batch]
                                        Display > Batches > Context menu – List > Batch
                                        Display > Filler orders > [Batch]
                                        Glass types > [Batch]
                                        Processings > [Batch]
                                        Details > [Batch]
                                        Lots > [Batch]
                                        Barcoding > [Batch]
                                        You can also open the Batch Creation dialog by using the context menu.




                                        Fig. C-49    Batch creation


                                        Use the Batch Creation dialog to create a batch or add orders to an existing
                                        batch. The batch is then shown in the Batches dialog.
                                         “Batches” on page C-84

                                        Batch You can create a new batch or add the order to an existing batch.
                                        • If you do not change anything, a new batch is created.
                                        • If you select a batch from the selection list, the order is added to an existing
                                          batch.

                                        Description Name of batch.

                                        Detailed scheduling organization Defines which rack organization shall be
                                        used for optimizing the batch. You can change this default setting during the
2.50 / 01-2023




                                        work step Detailed Scheduling.




                 C-88                                                              A+W Production Rough Scheduling
                 Software Reference                                                     Batches in Rough Scheduling




                                       Use selected organization as default Use rack organization selected in the
                                       Detailed Scheduling Organization field as the default.
                                       Rack organization selected will not be used as the default.
                                       Rack organization selected will be used as the default.

                                       Production date Here, you select a production start date for the batch.
                                       If you work with A+W Capacity Planner, you can confirm the calculated start
                                       date or specifically change it.

                                       Production shift Specifies in which shift the production of the batch is start-
                                       ed.

                                       Article type filter You can create special batches for Georgian bars, IG
                                       frames, LAMI foil and other non-glass articles. The batches are only created
                                       from the selected article types.
                                       For this option, the article types in the article master data must be defined as
                                       released parts.

                                       Keep order together You can keep the order items together. This means, all
                                       items (including those that have not specifically been selected) are run through
                                       the production together. This ensures that no items of the order are forgotten.
                                       The order items are not kept together.
                                       The order items are kept together.

                                       [OK] Saves the data.

                                       [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                 C-89
                 Batches in Rough Scheduling                                                        Software Reference




                                        Create Special Glass Batch
                                        Glass types > Context menu – List > Special glass > Add




                                        Fig. C-50    Create Special Glass Batch


                                        Use the Create Special Glass Batch to specifically create batches for special
                                        glass.

                                        Special glass batch You can either create a new special glass batch or add
                                        the order to an existing special glass batch.
                                        • If you do not change anything, a new special glass batch is created.
                                        • If you select a special glass batch from the selection list, the order is added
                                           to an existing batch.

                                        Description Name of the new special glass batch.

                                        Detailed scheduling organization Selection of racks for the special glass
                                        batch.

                                        Production date Selection of production date for the batch.

                                        Production shift Specifies the shift in which the batch should be started.

                                        [OK] Saves the data.

                                        [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 C-90                                                              A+W Production Rough Scheduling
                 Software Reference                                                   Batches in Rough Scheduling




                                       Edit Batch Description
                                       Display > Batches > Context menu – List > Change text




                                       Fig. C-51   Edit Batch Description


                                       Use the Edit Batch Description dialog to change the description, production
                                       date and production shift of a batch.

                                       Batch Selected batch.

                                       Name Name of batch.

                                       Production date Selection of production date for the batch.

                                       Production shift Selection of the shift in which the batch should be started.

                                       [OK] Saves the data.

                                       [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                               C-91
                 Items in Rough Scheduling                                                       Software Reference




                                        Items in Rough Scheduling
                                        This chapter provides you with information on all the dialogs with which you
                                        can get an overview of items or can further process these. You can monitor
                                        items, split items and import or export items views.
2.50 / 01-2023




                 C-92                                                            A+W Production Rough Scheduling
                 Software Reference                                                           Items in Rough Scheduling




                                          Items
                                          Display > Orders > Context menu – List > Items
                                          Display > Buckets > Context menu – List > Items
                                          Display > Batches > Context menu – List > Items
                                          Display > Filler orders > Context menu – List > Items
                                          Glass types > Context menu – List > Items
                                          Processings > Context menu – List > Items
                                          Details > Context menu – List > Items
                                          Lots > Context menu – List > Items
                                          Barcoding > Context menu – List > Items




                 A




                 B




                 C




                 A Navigation                                    C List
                 B Database columns
                 Fig. C-52   Items (example)


                                          The Items dialog provides you with an overview of items in the orders.
                                          In the Items dialog you can adapt tabs and columns to fit your needs so that
                                          exactly the required information is shown.
                                          You control this dialog mainly via context menus.
                                          The Items dialog includes the following information, for example:
2.50 / 01-2023




                                          Navigation
                                          Select in the navigation area which details shall be shown.



                 A+W Production Rough Scheduling                                                                   C-93
                 Items in Rough Scheduling                                                            Software Reference




                                        Order (order number) Order number of the selected order:
                                        • Item (item number): The individual items are listed.
                                        • Part (part number): The individual part numbers are listed.
                                        • Geometry: Shows details concerning the geometry of the lite.
                                        • Text: Shows texts stored for the order.
                                        • Processings: Shows included processings.

                                        Database columns

                                        Database column List of the database columns pertaining to the element
                                        you marked in the navigation.

                                        Value Value of the respective database column.

                                        List
                                        The list shows details pertaining to the element you marked in the navigation.

                                        Release part Specifies whether this is a release part.

                                        Part no. Specifies the part number.

                                        Type Specifies the article or part type.

                                        Procurement type Procurement type of article or part, e.g. additional pur-
                                        chase.

                                        Article no. Article number of article.

                                        Article description Article name.

                                        ProdDate Production date of the head section. In the case of multi-part or-
                                        ders, this is the date of assembly. In the case of single-part orders, the produc-
                                        tion date and the start date are identical.

                                        CoatPos Specifies whether the coating points to the outside or inside. This in-
                                        formation applies per lite, e.g. for an IG you specify several lites in one line. It
                                        is specified as follows:
                                        • 0: No coating
                                        • 1: Outside
                                        • 2: Inside
2.50 / 01-2023




                 C-94                                                               A+W Production Rough Scheduling
                 Software Reference                                                          Items in Rough Scheduling




                                       PatternPos Specifies whether the pattern points to the outside or inside. This
                                       information applies per lite, e.g. for an IG you specify several lites in one line.
                                       It is specified as follows:
                                       • 0: No coating
                                       • 1: Outside
                                       • 2: Inside

                                       Step Specifies whether it is a stepped IG or LAMI.

                                       ShpNo. Number of the shape that is being used.

                                           Database information from columns
                                           You can open the Column definition dialog by right-clicking on a column
                                           and selecting the option Show definition. In the Column definition dialog
                                           you will find the respective database information of a column.

                                        “Column Definition” on page C-126

                                       Context menus
                                       Context menus are offered in the following sections of the Items dialog:
                                       •   Navigation
                                       •   Database columns
                                       •   List
                                       The context menus vary, depending on which elements you have selected in
                                       Navigation.
                                       Context menus that appear in the entire area of production preparation are list-
                                       ed in the chapter Overlapping Context Menus.
                                        “Overlapping Context Menus” on page C-133
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                    C-95
                 Items in Rough Scheduling                                                           Software Reference




                                         Group        Path             Remark

                                         Navigation   Add order        Opens the Add Order to Items dialog with which
                                                                       you can add an order to the respective item.



                                                      Export view      Opens the Export/Import Item View dialog.

                                                      Import view      Opens the Export/Import Item View dialog.

                                         Split        Insert > Order   Inserts a new field in the list. Different
                                         database                      categories for orders are available.


                                         List         Insert > Item    Inserts a new column. Different categories are
                                                                       available.



                                                      Insert > Parts   Inserts a new column. Different categories are
                                                                       available.

                                                      Insert > Parts   Inserts a new column. Different categories are
                                                      cumulated        available.
                                                                       The cumulative view is the simultaneous
                                                                       retrieval of several database tables and fields,
                                                                       e.g. totals.

                 Tab. C-9   Items, context menus
2.50 / 01-2023




                 C-96                                                            A+W Production Rough Scheduling
                 Software Reference                                                      Items in Rough Scheduling




                                       Add Order to Items
                                       Items > Navigation > Context menu > Add order




                                       Fig. C-53    Add Order to Items


                                       In the Add Order to Items dialog you can load additional orders into the Items
                                       view.

                                       Order number Specifies the number of the order to be added.

                                       Delete selection first Checkbox with the following options:
                                       Previously displayed orders are not deleted prior to adding.
                                       Previously displayed orders are deleted prior to adding.

                                       [OK] Saves the data.

                                       [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                               C-97
                 Items in Rough Scheduling                                                          Software Reference




                                        Split Items
                                        Display > Orders > Context menu – List > Split items
                                        Processings > Context menu – List > Split items
                                        Details > Context menu – List > Split items




                                        Fig. C-54    Split items


                                        The Split Items dialog is used for splitting order items. Splitting of items can
                                        also be executed for several orders at the same time.

                                        Selected items
                                        The list shows the processings you have selected in the Processings dialog.
                                         “Processings” on page C-103

                                        Order Orders which have been selected for splitting.

                                        Item Number of items in the orders.

                                        Subitem Currently not being used.

                                        Quantity Number of parts in the orders.

                                        New Items
                                        The list shows the split items.

                                        Order Split orders.

                                        Item Number of items in the orders.

                                        Subitem Currently not being used.
2.50 / 01-2023




                                        New item New item resulting from the splitting.

                                        Quantity Number of lites in the orders.



                 C-98                                                              A+W Production Rough Scheduling
                 Software Reference                                                     Items in Rough Scheduling




                                       [Remove] Deletes a selected item.

                                       Split per item in … items Specifies into how many new items the splitting
                                       shall be executed.

                                       Create items with maximum … lites Specifies how many lites a new item
                                       may include at the most.

                                       Create per item an item with … lites Specifies that for every item, a new
                                       item with a certain number of lites shall be created.

                                       Split according to PMO result This option button defines that the items are
                                       going to be split according to the results of packing optimization.

                                       [Split] Splits the items.

                                       [Close] Closes the dialog.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                             C-99
                 Items in Rough Scheduling                                                           Software Reference




                                        Field Definition
                                        Items > Context menu – Database columns > Insert > Field definitions > Edit
                                        Items > Context menu – Database columns > Insert > Field definitions > Edit




                                        Fig. C-55     Field Definition


                                        Use the Field Definition dialog to edit the definitions of the respective fields.

                                        Menu group Selection of the menu group to which the field is allocated.

                                        Menu entry Selection of a description for the selected menu group.

                                        Column header Name of the column. If you do not specify a column header,
                                        the entry from the Menu Entry field is adopted as the column title.

                                        Description Field description. If you do not specify a description, the entry
                                        from the Menu Entry field is adopted as the description.

                                        Format Specifies the format of the field, e.g. whether it is date, length or area
                                        information.

                                        Database field Specifies the database table and corresponding field which is
                                        accessed by the new query or column.

                                        Options
                                        Select by which criteria the data shall be sorted:
                                        •    Sorting sequence ascending: The shown data is sorted in ascending order.
                                        •    Sorting sequence descending: The shown data is sorted in descending or-
                                             der.
                                        •    Cumulate: The shown data is cumulated.
2.50 / 01-2023




                                        Display options
                                        Different options as to how the fields shall be displayed are available:


                 C-100                                                              A+W Production Rough Scheduling
                 Software Reference                                                     Items in Rough Scheduling




                                       Hide identical content in following lines If successive fields have the
                                       same content, you can hide them in following lines.
                                        Show identical content in the following lines.
                                        Hide identical content in the following lines

                                       Value changeable (item view only) Specifies whether the values in the re-
                                       spective fields can be changed.
                                        Values cannot be changed.
                                        Values can be changed.

                                       Pull-down criterion (component display only) Selection whether there is
                                       a pull-down criterion.
                                        There is no pull-down criterion.
                                        There is a pull-down criterion.

                                       [Save] Saves the menu entry.

                                       [Delete] Deletes the entire menu entry.

                                       [Close] Closes the dialog.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                            C-101
                 Items in Rough Scheduling                                                        Software Reference




                                        Export/Import Item View
                                        Items > Navigation > Context menu > Export view
                                        Items > Navigation > Context menu > Import view




                                        Fig. C-56    Export/Import Item View


                                        Use the Export/Import Item View dialog to import or export changed or newly
                                        created views of the Items dialog. Select whether the export or import shall be
                                        carried out globally or locally.
                                         “Items” on page C-93

                                        View type

                                        Only global Saves the new view system-wide for all users.

                                        Only local Saves the new view for the currently logged in user only.

                                        [OK] Saves the data.

                                        [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 C-102                                                            A+W Production Rough Scheduling
                 Software Reference                                                  Processings in Rough Scheduling




                                          Processings in Rough Sched-
                                          uling
                                          This chapter provides you with information on all the dialogs with which you
                                          can get an overview of processings. You can monitor processings and change
                                          default times.


                                          Processings
                                          Display > Orders > Context menu – List > Processings
                                          Display > Buckets > Context menu – List > Processings
                                          Display > Batches > Context menu – List > Processings
                                          Display > Filler orders > Context menu – List > Processings
                                          Glass types > Context menu – List > Processings
                                          Details > Context menu – List > Processings
                                          Barcoding > Context menu – List > Processings
                                          Lots > Context menu – List > Processings




                 Fig. C-57   Processings (example)


                                          The Processings dialog provides you with an overview of processings in the
                                          orders.
                                          In the Processings dialog you can adapt tabs and columns to fit your needs so
2.50 / 01-2023




                                          that exactly the required information is shown.
                                          You control this dialog mainly via context menus.



                 A+W Production Rough Scheduling                                                                C-103
                 Processings in Rough Scheduling                                                   Software Reference




                                        The Processings dialog includes the following columns, for example:

                                        Date Date when this processing will be executed.

                                        Shift Shift during which the processing is executed.

                                        Sequence Sequence number for the processing.

                                        Type Type of the processing.

                                        ArtNo Article number.

                                        Processing name Name/description of the processing.

                                        MA-machine Machine used for this processing.

                                        Quantity Quantity of parts to be produced or processings to be executed.

                                        Registration point Registration point of the assigned machine.

                                        Total duration Total processing duration of the selected orders or items. Unit:
                                        hours.

                                            Database information from columns
                                            You can open the Column definition dialog by right-clicking on a column
                                            and selecting the option Show definition. In the Column definition dialog
                                            you will find the respective database information of a column.

                                         “Column Definition” on page C-126

                                        Totals row

                                        Total duration Total processing duration of the selected orders or items. Unit:
                                        hours.

                                        Total pcs Total of all parts in the selected orders or items.

                                        Filter

                                        [Add filter] Adds a filter.

                                        Drop-down menu The following options are available in the drop-down
                                        menu of the filter:
                                        • Click: Opens the drop-down menu from which you select a filter.
                                        • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                          Filter Definition dialog in which you edit the respective filter.
                                         “Filter Definition” on page C-128

                                        Context menus
2.50 / 01-2023




                                        Context menus are offered in the following sections of the Processings dialog:
                                        •   Tab


                 C-104                                                            A+W Production Rough Scheduling
                 Software Reference                                                         Processings in Rough Scheduling




                                          •   Columns
                                          •   List
                                          •   Totals row
                                          •   Filter
                                          Context menus that appear in the entire area of production preparation are list-
                                          ed in the chapter Overlapping Context Menus.
                                           “Overlapping Context Menus” on page C-133


                                          Group           Path                 Remark

                                          List            Set status           Opens the Set status dialog where you can
                                                                               select the status of the glass type.
                                                                               •   in production
                                                                               •   produced
                                                                               •   ready for shipment
                                                                               •   delivered

                                                          Work plan >          Opens the Rescheduling dialog to reschedule to
                                                          Rescheduling to      other machines.
                                                          other machines
                                                                               
                                                                               The results of the machine allocation within the
                                                                               scope of scheduling are overwritten.

                                                          Work plan >          Opens the Rescheduling dialog to reschedule
                                                          Rescheduling         dates.
                                                                               
                                                                               The results of the machine allocation within the
                                                                               scope of scheduling are overwritten.

                                                          Work plan >          Opens the Default Times dialog in which you
                                                          Change default       can change the default times.
                                                          times
                                                                                “Change Default Times” on page C-106
                                                                               The results of capacity planning within the
                                                                               scope of scheduling are overwritten.

                                                          Work plan >          Protects the processing date for the selected
                                                          Protect processing   processings.
                                                          date
                                                                               The results of capacity planning within the
                                                                               scope of scheduling are overwritten.

                                                          Work plan >          Removes the processing date protection for the
                                                          Processing date,     selected processings.
                                                          remove protection
                                                                               The results of capacity planning within the
                                                                               scope of scheduling are overwritten.

                 Tab. C-10   Processings, context menus

                                          Buttons
2.50 / 01-2023




                                          [Batch] Creates a batch from selected orders, items or parts.

                                          [Glass types] Shows the glass types for the selected orders.


                 A+W Production Rough Scheduling                                                                             C-105
                 Processings in Rough Scheduling                                                 Software Reference




                                        [Details] Shows the details for the selected orders.


                                        Change Default Times
                                        Processings > Context menu – List > Work plan > Change default times




                                        Fig. C-58   Change default times


                                        Use the Default Times dialog to change the default times for processings.

                                           Change default times
                                           The calculated default times of A+W Capacity Planner are overwritten for
                                           the respective selection if you define a value in the Change Default Times
                                           dialog.
                                           The defined default time formulas in the master data of capacity planning
                                           are not affected by this change.

                                        Factor The factor by which the default time shall be changed.

                                        [OK] Saves the data.

                                        [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 C-106                                                           A+W Production Rough Scheduling
                 Software Reference                                            Glass types, Details, Barcoding and Lots




                                          Glass types, Details, Barcod-
                                          ing and Lots
                                          This chapter provides you with information on all the dialogs with which you
                                          can get an overview of glass types, details, barcoding, and lots.


                                          Glass Types
                                          Display > Orders > Context menu – List > Glass types
                                          Display > Buckets > Context menu – List > Glass types
                                          Display > Batches > Context menu – List > Glass types
                                          Display > Filler orders > Context menu – List > Glass types
                                          Processings > Context menu – List > Glass types
                                          Details > Context menu – List > Glass types
                                          Lots > Context menu – List > Glass types
                                          Barcoding > Context menu – List > Glass types




                 Fig. C-59   Glass types (example)


                                          Use the Glass Types dialog to display an overview of the included glass types
                                          for selected orders or items and to create a batch. This batch is then displayed
                                          in the Batches dialog.
                                          In the Glass Types dialog you can adapt tabs and columns to fit your needs so
                                          that exactly the required information is shown.
2.50 / 01-2023




                                          You control this dialog mainly via context menus.
                                          The Types tab includes the following columns, for example:


                 A+W Production Rough Scheduling                                                                   C-107
                 Glass types, Details, Barcoding and Lots                                           Software Reference




                                          Batch Number of the batch.

                                          Glass type Name of the glass type that is included in the order or item.

                                          Thickness Thickness of the lites.

                                          Piece Quantity of the respective glass type.

                                          IG pcs Number of lites that are used for IG.

                                          TG pcs Number of lites that are used for TG.

                                          LAMI pcs Number of lites that are used for LAMI.

                                              Database information from columns
                                              You can open the Column definition dialog by right-clicking on a column
                                              and selecting the option Show definition. In the Column definition dialog
                                              you will find the respective database information of a column.

                                           “Column Definition” on page C-126

                                          Totals row

                                          Pcs Number of lites in selected orders or items.

                                          Total duration Total processing duration of the selected orders or items. Unit:
                                          hours.

                                          Area Total area of all selected orders or items. Unit: Square meters.

                                          Filter

                                          [Add filter] Adds a filter.

                                          Drop-down menu The following options are available in the drop-down
                                          menu of the filter:
                                          • Click: Opens the drop-down menu from which you select a filter.
                                          • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                            Filter Definition dialog in which you edit the respective filter.
                                           “Filter Definition” on page C-128

                                          Context menus
                                          Context menus are offered in the following sections of the Glass Types dialog:
                                          •   Tab
                                          •   Columns
                                          •   List
                                          •   Totals row
2.50 / 01-2023




                                          •   Filter




                 C-108                                                              A+W Production Rough Scheduling
                 Software Reference                                              Glass types, Details, Barcoding and Lots




                                          Context menus that appear in the entire area of production preparation are list-
                                          ed in the chapter Overlapping Context Menus.
                                           “Overlapping Context Menus” on page C-133


                                          Group           Path              Remark

                                          List            Special glass >   Opens the Create Special Glass Batch dialog.
                                                          Add
                                                                             “Create Special Glass Batch” on page C-90


                                                          Special glass >   Currently not being used.
                                                          Delete

                                                          Set status        Opens the Set status dialog where you can
                                                                            select the status of the glass type.
                                                                            •   in production
                                                                            •   produced
                                                                            •   ready for shipment
                                                                            •   delivered

                                                          Free shapes       Opens the A+W CAD Designer (Shapes) for
                                                                            postprocessing of the shape data.

                                                          Rescheduling to   Opens the Rescheduling dialog from capacity
                                                          other machines    planning.
                                                                            
                                                                            The results of the machine allocation within the
                                                                            scope of scheduling are overwritten.

                 Tab. C-11   Glass types, Context menus

                                          Buttons

                                          [Batch] Creates a batch from selected orders, items or parts.

                                          [Glass types] Shows the glass types for the selected orders or items.

                                          [Details] Shows the details for the selected orders or items.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                       C-109
                 Glass types, Details, Barcoding and Lots                                            Software Reference




                                          Details
                                          Display > Orders > Details
                                          Display > Buckets > Context menu – List > Details
                                          Display > Batches > Context menu – List > Details
                                          Display > Filler orders > Context menu – List > Details
                                          Glass types > Context menu – List > Details
                                          Processings > Context menu – List > Details
                                          Barcoding > Context menu – List > Details
                                          Lots > Context menu – List > Details




                 Fig. C-60   Details (example)


                                          Use the Details dialog to view details on selected orders, items, parts, batches
                                          or buckets. You can open the Details dialog from any view in Rough Schedul-
                                          ing.
                                          In the Details dialog you can adapt tabs and columns to fit your needs so that
                                          exactly the required information is shown.
                                          You control this dialog mainly via context menus.
                                          The Details dialog includes the following columns, for example:

                                          SN info Shows the shape status and associated geometry calculation within
                                          the scope of scheduling. The following display options are available:
                                          • 0: Status ok.
                                          • Number: There is an error.
2.50 / 01-2023




                 C-110                                                              A+W Production Rough Scheduling
                 Software Reference                                          Glass types, Details, Barcoding and Lots




                                       Cancellation Information as to whether the order has been canceled in the
                                       ERP system.

                                       Order Number of order.

                                       Batch Number of the batch.

                                       Delivery date Delivery date of the order.

                                       Production date Production date for the order, item, unit or part.

                                       IG total Number of IG lites included in the order.

                                       Frosted [partly], pcs Number of lites that are frosted or partly frosted.

                                       LAMI pcs Number of LAMI lites in the order or item.

                                       TG pcs Number of TG lites in the order or item.

                                       Georgian bars pcs Number of Georgian bars in the order.

                                       Shapes pcs Number of shapes in the order.

                                       Triple IG pcs Number of triple IG lites in the order.

                                       Stepped pcs Number of stepped IG or stepped LAMI in the order.

                                          Database information from columns
                                          You can open the Column definition dialog by right-clicking on a column
                                          and selecting the option Show definition. In the Column definition dialog
                                          you will find the respective database information of a column.

                                        “Column Definition” on page C-126

                                       Totals row

                                       Total pcs Total of all parts in the selected orders or items.

                                       Shapes Number of shapes in selected orders or items.

                                       Area shp Total area of shapes in the selected orders or items. Unit: Square
                                       meters.

                                       Filter

                                       [Add filter] Adds a filter.

                                       Drop-down menu The following options are available in the drop-down
                                       menu of the filter:
2.50 / 01-2023




                                       • Click: Opens the drop-down menu from which you select a filter.




                 A+W Production Rough Scheduling                                                               C-111
                 Glass types, Details, Barcoding and Lots                                                Software Reference




                                          •   Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                              Filter Definition dialog in which you edit the respective filter.
                                           “Filter Definition” on page C-128

                                          Context menus
                                          Context menus are offered in the following sections of the Details dialog:
                                          •   Tab
                                          •   Columns
                                          •   List
                                          •   Totals row
                                          •   Filter
                                          Context menus that appear in the entire area of production preparation are list-
                                          ed in the chapter Overlapping Context Menus.
                                           “Overlapping Context Menus” on page C-133


                                          Group        Path                  Remark

                                          List         Return order to the   Returns the selected orders back to the Orders
                                                       Pool                  dialog.
                                                                              “Orders” on page C-59

                                                       Set status            Opens the Set status dialog where you can
                                                                             select the status of the batch.
                                                                             •   in production
                                                                             •   produced
                                                                             •   ready for shipment
                                                                             •   delivered

                                                       Work plan >           Opens the Rescheduling dialog to reschedule to
                                                       Rescheduling to       other machines.
                                                       other machines
                                                                             
                                                                             The results of the machine allocation within the
                                                                             scope of scheduling are overwritten.

                                                       Work plan >           Carries out the machine allocation for selected
                                                       Machine allocation    orders or items again.
                                                                             The results of the machine allocation within the
                                                                             scope of scheduling are overwritten.

                                                       Work plan >           Currently not being used
                                                       Recalculate work
                                                       plan

                                                       Georgian bars print Starts print of production papers for Georgian
                                                                           bar production or processing.

                 Tab. C-12   Details, context menus
2.50 / 01-2023




                 C-112                                                                 A+W Production Rough Scheduling
                 Software Reference                                           Glass types, Details, Barcoding and Lots




                                          Group       Path                Remark

                                                      Change default      Opens the Default Times dialog in which you
                                                      times               can change the default times.
                                                                           “Change Default Times” on page C-106
                                                                          The results of capacity planning within the
                                                                          scope of scheduling are overwritten.

                 Tab. C-12   Details, context menus

                                          Buttons

                                          [Batch] Creates a batch from selected orders, items or parts.

                                          [Glass types] Shows the glass types for the selected orders or items.

                                          [Details] Shows the details for the selected orders or items.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                        C-113
                 Glass types, Details, Barcoding and Lots                                           Software Reference




                                          Barcoding
                                          Display > Orders > Context menu – List > Processings > Context menu – List
                                          > Barcoding
                                          Display > Buckets > Context menu – List > Processings > Context menu – List
                                          > Barcoding
                                          Display > Batches > Context menu – List > Barcoding
                                          Glass types > Context menu – List > Barcoding
                                          Details > Context menu – List > Barcoding




                 Fig. C-61   Barcoding - Product (example)


                                          The Barcoding dialog provides you with an overview of information relating to
                                          shop floor data collection.
                                          You can sort the orders by different criteria and edit them. You can configure
                                          the following components of the Barcoding dialog as you like:
2.50 / 01-2023




                 C-114                                                             A+W Production Rough Scheduling
                 Software Reference                                           Glass types, Details, Barcoding and Lots




                                       •   Tab
                                       •   Columns
                                       •   Totals row
                                       •   Filter
                                       You control this dialog mainly via context menus.
                                       The Product tab includes the following columns, for example:

                                       Order Number of order.

                                       Itm (int Itm) Internal item number from order entry.

                                       Part no. Part number of the respective part.

                                       Article description Name of respective article.

                                       Label No. Label number of the respective part.

                                           Database information from columns
                                           You can open the Column definition dialog by right-clicking on a column
                                           and selecting the option Show definition. In the Column definition dialog
                                           you will find the respective database information of a column.

                                        “Column Definition” on page C-126

                                       Totals row
                                       You can display different totals in the totals row, e.g. the following information:

                                       Total duration Total processing duration of the selected orders or items. Unit:
                                       hours.

                                       Total pcs Total of all parts in the selected orders or items.

                                       Filter

                                       [Add filter] Adds a filter.

                                       Drop-down menu The following options are available in the drop-down
                                       menu of the filter:
                                       • Click: Opens the drop-down menu from which you select a filter.
                                       • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                         Filter Definition dialog in which you edit the respective filter.
                                        “Filter Definition” on page C-128
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                  C-115
                 Glass types, Details, Barcoding and Lots                                                 Software Reference




                                          Context menus
                                          Context menus are offered in the following sections of the Barcoding dialog:
                                          •   Tab
                                          •   Columns
                                          •   List
                                          •   Totals row
                                          •   Filter
                                          Context menus that appear in the entire area of production preparation are list-
                                          ed in the chapter Overlapping Context Menus.
                                           “Overlapping Context Menus” on page C-133


                                          Group         Path                  Remark

                                          List          Return order to the   Returns the selected orders or items back to the
                                                        Pool                  Orders dialog.



                                                        Set status            Opens the Set status dialog where you can
                                                                              select the status of the batch.
                                                                              •   in production
                                                                              •   produced
                                                                              •   ready for shipment
                                                                              •   delivered

                                                        Work plan >           Opens the Rescheduling dialog to reschedule to
                                                        Rescheduling to       other machines.
                                                        other machines
                                                                              
                                                                              The results of the machine allocation within the
                                                                              scope of scheduling are overwritten.

                                                        Work plan >           Carries out the machine allocation for selected
                                                        Machine allocation    orders or items again.
                                                                              The results of the machine allocation within the
                                                                              scope of scheduling are overwritten.

                                                        Work plan >           Currently not being used.
                                                        Recalculate work
                                                        plan

                                                        Change default        Opens the Default Times dialog in which you
                                                        times                 can change the default times.
                                                                               “Change Default Times” on page C-106
                                                                              The results of capacity planning within the
                                                                              scope of scheduling are overwritten.

                 Tab. C-13   Barcoding, Context menus
2.50 / 01-2023




                 C-116                                                                  A+W Production Rough Scheduling
                 Software Reference                                        Glass types, Details, Barcoding and Lots




                                       Buttons

                                       [Batch] Currently not active.

                                       [Glass types] Shows the glass types for the selected orders or items.

                                       [Details] Shows the details for the selected orders or items.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                            C-117
                 Glass types, Details, Barcoding and Lots                                            Software Reference




                                          Lots
                                          Display > Batches > Context menu – List > Lots
                                          Details > Context menu – List > Lots




                 Fig. C-62   Lots - Cutting (exampe)


                                          The Lots dialog provides you with an overview of the created lots of the select-
                                          ed batches.
                                          You can sort the lots by different criteria and edit them. You control this Lots
                                          dialog mainly via context menus. You can configure the following components
                                          of the Lots dialog as you like:
                                          •   Tab
                                          •   Columns
                                          •   Totals row
                                          •   Filter
2.50 / 01-2023




                 C-118                                                              A+W Production Rough Scheduling
                 Software Reference                                           Glass types, Details, Barcoding and Lots




                                       The Cutting tab includes the following columns, for example:

                                       Lot type Specifies the lot type.

                                       Lot Name of lot.

                                       Rack Rack planned for the lot.

                                       Glass type Number of the glass type.

                                       Glass description Description for glass type for the lot.

                                       Pcs Number of items or parts in the lot.

                                           Database information from columns
                                           You can open the Column definition dialog by right-clicking on a column
                                           and selecting the option Show definition. In the Column definition dialog
                                           you will find the respective database information of a column.

                                        “Column Definition” on page C-126

                                       Totals row
                                       You can display different totals in the totals row, e.g. the following information:

                                       Total duration Total processing duration of the selected orders or items. Unit:
                                       hours.

                                       Pcs Number of individual lites or units in selected orders or items.

                                       Filter

                                       [Add filter] Adds a filter.

                                       Drop-down menu The following options are available in the drop-down
                                       menu of the filter:
                                       • Click: Opens the drop-down menu from which you select a filter.
                                       • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                         Filter Definition dialog in which you edit the respective filter.
                                        “Filter Definition” on page C-128

                                       Context menus
                                       Context menus are offered in the following sections of the Lots dialog:
                                       •   Tab
                                       •   Columns
                                       •   List
                                       •   Totals row
2.50 / 01-2023




                                       •   Filter




                 A+W Production Rough Scheduling                                                                  C-119
                 Glass types, Details, Barcoding and Lots                                            Software Reference




                                          Context menus that appear in the entire area of production preparation are list-
                                          ed in the chapter Overlapping Context Menus.
                                           “Overlapping Context Menus” on page C-133


                                          Group        Path                Remark

                                          List         Set status          Opens the Set status dialog where you can
                                                                           select the status of the batch.
                                                                           •   in production
                                                                           •   produced
                                                                           •   ready for shipment
                                                                           •   delivered

                 Tab. C-14   Lots, Context menus

                                          Buttons

                                          [Batch] Currently not active.

                                          [Glass types] Shows the glass types for the selected lots.

                                          [Details] Shows the details for the selected lots.
2.50 / 01-2023




                 C-120                                                               A+W Production Rough Scheduling
                 Software Reference                                                               Overlapping Dialogs




                                       Overlapping Dialogs
                                       This chapter will provide you with information concerning all the overlapping
                                       dialogs that you find in the entire production preparation process. You can edit
                                       properties of dialogs, manage document shortcuts and edit surface deletion.
                                       The chapter covers the following topics:
                                       •   “Properties of (tab)” on page C-125
                                       •   “Column Definition” on page C-126
                                       •   “(Filter Name)” on page C-127
                                       •   “Filter Definition” on page C-128
                                       •   “Links to Documents” on page C-130
                                       •   “Surface Deletion” on page C-131
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                C-121
                 Overlapping Dialogs                                                              Software Reference




                                         Work Plan
                                         Production monitor > Context menu – Shift > Work plan




                 Fig. C-63   Work plan (example)


                                         Use the Work Plan dialog to obtain an overview from within the production
                                         monitor view. The work plan shows you all the planned batches on a machine
                                         or in a shift.
                                         In the Work Plan dialog you can adapt tabs and columns to fit your needs so
                                         that exactly the required information is shown.
                                         You control this dialog mainly via context menus.
                                         The Details tab includes the following columns, for example:

                                         Batch Specifies the batch.

                                         Order Specifies the order.

                                         Itm (int Itm) Specifies the item number.

                                         Part no. Specifies the part number.

                                         Sequence Sequence number for the processing.
2.50 / 01-2023




                 C-122                                                              A+W Production Rough Scheduling
                 Software Reference                                                                 Overlapping Dialogs




                                       ProcNo Processing number.

                                       MA-machine Logical machine used for this processing.

                                           Database information from columns
                                           You can open the Column definition dialog by right-clicking on a column
                                           and selecting the option Show definition. In the Column definition dialog
                                           you will find the respective database information of a column.

                                        “Column Definition” on page C-126

                                       Totals row
                                       You can display different totals in the totals row, e.g. the following information:

                                       Total pcs Total of all parts in the selected orders or items.

                                       Total duration Total processing duration of the selected orders or items. Unit:
                                       hours.

                                       Filter

                                       [Add filter] Adds a filter.

                                       Drop-down menu The following options are available in the drop-down
                                       menu of the filter:
                                       • Click: Opens the drop-down menu from which you select a filter.
                                       • Right-click: Opens the dialog (Filter Name). The Manage button opens the
                                         Filter Definition dialog in which you edit the respective filter.
                                        “Filter Definition” on page C-128

                                       Context menus
                                       Context menus are offered in the following sections of the Work Plan dialog:
                                       •   Tab
                                       •   Columns
                                       •   List
                                       •   Totals row
                                       •   Filter
                                       Context menus that appear in the entire area of production preparation are list-
                                       ed in the chapter Overlapping Context Menus.
                                        “Overlapping Context Menus” on page C-133
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                  C-123
                 Overlapping Dialogs                                                                     Software Reference




                                         Group          Path                 Remark

                                         List           Set status           Opens the Set status dialog where you can
                                                                             select the status of the batch.
                                                                             •   in production
                                                                             •   produced
                                                                             •   ready for shipment
                                                                             •   delivered

                                                        Work plan >          Opens the Rescheduling dialog to reschedule to
                                                        Rescheduling to      other machines.
                                                        other machines
                                                                             
                                                                             The results of the machine allocation within the
                                                                             scope of scheduling are overwritten.

                                                        Work plan >          Opens the Rescheduling dialog to reschedule
                                                        Rescheduling         dates.
                                                                             
                                                                             The results of the machine allocation within the
                                                                             scope of scheduling are overwritten.

                                                        Work plan >          Opens the Default Times dialog in which you
                                                        Change default       can change the default times.
                                                        times
                                                                              “Change Default Times” on page C-106
                                                                             The results of capacity planning within the
                                                                             scope of scheduling are overwritten.

                                                        Work plan >          Protects the processing date for the selected
                                                        Protect processing   processings.
                                                        date
                                                                             The results of capacity planning within the
                                                                             scope of scheduling are overwritten.

                                                        Work plan >          Removes the processing date protection for the
                                                        Processing date,     selected processings.
                                                        remove protection
                                                                             The results of capacity planning within the
                                                                             scope of scheduling are overwritten.

                                                        Completion           The batches, orders or items are set to the
                                                        notification         status Completed.

                 Tab. C-15   Work plan, Context menus

                                         Buttons

                                         [Batch] Creates a batch from the selected batches, orders or items.

                                         [Glass types] Shows the glass types for the selected batches, orders or
                                         items.

                                         [Details] Shows the details for the selected batches, orders or items.
2.50 / 01-2023




                                             Export data
                                             Use Display > Export to export the data to a CSV file.



                 C-124                                                                 A+W Production Rough Scheduling
                 Software Reference                                                             Overlapping Dialogs




                                       Properties of (tab)
                                       Display > Orders > Context menu – tab > Insert
                                       Display > Orders > Context menu – tab > Properties




                                       Fig. C-64    Properties of (tab)


                                       In the Properties of (tab) dialog you can create new tabs or change existing
                                       tabs.

                                       Tab text Title of the tab.

                                       Description Description of the tab.

                                       System-wide display Checkbox with the following functions:
                                       The tab is displayed only in this dialog.
                                       The tab is displayed system-wide.

                                       [OK] Saves the data.

                                       [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                             C-125
                 Overlapping Dialogs                                                            Software Reference




                                       Column Definition
                                       Display > Orders > Context menu – Columns > Display definition
                                       Display > Buckets > Context menu – Columns > Display definition
                                       Display > Batches > Context menu – Columns > Display definition
                                       Order overview > Context menu – Columns > Display definition
                                       Glass types > Context menu – Columns > Display definition
                                       Processings > Context menu – Columns > Display definition
                                       Lots > Context menu – Columns > Display definition
                                       Barcoding > Context menu – Columns > Display definition
                                       Details > Context menu – Columns > Display definition




                                       Fig. C-65   Column Definition


                                       The properties of a column are displayed in the Column Definition dialog.

                                       Title Column name.

                                       Format Format of the column, e.g. the date format.

                                       Menu Specifies in which area of the context menu the respective selection is
                                       stored.

                                       SQL def. Name of the database table and database field. Those are de-
                                       scribed in detail in the A+W database documentation.
2.50 / 01-2023




                 C-126                                                         A+W Production Rough Scheduling
                 Software Reference                                                                Overlapping Dialogs




                                       SQL definition – parts Name of the database table and database field if you
                                       have selected the display option Parts in the Order Overview dialog. The da-
                                       tabase tables and fields are described in detail in the A+W database documen-
                                       tation.

                                       SQL definition processings Name of the database table and database field
                                       if you have selected the display option Processings in the Order Overview di-
                                       alog. The database tables and fields are described in detail in the A+W data-
                                       base documentation.

                                       [OK] Closes the dialog.


                                       (Filter Name)
                                       Display > Orders > Context menu – Filter




                                       Fig. C-66    (Filter Name)


                                       You can open the filter definition in the (Filter Name) dialog and delete filters
                                       in there.

                                       Manage Opens the Filter Definition dialog in which you can edit filters.
                                        “Filter Definition” on page C-128

                                       Delete Deletes the selected filter.

                                       [OK] Closes the dialog.

                                       [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                                 C-127
                 Overlapping Dialogs                                                                  Software Reference




                                       Filter Definition
                                       Display > Orders > Context menu – Filter > (Filter Name) > [Manage]




                                       Fig. C-67     Filter Definition


                                       Use the Filter Definition dialog to define and edit filters.

                                       Defined filters List of defined filters.

                                       Name Name of respective filter.

                                       Description Description of respective filter.

                                       SQL condition Defined formula or condition with reference to the corre-
                                       sponding database tables and fields.

                                       Default parameters Specifies a default value, e.g. default date which is used
                                       when the corresponding database tables or fields do not determine a value.

                                       Valid for view Dialog selection where the filter is available. Available options:
                                       • Pool view
                                       • Bucket view
                                       • Batch view
                                       • Filler order view
                                       • Details
                                       • Preselection barcoding view
                                       • Purchase parts bucket
                                       • Glass type view
                                       • Production lot view
                                       • Processing view
                                       • Barcoding
                                       • Packaging
2.50 / 01-2023




                 C-128                                                             A+W Production Rough Scheduling
                 Software Reference                                                            Overlapping Dialogs




                                       •   Breakage statistics
                                       •   Production statistics
                                       •   Production overview

                                       Save Saves the data.

                                       Delete Deletes the selected filter.

                                       Export Opens the Save as dialog in which you can save the respective filter.

                                       Import Opens the Open dialog in which you can select filters for importing.

                                       [Close] Closes the dialog without saving the data.
2.50 / 01-2023




                 A+W Production Rough Scheduling                                                            C-129
                 Overlapping Dialogs                                                           Software Reference




                                       Links to Documents
                                       Display > Orders > Context menu – List > Pertaining documents
                                       Display > Buckets > Context menu – List > Pertaining documents
                                       Display > Batches > Context menu – List > Pertaining documents
                                       Display > Filler orders > Context menu – List > Pertaining documents
                                       Glass types > Context menu – List > Pertaining documents
                                       Processings > Context menu – List > Pertaining documents
                                       Barcoding > Context menu – List > Pertaining documents
                                       Lots > Context menu – List > Pertaining documents




                                       Fig. C-68   Links to Documents


                                       Use the Links to Documents dialog to link orders to documents, e.g. specific
                                       delivery conditions and view which documents are linked to an order or item.

                                       Order Selected orders.

                                       Item Number of items per order.

                                       Type Type of linked document. Specify the document type with a number (that
                                       you can choose). Also define which document type is assigned to a number,
                                       e.g. 3 for text documents.

                                       Document Path of linked document.

                                       [Open] Opens an attached document.

                                       [Delete] Deletes a document link.

                                       [New] Creates a document link.

                                       [Edit] Opens the Links to Documents (Order Number) dialog where you can
                                       change the data.
2.50 / 01-2023




                                       [Close] Closes the dialog.



                 C-130                                                         A+W Production Rough Scheduling
                 Software Reference                                                              Overlapping Dialogs




                                       Surface Deletion
                                       Display > Orders > Context menu – List > Reentry > Edge deletion
                                       Display > Buckets > Context menu – List > Reentry > Edge deletion
                                       Display > Batches > Context menu – List > Reentry > Edge deletion
                                       Display > Filler ord. > Context menu – List > Reentry > Edge deletion
                                       Details > Context menu – List > Reentry > Edge deletion
                                       Barcoding > Context menu – List > Reentry > Edge deletion




                                       Fig. C-69   Surface deletion


                                       In the Surface Deletion dialog you can subsequently specify areas that should
                                       be deleted.

                                       Header
                                       The header shows information about the respective item:
                                       •   Order
                                       •   Item
                                       •   Sub-item
                                       •   Part number
                                       •   Glass type
                                       •   Shape

                                       Navigation window
2.50 / 01-2023




                                       The navigation window shows you the selected surface deletion areas.




                 A+W Production Rough Scheduling                                                               C-131
                 Overlapping Dialogs                                                             Software Reference




                                       Navigation

                                       1 Distance of the surface deletion area to corner 1. Unit: millimeters.

                                       2 Distance of the surface deletion area to corner 2. Unit: millimeters.

                                       [Left arrow] Changes the position of corners 1 and 2 on the lite.

                                       [Right arrow] Changes the position of corners 1 and 2 on the lite.

                                       Buttons

                                       [OK] Saves the data.

                                       [Cancel] Closes the dialog without saving the data.
2.50 / 01-2023




                 C-132                                                           A+W Production Rough Scheduling
                 Software Reference                                                              Overlapping Context Menus




                                         Overlapping Context Menus
                                         This chapter will provide you with information concerning all overlapping con-
                                         text menus that you find in the entire production preparation process.
                                         You will find the context menus in the following dialog sections:
                                         •   Tab
                                         •   Columns
                                         •   List
                                         •   Totals row
                                         •   Filter


                                         Group           Path                 Remark

                                         Tab             Autosave             Changes to the tab are automatically saved.


                                                         Save                 Manual saving of changes to the tab.

                                                         Insert               Opens the Properties of (tab) dialog.
                                                                               “Properties of (tab)” on page C-125

                                                         Delete               Deletes the selected tab.

                                                         Properties           Opens the Properties of (tab) dialog in which
                                                                              you can change the tab properties.
                                                                               “Properties of (tab)” on page C-125

                                                         Import               Opens the Importing a Tab dialog.

                                                         Export               Opens the Exporting a Tab dialog.

                                         Columns         Re-sorting           Sort column in ascending or descending order.
                                                                              Affects the first three columns in the dialog.

                                                         Formatting           Select format or unit for the columns, e.g. date
                                                                              format or length unit.

                                                         Insert               Inserts a new column. Different categories are
                                                                              available.

                                                         Insert > Field       Opens the Field Definition dialog in which you
                                                         definitions > Edit   can formulate queries in database tables and
                                                                              fields. These queries can then be inserted, e.g.
                                                                              part-, item- or order-related as a column.
                                                                               “Field Definition” on page C-100

                                                         Insert > Field       Opens the Import Field Definitions dialog.
                                                         definitions > Import

                                                         Insert > Field       Opens the Export Field Definitions dialog.
2.50 / 01-2023




                                                         definitions > Export

                                                         Delete               Deletes the selected column.

                 Tab. C-16   Overlapping Context Menus


                 A+W Production Rough Scheduling                                                                           C-133
                 Overlapping Context Menus                                                                Software Reference




                                         Group           Path                 Remark

                                                         Change               Currently not being used.

                                                         Display definition   Opens the Column Definition dialog that shows
                                                                              details concerning the respective column.
                                                                               “Column Definition” on page C-126

                                         List            Create batch         Opens the Batch Creation dialog.
                                                                               “Batch creation” on page C-88


                                                         Create bucket        Opens the Bucket Creation dialog.
                                                                               “Bucket Creation” on page C-81

                                                         Filler order         Changes the selected order to a filler order.
                                                                               “Filler Orders” on page C-65

                                                         Create packing       Opens the Packing groups dialog.
                                                         group

                                                         Create               Automatically creates packing groups.
                                                         automatically

                                                         Order overview       Opens the Order Overview dialog
                                                                               “Order Overview” on page C-62

                                                         Items                Opens the Items dialog.
                                                                               “Items” on page C-93

                                                         Glass types          Opens the Glass Types dialog.
                                                                               “Glass Types” on page C-107

                                                         Processings          Opens the Processings dialog.
                                                                               “Processings” on page C-103

                                                         Lots                 Opens the Lots dialog.
                                                                               “Lots” on page C-118

                                                         Barcoding            Opens the Barcoding dialog.
                                                                               “Barcoding” on page C-114

                                                         Details              Opens the Details dialog.
                                                                               “Details” on page C-110

                                                         Reentry > Edge       Opens the Surface Deletion dialog.
                                                         deletion
                                                                               “Surface Deletion” on page C-131

                                                         Reentry >            Opens the A+W CAD Designer (Shapes) to
                                                         Georgian bars        reenter Georgian bars.

                                                         Reentry > Free       Opens the A+W CAD Designer (Bars) for
2.50 / 01-2023




                                                         shapes               postprocessing of the shape data.

                 Tab. C-16   Overlapping Context Menus




                 C-134                                                                  A+W Production Rough Scheduling
                 Software Reference                                                               Overlapping Context Menus




                                         Group           Path                 Remark

                                                         Reentry > Surplus    Opens the Surplus Editor dialog for reentering
                                                                              business- and production-related surplus.
                                                                               “Surplus Editor” on page C-68

                                                         Work plan >          Opens the Rescheduling dialog to reschedule to
                                                         Rescheduling to      other machines.
                                                         other machines
                                                                               Capacity Planning: Software Reference,
                                                                                “Machine Reallocation” on page K-183
                                                                              The results of the machine allocation within the
                                                                              scope of scheduling are overwritten.

                                                         Work plan >          Carries out the machine allocation for selected
                                                         Machine allocation   orders or items again.
                                                                              The results of the machine allocation within the
                                                                              scope of scheduling are overwritten.

                                                         Work plan >          Currently not being used.
                                                         Recalculate work
                                                         plan

                                                         Split items          Opens the Split Items dialog.
                                                                               “Split Items” on page C-98

                                                         Change               Opens the Change procurement type dialog.
                                                         procurement type
                                                                               “Modification of Procurement Type” on
                                                                                page C-70
                                                                              The option only works with TG and LAMI.

                                                         Pertaining           Opens the Links to Documents dialog.
                                                         documents
                                                                               “Links to Documents” on page C-130

                                         Totals row      Re-sorting           Currently not being used.

                                                         Formatting           Select format or unit for the columns, e.g. date
                                                                              format or length unit.

                                                         Insert               Inserts a new field in the totals row. Different
                                                                              categories are available.

                                                         Insert > Field       Opens the Field Definition dialog in which you
                                                         definitions > Edit   can formulate queries in database tables and
                                                                              fields. These queries can then be inserted, e.g.
                                                                              part-, item- or order-related.
                                                                               “Field Definition” on page C-100

                                                         Insert > Field       Opens the Import Field Definitions dialog.
                                                         definitions > Import

                                                         Insert > Field       Opens the Export Field Definitions dialog.
                                                         definitions > Export
2.50 / 01-2023




                 Tab. C-16   Overlapping Context Menus




                 A+W Production Rough Scheduling                                                                           C-135
                 Overlapping Context Menus                                                   Software Reference




                                         Group           Path   Remark

                                         Filter                 Opens the dialog (Filter Name). The [Manage]
                                                                button opens the Filter Definition dialog in which
                                                                you can edit filters.
                                                                 “Filter Definition” on page C-128

                 Tab. C-16   Overlapping Context Menus
2.50 / 01-2023




                 C-136                                                    A+W Production Rough Scheduling
Rough Scheduling            C

                   Section index




               A+W Production
                 Section index                                                                  Index




                 Index
                 B                                   E
                 Barcoding C-114                     edge deletion C-131
                 Batch creation C-88                 Edit bucket description C-83
                 batch strategies C-45               exercises
                 Batches C-43, C-84                  – views C-33
                 – add order C-48                    Export/Import item view C-102
                 – batch strategies C-45
                 – create C-46                       F
                 – manage C-49                       Field definition C-100
                 batches                             Filler orders C-65
                 – change description C-91           Filter C-127
                 – create special glass batch C-90   filter
                 – resolve C-49                      – define C-128
                 Bucket creation C-81                – edit C-127
                 Buckets C-37, C-72                  Filter definition C-128
                 – add buckets C-40                  Find document C-53
                 – create C-39
                 – resolve C-42
                 buckets                             G
                 – create C-81                       Glass types   C-107
                 – edit description C-83
                 – purchase parts C-78               I
                 – reservation orders C-75           Items C-50, C-93
                                                     – add order C-97
                 C                                   – split C-52
                 Capacity planning C-14              items
                 Change batch description C-91       – field definition C-100
                 Change default times C-106          – import/export views C-102
                 Column definition C-126             – split C-98
                 columns
                 – definition C-126                  L
                 configure columns C-21              Links to documents    C-130
                 configure filters C-28              list C-23
                 configure tabs C-19                 Lots C-118
                 configure totals row C-24
                 Context menus C-133                 M
                 create batches C-46, C-88           manage batches C-49
                 create buckets C-39                 Modification of procurement type   C-70
                 Create special glass batch C-90
                                                     O
                 D                                   Order overview C-62
                 define column C-26                  Orders C-34, C-59
                 define totals row C-26              – capacity planning C-36
                 Details C-110                       – faulty information C-36
                 documents                           Overlapping dialogs C-121
2.50 / 01-2023




                 – link C-130                        Overview dialogs C-16




                 A+W Production Rough scheduling                                               C-139
                 Index                                                    Section index




                 P
                 pool C-34
                 Processings C-103
                 processings
                 – change default times C-106
                 procurement type
                 – modify C-70
                 Production scheduling C-13
                 Properties of tabs C-125
                 purchase parts C-78
                 Purchase parts bucket C-78

                 R
                 Reservation orders C-75
                 reservation orders bucket C-75
                 resolve batches C-49
                 resolve buckets C-42
                 right-click C-133
                 Rough Scheduling
                 – terms C-14

                 S
                 Set status C-14
                 shop floor data collection   C-114
                 Split items C-98
                 Surface deletion C-131
                 Surplus Editor C-68

                 T
                 tabs
                 – properties C-125
                 Terms in Rough Scheduling      C-14

                 V
                 Views C-16
                 – configurable components C-17
                 – configure C-19
                 – configure columns C-21
                 – configure filters C-28
                 – configure tabs C-19
                 – configure totals row C-24
                 – define column C-26
                 – exercises C-33
                 – white screen C-32
                 – working with the list C-23
                 views
                 – define totals row C-26
2.50 / 01-2023




                 W
                 white screen C-32
                 Work plan C-122


                 C-140                                 A+W Production Rough scheduling

