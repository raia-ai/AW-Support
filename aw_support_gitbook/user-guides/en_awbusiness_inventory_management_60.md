---
description: "EN AWBusiness Inventory Management 6.0"
---



# EN AWBusiness Inventory Management 6.0

Inventory Management      G




                           English




                 A+W Business
                                                                                                              Introduction




                                     Introduction
                                     This part of the documentation contains editorial notes.


                                     Revision Overview
                                     Section          Description
                                     Version/Date

                                     6.1/04-2020      New: Stock management > Critical stock on hand

                                     6.0/10-2019      Box management settings transfered to separate part and deleted
                                                      from Inventory Management part.

                                     5.2/08-2019      New settings for inventory lists and printing of box labels.

                                     5.10/01-2017     Revision of Inventory, new dialog Stock assessment.

                                     5.00/08-2013     Complete revision of ALFAK documentation and adjustment to
                                                      A+W Business.

                                     4.12/01-2013     Layout adapted to CI 2013.

                                     4.11/02-2012     Corrections

                                     4.10/11-2010     Update and conversion to documentation concept 2010

                                     4.00/08-2009     Complete revision

                                     3.02/09-2008     Illustrations and section number amended.

                                     3.01/08-2008     Correction of spelling errors

                                     3.00/12-2003     Structural conversion to program structure 4.0

                                     2.00/08-2000     Revision Stock

                                     1.00/03-1998     Original version



                                     Editorial
                                     The editorial provides information on the following topics:
                                     •   Notes on this document
                                     •   Copyrights
                                     •   Trademarks
                                     •   Contact
6.1 / 04-2020




                A+W Business Inventory Management                                                                    G-3
                Introduction




                               Notes on this document
                               This document is intended for end users of A+W Business.
                               The documentation and software described are licenses that must only be
                               used or copied in accordance with the conditions of our license agreement.
                               The contents of the documentation are only informative and are subject to
                               changes without prior notice. The text and illustrations were compiled with the
                               utmost care. Still, errors cannot be totally excluded. A+W Software GmbHcan-
                               not be held liable for errors or inaccuracies, unless they can be attributed to
                               wilful or grossly negligent action.
                               This document describes the full scope of A+W Business.

                               Copyrights
                               © 2020, A+W Software GmbH, all rights reserved, also those for reprinting, the
                               making of copies and translation.
                               The documentation may be copied, completely or in part, saved in an archiving
                               system or transferred in any other form only in accordance with our license
                               agreement. Transmission of the documentation is not allowed, neither elec-
                               tronically, nor mechanically, nor by recording or in any other way, without A+W
                               Software GmbH's prior written approval.

                               Trademarks
                               All hardware and software names mentioned in this documentation can also
                               be registered trademarks or other property rights of third parties. Third party
                               copyrights must be observed.

                               Contact
                               A+W Software GmbH

                               Am Pfahlgraben 4-10

                               D-35415 Pohlheim

                                  +49 6404 2051 0

                                  +49 6404 2051 877

                               aw.zentrale@a-w.com

                               http://www.a-w.com
6.1 / 04-2020




                G-4                                                   A+W Business Inventory Management
                                                                                                                                                    Contents




                                     Contents
                                     Introduction ............................................................................................................ G-3
                                       Revision Overview .............................................................................................. G-3
                                       Editorial .............................................................................................................. G-3

                                     Tutorial                                                                                                            G-7
                                     Overview ................................................................................................................ G-9
                                       Documentation ................................................................................................. G-10
                                         Tutorial structure ........................................................................................... G-10
                                         Display conventions ...................................................................................... G-11
                                       Menu Overview ................................................................................................ G-12
                                     Basic Principles of Stock ..................................................................................... G-14
                                     Master Data ......................................................................................................... G-17
                                       Stock ................................................................................................................ G-18
                                         Stock Definition ............................................................................................. G-19
                                         Stock Categories ........................................................................................... G-20
                                         Define Stock Levels ...................................................................................... G-20
                                         Define Storage Location ............................................................................... G-22
                                         Define Stock Categories ............................................................................... G-25
                                         Exercises ...................................................................................................... G-26
                                       Company Data ................................................................................................. G-27
                                         Stock Control Mode and Reservation ........................................................... G-28
                                         Check Company Data ................................................................................... G-29
                                       Status ............................................................................................................... G-32
                                         Status Changes due to Additions and Dispatches ........................................ G-33
                                         Check Status Allocations .............................................................................. G-33
                                       Product Definition ............................................................................................. G-35
                                         Product .......................................................................................................... G-36
                                         Products as Stock Articles ............................................................................ G-37
                                         Stock Sizes ................................................................................................... G-39
                                         Check Product Master Data .......................................................................... G-41
                                         Define Stock Sizes ........................................................................................ G-45
                                         Exercises ...................................................................................................... G-47
                                       Prices ............................................................................................................... G-48
                                         Purchase Price and Average PP ................................................................. G-49
                                         Check Settings for Purchase Price Calculation ............................................ G-54
                                         Check Prices ................................................................................................. G-55
                                         Exercises ...................................................................................................... G-57
                                       Stock control on BOM level .............................................................................. G-58
                                         Reservation and booking of BOM components ............................................ G-59
                                         Checking the setting ..................................................................................... G-61
                                         Checking Products ........................................................................................ G-62
                                     Stock Management .............................................................................................. G-64
                                       Stock Management .......................................................................................... G-65
                                         Elements in Stock management Dialog ........................................................ G-66
                                         Stock Articles ................................................................................................ G-67
                                         Main Stock Products ..................................................................................... G-67
                                         Minimum Stock ............................................................................................. G-68
                                         Prices ............................................................................................................ G-69
                                         Create a Stock Article ................................................................................... G-71
                                         Exercises ...................................................................................................... G-74
                                       Stock Booking .................................................................................................. G-75
6.1 / 04-2020




                                         Stock Movements ......................................................................................... G-76
                                         Booking Types .............................................................................................. G-76
                                         Withdrawals and Additions ............................................................................ G-77


                A+W Business Inventory Management                                                                                                          G-5
                Contents




                               Manual Input of Additions or Dispatches ...................................................... G-78
                               Change Storage Location ............................................................................. G-82
                               Exercises ...................................................................................................... G-84
                             Queries ............................................................................................................. G-85
                               Stock Query .................................................................................................. G-86
                               Show Booking Journal .................................................................................. G-87
                               Print reserved Stock Articles ......................................................................... G-89
                               Show Inventory Statistics .............................................................................. G-91
                               Exercises ...................................................................................................... G-93
                             Stock information .............................................................................................. G-94
                               Stock Search ................................................................................................. G-95
                               Stock on Hand .............................................................................................. G-95
                               Stock Information and Future Stock on Hand ............................................... G-96
                               Show Stock on Hand in Stock Search .......................................................... G-98
                               Exercises .................................................................................................... G-102
                             Stock P.O. (automatic) ................................................................................... G-103
                               P.O. Proposals ............................................................................................ G-104
                               Transfer Stock P.O. to Purchasing ............................................................. G-105
                               Compare Prices before Transfer to Purchasing .......................................... G-110
                               Exercises .................................................................................................... G-112
                           Stock Articles in Documents .............................................................................. G-113
                             Order Entry of Stock Products ........................................................................ G-114
                               Reservation and Booking of Stock Articles ................................................. G-115
                               Search Stock Article for an Item ................................................................. G-116
                               Check the Bookings .................................................................................... G-119
                               Exercises .................................................................................................... G-121
                             Manual Stock P.O. ......................................................................................... G-122
                               Manual Input of Stock P.O. ......................................................................... G-123
                               Exercises .................................................................................................... G-125
                             Production Orders .......................................................................................... G-126
                               Stock Article as Part of the Production Order ............................................. G-127
                               Manual Input by Copying ............................................................................ G-128
                               Settings in Supplier File .............................................................................. G-129
                               P.O. Quantity after Stocktaking ................................................................... G-130
                               Stock Addition based on Production Order ................................................. G-135
                           Inventory ............................................................................................................ G-136
                             Periodical Inventory ........................................................................................ G-137
                               Stocktaking ................................................................................................. G-138
                               Create Inventory List ................................................................................... G-140
                               Determine Target Inventory ........................................................................ G-145
                               Enter Counted Values ................................................................................. G-147
                               Finalize Inventory ........................................................................................ G-149
                               Add Supplementary Inventory ..................................................................... G-151
                               Exercises .................................................................................................... G-152
                             Initial Inventory ............................................................................................... G-153
                               Initial Inventory Process .............................................................................. G-154
                               Execute Initial Inventory .............................................................................. G-155
                           Exercises ........................................................................................................... G-157

                           Section Index                                                                                                 G-159
                           Index .................................................................................................................. G-161
6.1 / 04-2020




                G-6                                                                     A+W Business Inventory Management
Inventory Management        G

                        Tutorial




                 A+W Business
                Tutorial                                                                                      Overview




                                     Overview
                                     The tutorial for the Stock Management module deals with the stock manage-
                                     ment basics in A+W Business. The tutorial is based on the knowledge of mas-
                                     ter data, purchasing, and sales.

                                         The functions depend on the enabled modules
                                         Please note that the individual functions are only available if the corre-
                                         sponding modules and interfaces have been installed and enabled.

                                         If you detect functions in this description that are not available in your ver-
                                         sion, please contact A+W Software GmbH.

                                     Subjects
                                     This tutorial includes the following subjects:
                                     •   Basic Principles of Stock
                                     •   Master Data
                                     •   Stock Management
                                     •   Stock Articles in Documents
                                     •   Inventory

                                     Required knowledge
                                     This tutorial is meant for those who manage stock inA+W Business. Partici-
                                     pants must be familiar with the concept of master data, sales, and purchasing
                                     inA+W Business.

                                         Box management in stock
                                         The settings for box management are described in the separate part Box
                                         management.
6.1 / 04-2020




                A+W Business Inventory Management                                                                  G-9
                Overview                                                                                   Tutorial




                           Documentation
                           The following documents are available for the Stock Management module:

                           Format                       Volume

                           Handout                      Printout of tutorial for training session

                           PDF                          Complete documentation
                                                        • Tutorial
                                                        • Software reference
                                                        • Index

                           Online help <F1>             Context-sensitive dialog help of A+W Business software
                                                        reference and tutorials.


                           Tutorial structure
                           The tutorial consists of subjects with several training modules each. Each
                           training module consists of the following elements:

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
                                                        with cross references pointing out additional information
                                                        in the software reference and in other sections.
                                                        This will help you to extend your newly acquired
                                                        knowledge.


                           Reading instructions
                           The contents of a training module are based on the knowledge conveyed in the
                           previous module. We therefore recommend not to skip any training modules.
                           If you are already familiar with a subject you should at least read the summary at the
                           start of a training module in order to bring the main details to mind.
6.1 / 04-2020




                G-10                                                  A+W Business Inventory Management
                Tutorial                                                                                    Overview




                                     Display conventions
                                     Certain parts of sentences are specially marked. The meanings are:

                                     Italic                  marks character strings describing the software
                                                             elements, e. g. the Stock info dialog.

                                     Bold                    marks character strings to be entered via the keyboard,
                                                             e.g.: Enter the value 0.

                                     >                       The so-called breadcrumb trail marks shows how to
                                                             open a dialog, e. g. Stock management > Inventory >
                                                             Final inventory

                                     []                      Square brackets mark buttons in a dialog, e. g. [OK] to
                                                             save the data.

                                     <>                      Angle brackets refer to keys or shortcuts on the
                                                             keyboard, e. g. <F1> is used to open the online help.
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-11
                Overview                                                                                       Tutorial




                                      Menu Overview
                                      This chapter provides a brief overview of the program sections that will be ad-
                                      dressed in the subjects of this training.




                Fig. G-1   Stock Management menu


                                      Inventory
                                      In this section, prepare the inventory, enter counted values and finalize the in-
                                      ventory.
                                      “Stock Management menu” on page G-12
                                       “Inventory” on page G-136

                                      Stock management
                                      Use this dialog to enter and maintain data for stock articles.
                                       “Stock Management” on page G-65

                                      Stock movement
                                      Use this dialog to book goods received and issued, changes of stock locations
                                      and opening of boxes.
                                       “Stock Booking” on page G-75
6.1 / 04-2020




                G-12                                                         A+W Business Inventory Management
                Tutorial                                                                                   Overview




                                     Queries
                                     In this section, view the stock history, analyses and reservations.
                                      “Queries” on page G-85

                                     Search
                                     Use this dialog to check the product availability during a certain time period.
                                      “Stock information” on page G-94

                                     Stock P.O.
                                     Use this dialog to transfer purchase orders for stock articles to purchasing.
                                      “Transfer Stock P.O. to Purchasing” on page G-105


                                     Additional information
                                      Overview, “Elements of the Program Window” on page A-51
                                      Sales, “Document management dialog” on page C-39
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-13
                Basic Principles of Stock                                                                                      Tutorial




                                            Basic Principles of Stock
                                            A+W Business's Stock Management module allows you to manage jumbo siz-
                                            es, stock sizes, residual plates, boxes, all-glass doors, fittings, frame parts and
                                            accessories, such as mirror mountings, sealing tape, etc.
                                            It is possible to map your company's stock organization in the program. You
                                            define the locations, corridors, shelves, up to the individual trays and specify
                                            which single articles, sqm articles and linm articles are located at which stor-
                                            age location.



                                                          Order
                                                                                                      P.O. item

                                                                                      Stock



                                                                                 Stock on hand
                                                                                                                  Purchasing
                                                               Stock article
                                                                                   Reservation

                                                                               Materials planning

                                                                                 Stock shortage                    Supplier
                                                       Delivery note
                                                                               Booking out of stock
                                                         Invoices
                                                                               Booking addition to         Receipt of goods
                                                                                     stock




                                                                                    Analyses



                                            Fig. G-2        Overview of stock management


                                            All commercial transactions in A+W Business are based on the master data.
                                            Only if the master data is properly maintained, stock can be managed without
                                            problems. In conjunction with Sales and Purchasing, the following processes
                                            are created:
                                            •   Order:
                                                An order defines the customer's purchase order. You enter all the items that
                                                must be produced in accordance with the customer's specifications.
                                            •   Transfer to production:
                                                Order items to be produced are transferred to production.
6.1 / 04-2020




                                                The required materials are reserved and are booked out of stock when the
                                                delivery note or invoice is printed. At the same time, the available stock on
                                                hand is updated.

                G-14                                                                     A+W Business Inventory Management
                Tutorial                                                                     Basic Principles of Stock




                                     •   Stock P.O.
                                         If stock articles fall short of the minimum stock, these stock articles must be
                                         entered in the form of a stock P.O.
                                     •   Stock addition:
                                         The stock on hand of the stock articles is updated by entering the goods
                                         receipt. Articles that are not kept as stock articles cannot be kept as stock
                                         on hand.
                                     •   Inventory:
                                         With the inventory you correct the stock on hand figures in A+W Business.

                                     Stock management processes
                                     You usually maintain the stock on hand by carrying out the following activities:
                                     •   Set up master data:
                                     •   Enter stock articles (initial inventory)
                                     •   Book receipt and issue of goods (automatically, manually)
                                     •   Queries concerning stock turnover, prices, stocks on hand, etc.
                                     •   Enter, check and send stock P.O.
                                     •   Carry out inventory:
                                         – Create inventory list, add supplementary inventory
                                         – Determine target inventory
                                         – Print count lists
                                         – Enter counted values
                                         – Finalize inventory

                                     How should stock be managed
                                     All products that are entered in Sales are assigned with a code that defines the
                                     type of purchase. In addition to the code (procurement type) Stock Withdrawal,
                                     glass pieces that are kept on stock have a code (stock booking type) to indi-
                                     cate how its stock on hand is calculated. These two codes are described in the
                                     thematic block Master Data.
                                     Before you set up your stock in A+W Business, you have to decide on the ba-
                                     sis of how your stocks should be managed: as an area (sqm) or in numbers of
                                     pieces. A third possibility is the combined stockkeeping, whereby the size-de-
                                     pendent stock mode is combined with the reports from the optimization so that
                                     in addition to the stock dimensions, the stock sizes cut can be booked out au-
                                     tomatically.
                                     These different options have different effects:
6.1 / 04-2020




                A+W Business Inventory Management                                                                G-15
                Basic Principles of Stock                                                                                Tutorial




                Mode                        Meaning, example                                            Disadvantage
                (Stock code)

                sqm = area:                 the area is determined per glass piece:                     • no information about
                (not size-related)                                                                        the number of stock
                                            • Float 4 => 10,500 sqm
                                                                                                          sizes
                                                                                                        • no information about
                                                                                                          how many stock sizes
                                                                                                          were cut




                                            • Float 5 => 11,070 sqm




                                            • Float 6 => x sqm


                Piece:                      the quantity is determined per jumbo size and per stock     • no information on the
                (size-related)              size:                                                         cut jumbo and stock
                                                                                                          sizes
                                             • Float 4
                                                                                                        • Stock sizes must be
                                                                                                          booked out manually




                                                    3210 / 6000              900 / 1200        x/x
                                                     3 pieces                 3 pieces       n pieces

                                            • Float 5




                                                    3210 / 6000             800 / 1200        x/x
                                                     3 pieces                3 pieces       n pieces


                Piece incl. reports:        Combination of size-related stock and reports. The cut      (For this mode, A+W
                (combined)                  stock sizes and stock dimensions are automatically          Optimizer reports must
                                            booked out. The stock quantity of the quantities are        be permitted.)
                                            updated.

                                            After deciding about the mode, allocate the corresponding stock code per
                                            glass product and define the stockkeeping mode in the company data. These
6.1 / 04-2020




                                            settings are described in the thematic block Master Data.




                G-16                                                                  A+W Business Inventory Management
                Tutorial                                                                              Master Data




                                     Master Data
                                     In this thematic block, we will show you how you maintain the master data for
                                     managing your stock.
                                     This includes the following training modules:
                                     •   “Stock” on page G-18
                                     •   “Company Data” on page G-27
                                     •   “Status” on page G-32
                                     •   “Product Definition” on page G-35
                                     •   “Prices” on page G-48
6.1 / 04-2020




                A+W Business Inventory Management                                                           G-17
                Master Data                                                                                   Tutorial




                              Stock
                              Objectives

                              • Name stock levels.
                              • Define storage location.
                              • Define stock categories.


                              Benefits

                              • With storage places you can manage (the same) materials at different locations.
                              • Analyses can refer to certain storage locations or stock articles that are stored at
                                different locations.


                              Please note:

                              Levels                       Four different levels define e.g. various warehouses,
                                                           corridors, shelves, and trays.

                              Storage locations            The combination of the different differentiation levels
                                                           form the storage locations.

                              Stock categories             By using stock categories you can restrict the search
                                                           and analysis to certain products that are stored at
                                                           different locations.

                              Default settings             None
6.1 / 04-2020




                G-18                                                     A+W Business Inventory Management
                Tutorial                                                                                          Master Data




                                           Stock Definition
                                           Set the following settings to display your stock:
                                           •     Names of stock levels
                                           •     Stock levels
                                           •     Storage locations
                                           You can adjust the names of the different levels to the requirements in your
                                           company. You should also use this option if you only work with one level.

                                           Storage location
                                           You can specify up to four differentiation level to define storage places to dif-
                                           ferentiate for example between warehouses, aisles, shelves and trays. The
                                           storage locations are used for stock management and for the inventory.


                                                                    Warehouse 1




                                                                     Corridor A


                                         Shelf 1                                             Shelf 2


                           Tray 1        Tray 2            Tray 3                 Tray 4      Tray 5         Tray 6




                                                                    Corridor B


                                        Shelf m                                              Shelf n



                           Tray           Tray             Tray                   Tray        Tray




                Fig. G-3      Example: Storage location = Warehouse 1


                                           Stock level
                                           For each level you can define different names, e. g. on level 1 the warehouses
                                           at different storage places, on level 2 corridors A through F, etc.

                                                 Define at least one storage location
6.1 / 04-2020




                                                 You must define a storage location even if you did not divide your stock. In
                                                 this case, just define level 1 and then define all other levels in the storage
                                                 location as <n.e.>.


                A+W Business Inventory Management                                                                        G-19
                Master Data                                                                          Tutorial




                              Stock Categories
                              Stock categories provide you with another search criterion for stock manage-
                              ment. For example, if you manage the same material at different storage loca-
                              tions, you can use the stock category to analyze the materials together. For
                              this purpose you must have defined all storage locations where the materials
                              are actually kept.
                              Assign the defined stock categories to the products in the Stock Management
                              dialog.


                              Define Stock Levels
                              This module shows you how to adjust the stock levels to the requirements in
                              your company.
                              The following instructions exist for this training module:
                              •   “How you define your different stock levels” on page G-20
                              •   “How to name stock levels” on page G-22


                               How you define your different stock levels
                                  The following steps are the same for all stock levels. In this example, we
                                  will create a stock level 1 for finished products.
                              1 Select menu Master data > Stock > Level 1.
                                  Dialog Level 1 opens.
6.1 / 04-2020




                G-20                                                  A+W Business Inventory Management
                Tutorial                                                                               Master Data




                                     2 Go to the menu Start > New to switch to the input mode.




                                        Fig. G-4     Line for new stock level


                                     3 Enter a name for the stock level, e. g. name of the place, cutting, etc.
                                     4 Go to the menu Start > Save to save the data.
                                        The data is saved.
                                     5 Repeat steps 1 through 4 for all levels that you would like to differentiate
                                       between in your stock. For this purpose, also open the dialogs to stock lev-
                                       els 2 through 4 and proceed in the same way.
6.1 / 04-2020




                A+W Business Inventory Management                                                             G-21
                Master Data                                                                              Tutorial




                               How to name stock levels
                              1 Select menu Master data > Stock > Stock definition.
                                 Dialog Stock definition opens.
                              2 Go to menu Definition > Levels.




                                 Fig. G-5      Name stock levels


                              3 Define the names of the stock levels, e. g. Warehouse for level 1.
                              4 Click on [OK] to save the names.
                                 The dialog closes. The changes are adopted in the Stock definition dialog.
                              5 Close the Stock definition dialog or define the storage locations now.


                              Define Storage Location
                              This training module shows you how to set up storage locations in
                              A+W Business.
                              You must define a storage location even if you did not divide your stock. In this
                              case, just define level 1 and then define all other levels for the storage location
                              as <n.e.>. Please note that a storage location with the definition <n.e.> can
                              also be used for booking purposes as the storage location for all levels.

                                 Tip
                                 You can move certain materials from a warehouse to the production area.
                                 For this purpose, the storage location is changed. In this case, it is helpful
                                 if you define the storage location as precisely (detailed) as possible, e. g.
                                 concerning the trays.
6.1 / 04-2020




                G-22                                                   A+W Business Inventory Management
                Tutorial                                                                                    Master Data




                                      How to define a storage location
                                     1 Select menu Master data > Stock > Stock definition.




                                      A




                                      B




                                     A Your selected name of the levels       B List of defined storage locations
                                     Fig. G-6      Define storage locations


                                          Use this mode to change the defined storage location (A), by changing the
                                          names of the levels. The fields of the table are locked if you have chosen
                                          the input mode.
                                     2 Go to the menu Start > New to switch to the input mode.
6.1 / 04-2020




                A+W Business Inventory Management                                                                   G-23
                Master Data                                                                           Tutorial




                                              A                             B




                              A Selection of defined stock levels       B Parameters
                              Fig. G-7     Fields in the table locked


                              3 Select an entry on each level (A).
                              4 Define one of the parameters (B), if applicable, if the storage location shall
                                be specifically marked, e. g. as default stock.
                                 If you have selected the entry Hegla as stock type, you can specify the stor-
                                 age location for the goods receipt from the Hegla deliveries.
                              5 Go to Menu Start > Save to save the storage location.
                                 The data is saved.
                              6 Repeat steps 2 through 5 for all storage location that you require for man-
                                aging your stock.
6.1 / 04-2020




                G-24                                                    A+W Business Inventory Management
                Tutorial                                                                             Master Data




                                     Define Stock Categories
                                     This module shows you how you define the stock categories that you want to
                                     allocate to the stock articles.


                                      How to define a stock category
                                     1 Select menu Master data > Stock > Category.




                                        Fig. G-8     Stock categories


                                     2 Go to the menu Start > New to switch to the input mode.
                                     3 Enter an ID for the stock category, e. g. figures or names, such as raw ma-
                                       terial, production.
                                     4 Go to the menu Start > Save to save the data.
                                        The data is saved.
6.1 / 04-2020




                A+W Business Inventory Management                                                           G-25
                Master Data                                                                          Tutorial




                              Exercises
                              •   Rename all four stock levels.
                              •   Create four different storage locations from which at least one is intended
                                  for raw materials.


                              Additional information in the Master Data section
                               Master Data, “Level 1 to 4” on page B-735
                               Master Data, “Stock Definition” on page B-736
                               Master Data, “Stock Categories” on page B-738
6.1 / 04-2020




                G-26                                                 A+W Business Inventory Management
                Tutorial                                                                                       Master Data




                                     Company Data
                                     Objectives

                                     • Getting familiar with settings for reservations (Stock Control mode).
                                     • Getting to know the settings for determining the purchase price.
                                     • Define the time period for the stock preview.


                                     Benefits

                                     • Reservations have an impact on the stock on hand. The stock on hand can already
                                       be updated with the reservation so that reserved quantities are no longer available.
                                     • The stock preview shows the current stock on hand and the reserved quantities for
                                       a time period that you define.
                                     • The purchase price of stock articles can be updated automatically. Then, either the
                                       average PP is calculated or the one that was last entered.


                                     Please note:

                                     Stock control mode           The Stock Control mode in the company table defines
                                                                  how reservations influence the stock on hand.

                                     Stock code                   The stock code defines whether the stock on hand for an
                                                                  article is evaluated as a surface (sqm) or a quantity
                                                                  (pieces).

                                     Reservation                  To produce an order item, the required quantities are
                                                                  reserved. The quantities are marked in the stock on
                                                                  hand or booked out.

                                     Default settings             None
6.1 / 04-2020




                A+W Business Inventory Management                                                                    G-27
                Master Data                                                                            Tutorial




                              Stock Control Mode and Reservation
                              When a product with procurement type Stock Withdrawal is entered in an or-
                              der, the corresponding quantity (plus waste in the case of fixed sizes) of the
                              stock article is marked as reserved. The reservation can optionally either be
                              booked out of the current stock on hand or automatically when the delivery
                              note or invoice is printed.
                              •   Reservation without stock update:
                                  The quantity is marked as reserved, but is not yet booked out from the
                                  stock. Booking out must be carried out manually.
                              •   Reservation with stock update:
                                  The reserved quantity is booked out from the current stock by printing the
                                  delivery note or invoice. The status allocation determines which document
                                  triggers the booking process.
                              •   Execute stock booking before document printout:
                                  Stock articles can be booked out before the document is printed. In the
                                  event of a problem with the stock withdrawal booking, the order is not print-
                                  ed.
                              These settings are shown in the stock quantities display in dialog Stock Info
                              (stock preview) and the automatic purchase order suggestions that can be trig-
                              gered when minimum quantities are reached.
6.1 / 04-2020




                G-28                                                  A+W Business Inventory Management
                Tutorial                                                                                        Master Data




                                           Check Company Data
                                           This module shows you how to set the parameters to evaluate the stock and
                                           for the stock control mode.


                                            How to check the settings for the stock
                                           1 Select menu Master Data > Company > Company Data.
                                           2 Switch to the Parameter tab and check the settings for the virtual item num-
                                             bers.




                                                                                                                         A




                A Virtual item numbers for receipt of boxes
                Fig. G-9     Company Data > Parameters


                                               The virtual item number is necessary for booking the receipt of box items
                                               with a quantity of > 1 correctly. The receipt of boxes is described in detail
                                               in the Box management section.
                                           3 Go to the Stock / PP / EDI tab.
6.1 / 04-2020




                A+W Business Inventory Management                                                                      G-29
                Master Data                                                                                         Tutorial




                A




                B




                C




                A Settings for determining the purchase price          C Number of preview days for dialog Stock Info
                B Setting to update the stock on hand
                Fig. G-10     Company data - Stock / PP / EDI


                                              Learn about the settings for determining the purchase price in the Prices
                                              module.
                                           4 Select the settings for stock P.O.s (A):
                                              •   Include spacers in muntins orders:
                                                  Enable this checkbox if the spacers on a bill of materials (BOM) should
                                                  be ordered together with muntins, the procurement type of which is set
                                                  to P.O.
                                              •   IG as P.O. item (processing can be done in-house):
                                                  Activate this checkbox if the IG unit should be ordered without process-
                                                  ing. Processing is then carried out in-house.
                                              •   Show items w/o stock code at receipt of goods on stock:
                                                  Activate this checkbox if items in stock P.O.s without stock code should
                                                  be displayed in red at goods receipt.
                                           5 Select the functions that should be considered when updating the stock on
                                             hand in the Stock Control Mode (B).
6.1 / 04-2020




                                              •   Reservation w/o stock update:
                                                  Enable this option if reserved quantities should not be booked out of the



                G-30                                                              A+W Business Inventory Management
                Tutorial                                                                                Master Data




                                            current stock. You must then manually carry out the withdrawal booking.
                                            The current stock is therefore not shown at order entry.
                                        •   Reservation with stock update:
                                            This option is enabled by default so that reserved quantities are booked
                                            out from the current stock when the delivery note or invoice is printed.
                                        •   Stock control on BOM level:
                                            Check this checkbox if products should be managed in the stock even
                                            if they are part of a BOM.
                                        •   Execute stock booking before document printout:
                                            Check this checkbox if stock articles should be booked out before the
                                            document is printed. In the event of a problem with the stock withdrawal
                                            booking, the order is removed from the documents to be printed and is
                                            therefore not printed.
                                     6 Enter the number of workdays (C).
                                        The number of workdays is analyzed for the preview in the Stock Info dia-
                                        log. It specifies the time period for which the future stock on hand will be
                                        shown.
                                     7 Go to the menu Start > Save to save the changes.
                                        The data is saved. You should restart A+W Business after changing the
                                        company data.

                                        Status allocation for stock withdrawal booking
                                        If you have enabled the option Execute stock booking before document
                                        printout you should check the status allocation for the stock withdrawal
                                        booking. The minimum, assigning and lock status must be organized in a
                                        manner that stock withdrawal bookings can be executed prior to printing. If
                                        the status allocation does not allow reversal of the order it may be possible
                                        that the stock withdrawal booking is not executed.

                                        You will learn about status allocations in the next module.
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-31
                Master Data                                                                                Tutorial




                              Status
                              Objectives

                              • Getting familiar with status changes due to goods received and goods issued.
                              • Check relevant status points and allocations.


                              Benefits

                              • With status allocations, you create the prerequisites for automatic status changes
                                in documents and for the stock bookings.


                              Please note:

                              Status                      The status defines when the stock values shall be
                                                          updated.

                              Default settings            None
6.1 / 04-2020




                G-32                                                    A+W Business Inventory Management
                Tutorial                                                                                 Master Data




                                     Status Changes due to Additions and Dispatches
                                     Goods dispatches and receipts can change the status of documents and result
                                     in stock changes due to the status change. If the status points and status allo-
                                     cations are defined correspondingly, this will also apply to partial deliveries.
                                     If you have enabled the option Execute stock booking before document print-
                                     out, the minimum, assigning and lock status must be organized in a manner
                                     that stock withdrawal bookings can be executed prior to printing. If the status
                                     allocation does not allow reversal of the order it may be possible that the stock
                                     withdrawal booking is not executed.


                                     Check Status Allocations
                                     This module shows you how to check and, if applicable, change the status al-
                                     location.
                                     The following instructions exist for this training module:
                                     •   “How to check the status management” on page G-33
                                     •   “How to check the status allocation” on page G-34


                                      How to check the status management
                                     1 Go to menu Master data > Order > Status management.




                                         A




                                         B



                                         A Status for stock addition           B Status for stock dispatch
                                         Fig. G-11    User status (examples)


                                     2 Check whether the user status for stock additions and stock dispatch ex-
                                       ists. Create them if necessary.
                                     3 For this purpose, go to the menu Start > New to switch to the input mode.
                                         A new line is enabled.
6.1 / 04-2020




                                     4 Enter the number and name.
                                     5 Go to the menu Start > Save to save the data. The data is saved.


                A+W Business Inventory Management                                                               G-33
                Master Data                                                                          Tutorial




                              6 Repeat the steps 3 to 5 to create another user status.
                              7 Next, check the status allocations.


                               How to check the status allocation
                              1 Select menu Master Data > Order > Status allocation.




                                 Fig. G-12    Master Data > Order > Status allocation


                              2 Check whether the status allocations of stock addition and stock dispatch
                                for document types Order and P.O. have been defined:
                                 •   Stock goods dispatch: Status Delivery note printed or Invoice printed
                                 •   Stock goods receipt: Status Goods receipt booked
                                 For goods receipts and partial goods receipts the following allocations must
                                 be defined:
                                 •   OC supplier partial/order
                                 •   OC supplier complete/order
                                 •   Receipt of goods partial/order
                                 •   Receipt of goods - complete/order
                                 •   Receipt of goods partial/P.O.
                                 •   Receipt of goods - complete/P.O.
                                 •   OC supplier partial/P.O.
                                 •   OC supplier complete/order
                              3 Create missing allocations and correct existing ones if necessary.
                              4 Go to the menu Start > Save to save the data.
                                 The data is saved.
6.1 / 04-2020




                G-34                                                  A+W Business Inventory Management
                Tutorial                                                                                       Master Data




                                     Product Definition
                                     Objectives

                                     •   Knowing the difference between stock size and stock article.
                                     •   Knowing the interaction of product, stock article, and stock size.
                                     •   Getting familiar with product and stock codes.
                                     •   Differentiate between settings in the main product and in the BOM.


                                     Benefits

                                     • If the products are defined correctly, pieces and surfaces can be calculated and
                                       reserved.
                                     • The display of the actual stock on hand including reservations makes purchasing
                                       easier.


                                     Please note:

                                     Products                     The products from the master data are used for entry
                                                                  and pricing in documents. They are not automatically
                                                                  kept as stock on hand; this is only the case as a result of
                                                                  additional settings and definitions.

                                     Stock articles               All products that are kept in the warehouse with stock
                                                                  quantities must be created as stock articles.

                                     Jumbo size                   Glass plate as delivered by the manufacturer. It is used
                                                                  to cut the glass pieces for Sales.

                                     Stock plate                  Glass in certain sizes that is actually on hand in the
                                                                  warehouse, e. g. Float 4 mm in 1200 x 1800 mm or
                                                                  3500 x 5100 mm. Stock plates with defined sizes are
                                                                  also called stock size.
                                                                  Stock plates can be processed as a whole
                                                                  (1200 x 1800). However, it is also possible to use them
                                                                  to cut glass pieces, e. g. 600 x 900 from the plate
                                                                  1200 x 1800 or from the plate 3210 x 5100.

                                     Stock size (fixed dimension) Sheets defined as stock sizes are sold without being cut.
                                                                  They have special price tables (stock size tables)
                                                                  allocated. A size-related stock article is always also a
                                                                  stock size.

                                     Stock code (stock booking The stock code defines whether the stock on hand for an
                                     type)                     article is evaluated as a surface (sqm) or a quantity
                                                               (pieces).

                                     Procurement type             This code defines the standard way of obtaining a
                                                                  product, e. g. by cutting, stock withdrawal, production,
                                                                  purchase order.

                                     Default settings             None
6.1 / 04-2020




                A+W Business Inventory Management                                                                      G-35
                Master Data                                                                                             Tutorial




                                             Product
                                             Products are entered with specific sizes for the order items from where they
                                             are transferred to Production. In Production, the sheets for the order item are
                                             cut from stockplates or taken from the stock sizes on hand.
                                             Information on material consumption is essential for keeping stock. Consump-
                                             tion includes the waste. The calculated surface or quantity is reserved on stock
                                             after order entry.



                   Sales                                               Stock (on hand)

                            Order                         Cutting of stock article        Stock article Float 4 (stock
                    Item:                                 Float 4 (stock plate)           size 400 x 600)

                    • Float 4
                    • 400 x 600 mm




                                                          Consumption = surface           Consumption = units
                                                          (glass + waste)




                                                                       Price

                            Order                         Fixed size (cutting)            Stock size
                                                          Float 4 per sqm                 Float 4 400 x 600 per piece
                    Item:                                                                 Purchase price list
                    Sales price list                      Purchase price list
                                                                                          Price table stock sizes
                                                          Price table fixed sizes




                Fig. G-13      Relations between product, stock size, and price
6.1 / 04-2020




                G-36                                                                 A+W Business Inventory Management
                Tutorial                                                                                  Master Data




                                     Procurement type
                                     Each product is allocated to a procurement type, e. g.:
                                     •   Stock withdrawal (for stock articles)
                                     •   Cutting (for glass that must be cut)
                                     •   Production (for lite that shall be assembled, e. g. IT, laminated glass)
                                     •   P.O. (for products that are not kept on stock)
                                     At the time of the initial inventory, stock articles are automatically created
                                     based on the procurement type Stock withdrawal and the stock code (sqm or
                                     piece).


                                     Products as Stock Articles
                                     All products that are kept in the warehouse with stock quantities must be cre-
                                     ated as stock articles.
                                     Stocks of stock articles can be kept differently in the warehouse, namely either
                                     by considering their dimensions or the number of pieces. With the code for the
                                     stock booking type you are defining one of these options. These correlations
                                     are illustrated in the basic principles regarding stock management:
                                      “How should stock be managed” on page G-15

                                     Stock booking type (stock code)
                                     Each product is allocated to one of the following stock booking types in the
                                     master data:
                                     •   Size-related:
                                         several stock articles per product (glass in different sizes)
                                         Stock booking type = pieces
                                         Products with this code are kept on stock as units. These are usually glass
                                         sheets with fixed dimensions. Each stock size is then a separate unit.
                                         In the stock on hand, the total area of these stock sizes is not valuated, but
                                         for example 6 pieces of stock size Float 4 in size 600 x 800 mm, 12 pieces
                                         of Float 4 with 800 x 1200 mm.
                                     •   Not size-related:
                                         one stock article per product without sizes
                                         stock booking type = sqm
                                         Products with this code are kept in the warehouse by the quantity unit of
                                         the product, e. g. hinges, handles as units, glass sheets by square meter.
                                         The total area of the glass sheet can then consist of any number of plates
                                         and residual pieces. Stock sizes must then be booked out manually.
                                     •   Combined:
                                         Stock booking = Piece or sqm
                                         Products with this code are kept by sqm as well as a unit. This setting only
                                         makes sense if stock keeping analyzes reports from A+W Optimizer. These
                                         reports show which stock sizes were cut. The code is used to automatically
6.1 / 04-2020




                                         keep stock of jumbos as well as stock sizes.




                A+W Business Inventory Management                                                                G-37
                Master Data                                                                           Tutorial




                              Stock bookings for combined stock control
                              The combined stock control mode allows stock keeping for cut and fixed sizes
                              on square meter, as well as on piece basis. With the A+W Optimizer report it
                              is then possible to automatically book stock sizes that have been cut out of the
                              stock (instead of only the sqm quantity).
                              A sqm stock article of the size 0 x 0 mm will be used for the reservation; it
                              serves as a kind of temporary buffer.
                              •   The quantity is reserved from the sqm article.
                              •   After the report from production, this reservation is canceled.
                              •   The quantity is transferred to the jumbo.
                              •   By printing the delivery note, the quantity is booked out. This reduces the
                                  number of pieces in the stock size. The remaining quantity is transferred to
                                  the sqm stock.
                              Exception:
                              If the delivery note is printed prior to the A+W Optimizer report, the corre-
                              sponding square meters are initially booked out (dummy booking). Then when
                              the A+W Optimizer report is received, this sqm booking is corrected and the
                              corresponding stock sizes are booked out. For the dummy booking, a different
                              product number may have to be entered in the field Key Optimizing in the
                              Product Management, tab Production.
6.1 / 04-2020




                G-38                                                 A+W Business Inventory Management
                Tutorial                                                                                             Master Data




                                             Stock Sizes
                                             Glass panes in fixed sizes can be defined as stock sizes and/or boxes. In ad-
                                             dition to the stock sizes, you must also create stock articles. Stock articles are
                                             used for inventory management. If you have created a stock size in the master
                                             data, A+W Business provides you with the option to immediately switch to
                                             stock management. In the thematic block Stock Management you will be
                                             shown how you create stock articles.


                                                                                                      A


                                                                                                      B

                                                                                                      C
                                                                                                                     D




                            F            E




                A Product management – stock       C      Stock sizes with different           E Allocation of price tables
                  sizes (master data)                     dimensions                           F Determining the PP in the stock
                B Product number pertaining to the D      Stock articles relating to the stock
                  stock sizes                             sizes (stock management)
                Fig. G-14       Stock sizes (product management) and related stock articles


                                             Each stock size can be allocated to a separate price table.
                                             If you work with the stock code size-related, you must create stock articles for
                                             all stock sizes.

                                                 Create stock size box in the dialog Stock sizes
                                                 The stock size Box is mandatory for stock bookings. For entering a box as
                                                 an order or purchase order item, a stock article/size called Box must there-
6.1 / 04-2020




                                                 fore have been created. For a detailed description, please see the Box
                                                 management section.




                A+W Business Inventory Management                                                                           G-39
                Master Data                                                                                   Tutorial




                              Stock sizes vs. stock articles
                              Stock sizes are defined in the master data for all products you are keeping on
                              stock as fixed sizes, e.g. for Float 4, the sizes 600 x 800 mm, 1200 x 1800,
                              2400 x 2800 mm, etc. These stocksizes do not serve the purpose of stock-
                              keeping; they are used for pricing only.
                              Every stock size can be allocated its own price table in order to distinguish e.g.
                              prices with and without cutting. Usually, sqm prices will also be used for stock
                              sizes. You can also enter stock sizes which are only ordered. Every stock size
                              can be allocated to a special product group.
                              Stock sizes defined in master data must also be defined in stock management
                              if they are to be kept as stock articles (with stock on hand). A+W Business al-
                              lows to switch directly from master data to stock management.


                                            Master data                               Stock management

                               Product              Stock size                          Stock articles

                               Float 4 mm            600 x 800 mm                        600 x 800 mm
                                                    1200 x 1800 mm                      1200 x 1800 mm
                                                    2400 x 2800 mm                      2400 x 2800 mm


                              Fig. G-15     Product, stock size, and stock article


                              Special case: Non size-related stock withdrawal
                              Except one special case, the stock size table (master data) is not linked with
                              the stock but is only used to show the price differences for statistical purposes.
                              This special case relates to stock articles with the code non size-related for
                              which a stock size has been entered in the stock size table.
                              No waste will be reserved for this non size-related stock article, and there is
                              no transfer to production if there is such a size in the product stock size table.

                                 Example: Reservation with/without waste

                                 Product                                             Stock article


                                                                   without stock size      with stock size in
                                                                   in stock size table     stock size table

                                 Float 4 mm                        not size-related        not size-related
                                                                   500 x 500 mm            500 x 500 mm
                                 Waste 10%
                                 Ordered quantity 500 x 500 mm

                                  Reserved quantity                0.275 sqm               0.25 sqm
6.1 / 04-2020




                G-40                                                    A+W Business Inventory Management
                Tutorial                                                                                       Master Data




                                            Check Product Master Data
                                            The products defined in master data serve as a basis for item input in the doc-
                                            uments. On the shop floor, the sheets for the order item are cut from stock-
                                            plates or taken from the stock sizes on hand.
                                            This session shows you how to define product data in such a way that the
                                            stock on hand and prices are calculated correctly.


                                             How to check a product's master data
                                            1 Select menu Master Data > Products > Articles > Articles.
                                               Dialog Product Management opens.
                                            2 Search the product you want to keep in stock and check the quantity unit.




                                                                                                                      A




                A Quantity unit for calculating prices and stock on hand
                Fig. G-16     Product Management - Product


                                               The quantity unit has to be selected to allow the correct calculation of the
                                               stock on hand, e.g. pcs. for hinges and sqm for glass.
                                            3 Go to tab Price/Surcharge and check the settings.
6.1 / 04-2020




                A+W Business Inventory Management                                                                    G-41
                Master Data                                                                             Tutorial




                                                                                      A




                                                                                      B


                                                                                      C



                                 A Price table for purchasing              C Sales and purchase price
                                 B Waste to be taken into account for        calculation
                                   reservation
                                 Fig. G-17    Product management - Price/Surcharge


                                 •   Are price tables (A), waste (B), and the checkboxes Price-relevant (C)
                                     for sales/purchasing correctly enabled?
                                 •   The checkbox Price-relevant PP must be checked so that the purchase
                                     price can be calculated.
                              4 Go to tab Stock/purchasing and check the setting.
6.1 / 04-2020




                G-42                                                    A+W Business Inventory Management
                Tutorial                                                                                   Master Data




                                                                                           A

                                                                                           B




                                                                                           C

                                     A Stock booking type (stock code)          C Maximum sizes for ordering the
                                     B Availability check                         stockplate

                                     Fig. G-18    Product management - stock/purchasing


                                        You can choose from the following stock booking types for stock articles
                                        (A):
                                        •   Size-related:
                                            Choose this setting if stock sizes are to be kept as units. This setting
                                            only makes sense for glass.
                                            Please still set the quantity unit on tab Product to sqm so that the sur-
                                            face can be calculated.
                                        •   Not size-related:
                                            Choose this setting for all stock articles to be kept with their actual quan-
                                            tity unit, e.g. units, fittings.
                                            Also use this setting for glass which is to be kept in sqm.
                                        •   Combined:
                                            Choose this setting if you are using reports from A+W Optimizer. This set-
                                            ting only makes sense for glass.
                                            Please note that you have to define a dummy stock size in sqm but with-
                                            out sizes for this purpose.
                                            The setting w/o will not be used in this context.
                                     5 Define whether the availability (B) of the product shall be checked.
                                        If the stock article does not have to be taken into account in the stock pre-
                                        view, an availability check is not necessary.
                                     6 If the product in question includes BOM components, please go to tab
                                       BOM.

                                        Stock control on BOM level
                                        If you have chosen the option Stock control on BOM level in the company
                                        data, the procurement type of the corresponding BOM component must be
                                        set.
                                        This stock control type will be introduced in section Stock control on BOM
                                        level.
6.1 / 04-2020




                A+W Business Inventory Management                                                                 G-43
                Master Data                                                                                    Tutorial




                                                                                                                A
                                                                                                                B




                A Procurement type of the component         B Calculate purchase price
                Fig. G-19     Product management – BOM components


                                         7 Mark the corresponding BOM component and select the procurement type
                                           (A) if this shall differ from the procurement type defined in this element's
                                           master data.
                                            If the procurement type for the main product has been set to Production,
                                            the BOM components can be kept as stock products at the same time.
                                            When you enter such a main product in your order, all BOM components
                                            will be set to reserved in the stock info.
                                         8 Go to Menu Start > Save to save the data.
                                            The data is saved.
6.1 / 04-2020




                G-44                                                           A+W Business Inventory Management
                Tutorial                                                                                         Master Data




                                           Define Stock Sizes
                                           This session shows you how to define stock sizes for the products to allow you
                                           to differentiate pricing.


                                            How to define stock sizes in master data
                                           1 Select menu Master data > Product > Products > Stock sizes
                                               The dialog Stock sizes opens.
                                           2 Go to menu Start > New and enter the stock size.




                                                                                                                     A




                                                                                                                     B

                                                                                                                     C




                A Sheet size (contents only for boxes)             B Set price tables for sales and purchasing
                                                                   C Pricing in stock
                Fig. G-20    Create stock size for pricing


                                               If you have already defined a corresponding stock article in stock manage-
                                               ment, enter the same values for width and height (A).
6.1 / 04-2020




                A+W Business Inventory Management                                                                        G-45
                Master Data                                                                          Tutorial




                              3 You can make the following, different settings:
                                 •   Price code for sales and purchasing (B).
                                 •   Name and short name (matchcode), e.g. for better identification of stock
                                     articles.
                                 •   Procurement type, e.g. Stock withdrawal for stock articles.
                              4 Check the checkbox Search stock PP (C) if the stock size is to be included
                                in pricing.
                                 Section Prices explains the necessary settings for the different calculation
                                 types.
                                  “Purchase Price and Average PP” on page G-49
                              5 Go to the menu Start > Save to save the data.
                                 The data is saved. Next, the system will want to know whether you want to
                                 define this stock size as a stock product as well.
                              6 Choose [Yes] if the stock size is also to be managed as a stock article.
                                 The Stock management dialog opens.
                                 The steps for creating a stock article are described in a separate unit.
                                  “Create a Stock Article” on page G-71
6.1 / 04-2020




                G-46                                                 A+W Business Inventory Management
                Tutorial                                                                               Master Data




                                     Exercises
                                     •   Define stock sizes for some of your products.
                                     •   Make sure that these stock sizes are also defined as stock articles.


                                     Additional information
                                      “Stock Sizes” on page G-39
                                      “Stock Control Mode and Reservation” on page G-28
                                      Master Data, “Product Definition” on page B-182
                                      Master Data, “Product Management” on page B-590
                                      Master Data, “Stock Sizes” on page B-635
                                      Master Data, “Company Data – Stock/Purchasing/EDI” on page B-955
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-47
                Master Data                                                                                Tutorial




                              Prices
                              Objectives

                              • Check price definitions for the purchase price.
                              • Learn about the pricing types for purchase prices (PP).


                              Benefits

                              • The price development of stock articles can be traced in different ways: You can
                                consider either the last purchase price, or an average purchase price.
                              • In stock management, the average purchase price can be calculated for all sizes of
                                the stock article, or just for the present stock size.


                              Please note:

                              Purchase price              Purchase prices are defined in price master data in the
                                                          same way as sales prices.

                              Average purchase price      The average purchase price is determined as a unit
                                                          price. The calculation function must be enabled in the
                                                          company data first.

                              Average purchase price per Calculation of the average purchase price can be
                              stock size                 disabled per stock size.

                              Default settings            Product management – stock sizes
                                                          • Checkbox Search stock PP
                                                          Company data
                                                          • Tab Stock/ PP / EDI
6.1 / 04-2020




                G-48                                                   A+W Business Inventory Management
                Tutorial                                                                                             Master Data




                                             Purchase Price and Average PP
                                             You can determine the value of a stock article in different ways, either as av-
                                             erage PP or the latest PP. You have already made this decision in Company
                                             data > tab Stock / PP / EDI.
                                             Among others, two codes are essential for pricing; these are set in stock sizes
                                             and stock articles.




                            A


                                         B


                A Stock sizes: PCH search stock                           B Stock management: Include in total PP
                Fig. G-21       PP calculation


                                             •   Stock sizes:
                                                 This code (A) defines whether or not the average cost of this stock size
                                                 shall be determined from stock.
                                             •   Stock management:
                                                 This code (B) defines whether the corresponding stock article is included
                                                 in the calculation of the overall average price for all variants of this article.
                                                 The corresponding prices per stock article and storage place are shown in
                                                 sections Purchase price and Calculation of the average price.
                                             A detailed description of pricing in dialog Stock management can be found in
                                             the Software Reference.

                                             Average purchase price
6.1 / 04-2020




                                             The purchase price is recalculated with every addition to stock or if prices are
                                             changed in the P.O. The system saves this information for every addition to




                A+W Business Inventory Management                                                                           G-49
                Master Data                                                                              Tutorial




                              stock in order to include price amendments in purchase orders which are
                              made after receipt of goods, in the average purchase price.
                              The following formula is used to calculate the average purchase price:
                              Average PP = ((stock on hand * price) + (stock addition * price of goods add-
                              ed)) / (qty. + qty. added)

                                 Example

                                 The stock on hand for a certain article is 100 sqm at 10 €/sqm. (Average PP
                                 = 10 €/sqm). Based on a P.O., 10 sqm at 15 €/sqm are added. The average
                                 purchase price is recalculated:
                                 ((100 sqm * 10 €) + (10 sqm * 15 €)) / (100 sqm + 10 sqm) = 10.45 € pro sqm


                              The PP is updated until the invoices for all purchase orders have been
                              checked, or until the P.O. has been transferred to archives. After that, price
                              changes in the purchase order will not be taken into account for calculating the
                              average price. Purchase orders are no longer listed in the stock management
                              view when they are deleted (after archiving).

                              PP calculation for combined stockkeeping mode
                              If you are using combined stockkeeping, the quantity reserved for the 0 x 0 re-
                              cord will be deleted by the report from production; the corresponding stock-
                              plates will be withdrawn.
                              If there is no report from production, the stock of sqm articles will soon become
                              negative and will falsify the costs.
                              You can therefore define in the company data that combined stock articles for
                              which no sizes have been defined shall be ignored when calculating the aver-
                              age purchase price. In this case, only the average cost of the stock sizes will
                              be calculated.
6.1 / 04-2020




                G-50                                                   A+W Business Inventory Management
                Tutorial                                                                                                                                       Master Data




                                                            The pricing process


                                                                                               Start
                                                                                           price search




                                                                                              Manual
                                                                                                                                      Yes
                                                                                        input of price code?



                                                                                                                                                   Search PP in rate allocation
                                                                                                No                                                   of the defined price key




                                                                                                                                                               End
                                                                                             Existing
                                                                         No                                           Yes
                                                                                            in product
                                                                                           stock sizes?




                                                                                                                                            Yes            Search by
                                                                                                                                                          average price
                                                                                                                                                             active?




                                            Yes          Does this exact product                                                                               No
                                                                 variant
                                                             exist in stock
                                                            management?

                                                                   No

                  Select average PP
                   from stock article               Create weighted average price for
                                                            all stock products
                                                    for which the corresponding code
                                                            has been enabled.
                                                                                                                                              No       Different price code
                                                                                                                                                         for PP defined?




                                                                                                                                                               Yes


                                        Is the calculated                                                      No
                                            price > 0?




                                              Yes                                                                    Search PP in                        Search PP in rate
                                                                                                                standard rate allocation             allocation of the defined
                                                                                                                                                             price key




                                              End                                                                                            End
6.1 / 04-2020




                Fig. G-22          The pricing process




                A+W Business Inventory Management                                                                                                                         G-51
                Master Data                                                                               Tutorial




                              Notes on the pricing process
                              Pricing first searches in product stock sizes whether the article exists in just
                              the defined variant.
                              •   If so, the average price of the stock article will or will not be calculated, de-
                                  pending on the code. If the code is inactive, the system will search for the
                                  price in the standard purchase rate. If a different PP code has been de-
                                  fined, it has priority over the standard rate.
                              •   If the article cannot be found in product stock sizes, the system goes on
                                  searching for the average price on stock.

                              Average price
                              Average price calculation goes through the following levels:
                              •   If the average price is determined from stock, the system first searches for
                                  the exact stock article. If this article exists, the defined price will be used.
                              •   If the article does not exist, the weighted average price for all products of
                                  this article number with an active code will be determined.
                              •   If the determined price is 0, the system will search for the price in the stan-
                                  dard purchase price allocation.
                              •   If the price code has been entered manually at order entry, the price is cal-
                                  culated only from the rate allocated to the selected price key, without
                                  searching for an average price.
                              The codes do not influence the saving of costs for the corresponding stock ar-
                              ticle.
                              Here are some examples for the price search process.

                                  Product stock dimensions

                                  Article     Size          Calculate average      Diff. price key
                                                            price

                                  1004        3210 x 6000   Yes                    Stock sizes
                                  1004        3210 x 3000   No                     <n.e.>
                                  1004        3210 x 2000   No                     Stock sizes


                                  Stock management

                                  Article     Size          Overall average price Stock on Average price
                                                            calculation           hand

                                  1004        3210 x 6000   Yes                    100 pcs    1.25 €/qm
                                  1004        2000 x 2000   Yes                    40 pcs     1.84 €/qm
                                  1004        1500 x 3000   No                     45 pcs     1.99 €/qm


                                  Prices acc. to rate allocation in price management
6.1 / 04-2020




                                  Price Key                 Price




                G-52                                                    A+W Business Inventory Management
                Tutorial                                                                                  Master Data




                                        Prices acc. to rate allocation in price management

                                        Default                 1.50 €/qm
                                        Stock sizes             1.00 €/qm


                                        Order with calculated purchase prices

                                        Itm.        Article      Size              Price key definition   PP

                                        1           1004         3210 x 6000       No                     1.25 €/qm
                                        2           1004         2000 x 2000       No                     1.44 €/qm
                                        3           1004         3210 x 3000       No                     1.50 €/qm
                                        4           1004         3210 x 2000       No                     1.00 €/qm
                                        5           1004         1250 x 1433       No                     1.30 €/qm
                                        6           1004         3210 x 6000       yes (stock sizes)      1.00 €/qm
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-53
                Master Data                                                                                        Tutorial




                                           Check Settings for Purchase Price Calculation
                                           You have already set the stock control mode in the company data. Now enable
                                           the purchase price calculation and select the calculation type.


                                            How to check the settings for the purchase price
                                           1 Select menu Master Data > Company > Company Data.
                                           2 Go to the Stock / PCH / EDI tab.




                A
                B
                C




                A Enable purchase price calculation                  C Additional function for the combined stock control
                B Purchase price calculation type                      mode

                Fig. G-23     Company data - Stock / PCH / EDI
6.1 / 04-2020




                G-54                                                             A+W Business Inventory Management
                Tutorial                                                                                 Master Data




                                     3 Check the checkbox Calculate purchase price (A) to enable the options:
                                         •   Average PP:
                                             The average purchase price will be recalculated whenever goods are
                                             added to stock.
                                         •   Last PP:
                                             The last purchase price booked on stock when goods were received or
                                             an invoice was checked, will be used for stock evaluation.
                                         •   Ignore combined articles without sizes:
                                             Check this checkbox if combined stock articles without sizes shall not
                                             be considered for average purchase price calculation.
                                     4 Go to Menu Start > Save to save the data.
                                         The data is saved.


                                     Check Prices
                                     This section tells you how to define purchase prices.
                                     The following conditions must be fulfilled to calculate the average purchase
                                     price:
                                     •   The product has to be defined as a stock article.
                                     •   The PP code must be set in company data.
                                     As a general rule, just one price key is entered for the PP but you can use sev-
                                     eral PP price keys if required. Next, all price keys for the PP have to be defined
                                     as a combined rate. If there are several price keys for the PP, a default price
                                     list should be defined. You can enter a price if required. This will not be
                                     changed when the average price is calculated. The average PP appears in
                                     special fields in stock management.
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-55
                Master Data                                                                                    Tutorial




                                         How to check the master data of your price lists
                                        1 Go to menu Master data > Prices and check the settings in the dialogs
                                          Year, Key, and Rate.
                                            You only need to check the entries used for the prices (and other internal
                                            calculations) for stock sizes and boxes.
                                        2 Select menu Master Data > Prices > Prices.




                  Fig. G-24   PP price tables


                                        3 Please check if all purchase and sales prices have been defined and are
                                          up to date, and complete or correct them as necessary.
                                        4 Go to the tab in which the price is defined, check if the purchase price has
                                          been entered correctly, and correct it if necessary.




                  Fig. G-25   Defined purchase prices


                                        5 Go to Menu Start > Save to save the data.
                                            The data is saved.
6.1 / 04-2020




                G-56                                                           A+W Business Inventory Management
                Tutorial                                                                                  Master Data




                                     Exercises
                                     •   Check whether the correct price lists have been allocated to the stock siz-
                                         es.
                                     •   Create a new price list with an individual purchase price for a stock article.


                                     Additional information
                                      Software Reference, “Reserved Stock Products” on page G-215
                                      Software Reference, “Purchase prices” on page G-190
                                      Master Data, “Status Allocation” on page B-426
                                      Master Data, “Input of Unit Prices” on page B-236
                                      Master Data, “Prices” on page B-713
                                      Master Data, “Rates” on page B-662
                                      Master Data, “Calculate purchase price” on page B-955
                                      Master Data, “Stock control mode” on page B-958
6.1 / 04-2020




                A+W Business Inventory Management                                                                G-57
                Master Data                                                                                     Tutorial




                              Stock control on BOM level
                              Objectives

                              • Getting familiar with the relation of the procurement type on the main product levels
                                and the BOM components.
                              • Checking the settings in the company data.


                              Benefits

                              • BOM components required for production can be kept as stock articles.


                              Please note:

                              Level: main article          If the main article is already defined as a stock article, all
                                                           BOM components are automatically defined as stock
                                                           articles.

                              Level: BOM                   Each BOM component can be defined as a stock article
                                                           even if the main product's procurement type is
                                                           Production.

                              Default settings             Master data:
                                                           • Product management
                                                           • Supplier file
                                                           Company data:
                                                           • Parameters tab
                                                           • Tab Stock/ PP / EDI
6.1 / 04-2020




                G-58                                                      A+W Business Inventory Management
                Tutorial                                                                                   Master Data




                                         Reservation and booking of BOM components
                                         Stock articles can be both main products or BOM components. For a complete
                                         door which is sold including the fittings, you can define the glass as an in-
                                         house product and the fittings as stock articles.
                                         If the main article is already defined as a stock article, all BOM components
                                         are automatically defined as stock articles.




                                                                                                            A




                                                                                                                         B




                A Procurement type main product                      B Procurement type BOM component
                Fig. G-26   Setting the procurement type for a main product with BOM


                                         When you enter such a BOM article in the order, every component defined as
                                         a stock article will be displayed in the stock search.
6.1 / 04-2020




                                         If you check this main product on the Stock info dialog, all BOM components
                                         will be shown as well.



                A+W Business Inventory Management                                                                G-59
                Master Data                                                                                        Tutorial




                A




                                         B




                A Order item                                         B Stock info - BOM components
                Fig. G-27     Order entry and stock info


                                             All BOM components will be reserved after you have saved the order.
6.1 / 04-2020




                G-60                                                             A+W Business Inventory Management
                Tutorial                                                                                    Master Data




                                     Fig. G-28   Reserved BOM components


                                     If the BOM shows 2 pcs. of a primary component, the quantity of the second-
                                     ary components (children) to be booked on stock is multiplied by 2.


                                     Checking the setting
                                     Option Stock control on BOM level must be enabled in the company data.




                                     Fig. G-29   Company data – Stock / PP / EDI: Settings for the stock control of bills
                                                 of material
6.1 / 04-2020




                A+W Business Inventory Management                                                                  G-61
                Master Data                                                                                      Tutorial




                                         Checking Products
                                         This module shows you how to check the procurement type of the BOM com-
                                         ponents in product management.


                                          How to set up your bills of material for stockkeeping
                                         1 Select menu Master Data > Products > Articles > Articles.
                                            Dialog Product Management opens.
                                         2 Search the product you want to keep on stock by means of bills of material.
                                         3 Go to tab BOM.




                                                                                                                 A

                                                                                                                 B




                A Procurement type of the component          B Calculate purchase price
                Fig. G-30     Product management – BOM components


                                         4 Tag the corresponding BOM component and select the procurement type
                                           if this shall differ from the procurement type defined in this component's
                                           master data.
                                            If the procurement type for the main product is set to Stock withdrawal, this
                                            applies to all BOM components.
                                            If the procurement type for the main product has been set to Production,
6.1 / 04-2020




                                            the BOM components can be kept as stock products at the same time.
                                            When you enter such a main product in your order, all BOM components
                                            will be set to reserved in the stock info.


                G-62                                                            A+W Business Inventory Management
                Tutorial                                                             Master Data




                                     5 Go to Menu Start > Save to save the data.
                                        The data is saved.
                                     6 Repeat the steps for all eligible products.
6.1 / 04-2020




                A+W Business Inventory Management                                         G-63
                Stock Management                                                                           Tutorial




                                   Stock Management
                                   In this thematic block you will learn how to enter and maintain stock articles.
                                   This includes the following training modules:
                                   •   “Stock Management” on page G-65
                                   •   “Stock Booking” on page G-75
                                   •   “Queries” on page G-85
                                   •   “Stock information” on page G-94
                                   •   “Stock P.O. (automatic)” on page G-103
6.1 / 04-2020




                G-64                                                      A+W Business Inventory Management
                Tutorial                                                                             Stock Management




                                     Stock Management
                                     Objectives

                                     • Getting familiar with the Stock Management dialog
                                     • Create stock article


                                     Benefits

                                     • Stock articles serve to define and maintain the stock on hand.
                                     • Stock on hand of stock articles is updated with the booking of goods withdrawals
                                       and additions.
                                     • Based on the stock articles, you can determine the current stock on hand including
                                       reservations and purchase orders.


                                     Please note:

                                     Calculate the stock on hand Quantities and surfaces can be calculated correctly only
                                                                 if the stock articles have been properly created.

                                     Stock articles              Only stock articles can be managed in the stock.
                                                                 Products defined in the master data will not be
                                                                 automatically kept as stock on hand.

                                     Receipt of goods, issue     Receipt and issue of goods can only be booked for stock
                                                                 articles.

                                     Default settings            Master data:
                                                                 • Storage locations
                                                                 • Products
                                                                 • Stock sizes
6.1 / 04-2020




                A+W Business Inventory Management                                                                   G-65
                Stock Management                                                                                          Tutorial




                                             Elements in Stock management Dialog
                                             Each stock article can be created in different variants, e. g. Float 5 mm in sev-
                                             eral sizes.


                                                J                    I




                A

                                                                                                                              H
                B

                C


                D

                E
                                                                                                                              G




                                                         F
                A   Product number                                       F   Inventory audit for the stock preview
                B   Stock article sizes                                  G   Defined stock articles
                C   Standard storage location                            H   Main product
                D   Stock category                                       I   Number of sheets in boxes
                E   Main stock article code                              J   Storage place (4 levels)
                Fig. G-31     Stock article definition


                                             If the stock on hand is not checked for each storage location (F), a main prod-
                                             uct (E, H) must be allocated to determine the available square meters of the
                                             glass.
                                             The stock on hand can be kept per storage location (J). The defined storage
                                             locations are allocated to the stock articles for this purpose. If a stock article is
                                             kept in different storage location, you must define a standard storage loca-
                                             tion(C).
                                             Additions and withdrawals will be automatically booked at the standard stor-
                                             age place place but can be changed manually.
6.1 / 04-2020




                G-66                                                                   A+W Business Inventory Management
                Tutorial                                                                             Stock Management




                                     Stock Articles
                                     Products defined in master data will not be kept on stock automatically. This
                                     makes sure that stockkeeping includes only articles that are actually kept on
                                     stock. Other articles which are stored only temporarily for the production of a
                                     special order, do not have to be kept as stock articles.
                                     Every (glass) product is related to a stock size and a stock article. The rela-
                                     tions have already been explained in the training module on Products.


                                     Main Stock Products
                                     You can link several stock sizes in stock management by defining a main stock
                                     product. The inventory check (for the stock preview in dialog Stock info) is ex-
                                     ecuted only for the main stock product in this case; a minimum stock has to be
                                     defined only for this article.

                                        Example

                                        Article 1004 has been entered with the following sizes:
                                        0 x 0, 500 x 600, 1200 x 1800, 3210 x 4000 and 3210 x 5000.
                                        For the sizes 3210 x 4000 and 3210 x 5000, article 0 x 0 has been defined as
                                        the main stock product. The minimum stock for this article has been specified
                                        as 19,000.00 sqm.
                                        The stock on hand of the sizes 3210 x 4000 and 3210 x 5000 are summed up
                                        and compared with the minimum stock of 19,000.00 sqm.
                                        Separate minimum stock has been defined for sizes 500 x 600 and
                                        1200 x 1800 which will be used for checking.


                                     If you have defined the stock articles each with a minimum stock, you can still
                                     allocate them to a main product later. Determination of the minimum stock only
                                     checks the settings for the main product; the minimum stock defined for the
                                     stock articles will be ignored.
6.1 / 04-2020




                A+W Business Inventory Management                                                                   G-67
                Stock Management                                                                             Tutorial




                                   Minimum Stock
                                   If the stock on hand for an article falls below a certain minimum quantity (taking
                                   into account the orders and purchase orders), replacement must be ordered
                                   in good time so as not to impede the production. A+W Business allows you to
                                   enter a threshold for the minimum stock. This is defined by article.
                                   The minimum stock is a parameter the stock should not fall short of, neither in
                                   reality nor in connection with reservations made.
                                   Based on the defined minimum stock, the inventory will automatically issue
                                   purchasing suggestions. These have to be released manually. Automatic pur-
                                   chase suggestions use the following key figures as a basis for calculating the
                                   quantities to be ordered:
                                   •   Ordered quantity
                                   •   Reservation
                                   •   Minimum stock
                                   •   Standard purchase quantity
                                   •   Current stock on hand
                                   To define the article precisely, width and height are evaluated, among other
                                   things.
                                   Calculation of the purchase quantity will be introduced in a separate module.
                                    “P.O. Quantity after Stocktaking” on page G-130
6.1 / 04-2020




                G-68                                                       A+W Business Inventory Management
                Tutorial                                                                                      Stock Management




                                             Prices
                                             The prices of a stock article are shown as average purchase prices (purchase
                                             prices) if this function is enabled in the company data.
                                             The display of the average prices is updated for the respective stock article
                                             during archiving or auditing (invoice check).
                                             A+W Business assumes that the prices will not be changed after this process.
                                             However, if you still change prices after one of the processes, these changes
                                             are not included in the calculation of the average price.


                                                           E




                A


                B




                C
                D

                A Display mode (e. g. for lite with different stock   D Average price per article or for all sizes if C has been
                  sizes)                                                enabled
                B Average prices in purchasing                        E Stock values of the tagged article
                C Include in total PP
                Fig. G-32     Average prices for stock articles


                                             You can specify whether all sizes of an article shall be included in the average
                                             price calculation. Only if you have checked the check-box Include in total PP
                                             (C), the prices of the current article will be included in the calculation.
                                             The selected mode (A) determines the price view:
                                             •   Only this article:
                                                 For the calculation only the displayed article in the selected size is taken
                                                 into account. The PP history of the current article is displayed.
6.1 / 04-2020




                                             •   All sizes:
                                                 For the calculation all dimensions of the displayed glass are taken into ac-
                                                 count. The PP history of all dimensions of the article is displayed.


                A+W Business Inventory Management                                                                             G-69
                Stock Management                                                                            Tutorial




                                   The average PP is calculated for every record, except for goods issued.
                                   Goods issued only reduce the stock. The displayed list of recalculations (B) is
                                   reduced by archiving and the invoice check. As a result, the view remains
                                   clearer.
                                   The first data record shows the opening stock and the original price. Under-
                                   neath you will find the goods received and issued (minus sign). If goods have
                                   been received as a result of a stock P.O., the P.O. number and the P.O. item
                                   are furthermore displayed.
                                   The average PP is updated during entering or changing purchase orders. It is
                                   determined by taking the total quantity into account.

                                      Example:

                                       100 pieces        on stock           each 15.00 €                 1500.00 €

                                        40 pieces        new booking        each 18.00 €       +           720.00 €

                                                                                                =        2200.00 €
                                                                                                         ========
                                       2200.00/140 pcs. = 15.86 €



                                   Automatic surcharges that are listed in the purchase orders, e. g. energy and
                                   transportation surcharge, are also included in the calculation.

                                   Distribution of surcharges
                                   Costs incurred by a stock P.O. will be added to the purchase prices of all arti-
                                   cles of the P.O. These costs can be freight, energy surcharge, or any other
                                   costs related to the provision of stock articles.
                                   This redistribution depends on the price unit of the surcharge. If the price unit
                                   is kg, the surcharge is redistributed based on the item weight. For all other
                                   price units, redistribution is based on the item price.
                                   Since every change of item will influence the redistribution to all other items,
                                   redistribution for the entire document will always be made after an item has
                                   been changed, i.e. when all items have been entered.
                                   Changes of items will update the PP only until the invoice is checked.
                                   Footer surcharges have been introduced in the training session on Purchas-
                                   ing.
6.1 / 04-2020




                G-70                                                       A+W Business Inventory Management
                Tutorial                                                                           Stock Management




                                     Create a Stock Article
                                     This module shows you how to create the required stock articles. You have to
                                     define at least the following settings in order to manage the stock:
                                     •   Article number and name
                                     •   Dimensions for stock dimensions
                                     •   Storage location and standard storage location (default storage location)
                                     •   Stock on hand

                                         Inventory start-up
                                         If no stock articles have been entered at all, you can facilitate this task by
                                         running the so-called initial inventory. This process will be introduced in a
                                         separate training session.


                                      How to create a stock article
                                     1 Go to menu Stock management > stock management.
                                         The Stock management dialog opens.
                                     2 Go to the menu Start > New to switch to the input mode.
                                         If you open the Stock management dialog from the master data, this step
                                         can be omitted. The fields for articles and sizes are filled in already.
6.1 / 04-2020




                A+W Business Inventory Management                                                                G-71
                Stock Management                                                                                        Tutorial




                A


                B

                C




                D




                E




                                                   F
                A Stock article number                                   D Main product
                B Dimensions                                             E Stock on hand
                C Storage location                                       F Inventory audit
                Fig. G-33    Fields for new stock articles are enabled


                                           3 Enter the number (A) and size (B), if applicable.
                                           4 Choose a storage location (C).
                                               If no storage location is selected, the storage location <n.e.> will be en-
                                               tered. In stock management, this will be treated like the defined storage lo-
                                               cations, e. g. for stocktaking purposes and queries.
                                               If a stock article is kept in different storage locations, you have to define one
                                               of them as the standard storage location.
                                           5 Check checkbox Default storage location.
                                           6 Go to field Main product (D) and select the article for which you want to en-
                                             ter the minimum stock for the inventory audit.
                                               To define a separate minimum stock for the new stock article, select the
                                               size of the new article. However, the new size will be displayed only after
                                               you have saved the new article. We recommend to select any size then
                                               change it after you have saved the article.
                                           7 Check the checkbox Inventory audit per stock location (F) if all storage lo-
6.1 / 04-2020




                                             cations shall be evaluated separately when checking the inventory for this
                                             stock article.



                G-72                                                                   A+W Business Inventory Management
                Tutorial                                                                       Stock Management




                                     8 Enter the quantities in section Stock on hand (E) if required.
                                        Please make sure to enter an appropriately high minimum stock if you have
                                        defined the same main product for several sizes.
                                        The checkboxes are enabled only in selection mode. They serve to filter
                                        the search by stock article.
                                        These are the minimum entries for stock articles.
                                     9 Select in the menu Start > Save to save the data.
                                        The data is saved. At the same time, a dummy stock article without dimen-
                                        sions is created for the combined stock control mode.
                                        Thus all necessary information A+W Business needs for reservations and
                                        booking have been defined. Bookings for the new stock article can be
                                        made now.
6.1 / 04-2020




                A+W Business Inventory Management                                                          G-73
                Stock Management                                                                             Tutorial




                                   Exercises
                                   Enter the following stock articles and allocate the appropriate price list:
                                   •   Stock article kept on stock in units.
                                   •   Stock article Handle which is kept on stock in its individual quantity unit.


                                   Additional information
                                    Software Reference, “Management” on page G-176
                                    Purchasing, “Document P.O.” on page D-43
6.1 / 04-2020




                G-74                                                       A+W Business Inventory Management
                Tutorial                                                                              Stock Management




                                     Stock Booking
                                     Objectives

                                     • Introducing the booking types for stock articles.
                                     • Introducing automatic stock bookings.
                                     • Manual trigger of stock bookings.


                                     Benefits

                                     • When stock articles are ordered, receipt of goods is automatically booked on
                                       stock, as is the issue of goods for order items.
                                     • You can correct the stock on hand for individual storage places by transferring
                                       stock articles.


                                     Please note:

                                     Automatic booking            • Automatic bookings of additions will be triggered if the
                                                                    status of the P.O. is changed upon receipt of goods.
                                                                  • Automatic dispatch bookings will be released if the
                                                                    status of an order is changed by printing.

                                     Booking types                The booking types for stock bookings are fixed in the
                                                                  system.

                                     Manual bookings              The following bookings can be triggered manually:
                                                                  • Addition and dispatch of goods
                                                                  • Change storage location

                                     Default settings             Master data:
                                                                  • Status allocations
                                                                  Company data:
                                                                  • Tab Stock/ PP / EDI
6.1 / 04-2020




                A+W Business Inventory Management                                                                     G-75
                Stock Management                                                                          Tutorial




                                   Stock Movements
                                   Stock management keeps, maintains, and checks the stock on hand. In addi-
                                   tion to that there is the dialog Stock management for manual receipt and issue
                                   of goods, and for rebooking storage locations.




                                   Fig. G-34    Stock management for manual stock bookings


                                   All stock movements are recorded to allow you to trace all transactions.
                                   Stock movements are automatically booked via orders, purchase orders, and
                                   receipt of goods.

                                   Scanning
                                   In connection with AWPort, stock bookings can also be entered via barcode.
                                   This does not only include receipt and withdrawal of goods but also realloca-
                                   tions.
                                   For more information on barcodes and barcode formats, please refer to the
                                   documentation on AWPort.


                                   Booking Types
                                   The booking types for stock booking are fixed in the system and cannot be ed-
                                   ited. Whenever a stock article is booked, the corresponding booking type is al-
                                   located. These booking types can be used to create analyses which give
                                   details on the stock on hand or the type of stock movement, e. g. ordered and
                                   reserved quantities.
6.1 / 04-2020




                                   The following booking types are available:




                G-76                                                     A+W Business Inventory Management
                Tutorial                                                                          Stock Management




                                     •   Reserved:
                                         An order reserves an article until the delivery note or invoice is printed.
                                     •   Shipped:
                                         An article is marked as shipped when the delivery note or the invoice has
                                         been printed.
                                     •   Cut LM:
                                         This booking type is used by the A+W Optimizer report if an item has been
                                         cut from a stock size. The number of stock plates is analyzed.
                                     •   Ordered:
                                         This code is set by a stock P.O.
                                     •   Received:
                                         An article is considered shipped and received when its receipt has been
                                         booked.
                                     •   Manual stock addition, manual stock dispatch:
                                         Manually booked stock additions or withdrawals are marked by special
                                         booking types.
                                     •   Stock transfer:
                                         Stock transfers are triggered manually.
                                     •   New entry:
                                         Data for new stock articles may have been entered via stocktaking, or man-
                                         ually. All new articles as of the last archiving process are included.
                                     •   Correction:
                                         The stock on hand can be corrected in the course of inventory taking. All
                                         corrections as of the last archiving process are included.
                                     •   Deleted from stock:
                                         Internal booking type


                                     Withdrawals and Additions
                                     Stock articles are withdrawn when the defined status has been reached, i.e.
                                     when the delivery note or invoice is printed. Up to that point, the stock articles
                                     are just reserved.
                                     The stock control mode selected in the company data defines whether or not
                                     the stock on hand will be updated based on a reservation.
                                     Receipt of goods in the purchasing module automatically adds the stock arti-
                                     cles from stock POs.
                                     When goods are received for stock POs, you can even enter goods which
                                     have not been defined as stock articles. These quantities will not be added to
                                     stock however. No stock bookings will be made for these products.

                                         Stock bookings for boxes
                                         Boxes are generally booked via ID numbers (ID). There is a detailed de-
                                         scription in the Box management section.
6.1 / 04-2020




                A+W Business Inventory Management                                                                G-77
                Stock Management                                                                            Tutorial




                                   Manual Input of Additions or Dispatches
                                   This module shows you how to book stock additions or dispatches manually.
                                   The following instructions exist for this training module:
                                   •   “How to book the receipt of goods manually” on page G-78
                                   •   “How to book the dispatch of goods manually” on page G-81


                                    How to book the receipt of goods manually
                                   1 Go to menu Stock management > Stock movements.
                                       Dialog Stock movement opens.
                                   2 Go to tab Addition.




                                       Fig. G-35    Search for stock articles


                                   3 Enter the product number in the Product field and select Start > Search in
                                     the menu.
                                       Section Storage locations lists all stock articles matching the search crite-
                                       rion.
6.1 / 04-2020




                G-78                                                            A+W Business Inventory Management
                Tutorial                                                                           Stock Management




                                                                                                                B




                                      A




                                     A Select article                           B Added quantity
                                     Fig. G-36     Stock movement – Addition


                                     4 Mark the appropriate stock article (A).
                                          The fields in section Change stock on hand will be filled with the updated
                                          values.
                                     5 Enter the quantity added (B) and/or the new evaluation price.
                                     6 Change the booking date if required.
                                     7 Go to Menu Start > Save to save the data.
                                          Data will be saved, and the stock on hand updated.
                                          If the option Report on closing is enabled, the dialog Stock history opens
                                          when you close the Stock movement dialog.
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-79
                Stock Management                                                                            Tutorial




                Fig. G-37   Stock history


                                             All stock movements can then be printed in a log.




                                                                                                 A



                                                                                                 B




                A Legend                          B Booking details of manual addition booking
                Fig. G-38   Stock addition booking log
6.1 / 04-2020




                G-80                                                             A+W Business Inventory Management
                Tutorial                                                                         Stock Management




                                      How to book the dispatch of goods manually
                                     1 Go to menu Stock management > Stock movement > tab Dispatch
                                     2 Enter the product number in the Product field and select Start > Search in
                                       the menu.
                                        Section Storage locations lists all stock articles matching the search crite-
                                        rion.
                                     3 Mark the appropriate stock article.
                                        The fields in section Change stock on hand will be filled with the updated
                                        values.




                                        Fig. G-39    Manual stock dispatch


                                     4 Enter the quantity to be booked from the stock on hand.
                                     5 Change the booking date if required.
                                     6 Go to Menu Start > Save to save the data.
                                        Data will be saved, and the stock on hand updated.
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-81
                Stock Management                                                                          Tutorial




                                   Change Storage Location
                                   This module will show you how to move a stock article from one storage loca-
                                   tion to another, e. g. from the warehouse to the production area. This move-
                                   ment is registered by means of a transfer booking. The stock articles are
                                   booked as a dispatch from their old storage location, and an addition to the
                                   new one.

                                      Change storage location for part of the stock on hand
                                      Changing the storage location in the Transfer tab always transfers the en-
                                      tire stock from one storage location to another.
                                      To transfer just part of the stored quantity, you have to withdraw just this
                                      quantity from the old storage location and add it to the new storage loca-
                                      tion.


                                    How to transfer the storage location
                                   1 Go to menu Stock management > Stock movements.
                                      Dialog Stock movement opens.
                                   2 Go to tab Transfer.
                                   3 Enter the product number or the ID in the Product field.
                                   4 To start the search, go to the menu Start > Search.
6.1 / 04-2020




                G-82                                                     A+W Business Inventory Management
                Tutorial                                                                          Stock Management




                                                                              A                      B




                                        A Current storage location                B Select new storage location
                                        Fig. G-40    Stock movement – Transfer


                                        Section Storage locations (A) lists all stock articles matching the search cri-
                                        terion.
                                     5 Mark the appropriate stock article.
                                     6 Choose the new storage location in section storage location (B).
                                     7 Go to Menu Start > Save to save the data.
                                        The data is saved. The stock article is withdrawn from the old storage loca-
                                        tion, and added to the new one.
6.1 / 04-2020




                A+W Business Inventory Management                                                                 G-83
                Stock Management                                                                         Tutorial




                                   Exercises
                                   •   Transfer a storage location. Please make sure that all stock articles are
                                       transferred.
                                   •   Book the addition on stock manually. If there is no open stock P.O. make
                                       up for this exercise in module Stock P.O.


                                   Additional information
                                    “Stock Definition” on page G-19
                                    Software Reference, “Booking type” on page G-203
                                    Purchasing, “Dealing with boxes” on page D-134
                                    Purchasing, “Enter the receipt of boxes” on page D-136
6.1 / 04-2020




                G-84                                                      A+W Business Inventory Management
                Tutorial                                                                             Stock Management




                                     Queries
                                     Objectives

                                     • Check stock on hand.
                                     • Monitor stock movements.
                                     • Check stock development.


                                     Benefits

                                     • These queries will give you a quick overview of the stock on hand (beyond
                                       inventory taking).
                                     • You can identify slow and fast sellers and adapt stock management accordingly.


                                     Please note:

                                     Booking journal            The booking journal shows all automatic bookings
                                                                resulting from documents.

                                     Stock history              Stock history analyzes all stock booking types.

                                     Stock statistics           Stock statistics help to consider different key figures by
                                                                defined periods.

                                     Default settings           None
6.1 / 04-2020




                A+W Business Inventory Management                                                                    G-85
                Stock Management                                                                           Tutorial




                                   Stock Query
                                   Various queries serve to give you an overview of the bookings, the total value
                                   of the stock on hand, statistics, and a list of reservations.
                                   You can also see who has changed which data.

                                   Booking journal
                                   The booking journal offers analyses on stock bookings created from orders
                                   and purchase orders. You can e.g. view stock bookings by product.

                                   Stock history
                                   Stock history gives a quick overview of the daily events on stock, by product.

                                   Stock statistics
                                   Stock statistics inform you which ones of your stock articles are hits and which
                                   ones are slow sellers. This provides you with a criterion to decide whether ar-
                                   ticles should be added or withdrawn from stock.
                                   The development of individual stock articles can be analyzed for a defined pe-
                                   riod, e. g. for an entire year or just for one month.
                                   The analyses show initial and end stocks and additions and dispatches of your
                                   stock articles per month. This will provide you with information about the stock
                                   turnover, average storage duration and average stock on hand of your stock
                                   articles.

                                   Inventory evaluation
                                   The current value of the entire stock can be checked at all times, apart from
                                   during the inventory taking.
                                   In addition to that, stock management shows the highest, lowest, and average
                                   purchase price as well as the corresponding stock value for every single stock
                                   article.

                                   Reserved stock articles
                                   Stock articles reserved by orders can be listed by number manager. The re-
                                   served stock articles are shown by article number and storage location.
6.1 / 04-2020




                G-86                                                      A+W Business Inventory Management
                Tutorial                                                                           Stock Management




                                     Show Booking Journal
                                     This module will show you how the individual criteria can be used in the book-
                                     ing journal and/or stock history. These two dialogs are structured in the same
                                     way but show different facts:
                                     •   The booking journal shows all automatic bookings. Orders can be edited
                                         only until they have been archived and deleted.
                                     •   Stock history shows all manual and automatic bookings, new entries, real-
                                         locations, and corrections from inventory taking.
                                     These instructions describe the two dialogs, using the Booking journal as an
                                     example.


                                      How to display reservations
                                     1 Go to menu Stock management > Queries > Booking journal.

                                                       A       B                           C            D




                                     A Booking type                          C Article
                                     B Query time period                     D Article selection
                                     Fig. G-41    Booking journal


                                         The bookings displayed can be restricted by means of various filters, e. g.
                                         to just one article.
6.1 / 04-2020




                A+W Business Inventory Management                                                             G-87
                Stock Management                                                                             Tutorial




                                   2 Select the entry Reserved in the field Booking type (A).
                                      If there is no entry in this field, all bookings will be shown.
                                   3 Restrict the view further if required, e.g. to an article (C, D) or period (B).
                                   4 To generate the booking journal go to the menu Start > Execute.




                                   Fig. G-42    Booking journal – Result


                                      The list shows all reservations. If you have not restricted the view any fur-
                                      ther, all orders and purchase orders will be shown that have not been ar-
                                      chived yet.
                                      You can analyze every single booking type in the same way.
6.1 / 04-2020




                G-88                                                        A+W Business Inventory Management
                Tutorial                                                                           Stock Management




                                     Print reserved Stock Articles
                                     Reservations are shown in the dialogs Booking journal, Stock history, and
                                     Stock info. Dialog Reserved stock articles gives a quick overview of the reser-
                                     vations based on orders in a number manager. This module shows you how
                                     to print a list of these reserved stock articles.


                                      How to print a list of reserved stock articles
                                     1 Go to menu Stock management > Queries > Reserved stock articles.
                                        Dialog Reservations opens.
                                     2 Select the Number Manager in which the current orders are collected.




                                        Fig. G-43     Reserved stock articles


                                        The orders are listed in section Table. You can print the list from the display.
                                        You can print the list directly via menu Print > Printer.
                                     3 Go to menu Print > Screen to display the list.
6.1 / 04-2020




                                     4 Select breaks for the printer.



                A+W Business Inventory Management                                                                 G-89
                Stock Management                                                                          Tutorial




                                   5 Click on [OK] to adopt the settings.
                                      The dialog Print - Stock protocol opens.
                                      If you choose display on screen, the monitor will show the list of reserved
                                      stock articles.




                                      Fig. G-44    Reserved stock articles - output on the screen


                                      The reserved stock articles are listed per article number and storage loca-
                                      tion. If there are several storage locations the total amount is displayed.
                                      The buttons can be used to scroll forwards and backwards if the list has
                                      more than one page.
6.1 / 04-2020




                G-90                                                       A+W Business Inventory Management
                Tutorial                                                                                  Stock Management




                                          Show Inventory Statistics
                                          This module will show you how to display various stock key figures for a prod-
                                          uct in inventory statistics.


                                           How to display the inventory statistics
                                          1 Go to menu Stock management > Queries > Inventory statistics.
                                              Dialog Statistics opens.
                                              You can restrict the view to a product and/or a period. If no selection is
                                              made, all products will be shown.




                   Fig. G-45   Inventory statistics - Product selection


                                          2 Go to the menu Start > Execute to create the analysis.
                                              The products are listed according to the filter settings.
6.1 / 04-2020




                A+W Business Inventory Management                                                                    G-91
                Stock Management                                                                                Tutorial




                                         3 Select an entry and go to tab Statistics to analyze the details.




                  Fig. G-46   Stock statistics – Statistics


                                             The values for the selected product are shown, e. g. the stock on hand plus
                                             the additions and withdrawals per month, stock turnover, and average stor-
                                             age time. The totals line shows the accumulated values for the period dis-
                                             played.
6.1 / 04-2020




                G-92                                                            A+W Business Inventory Management
                Tutorial                                                                       Stock Management




                                     Exercises
                                     •   Check the reservations for Float 4 mm in the booking journal.
                                     •   Print the reservations for Float 5 mm for the next month.


                                     Additional information
                                      Software Reference, “Booking Journal” on page G-202
                                      Software Reference, “Stock History” on page G-204
                                      Software Reference, “Stock Statistics” on page G-209
                                      Software Reference, “Reserved Stock Products” on page G-215
6.1 / 04-2020




                A+W Business Inventory Management                                                         G-93
                Stock Management                                                                                 Tutorial




                                   Stock information
                                   Objectives

                                   • Learning about the Stock search dialog.
                                   • Recognizing changes on stock and in reservations


                                   Benefits

                                   • The overview of the future stock on hand and reservations is another means of
                                     stock management.
                                   • You can see when further purchase orders have to be entered so that production is
                                     not interrupted.


                                   Please note:

                                   Stock on hand              The stock on hand is updated upon receipt of stock
                                                              articles, and after withdrawal bookings.
                                                              Printing of the delivery note or the invoice for an order
                                                              triggers the withdrawal booking.

                                   Default settings           Master data
                                                              • Supplier file:
                                                                Delivery time in days (replacement time)
                                                              • Status allocation
                                                              Company data
                                                              • Tab Stock / PP / EDI > Stock preview
                                                              Stock management
                                                              • Tab Stock article > Main article
6.1 / 04-2020




                G-94                                                        A+W Business Inventory Management
                Tutorial                                                                                    Stock Management




                                             Stock Search
                                             Use dialog Stock search to display all stock articles per storage location and
                                             size. You can also open this dialog at item entry. The stock search is already
                                             restricted to one stock article in this case.




                A




                       B                         C                           D
                A Filter for setting the search       C Is kept as a stock size but there D P.O. items that are not kept on stock,
                B Is kept as a stock article and is     is no article on stock, e.g. Stock  e. g. stock sizes of procurement type
                  booked accordingly                    sizes on a sqm stock.               P.O.

                Fig. G-47     Stock info – stock search


                                             Stock on Hand
                                             Calculation of the stock on hand depends on the mode in which the stock is
                                             kept. You have been introduced to these relations right at the start of the train-
                                             ing session.
                                              “How should stock be managed” on page G-15
                                             Calculation of sqm articles takes into account both the reservation and the
                                             waste. If you have allocated one or more articles to a main article, the stock
                                             on hand is no longer displayed for the individual articles.
                                             At order entry, the quantity or the number of square meters (sqm) of the stock
6.1 / 04-2020




                                             articles is automatically reserved for the customer order. Goods withdrawn
                                             from stock are automatically booked upon printing of the delivery note or in-
                                             voice.


                A+W Business Inventory Management                                                                           G-95
                Stock Management                                                                                           Tutorial




                                           Stock Information and Future Stock on Hand
                                           A detailed view in dialog Stock info shows delivery date, quantity, reservations,
                                           etc. The available stock sizes of a size are displayed by storage location.




                A




                B




                C




                A Selected stock article                                  C Stock articles linked with the main article.
                B Preview
                Fig. G-48    Stock info – future stock on hand


                                           Three lists show the future stock on hand:
                                           •   The first list (A) shows the selected stock article. If this is a main stock prod-
                                               uct, the third list shows the linked stock articles.
                                           •   The second list (B) is a preview of the next days. The number of days can
                                               be defined in the company master data.
                                           •   The third list (C) shows the stock sizes linked with the main stock article.
                                               Here, the critical stock can also be displayed.
                                           Problems with entered orders are shown by means of color highlights:
                                           •   Red: Dates cannot be kept.
                                           •   Yellow: Replacement time is sufficient.
6.1 / 04-2020




                G-96                                                                 A+W Business Inventory Management
                Tutorial                                                                                  Stock Management




                       A    B            C




                      I                              H             G           F         E                   D
                A   Selected stock article                             F Open purchase orders for the corresponding date
                B   Period displayed                                     (delivery date)
                C   Storage location                                   G Reservation for date
                D   Minimum stock according to stock management        H Stock on hand on date
                E   Calculated final stock = H - G + F                 I Size of stock article

                Fig. G-49    Display of the future stock on hand


                                           Open P.O. quantities (F) for a stock article are displayed until receipt of goods
                                           is booked. The current stock on hand is updated after that.

                                           Replacement time
                                           The replacement time results from the delivery time that has been defined in
                                           the supplier file for the article and the supplier's route days that are defined in
                                           route management.
                                           When you enter an order item you can retrieve the future stock on hand. Two
                                           things can happen if the stock (D) fails to reach the defined minimum:
                                           •   The replacement time for the article is sufficient to order the goods until that
                                               date. The corresponding lines are marked in yellow in the stock preview.
                                           •   The replacement time is insufficient. The corresponding lines are marked
6.1 / 04-2020




                                               in red in the stock preview.




                A+W Business Inventory Management                                                                        G-97
                Stock Management                                                                              Tutorial




                                   You can change the supplier and/or the delivery date when you enter an order.
                                   Section Order entry of stock articles describes this in detail.
                                    “Search Stock Article for an Item” on page G-116

                                   Stock availability and replacement time settings
                                   To calculate the future stock on hand, all reservations per day are deducted
                                   from the current stock on hand, and ordered quantities are added. The result
                                   is the probable stock on hand, depending on the date.
                                   To increase the performance, you can restrict the view in dialog Stock info by
                                   the following settings:
                                   •   You can remove certain articles from the stock preview and availability
                                       check in dialog Product management > tab Stock/Purchasing > No avail-
                                       ability check checkbox, by disabling the availability check for these articles.
                                   •   In the Company data dialog you can set the time period displayed in the
                                       preview. Two to four weeks are usually sufficient. If you enter zero, the pre-
                                       view is shown for 14 days.
                                   •   In dialog Stock management you can link several stock sizes. As a result
                                       you only have to define a minimum stock for the main article the stock on
                                       hand of which is checked. This function has been introduced in section
                                       Stock management.

                                   Booking dates
                                   To get a tangible statement on the stock on hand at a certain date, the expect-
                                   ed booking date has to be defined for all goods to be received and issued in
                                   future.
                                   The expected booking dates will be fixed as follows at item input.
                                   •   BOM components and products with procurement type Stock withdrawal
                                       which have to be cut, are entered at the start-of-production date.
                                   •   For all other stock articles, the shipping date stated in the document will be
                                       used as a booking date.
                                   If the order is dispatched in AWCapacity Planning afterwards, these expected
                                   dates will be replaced by the calculated, actual dates.


                                   Show Stock on Hand in Stock Search
                                   The stock on hand is updated by booking stock withdrawals and additions. The
                                   stock is closely linked with the sales and purchasing documents. You can
                                   therefore check the current stock on hand by means of stock information at
                                   document input.
                                   The stock on hand is also displayed when you enter quotations, orders, and
                                   purchase orders. Both purchase orders and reservations will be taken into ac-
                                   count.
                                   This session shows you how display the stock on hand and reservations for
                                   stock articles.
6.1 / 04-2020




                G-98                                                        A+W Business Inventory Management
                Tutorial                                                                               Stock Management




                                               Open dialog Stock search
                                               The Stock search dialog is also available in module Documents. You can
                                               therefore check even when you enter an order whether a sufficient quantity
                                               of the required products is available.


                                            How to display the stock on hand
                                           1 Go to menu Stock management > Search.




                   A




                   B




                   A Product – Stock article                              B Filter
                   Fig. G-50    Filter for searching for stock articles


                                           2 Restrict the search e.g. by selecting a product (A).
                                           3 Select in the Filter options (B) section which stock articles shall be dis-
                                             played.
                                               If you disable the setting Stock articles, only stock sizes defined in the
                                               Stock size product management dialog will be listed, even if they are gen-
                                               uine stock articles, i.e. stock articles from stock management.
                                           4 To start the search, go to the menu Start > Search.
                                               The hit list is shown in the overview.
6.1 / 04-2020




                A+W Business Inventory Management                                                                    G-99
                Stock Management                                                                                Tutorial




                  Fig. G-51   Search result


                                              In this example, a search for product Float 5 mm was executed.
                                        5 To view the corresponding documents, select a line and open the context
                                          menu (right mouse key).
                                        6 Click on corresponding documents.




                                              Fig. G-52   Corresponding documents
6.1 / 04-2020




                                              This dialog shows all orders and purchase orders in which this product has
                                              been entered.



                G-100                                                           A+W Business Inventory Management
                Tutorial                                                                           Stock Management




                                         7 Click on [End] to close the dialog.
                                            Dialog Stock search reopens.
                                         8 To view the next withdrawals and receipts for a product or the future stock
                                           on hand, select the product in question and go to tab Future stock on hand.




                   Fig. G-53   Future stock on hand


                                            The future stock on hand is shown for the future period that has been de-
                                            fined in the company data for the preview. Sundays and public holidays will
                                            be shown as well but they do not count.
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-101
                Stock Management                                                                            Tutorial




                                   Exercises
                                   •   Check the stock and reservations for Float 4 mm:
                                       Take a note of the individual values on tab Future stock on hand. In the next
                                       module, you are going to enter a P.O.and subsequently check how the val-
                                       ues have changed.


                                   Additional information
                                    Software Reference, “Search” on page G-217
6.1 / 04-2020




                G-102                                                      A+W Business Inventory Management
                Tutorial                                                                              Stock Management




                                     Stock P.O. (automatic)
                                     Objectives

                                     •   Getting familiar with the Stock P.O. dialog.
                                     •   Learning about automatic stock P.O.s.
                                     •   Transferring automatic P.O. proposals to Purchasing.
                                     •   Check the changes to the displayed values in the future stock on hand.


                                     Benefits

                                     • Purchase orders serve to complete the stock on hand to achieve the required
                                       target inventory or match the reservations.
                                     • If the stock on hand fails to reach the defined minimum, a P.O. proposal is created
                                       automatically. You can check this in dialog Stock P.O. and transfer it to Purchasing.


                                     Please note:

                                     Manual input of stock P.O.   Stock POs are entered and edited in module Documents.
                                                                  This process is described in section Purchasing.

                                     P.O. proposals               Automatic P.O. proposals are triggered when the stock
                                                                  fails to reach the defined minimum quantity.
                                                                  Reservations and open purchase orders are taken into
                                                                  account.
                                                                  P.O. proposals are created automatically and are
                                                                  manually transferred to Purchasing. This transfer creates
                                                                  a P.O. which can be sent to the supplier.

                                     Default settings             Master data:
                                                                  • Product management
                                                                  • Supplier file
                                                                  Company data:
                                                                  • Parameters tab
                                                                  • Tab Stock/ PP / EDI
                                                                  Stock management
                                                                  • Minimum stock
                                                                  • Purchase order quantity
6.1 / 04-2020




                A+W Business Inventory Management                                                                    G-103
                Stock Management                                                                                Tutorial




                                         P.O. Proposals
                                         Purchase orders are usually created through stock management in order to
                                         keep the stock on hand on the required level.




                A
                B




                A Minimum stock                                    B Quantity for P.O. proposal
                Fig. G-54   Stock management - Stock on hand figures


                                         If you have defined minimum quantities (A) for a stock article in dialog Stock
                                         management, P.O. proposals are created automatically with the stored P.O.
                                         quantity (B). You can check these before they are transferred to Purchasing,
                                         and change the supplier and date if necessary. Transfer to Purchasing turns
                                         the proposal into a stock P.O.
                                         Stock P.O.s can also be created manually, via document management. Man-
                                         ual stock P.O.s will be introduced in a separate training module.
6.1 / 04-2020




                G-104                                                          A+W Business Inventory Management
                Tutorial                                                                          Stock Management




                                     Transfer Stock P.O. to Purchasing
                                     Automatically created P.O. proposals are shown in the dialog Stock P.O - Or-
                                     der pool. You can change the supplier and the date. The P.O. is issued upon
                                     transfer to Purchasing. This has to be sent to the supplier.
                                     If several suppliers have been entered for a product, you can compare delivery
                                     dates and prices in the order pool and select another supplier if required.
                                     This module shows you how to transfer a P.O. proposal to Purchasing.

                                         Stock P.O. dialog
                                         Dialog Stock P.O. - Order pool is almost identically structured as the dialog
                                         P.O. transfer which has been introduced in the session on Purchasing. The
                                         dialogs are different however. For every P.O. proposal you will therefore
                                         find just one entry for which there are no reference documents.

                                     The following instructions exist for this training module:
                                     •   “How to transfer P.O. proposals to Purchasing” on page G-105
                                     •   “How to change the supplier and the delivery date” on page G-108


                                      How to transfer P.O. proposals to Purchasing
                                     1 Go to menu Stock management > Stock P.O.
                                         Dialog Stock P.O. opens.
                                         If you do not want to view P.O. proposals for the entire stock, you can re-
                                         strict the view to certain storage locations.
                                     2 To restrict the view, define the requested storage location in the fields
                                       Warehouse, Corridor, Shelf, and Tray.
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-105
                Stock Management                                                                                 Tutorial




                  Fig. G-55   Order pool


                                              In this example, no storage location is selected so that the stock on hand
                                              is listed for all storage locations.
                                           3 To start the search, go to the menu Start > Search.
                                              The proposals are loaded and listed.
6.1 / 04-2020




                G-106                                                            A+W Business Inventory Management
                Tutorial                                                                               Stock Management




                   Fig. G-56   Stock P.O.– P.O. proposals


                                         4 Select the P.O. proposals you want to transfer to Purchasing.

                                            Select several entries at once
                                            You can select several P.O. proposals at once by opening the dialog Mark-
                                            ing options in the Functions menu. For example, if you enter a certain prod-
                                            uct in this dialog, then all P.O. proposals for this product are marked with a
                                            cross in the line header.
6.1 / 04-2020




                A+W Business Inventory Management                                                                 G-107
                Stock Management                                                                             Tutorial




                  Fig. G-57   Selected P.O. proposals


                                           Double-click on the corresponding line header. Only the proposals marked
                                           by an X will be selected.
                                        5 To start the transfer to Purchasing, go to the menu Start > Execute.
                                           Confirm the message regarding the number of transferred proposals.
                                           Purchase orders are created and the transferred proposals are removed
                                           from the list.


                                         How to change the supplier and the delivery date
                                        1 Load the P.O. proposals in dialog Stock P.O. as described above.
                                        2 Select the proposal the supplier and/or delivery date of which shall be
                                          changed.
                                           Double-click on the corresponding line header. Only the proposals marked
                                           by an X will be selected.
6.1 / 04-2020




                G-108                                                        A+W Business Inventory Management
                Tutorial                                                                             Stock Management




                   Fig. G-58   Proposal to be assigned a different supplier


                                         3 Go to the menu Functions > Change supplier/delivery dates.




                                             Fig. G-59     Change delivery date


                                         4 Enter another supplier and/or delivery date.
                                         5 Click on [OK] to adopt the change.
                                             The dialog Change supplier and delivery date closes. The proposal is listed
                                             with the new supplier and/or delivery date.
6.1 / 04-2020




                                             You can now transfer the P.O. proposal to Purchasing.




                A+W Business Inventory Management                                                                G-109
                Stock Management                                                                               Tutorial




                                        Compare Prices before Transfer to Purchasing
                                        If several suppliers have been selected for a product, you can compare prices
                                        before the transfer, and choose a different supplier. This module shows you
                                        how to compare prices and choose the supplier with the best price or the short-
                                        est delivery time.


                                         How to compare the prices in a P.O. proposal
                                        1 Go to menu Stock management > Stock P.O.
                                           Dialog Stock P.O. opens.
                                        2 Select the requested storage location in the fields Warehouse, Corridor,
                                          Shelf, and Tray.
                                        3 To import the P.O. proposals, go to the menu Start > Execute.
                                           The proposals are loaded and listed.
                                        4 Select the proposal the supplier prices of which you want to compare.
                                           Double-click on the corresponding line header. Only the proposals marked
                                           by an X will be selected.




                  Fig. G-60   Item the prices of which shall be compared
6.1 / 04-2020




                                        5 Go go the menu Functions > Supplier prices.




                G-110                                                         A+W Business Inventory Management
                Tutorial                                                                              Stock Management




                                                       A       B         C          D




                                                                     H

                                                  E
                                                  F
                                                  G

                                     A Standard supplier (text in red)        E   Text color red: Standard supplier
                                     B Checkbox of standard supplier (not F       Text in green: most favorable supplier in
                                       selected)                                  terms of price
                                     C Selected supplier for the current P.O. G   Text color blue: Standard supplier is the
                                     D Checkbox for selecting the supplier        most favorable in terms of price
                                       (selected)                             H   !!! for all text colors: Delivery date may be
                                                                                  too late for timely production and shipment
                                                                                  to the customer
                                     Fig. G-61     Change the supplier of the selected item


                                     6 Check the checkbox left from the supplier to whom the purchase order for
                                       this item is to be sent.
                                     7 Click on [OK] to adopt the change.
                                        The dialog Price comparison closes. The proposal is listed with the new
                                        supplier and/or delivery date.
                                        You can now transfer the P.O. proposal to Purchasing.
6.1 / 04-2020




                A+W Business Inventory Management                                                                     G-111
                Stock Management                                                                          Tutorial




                                   Exercises
                                   •   Define the minimum and P.O. quantity for a stock article so that an auto-
                                       matic P.O. proposal is created. Choose the stock article for which you have
                                       noted the values of the future stock on hand in the previous exercise.
                                   •   Check the P.O. proposal and change the supplier or delivery date. If no al-
                                       ternative suppliers are displayed, you have to check and amend the sup-
                                       plier file in the master data.
                                   •   Transfer the P.O. proposals to Purchasing.
                                   •   Check the changed values in dialog Stock search.


                                   Additional information in section Sales
                                    Sales, “Order Header” on page C-38
                                    Sales, “Change P.O. Code” on page C-306
                                    Purchasing, “Supplier file amendment” on page D-32
                                    Purchasing, “Document P.O.” on page D-43
                                    Purchasing, “Enter receipt of goods” on page D-125
                                    Purchasing, “Dealing with boxes” on page D-134
6.1 / 04-2020




                G-112                                                     A+W Business Inventory Management
                Tutorial                                                             Stock Articles in Documents




                                     Stock Articles in Documents
                                     In this thematic block you will learn how orders and manual purchase orders
                                     access stock management.
                                     This includes the following training modules:
                                     •   “Order Entry of Stock Products” on page G-114
                                     •   “Manual Stock P.O.” on page G-122
                                     •   “Production Orders” on page G-126
6.1 / 04-2020




                A+W Business Inventory Management                                                         G-113
                Stock Articles in Documents                                                                           Tutorial




                                        Order Entry of Stock Products
                                        Objectives

                                        • Search stock articles for item entry.
                                        • Check reservation.
                                        • Check changes to stock on hand after a change of order.


                                        Benefits

                                        • The availability of a product can be checked at item entry. In case of bottlenecks,
                                          the supplier or delivery date can be changed directly in the document.


                                        Please note:

                                        Item entry                   Stock articles are selected at item entry by means of the
                                                                     stock search [F3].

                                        Reservation                  Stock articles entered in the order are marked as
                                                                     reserved on stock.

                                        Default settings             Master data:
                                                                     • Product management
                                                                     • Supplier file
                                                                     Company data:
                                                                     • Parameters tab
                                                                     • Tab Stock/ PP / EDI
6.1 / 04-2020




                G-114                                                               A+W Business Inventory Management
                Tutorial                                                                 Stock Articles in Documents




                                     Reservation and Booking of Stock Articles
                                     At order entry, the quantity or number of sqm of the stock articles is automati-
                                     cally reserved for the customer order. Goods withdrawn from stock are auto-
                                     matically booked upon printing of the delivery note or invoice. Based on the
                                     quantities sold and ordered, A+W Business calculates the actual stock on
                                     hand.

                                     Stock on hand after a change of order
                                     What happens to the stock on hand if orders are changed for which goods
                                     have already been withdrawn? In the following examples, withdrawal of goods
                                     will be booked when the delivery note is printed.

                                        Change of order           Result in order         Stock booking

                                        Change order header, no Status remains the        When the initial delivery note
                                        change of items         same.                     is printed again, no additional
                                                                                          stock withdrawal will be
                                                                                          booked.

                                        Delete item afterwards    Status is 72 and remains Query whether the stock on
                                                                  unchanged.               hand shall be corrected.

                                        Add new item afterwards                           Query whether the stock on
                                                                                          hand shall be corrected.

                                        Additional change of                              Stock on hand is automatically
                                        quantity afterwards                               corrected, without any further
                                                                                          notification.


                                     The next modules will show you how to enter a stock article in a document,
                                     and check the booking.
6.1 / 04-2020




                A+W Business Inventory Management                                                                 G-115
                Stock Articles in Documents                                                                             Tutorial




                                        Search Stock Article for an Item
                                        This module will show you how to enter an item, at the same time checking the
                                        availability of the required product. Open dialog Stock search (which has been
                                        introduced in the previous module).

                                              Stock search at a P.O. entry
                                              You can also select a stock article via dialog Stock search when you enter
                                              a stock P.O. manually. The manual stock P.O. is described in the training
                                              module of the same name.

                                              


                                         How to enter a stock article as an item
                                        1 Go to menu Documents > Order > Order and enter the order header.
                                        2 Go to item entry and enter the product number in the input line.
                                        3 Go to the menu Start > Stock search to open the dialog Stock info.
                                              The selection in dialog Stock info is already restricted to the article you
                                              have entered for the item. You have to filter the view further now, e. g. by
                                              restricting the settings to stock sizes and stock on hand which are over ze-
                                              ro.


                                              A                                                          B



                                              A Switch stock size display on or off      B Show only stock articles with a stock
                                                                                           on hand of over 0
                                              Fig. G-62     Filter for searching for stock articles
6.1 / 04-2020




                G-116                                                                 A+W Business Inventory Management
                Tutorial                                                                      Stock Articles in Documents




                                          4 Go to tab Future stock on hand to check whether the production dates are
                                            jeopardized.
                                              Display of the future stock on hand in dialog Stock info has already been
                                              introduced in the module on Stock info.
                                               “Display of the future stock on hand” on page G-97




                   Fig. G-63   Future stock on hand


                                              If the replacement time is too short, you can still enter the product then
                                              check whether another supplier is available or whether you have to change
                                              the delivery date.
                                          5 Go to tab Stock search and double-click on the stock article you want to
                                            adopt for item entry.
6.1 / 04-2020




                   Fig. G-64   Select stock article


                A+W Business Inventory Management                                                                 G-117
                Stock Articles in Documents                                                                            Tutorial




                                               Dialog Stock info closes and the item entry data is updated.
                                           6 Enter all item data and return to the document header.
                                               If the replacement times are too short, you can view the articles in question
                                               in dialog Change delivery date.
                                           7 Click on the icon next to the shipping date to open the dialog.




                                                                                                                       A




                                                                                                                       B




                                                                                                                       C




                A Check delivery date                                   C List of possible suppliers and shipping dates for
                B Products for which the stock on hand is too low         the selected product

                Fig. G-65    Check delivery date in the order


                                               Alternative suppliers from the supplier file are shown with the defined re-
                                               placement time and the corresponding date.
                                               Double-click on the article in the list on top (B) to open the Stock info with
                                               details on the articles.
                                           8 If the scheduled delivery date is jeopardized, the following options are
                                             available:
6.1 / 04-2020




                                               •   Change the supplier for the item in question or for the entire order.
                                               •   Change the delivery date and inform the customer.


                G-118                                                              A+W Business Inventory Management
                Tutorial                                                               Stock Articles in Documents




                                           These steps are described in detail in the tutorial on Sales.
                                     9 Go to the menu Start > Save to save the data.
                                        The data is saved. You can now check the reservation of stock articles.


                                     Check the Bookings
                                     In this module you will learn how to check the bookings for stock articles. Sav-
                                     ing reserves the item. Withdrawal of goods is generally booked when the de-
                                     livery note is printed. Printing depends on the settings in status management.


                                      How to check the bookings
                                     1 Open the Booking journal dialog as described in section Queries.
                                     2 Restrict the selection to the order for which you want to check the reserva-
                                       tion.
                                        The list shows all order items with the current booking type.




                                     Fig. G-66    Booking – reserved


                                        The booking journal shows the booking type reserved only until withdrawal
                                        of goods is booked.
6.1 / 04-2020




                A+W Business Inventory Management                                                            G-119
                Stock Articles in Documents                                                                     Tutorial




                                              After the goods are withdrawn, the order items are marked as shipped.




                                        Fig. G-67         Booking – shipped


                                              The order history shows the individual status changes based on the print-
                                              outs and inventory bookings
6.1 / 04-2020




                                              Fig. G-68      Order history



                G-120                                                           A+W Business Inventory Management
                Tutorial                                                                 Stock Articles in Documents




                                     Exercises
                                     •   Enter an order with existing stock articles and check the entries in the book-
                                         ing journal:
                                         – After order input.
                                         – After printing the delivery note. Which changes are visible?
                                     •   Enter an order and check the stock on hand and the reservations.
                                     •   Issue an invoice for the order and check the stock reservations again.
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-121
                Stock Articles in Documents                                                                         Tutorial




                                        Manual Stock P.O.
                                        Objectives

                                        • Introducing the special features of the stock P.O. in document management.


                                        Benefits

                                        • Manual stock P.O.s are used to complete the stock on hand, e. g. for large-scale
                                          orders for which automatic reordering alone is insufficient.


                                        Please note:

                                        Document type               The document Stock P.O.is a separate document type.
                                                                    Receipt of goods can be booked to stock only for stock
                                                                    P.O.s.

                                        Default settings            Master data:
                                                                    • Product management
                                                                    • Supplier file
                                                                    Company data:
                                                                    • Parameters tab
                                                                    • Tab Stock/ PP / EDI
6.1 / 04-2020




                G-122                                                              A+W Business Inventory Management
                Tutorial                                                                    Stock Articles in Documents




                                         Manual Input of Stock P.O.
                                         Purchase orders for stock articles can be triggered automatically, or entered
                                         manually. Automatic P.O. proposals have been introduced already in the mod-
                                         ule on the automatic stock P.O.
                                         This module will show you how to enter a stock P.O. manually. Document input
                                         is described in detail in sections Sales and Purchasing. The following instruc-
                                         tions therefore concentrate on the main steps.


                                          How to enter a stock P.O. manually
                                         1 Go to menu Documents > P.O. > P.O.
                                            The dialog Document management opens.
                                         2 Enter the document header. Enter at least the supplier and the delivery
                                           date.


                                                                                                                     A




                                                                                                                     B




                A Document type                                    B Setting the document type
                Fig. G-69   Stock P.O.


                                         3 Select the entry Stock P.O. in field Type (B).
6.1 / 04-2020




                                            If you set another document type, receipt of goods is not automatically add-
                                            ed to the stock on hand.



                A+W Business Inventory Management                                                               G-123
                Stock Articles in Documents                                                                     Tutorial




                                        4 Enter the item(s).

                                              Items without stock codes
                                              If you enter stock P.O.s with items which are not recorded as stock items,
                                              they will not be displayed at receipt of goods. You can however enable the
                                              corresponding option in master data Company > Company data > tab Stock
                                              / PP / EDI.

                                        5 Go to the menu Start > Save to save the data.
                                              The data is saved.
                                        6 Print and send the purchase order.
                                              This process is described in section Sales.
                                              
6.1 / 04-2020




                G-124                                                           A+W Business Inventory Management
                Tutorial                                                             Stock Articles in Documents




                                     Exercises
                                     •   Check the stock on hand for a stock article.
                                     •   Enter a stock P.O. manually and check the corresponding values again in
                                         the Stock info dialog.
6.1 / 04-2020




                A+W Business Inventory Management                                                        G-125
                Stock Articles in Documents                                                                             Tutorial




                                        Production Orders
                                        Objectives

                                        • Introducing production orders.
                                        • Introducing the manual and automatic creation of work orders.


                                        Benefits

                                        • Work orders are used to replenish the stock on hand.
                                        • When the stock on hand falls below the defined minimum, work orders can be
                                          created automatically if the diversion to an internal customer is enabled in the
                                          supplier file.


                                        Please note:

                                        Procurement type             All articles entered in a production order have to have the
                                                                     procurement type Production.

                                        Booking type                 Unlike common orders, the entered items are not
                                                                     reserved on stock but are marked as ordered.

                                        Addition to stock            Stock additions based on work orders can be booked
                                                                     automatically or by hand:
                                                                     • Manual status change in module Production.
                                                                     • Automatic status reports from production.

                                        Default settings             Stock management:
                                                                     • Minimum stock
                                                                     • Purchase order quantity
                                                                     Master data:
                                                                     • Product management
                                                                     • Partner management (internal customer)
                                                                     • Supplier file (diversion to internal customer)
                                                                     Company data:
                                                                     • Parameters tab
                                                                     • Tab Stock / PP / EDI > Registration point
6.1 / 04-2020




                G-126                                                               A+W Business Inventory Management
                Tutorial                                                                Stock Articles in Documents




                                     Stock Article as Part of the Production Order
                                     Work orders are used to replenish the stock on hand. All articles entered in
                                     such an order are automatically changed to procurement type Production. Un-
                                     like customer orders, the items are not reserved on stock but are marked as
                                     ordered.




                                     Fig. G-70    Item entry – procurement type Production


                                     A production order differs from other orders only in its document type:




                                     Fig. G-71    Order entry – document type Production Order


                                     Work orders can be entered in different ways:
                                     •   Enter a new document manually.
                                     •   Copy a saved (dummy) article.
                                     •   Automatic creation based on a shortage in the stock on hand.
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-127
                Stock Articles in Documents                                                                          Tutorial




                                             Manual Input by Copying
                                             If you enter work orders on a regular basis, you can copy the previously en-
                                             tered order to make this task easier.
                                             •   Before copying, you have to set the document type of the target document
                                                 to Production Order.
                                             •   If only certain items shall be adopted from the order, you can select them.
                                             •   You can amend the data in the new document.




                A


                                                                                                                            B




                A Copy from order to order                                     B Document type of the target order
                Fig. G-72    Create production order by copying


                                             A detailed description of the function Copy documents can be found in section
                                             Sales.
6.1 / 04-2020




                G-128                                                               A+W Business Inventory Management
                Tutorial                                                                       Stock Articles in Documents




                                           Settings in Supplier File
                                           If a minimum stock and a (standard) order quantity have been defined for the
                                           stock article in dialog Stock management, the system can create automatic
                                           P.O. proposals. These are listed in dialog Stock P.O.
                                           This is how purchase orders of the type Stock P.O. are usually created. How-
                                           ever, if an internal customer is entered in the supplier file instead of a standard
                                           supplier, work orders can be created automatically.




                A




                B




                                     C
                A Product for which work orders shall be created    B Diversion to internal customer
                                                                    C Customer selection
                Fig. G-73    Internal customer for work orders


                                           In the supplier file, an internal customer is defined for which the work order is
                                           entered automatically. The option Internal customer can be enabled on prod-
                                           uct group or product level. The product settings have priority over the product
                                           group settings.
6.1 / 04-2020




                A+W Business Inventory Management                                                                     G-129
                Stock Articles in Documents                                                                         Tutorial




                                        P.O. Quantity after Stocktaking
                                        The program checks whether the current stock on hand plus the already or-
                                        dered quantities and minus the reserved quantities will fall below the minimum
                                        stock on hand.
                                        If this is the case, the P.O. proposal shows the multiple of the (standard) P.O.
                                        quantity.

                                        Manual and automatic stock P.O.


                                                                                 Stock P.O.
                                                                              Storage location




                                                                              Below minimum
                                                                                  stock?



                                                                                     Yes




                                                                                Standard P.O.
                                                                                  quantity?



                                                                                     Yes




                                                                            Search in supplier file




                                                              Standard                                 Internal
                                                              supplier?                               customer



                                                                 Yes                                     Yes




                                                            P.O. proposal                        Production order
                                                              Stock P.O.                      Document management
6.1 / 04-2020




                                        Fig. G-74    Stock P.O. vs. production order




                G-130                                                                   A+W Business Inventory Management
                Tutorial                                                                   Stock Articles in Documents




                                     This flow chart shows A+W Business's reactions to different presettings in the
                                     supplier file.

                                     Purchase order quantity
                                     The multiplier will be calculated so that as a result of the P.O. proposal the min-
                                     imum stock is exceeded.




                                     Fig. G-75     Quantities for stock articles (dialog Stock management)


                                        Example

                                        Tempered glass with article number 4008 is kept as a stock article.
                                        Current stock on hand: 10 pcs.
                                        Minimum stock: 30 pcs.
                                        P.O. quantity: 5 pcs.
                                        The P.O. quantity for tempered glass 4008 is calculated as follows:
                                        Difference between current stock on hand and minimum stock on hand: 20
                                        pcs. This difference includes the P.O. quantity of 5 pcs. four times.
                                        P.O. quantity: 4 x 5 = 20 pcs.
                                        Current stock on hand plus ordered quantity: 10 + 20 = 30 pcs.


                                     The calculated quantity is adopted for the P.O. proposal. It can be amended in
                                     the Stock P.O. dialog.
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-131
                Stock Articles in Documents                                                                         Tutorial




                A




                B




                A Restriction to storage location                     B P.O. proposal for production order
                Fig. G-76     Stock P.O.– P.O. proposals


                                            In the Stock P.O. module you have already been shown how to edit and trans-
                                            fer purchase orders.
                                             “Transfer Stock P.O. to Purchasing” on page G-105
                                            The production order is created by the transfer, in the last active order Number
                                            Manager.
6.1 / 04-2020




                G-132                                                              A+W Business Inventory Management
                Tutorial                                                                Stock Articles in Documents




                A




                A Automatically created production order
                Fig. G-77    Production order in Number Manager for orders


                                           The production order can now be opened as a document.
6.1 / 04-2020




                A+W Business Inventory Management                                                           G-133
                Stock Articles in Documents                                                              Tutorial




                                                                                  A




                                                        B
                A Order header – Production order                     B Ordered quantity
                Fig. G-78   Document Production Order


                                         The work order can be edited and transferred to production.
6.1 / 04-2020




                G-134                                                         A+W Business Inventory Management
                Tutorial                                                                 Stock Articles in Documents




                                     Stock Addition based on Production Order
                                     On tab Stock / PP / EDI in company data, set the limit status for registration
                                     points to define from which point on an order counts as produced. The limit sta-
                                     tus is the status defined for the selected registration point.




                                     Fig. G-79    Company data – Stock / PP / EDI: Registration point for status change


                                     There are two ways of entering additions to stock based on production orders:
                                     •   If the status of the work order exceeds the defined status due to a report
                                         from production, the addition to stock is booked automatically.
                                     • If you do not use production reports, you can enter the addition to stock by
                                         means of the manual status report in the Production module. If you set the
                                         production order there to a status above the aforementioned limit, the stock
                                         withdrawal of the material consumed and the addition of produced stock ar-
                                         ticles to stock are booked automatically.
                                     If no other storage location has been defined, the order quantity is allocated to
                                     the standard storage location.
                                     The booking of work orders is described in detail in section Production.


                                     Additional information
                                      Master Data, “Company Data – Stock/Purchasing/EDI” on page B-955
                                      Sales, “Order Header” on page C-38
                                      Sales, “Change P.O. Code” on page C-306
                                      Production, “Production Orders” on page E-128
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-135
                Inventory                                                                      Tutorial




                            Inventory
                            This section shows you how to correct the stock on hand in A+W Business by
                            means of an inventory.
                            This includes the following training modules:
                            •   “Periodical Inventory” on page G-137
                            •   “Initial Inventory” on page G-153
6.1 / 04-2020




                G-136                                             A+W Business Inventory Management
                Tutorial                                                                                            Inventory




                                     Periodical Inventory
                                     Objectives

                                     • Getting familiar with the inventory process.
                                     • Learning about the inventory dialogs.
                                     • Carry out inventory.


                                     Benefits

                                     • An inventory can be used to correct the stock on hand in A+W Business.
                                     • For big storage locations, the inventory can be organized in such a way that
                                       common business operations are impeded as little as possible.


                                     Please note:

                                     No change of stock during     On the day of the count, no orders, purchase orders or
                                     the inventory                 receipt of goods must be entered; no goods must be
                                                                   removed from or added to stock.
                                                                   The target inventory should be determined on the day of
                                                                   the count.

                                     The inventory process         The inventory is run in three steps:
                                                                   •   Create inventory list
                                                                   •   Determine target inventory
                                                                   •   Enter counted values
                                                                   •   Finalize inventory

                                     Split stocktaking             For large storage locations it may be useful to run the
                                                                   inventory in smaller units.

                                     Separate stocktaking for      A special inventory list is created for boxes. The existing
                                     boxes                         boxes are scanned individually.

                                     No changes to the product As soon as the inventory list has been created, all the
                                     master data               products that are listed on the inventory list are marked
                                                               in product management (master data). The procurement
                                                               type and stock code in these products are then blocked.
                                                                   The marking will be deleted once the inventory has been
                                                                   taken.

                                     Complete the inventory list Additions must be made only before the target stock is
                                                                 determined.

                                     Target inventory in the       To print the target inventory on the count list you have to
                                     count list                    determine the target inventory before printing.

                                     Final inventory by inventory The final inventory can be run just once per inventory list.
                                     list

                                     Default settings              None
6.1 / 04-2020




                A+W Business Inventory Management                                                                      G-137
                Inventory                                                                              Tutorial




                            Stocktaking
                            At least once in every business year, stock has to be taken to check if the
                            booked or target inventory shown in A+W Business Stockkeeping matches the
                            actual stock. Inventory lists are created for this statutory annual stocktaking
                            which help to count and enter the actual stock on hand. Stocktaking deter-
                            mines the existing stock by type, quantity, and value.
                            Basis for any stocktaking is the inventory list which can refer to selected stock
                            articles and/or storage locations. This way, stock can be taken in several steps
                            which presents less of an obstruction to the daily business.
                            A+W Business provides inventory lists and the target inventory for stocktak-
                            ing. Stocktaking can be done in the conventional way or, for boxes, with the
                            help of barcode registration.
                            Stocktaking is completed by the final inventory. After that, the quantities will be
                            updated in A+W Business.

                            Actual stock on hand
                            The stock on hand is entered on the basis of count lists. New stock articles can
                            be entered at the same time. During stocktaking, the stock articles on the in-
                            ventory list are not locked for document entry. This is why no orders, purchase
                            orders, or receipt of goods must be entered on the day of the count.

                            Target inventory
                            The target inventory must be determined no later than on the day of the count.
                            This allows you to create the inventory list well in advance of the actual count-
                            ing, input of the counted quantities, and the final inventory.

                               Example

                               Activity                   Date             Stock on hand         Target
                                                                                              inventory

                               Inventory list created     15 Dec                                     100

                               Count stock on hand        31 Dec                       80            100

                               Sales                      01 Jan to                   -30            -30
                               Purchasing                 14 Jan                      +10            +10

                                                          15 Jan           Actual stock on            80
                                                                                  hand 60

                               Final inventory                                 New target             60
                                                                                inventory:


                            With the final inventory, the actual stock is saved in the system as the new tar-
                            get inventory.
                            The target inventory can be printed on the count lists if required. If you do not
                            print the target inventory you can practically neglect the "counted" quantities
6.1 / 04-2020




                            estimated on the basis of the target inventory.




                G-138                                                 A+W Business Inventory Management
                Tutorial                                                                                     Inventory




                                     sqm articles
                                     If individual sheets of defined sizes are counted for a sqm article, these can be
                                     entered as units. At the final inventory, these will be converted into sqm and
                                     booked as such on stock (the printed closing inventory will show the counted
                                     quantity however).

                                     Stocktaking of boxes
                                     To take stock of boxes for the inventory list, first create an inventory list then
                                     determine the target inventory. Now scan or manually enter the box ID, the
                                     storage location, and - if applicable - a different number of sheets. Scanning a
                                     box will always add it to the latest inventory list. Now enter the remaining stock
                                     in Inventory Management if necessary, and book the final inventory.

                                     Example count list




                                     Fig. G-80    Count list with fields for the counted quantities


                                     The counted quantities are entered in the count list and, later, in inventory
                                     management.
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-139
                Inventory                                                                            Tutorial




                            Create Inventory List
                            The inventory is based on lists in which the manually counted quantities are
                            noted. These lists can be based on various criteria, and can be printed.
                            When you print these lists and realize that certain articles are missing, you can
                            add a supplementary inventory. This way, you will not have to print all lists
                            again.

                                No changes to the product master data
                                When the inventory list has been created, all products that appear on the
                                inventory list are marked in product management (master data). The pro-
                                curement type and stock code in these products are then blocked. This
                                mark will be deleted when the inventory has been finalized; the data can be
                                edited again.

                            This session shows you how to create inventory lists and open them again.
                            The following instructions exist for this training module:
                            •   “How to start an inventory” on page G-141
                            •   “How to print the count lists” on page G-143
                            •   “How to load a saved inventory list” on page G-144
                            •   “How to complete an inventory list before counting” on page G-144
6.1 / 04-2020




                G-140                                               A+W Business Inventory Management
                Tutorial                                                                                      Inventory




                                      How to start an inventory
                                     1 Go to menu Stock management > Stocktaking > Inventory list.
                                        Dialog Inventory list opens.
                                     2 Go to the menu Start > New to switch to the input mode.

                                       A           B                     C




                                                                                                                       D


                                                                                                                       E




                                     A All articles or sequence of article        C Restrictions
                                       numbers                                    D Inventory evaluation
                                     B Inventory date                             E Sorting the list
                                     Fig. G-81     Fields for the new inventory list are enabled


                                        The name for this inventory is a date (B). The system will suggest the cur-
                                        rent date by default. You can enter or select any other date of course.
                                     3 Choose the articles (A) for the inventory:
                                        •   All articles:
                                            You can take stock of all articles defined as products in the master data.
                                            In this case, the fields for the article numbers are locked.
                                            Enable this option for the initial inventory; for all other inventories, you
                                            can restrict the inventory lists to certain articles.
                                        •   Article number:
                                            You can restrict the inventory list to a sequence of article numbers. The
                                            fields are locked if you have selected the option All articles.
                                     4 If applicable, restrict the list further (C):
                                        •   Only products with stock > 0:
6.1 / 04-2020




                                            You can restrict the inventory to stock articles with inventory. If you do
                                            not check the checkbox, the complete product master data will be in-



                A+W Business Inventory Management                                                                G-141
                Inventory                                                                              Tutorial




                                   cluded in the inventory list unless the selection is not restricted by other
                                   criteria.
                               •   Only products with assigned stock product:
                                   You can restrict the inventory to the stock articles in stock management.
                                   If you do not select this checkbox, the entire product master data includ-
                                   ing stock size table will be included in the inventory list unless the selec-
                                   tion is restricted by other criteria.
                               •   Only products with stock in the product:
                                   You can restrict the inventory to products with procurement type Stock
                                   withdrawal.
                               •   No box with ID number and inventory = 0:
                                   The stock on hand can include boxes which have already been shipped
                                   but not deleted. Their stock is correctly displayed as 0. You can hide
                                   these boxes because no quantities will be entered for them.
                               •   Only for defined storage location:
                                   This setting activates the fields for selecting the storage location.
                                   If you want to take stock only for certain storage locations, you can cre-
                                   ate separate inventory lists. Please note that articles can also be
                                   booked to storage location <n.e.>.
                                   In case of comprehensive stocktaking you can also split the inventory
                                   list by storage location for the printout.
                            5 Choose the inventory evaluation type (D).
                               If you have enabled the options for PP calculation in the company data, you
                               can have the stock evaluation calculated as follows:
                               •   PP price list:
                                   The individual prices of the products from the PP rate assignment are
                                   used.
                               •   Lowest PP:
                                   For all articles, the lowest value is used for the inventory valuation each
                                   time.
                               •   Cut PP:
                                   For all articles, the average PP is used. For this, the Article PP option
                                   must be activated in the company data.
                            6 Choose the sorting type (E).
                               Sorting of articles on the inventory list should be based on the defined cri-
                               teria. The option Size is useful for stock sizes for example.
                            7 Go to the menu Start > Save to create the inventory list.
                               The inventory list opens in the overview. You can now print the count lists
                               and/or determine the target inventory.

                               No changes to the product master data
                               As soon as the inventory list has been created, all the products that are list-
                               ed on the inventory list are marked in product management (master data).
                               The procurement type and stock code in these products are then blocked.
                               As soon as the inventory has been completed, the marking is deleted and
6.1 / 04-2020




                               the data can be edited again.




                G-142                                                A+W Business Inventory Management
                Tutorial                                                                                     Inventory




                                      How to print the count lists
                                        To print the target inventory on the count list you have to determine the tar-
                                        get inventory prior to printing.
                                     1 Go to menu Stock management > Stocktaking and select the date of the
                                       inventory list.
                                     2 Go to the menu Start > Search to load the inventory list.
                                        These steps are redundant if you print the count list immediately after cre-
                                        ating the inventory list.
                                     3 Go to menu Print > Printer.
                                        To check the result on screen first, select Screen. You can start the printout
                                        if you are satisfied with the result. The following steps are the same for both
                                        settings.



                                        A

                                        B


                                        C




                                        A Page break                                 C Sorting
                                        B Articles that shall be printed
                                        Fig. G-82     Inventory - Print count list


                                        Print the count lists so that they match the tasks of your stocktaking staff.
                                     4 Define the point at which a new page (A) shall be started.
                                        If you did not define different storage locations, this setting can be omitted.
                                        If you have split the count areas by storage location, start a new page after
                                        the corresponding storage locations.
                                        You must select at least one warehouse (level 1) for the printout.
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-143
                Inventory                                                                             Tutorial




                            5 Define the stock articles (B) to be printed on the list.
                               If different stock articles are stored in the individual storage locations, you
                               can distinguish finished products and raw material. Finished products are
                               stock articles which are not stored in the raw material stock.
                               The characteristics Finished products and Raw material have been as-
                               signed in stock definition.
                                “Define Storage Location” on page G-22
                            6 Sort (C) the articles on the count list depending on the selected criteria. The
                              option Article makes sense for instance if the stock is organized by prod-
                              ucts.
                            7 Click [OK] to start printing.
                               The list is printed and can be used for counting.


                             How to load a saved inventory list
                            1 Go to menu Stock management > Inventory.
                            2 Go to field Inventory date and select the date on which the inventory list has
                              been saved.
                            3 Go to the menu Start > Search to load the inventory list.
                               The inventory list opens.


                             How to complete an inventory list before counting
                               If you have already determined the target inventory for an inventory list, you
                               cannot complete this list. In this case, close the inventory and enter the
                               missing articles in a new inventory list.
                            1 Go to menu Stock management > Inventory.
                            2 Go to the menu Start > New to switch to the input mode.
                               The fields will be enabled.
                            3 Select the inventory list to which articles shall be added.
                            4 Select the stock articles and/or storage locations.
                            5 Go to the menu Start > Save to save the data.
                               A query is displayed that allows you to abort this process or complete it.
                            6 Select
                               •   [Yes]: The existing list is displayed, the new articles are added at the
                                   end.
                               •   [No] or [Abort]: The query is closed. You can change the date or other
                                   criteria and create a new inventory list.
6.1 / 04-2020




                G-144                                               A+W Business Inventory Management
                Tutorial                                                                                     Inventory




                                     Determine Target Inventory
                                     The target inventory has to be determined for every inventory list. It defines the
                                     quantities that should be on stock according to the system. To print the target
                                     inventory on the count lists you have to determine the target quantity prior to
                                     printing a list.

                                        No inventory bookings on the count day
                                        After the target quantity has been determined, the stock quantities must be
                                        counted. On the day of the count, no stock articles may be withdrawn and
                                        no stock movements may be booked until counting has been finalized. This
                                        applies to all manual or automatic stock withdrawals/additions, and all
                                        goods received into stock based on purchase orders. A+W Business is not
                                        automatically blocked for bookings.

                                     This module shows you how to determine the target inventory for a saved in-
                                     ventory list.


                                      How to determine the target inventory for an inventory list
                                     1 Go to menu Stock management > Inventory > Target inventory
                                        Dialog Target inventory opens.
                                     2 Load the inventory list for which you want to determine the target inventory.




                                        Fig. G-83     Determine target inventory


                                     3 Go to menu Start > Execute to determine the target inventory and confirm
6.1 / 04-2020




                                       the query by [Yes].




                A+W Business Inventory Management                                                               G-145
                Inventory                                                                          Tutorial




                            The target inventory is entered in column Target. You can determine the
                            target inventory just once per inventory list. The result will not be updated
                            even if you execute this function several times.
                            If the target inventory shall be printed on the count list, you can start the
                            printout now.
                            You can now start counting and subsequently enter the counted quantities.
6.1 / 04-2020




                G-146                                            A+W Business Inventory Management
                Tutorial                                                                                   Inventory




                                     Enter Counted Values
                                     Once you have entered the counted quantities in the printed count lists, you
                                     can enter the values in dialog Inventory management.
                                     This module will show you how to enter the counted quantities in
                                     A+W Business plus a new stock article if necessary.
                                     The following instructions exist for this training module:
                                     •   “How to enter the counted quantities” on page G-147
                                     •   “How to enter a new stock article during stocktaking” on page G-148


                                      How to enter the counted quantities
                                     1 Go to menu Stock management > Inventory > Inv. Management.
                                         Dialog Inv. Management opens.
                                     2 Load the inventory list.
                                         The table shows the records in the same sequence as on the printed list.
                                         Menu Sorting can be used to choose another sequence if this will facilitate
                                         the entry of the counted values.




                                                                                                                  A




                                                                                                                  B




                                     A Enter counted quantity                 B List of records
                                     Fig. G-84    Inventory - Enter counted quantities


                                     3 Enter the quantity (A) for the first item in field Qty and confirm by <Enter>.
                                         The marking automatically switches to the next line where you can enter
6.1 / 04-2020




                                         the next quantity.
                                     4 To enter the quantities in a different sequence, just select the line in ques-
                                       tion.


                A+W Business Inventory Management                                                            G-147
                Inventory                                                                            Tutorial




                               Quantity and storage location for several articles
                               You can select several records and set the quantity for all to zero or change
                               the storage location by using the Functions menu.

                            5 If necessary, you can change the storage location, the inventory price, and
                              the category to be used for inventory evaluation.
                               Changed inventory prices will not be saved in the purchase price table after
                               the finalization of the inventory, and will not be considered for calculating
                               the average purchase price.
                            6 Go to the menu Start > Save to save the data.
                               The data is saved. If you have not entered the data completely yet, you can
                               resume the input later. Start from step 1 in this case.
                               You can finish stocktaking when you have entered all quantities.


                             How to enter a new stock article during stocktaking
                            1 Go to menu Stock management > Inventory > Inv. Management and select
                              the current inventory.
                            2 Select the record for which you want to enter a new stock article.
                            3 Go to the menu Start > New to switch to the input mode.
                               All data of the original stock article will be copied so that you only have to
                               edit the data for the new stock article.
                            4 Enter the width, height, storage location etc.
                            5 Go to the menu Start > Save to save the data.
                               The list is completed by the new stock article.
6.1 / 04-2020




                G-148                                              A+W Business Inventory Management
                Tutorial                                                                                   Inventory




                                     Finalize Inventory
                                     Stocktaking is finalized by booking the results of counting and updating the
                                     stock on hand.
                                     The final inventory can be run just once per inventory list. Should you detect
                                     errors in the counted or entered quantities after closing, you have to correct
                                     the quantities in dialog Inventory management, or create and finalize a new in-
                                     ventory list for the corresponding article.
                                     This module shows you how to to finalize the inventory for an inventory list.
                                     For instructions on this subject, please see:
                                     •   “How to finalize the inventory” on page G-149
                                     •   “How to delete an inventory list after the final inventory” on page G-150


                                      How to finalize the inventory
                                     1 Go to menu Stock management > Inventory > Final Inventory.
                                         Dialog Final Inventory opens.
                                     2 Load the inventory you want to finalize.




                                         Fig. G-85    Inventory - Final Inventory


                                         The inventory list is displayed with the quantities entered.
                                     3 Check in the Options menu whether the stock on hand should be set to
                                       zero with or without query when no quantities have been entered.
6.1 / 04-2020




                                     4 Select production preparation for which stocktaking has been restricted.
                                     5 Go to menu Start > Execute and confirm the query by [Yes] in order to fi-
                                       nalize the inventory.


                A+W Business Inventory Management                                                            G-149
                Inventory                                                                              Tutorial




                               The data will be saved and the stock on hand values and the prices for the
                               inventory evaluation will be updated. Booked records are deleted from the
                               list. The locks in the product master data will be removed.
                               Records that could not be booked are kept on the list. You can complete
                               the missing entries in dialog Inv. Management.
                               If all records could be booked, the complete inventory list will be deleted
                               from the final inventory.

                               Inventory errors
                               If errors have occurred during stocktaking and individual records are not
                               deleted from the inventory list, you can use the log to search for the cause.
                               Open the log via System > Log.


                             How to delete an inventory list after the final inventory

                               Do not delete individual records
                               After the final inventory, individual records cannot be deleted from the list.

                            1 Go to menu Stock management > Stocktaking > Inventory list.
                            2 Load the inventory list you have finalized.
                            3 Go to menu Start > Delete and confirm the query by [Yes].
                               The inventory list is deleted. If further inventory lists were created, the next
                               list will be loaded now.
6.1 / 04-2020




                G-150                                               A+W Business Inventory Management
                Tutorial                                                                                  Inventory




                                     Add Supplementary Inventory
                                     You can combine two separate inventories to print the final inventory. Both in-
                                     ventories have to be final (i.e. booked) for this purpose.
                                     Chapter Create inventory list describes how to add further stock articles to an
                                     inventory list.
                                     This module shows you how to add a supplementary inventory to a main in-
                                     ventory.


                                      How to add a supplementary inventory
                                     1 Go to menu Stock management > Inventory > Final Inventory.
                                        Dialog Final Inventory opens.
                                     2 Select the main inventory in field Inventory date.
                                     3 Select Functions > Add supplementary inventory from the menu.




                                        Fig. G-86    Select supplementary inventory


                                     4 Select the date of the supplementary inventory and press [OK] to adopt it.
                                        The main inventory list will be enhanced by the items of the supplementary
                                        inventory. The supplementary inventory list is then deleted from dialog In-
                                        ventory list.
6.1 / 04-2020




                A+W Business Inventory Management                                                            G-151
                Inventory                                                                               Tutorial




                            Exercises
                            •   Create an inventory list for a sequence of 5 articles.
                            •   Add two articles to the inventory list.
                            •   Determine the target inventory for the entire inventory list.
                            •   Enter the counted quantities.
                            •   Finalize the inventory.
                            •   Create another inventory list consisting of three articles. Add it to the first
                                inventory as a supplementary inventory.


                            Additional information
                             Software Reference, “Inventory List” on page G-167
                             Software Reference, “List Printing” on page G-171
                             Software Reference, “Target Quantity” on page G-173
                             Software Reference, “Management” on page G-176
                             Software Reference, “Finalization” on page G-181
6.1 / 04-2020




                G-152                                                A+W Business Inventory Management
                Tutorial                                                                                            Inventory




                                     Initial Inventory
                                     Objectives

                                     • Getting familiar with the function of the initial inventory


                                     Benefits

                                     • The initial inventory is used to put your stock into operation, including the stock
                                       articles and the current stock on hand.


                                     Please note:

                                     Support for your initial      Before starting the initial inventory, please contact A+W
                                     inventory                     Software GmbH. Your contacts there will support you
                                                                   with the completion.

                                     No order processing           As no orders must be processed during the initial
                                                                   inventory, the initial inventory should take place out of
                                                                   the daily business hours, e. g. on a weekend.

                                     Prerequisite                  You have to be familiar with the process of periodical
                                                                   stocktaking before you start with the initial inventory.
                                                                   Please study the training module on section Periodical
                                                                   inventory carefully.

                                     Default settings              None
6.1 / 04-2020




                A+W Business Inventory Management                                                                      G-153
                Inventory                                                                            Tutorial




                            Initial Inventory Process
                            •   Stock initialization: the stock is deleted (module Utilities).
                                From now on, new orders must not be entered, nor must old orders be pro-
                                cessed.
                            •   Create inventory list.
                            •   Determine target inventory.
                            •   Stock management: Set all stock on hand to 0 and define the standard stor-
                                age location for all stock articles.
                            •   Finalize inventory.
                            •   Initialize stock (module Utilities).
                                Until now you have entered all actual stock articles and have set their quan-
                                tities to 0. All previous (incorrect) values, e. g. test products and stock
                                quantities to test functions, have been deleted.
                                The values for purchase orders and reservations are checked and correct-
                                ed if necessary.
                            •   Execute complete inventory:
                                – Create new inventory list.
                                – Print count list.
                                – Determine target inventory.
                                – Count quantities of stock articles.
                                    Do not book any stock withdrawals or additions while counting.
                                – Enter counted values.
                                – Finalize inventory.
                            •   Initialize stock (module Utilities).
                                The values for purchase orders and reservations are checked again and
                                applied to the stock articles.
6.1 / 04-2020




                G-154                                                A+W Business Inventory Management
                Tutorial                                                                                         Inventory




                                           Execute Initial Inventory
                                           Initial stocktaking takes place before you start working with A+W Business in-
                                           ventory management for the first time. It is used to start up the stock with its
                                           articles and initial stock on hand.

                                               You should be familiar with the regular stocktaking procedure
                                               Before starting on the following actions you should read the instructions on
                                               the regular stocktaking process. The description of the initial inventory is
                                               based on the assumption that you are familiar with this process.


                                            How to execute the initial inventory

                                               Please contact our service team before you start the initial inventory
                                               Before starting the initial inventory, please contact A+W Software GmbH.
                                               Your contacts there will support you with the completion.

                                           1 Start module Utilities.
                                           2 Go to menu System > Initialize Stock.




                   Fig. G-87   Utilities – Initialize stock


                                           3 Go to menu Functions > Delete stock.
6.1 / 04-2020




                                               From now on, you must not enter new orders or edit existing orders until
                                               the stock has been initialized. If someone is still using the Document man-



                A+W Business Inventory Management                                                                   G-155
                Inventory                                                                             Tutorial




                               agement dialog, storage location n.e. will be created again in inventory
                               management, and is allocated to all stock articles.
                            4 Now take the following steps to execute the initial inventory:
                               •   Create Inventory List.
                                   Select the following criteria in dialog Inventory list:
                                   – For stock articles only:
                                      Setting All articles would e. g. put even P.O. items on the list.
                                   – All storage locations.
                               •   Determine Target Inventory.
                               •   Enter Counted Values.
                                   Set the quantities of all counted articles to 0 in dialog Stock manage-
                                   ment – Management .
                                   This process is described in the operation instructions for entering the
                                   counted quantities in the notes on step 4 and step 5.
                               •   Finalize Inventory.
                            5 Return to dialog Initialize Stock.
                            6 To start the activity, go to the menu Start > Execute.
                            7 Use a new inventory list for complete inventory taking:
                               •   “How to start an inventory” on page G-141
                               •   “How to print the count lists” on page G-143
                               •   “How to determine the target inventory for an inventory list” on
                                   page G-145
                               Please make sure that no stock additions or withdrawals are booked during
                               the counting. This also applies to entering received goods.
                            8 Enter the counted quantities and the correct storage locations and finalize
                              the inventory:
                               •   “How to enter the counted quantities” on page G-147
                               •   “How to finalize the inventory” on page G-149
                            9 Open dialog Stock initialization as described in step 1 and 2.
                            10 To start the activity, go to the menu Start > Execute.
                               From now on, the stock on hand and the storage locations reflect correct
                               values.
6.1 / 04-2020




                G-156                                                A+W Business Inventory Management
                Tutorial                                                                                   Exercises




                                     Exercises
                                     Answer the following questions by explaining the corresponding settings.
                                     •   When does the stock take reports from production, e. g. from
                                         A+W Production, into consideration?
                                     •   Where do you define whether reserved stock products are withdrawn after
                                         delivery note printing or after invoice printing?
                                     •   What do you have to do to book stock products which belong to an item in
                                         the shape of BOM components, automatically on stock?
                                     •   What is the difference between the definition of stock sizes in dialog Master
                                         data > Products > Article > Stock sizes and in dialog Stockkeeping > Inven-
                                         tory management?
                                     •   What is displayed on the first two tabs in dialog Stock management > Stock
                                         management? Describe the differences!
                                     •   What is the difference between the booking journal and the stock history?
                                     •   What is the purpose of the Stock management > Stock P.O. dialog?
                                     •   What is the difference between a manual and an automatic stock P.O.?
6.1 / 04-2020




                A+W Business Inventory Management                                                             G-157
                Exercises                              Tutorial
6.1 / 04-2020




                G-158       A+W Business Inventory Management
Inventory Management          G

                Software Reference




                 A+W Business
                Software Reference                                                                     Overview




                                     Overview
                                     Use the module Stock Management to maintain and analyze all data concern-
                                     ing stock. Furthermore, use this module to carry out the inventory and book
                                     stock movements.
                                     The Software Reference provides information on the following subjects:
                                     •   “Inventory” on page G-166
                                     •   “Stock Management” on page G-184
                                     •   “Stock Movement” on page G-195
                                     •   “Queries” on page G-202
                                     •   “Search” on page G-217
                                     •   “Stock P.O.” on page G-220
                                     •   “Inventory Assessment” on page G-226
6.1 / 04-2020




                A+W Business Inventory Management                                                        G-165
                Inventory                                                               Software Reference




                            Inventory
                            Stock management > Inventory
                            Carry out inventory taking in individual steps by using the dialogs in the Inven-
                            tory menu: Create an inventory list, determine the target inventory, enter
                            counted quantities and finalize the inventory.
                            You will find the following program items in the Inventory menu:
                            •   Inventory List
                            •   Target Quantity
                            •   Inventory Management
                            •   Final Inventory

                            Additional information
                             Tutorial, “Periodical Inventory” on page G-138
                             Tutorial, “Initial Inventory” on page G-154
6.1 / 04-2020




                G-166                                               A+W Business Inventory Management
                Software Reference                                                                           Inventory




                                     Inventory List
                                     Stock management > Inventory > Inventory list

                                     Functions menu
                                     The old inventory list is deleted with the function Clear stock. At the same time,
                                     all products from the stock master data that do not have a stock code or that
                                     do not make any sense are deleted, e. g a product without reference to the
                                     storage location.

                                        This process may take quite a while
                                        Depending on the size of the database and the computer performance,
                                        clearing the stock may run for a longer period of time. It may even run for
                                        several hours. During this time, you cannot work with A+W Business.




                                     Fig. G-88    Inventory list


                                     The inventory list forms the basis for the actual inventory process. Select the
                                     criteria for which the list shall be created. Since you cannot carry out any
                                     changes to the stock during the counting process, it makes sense for large
                                     stock to take inventory in smaller units, e. g. by storage places.
                                      Tutorial, “Create Inventory List” on page G-141

                                        No changes to the product master data
                                        As soon as the inventory list has been created, all the products that are list-
                                        ed on the inventory list are marked in product management (master data).
6.1 / 04-2020




                                        The procurement type and stock code in these products are then blocked.
                                        As soon as the inventory has been completed, the marking is deleted and
                                        the data can be edited again.


                A+W Business Inventory Management                                                               G-167
                Inventory                                                                 Software Reference




                            Once the inventory list has been created, the target stock for the articles that
                            are listed on the inventory list can be determined.
                             Tutorial, “Inventory” on page G-137

                               Delete inventory list
                               Once you have completely finalized inventory taking, you should delete the
                               relevant inventory list. However, you are also able to delete any inventory
                               list at any time. The indicator Article is on the inventory list in the order and
                               the block in the product master data are then removed.

                            Parameters
                            The fields in this area are only released when you create a new inventory list.
                            You can have an inventory list displayed in the selection mode by using the
                            date.

                            Inventory date The inventory list is created at a certain date. All other inven-
                            tory processes will always refer to the inventory date. The current date is
                            shown automatically. It can be overwritten with the requested date, e. g. if you
                            are preparing for inventory taking that will take place at a later date.

                            All articles You can execute inventory taking for all articles that have been
                            entered as products in the master data.

                            Article number from ... to You can create the inventory list for a certain
                            range of article numbers by entering the corresponding numbers. These fields
                            are locked if the checkbox All articles is checked.

                            Inventory valuation
                            Choose an option to define how the inventory value for the inventory shall be
                            determined. The corresponding value is shown in the column PP/PU on the
                            inventory list. The value can be printed on the count list.
                            • PP price list:
                               The individual prices of the products from the PP rate assignment are used
                               for stock evaluation.
                            • Lowest PP:
                               For all articles, the lowest value is used for the inventory valuation each
                               time.
                            • Average PP:
                               For all articles, the average purchase price is used for the inventory valua-
                               tion each time. For this purpose, the option Average PP must be activated
                               in the company data.
                                Master Data, “Average PP: The average purchase price will be recalculated in
                                 the following cases:” on page B-955

                            Only products with stock on hand > 0 You can limit the inventory to the
                            stock articles with inventory.
                            ☐ The complete product master data including stock dimension table is includ-
6.1 / 04-2020




                            ed in the inventory list, insofar as this selection is not limited by other criteria.
                            ☑ Only the stock articles are taken over into the inventory list for which there
                            is inventory.


                G-168                                                A+W Business Inventory Management
                Software Reference                                                                             Inventory




                                     The Only products with assigned stock product and No box with ID and inven-
                                     tory = 0 check boxes are checked and locked.

                                     Only products with assigned stock product You can limit the inventory to
                                     the stock articles.
                                     ☐ The complete product master data including stock dimension table is includ-
                                     ed in the inventory list, insofar as this selection is not limited by other criteria.
                                     ☑ Only the stock articles are taken over into the inventory list that are created
                                     in the stock management.

                                     Only products with stock flag in products You can limit the inventory to
                                     the products with a stock flag.
                                     ☐ The complete product master data including stock dimension table is includ-
                                     ed in the inventory list, insofar as this selection is not limited by other criteria.
                                     ☑ Only items with the procurement type Stock removal will be included in the
                                     inventory list.
                                     The check box is checked and locked if the Only products with stock on hand
                                     > 0 check box is checked.

                                     No box with ID and inventory = 0 The stock on hand may include boxes
                                     that have already been delivered, but have not been deleted. Their stock is
                                     correctly displayed as 0.
                                     ☐ All boxes are listed on the inventory list.
                                     ☑ Boxes with an ID and an inventory = 0 are not included in the inventory list.
                                     The check box is checked and locked if the Only products with stock on hand
                                     > 0 check box is checked.

                                     Only for defined storage place You can limit the inventory to a storage
                                     place.
                                     ☐ Inventory is kept for all storage places. It is not limited to one storage place.
                                     ☑ The inventory is kept for a storage place. For determination of the storage
                                     place, the combo boxes Warehouse, Corridor, Shelf and Tray (levels 1 to 4)
                                     are enabled. This setting only makes sense if the inventories of your storage
                                     locations are checked in different periods.

                                        Storage location <n/a>
                                        Even if you have defined your own storage locations, storage locations <n/
                                        a> will remain and can be booked.

                                     Warehouse, Shelf, Corridor, Tray You can limit the Inventory list to a stor-
                                     age place. These fields are only enabled if the Only for defined storage place
                                     check box is checked.

                                     Sort by
                                     With the selection of this option, you specify the sorting for the inventory list.
                                     By default, the Articles option is activated.
6.1 / 04-2020




                A+W Business Inventory Management                                                                 G-169
                Inventory                                                                Software Reference




                            Overview
                            The overview lists all articles that should be counted in the inventory and
                            should be assessed.
                            •   Record no.:
                                Sequential number in the inventory list.
                            •   Art. no.:
                                Product number from the master data.
                            •   Name:
                                Product name from the master data.
                            •   Color:
                                The color is only specified if the product has been entered with variants/col-
                                ors.
                            •   Width, Height:
                                The dimensions are only displayed if the product is created as stock dimen-
                                sion or box with fixed dimensions. For all non-dimension-dependent prod-
                                ucts, the value 0 is displayed.
                            •   PP / PU:
                                Purchase price (PP) per price unit. Depending on the settings, this is the
                                lowest or the average PP.
                            •   PU:
                                Price unit of the purchase price.
                            •   PP / Sheet:
                                The purchase price per sheet is only displayed for stock dimensions. It is
                                calculated from the PP/PU and the actual size of the sheet. If a piece price
                                is stored, the values are identical in the PP/PU and PP/Sheet columns.
                            •   nominal:
                                The nominal inventory specifies what quantity is stored in A+W Business
                                according to the bookings made. It is only stored if the nominal inventory
                                was determined.
                                 “Target Quantity” on page G-173
                            •   QU:
                                Quantity unit with which the product is kept in stock.
6.1 / 04-2020




                G-170                                               A+W Business Inventory Management
                Software Reference                                                                          Inventory




                                     List Printing
                                     Stock management > Inventory > Inventory list > Print menu




                                     Fig. G-89     Print - Inventory list


                                     Use this dialog to set printing of the count lists. You can design the sheets ac-
                                     cording to manual stock entry and the inventory tasks of your employees.
                                      Tutorial, “How to print the count lists” on page G-144

                                        Target inventory in the count list
                                        The target inventory can only be printed on the count list if it has been de-
                                        termined prior to printing.

                                         “Target Quantity” on page G-173

                                     Page break after changing from

                                     Warehouse, Warehouse corridor, Warehouse shelf, Warehouse tray If
                                     you sort the count list by the storage location, you can also define after which
                                     storage levels a page break should be executed.
                                     This setting makes sense if you print the count list sorted by storage locations.
                                     You can then print an individual sheet for every level.
                                      “Sorted by” on page G-172

                                     Parameters
                                     Select an option to define which products shall be listed on the count list.
                                     The options Finished products and Raw material refer to the Raw material in-
                                     dicator according to the stock definition. If the Raw material indicator has not
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-171
                Inventory                                                                 Software Reference




                            been set, the system automatically takes the corresponding storage location
                            as the storage location for the finished products.
                             Master Data, “Stock Definition” on page B-736
                            •   All articles:
                                All articles from the inventory list are printed on the count list.
                            •   Finished products:
                                Only those articles from the inventory list, of which the storage location is
                                not intended for raw materials, are printed.
                            •   Raw material:
                                Only those products from the inventory list that are located at a storage lo-
                                cation for raw materials are printed.
                            •   Print prices:
                                The count list can be printed with or without prices.
                            •   Print target inventory:
                                The target inventory can only be printed on count lists if the target inventory
                                has been determined.

                            Sorted by Select an option to define how the articles shall be sorted on the
                            count list:
                            • Article:
                               The list is sorted by product numbers.
                            • Dimensions:
                               If the count list includes stock sizes, those entries will be printed sorted by
                               width/height.
                            • Storage location:
                               If the articles of the count list are stored at different storage locations sort-
                               ing by storage locations makes sense. In addition, you can define the page
                               feeds.
                                 “Page break after changing from” on page G-171

                            Print storage locations
                            All the storage locations that have been defined in the master data or that have
                            been selected for the inventory list are listed in the overview. You can deter-
                            mine whether the storage places should be printed on the count list. If you
                            want to print the storage places you must select at least one.

                                Storage location <n/a>
                                Even if you have defined your own storage locations, storage locations <n/
                                a> will remain and can be booked.
6.1 / 04-2020




                G-172                                                A+W Business Inventory Management
                Software Reference                                                                              Inventory




                                     Target Quantity
                                     Stock management > Inventory > Target quantity




                                     Fig. G-90     Target quantity


                                     The target quantity corresponds to the quantity that has been determined by
                                     the system resulting from automatic or manual bookings. It is determined each
                                     time for a certain inventory list or for all articles that are listed on the selected
                                     inventory list.
                                      Tutorial, “Determine Target Inventory” on page G-146

                                        No inventory change on the day of the count
                                        After the target quantity has been determined, the stock quantities must be
                                        counted. On the day of the count, no stock articles may be withdrawn and
                                        no stock movements may be booked until counting has been finalized.
                                        A+W Business is not automatically blocked for bookings.

                                     Parameters

                                     Inventory date All inventory lists that are stored in the system are listed in the
                                     combo box. You cannot determine from the date whether the inventory has
                                     been concluded.
6.1 / 04-2020




                A+W Business Inventory Management                                                                 G-173
                Inventory                                                             Software Reference




                            List
                            •   Record no.:
                                Sequential number on the inventory list.
                            •   Art. no.:
                                Product number according to the master data.
                            •   Name:
                                Product name from the master data.
                            •   ID:
                                Box ID (manual booking or from receipt of goods).
                            •   Contents:
                                Value 1 is shown for stock articles and stock sizes and the number of
                                sheets for boxes.
                            •   Width, Height:
                                Dimensions are only shown if the product has been defined as a stock size
                                or box.
                            •   Color:
                                The color is only specified if the product has been entered as a variant.
                            •   Storage location:
                                Storage location in the order of level 1 through 4.
                            •   PP / PU:
                                Purchase price (PP) per price unit. Depending on the settings, this is the
                                lowest or the average PP.
                            •   PU:
                                Price unit of the purchase price.
                            •   Cat.:
                                This function is used only for certain customers.
                            •   nominal:
                                Quantity that should be available according to the system. The values are
                                only shown if the target quantity has been determined.
                            •   QU:
                                Quantity unit with which the product is kept in stock.
6.1 / 04-2020




                G-174                                             A+W Business Inventory Management
                Software Reference                                                            Inventory Management




                                     Inventory Management
                                     Stock management > Inventory > Management
                                     Enter the counted quantities in the Inventory Management dialog. You can
                                     book stock again directly after counting.
                                     This chapter provides information on the following subjects:
                                     •   “Menus in Inventory Management” on page G-175
                                     •   “Management” on page G-176
                                     •   “Go to Product” on page G-179


                                     Menus in Inventory Management
                                     Stock management > Inventory > Management
                                     The inventory management menus allow you to define the default settings for
                                     the dialog and open other dialogs without having to close inventory manage-
                                     ment.
                                     This chapter provides information on the following subjects:
                                     •   “Options menu” on page G-175
                                     •   “Functions menu” on page G-176


                                     Options menu
                                     Stock management > Inventory > Management

                                     Stock size group
                                     •   Calculate stock size surface automatically:
                                         The surface of the counted stock plates is automatically shown in square
                                         meters.

                                     Sort group
                                     •   Article / Storage location / Size:
                                         The list is sorted by articles. This sorting makes sense if the same articles
                                         are stored at several different storage locations.
                                     •   Dimension / article / storage location:
                                         The list is sorted by sizes of the stock size. This type of sorting makes
                                         sense if you have entered the stock sizes in individual count lists.
                                     •   Storage location / Article / Dimension:
                                         The list is sorted by storage places. This type of sorting makes sense if you
                                         have also sorted the count lists by storage locations.
                                     •   Record no.:
                                         Record number from the inventory list
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-175
                Inventory Management                                                              Software Reference




                                       Functions menu
                                       Stock management > Inventory > Management
                                       The following entries are displayed:
                                       •   Go to article:
                                           Opens the Go to Article dialog.
                                            “Go to Product” on page G-179
                                       •   Change quantity for marked articles to zero:
                                           The quantity is changed to zero. This function is helpful if you are marking
                                           several documents. You do not need to change every single one to zero.
                                       •   Define storage location for tagged article:
                                           The storage location is changed for all tagged documents.


                                       Management
                                       Stock management > Inventory > Management




                                       Fig. G-91    Inventory management


                                       Use this dialog to enter counted quantities. The list shows the entries that you
                                       have selected with the inventory list. You can book stock again directly after
                                       counting.
                                        Tutorial, “Enter Counted Values” on page G-148
6.1 / 04-2020




                G-176                                                         A+W Business Inventory Management
                Software Reference                                                            Inventory Management




                                        Take inventory of boxes
                                        Once the target quantity for the inventory list has been created, boxes can
                                        also be entered by scanner and included on the inventory list. For this pur-
                                        pose, the box ID, storage location and any deviating sheet quantities must
                                        be scanned.

                                     Input screen

                                     Inventory date Enter the date of the inventory list.

                                     Article number Number of the article the quantity of which shall be entered.

                                     Width, Height The sizes are entered only for stock plates and boxes. For all
                                     other articles, both fields will show a zero (0).

                                     Category This function is used only for certain customers in order to use cat-
                                     egories for value correction of stock.

                                     Inv. price You can manually enter an inventory price for the inventory valua-
                                     tion. After completion of the inventory taking process, this price is not saved in
                                     the PP price table and is not included in the calculation of the average PP.
                                     If no inventory price is entered, depending on the inventory list settings, the
                                     lowest or the average PP applies.

                                     Content Shows the quantity of boxes. If boxes have been counted as a unit,
                                     a box make not be broken down, i. e. plates may not have been withdrawn.

                                     Name Article name from the product master data.

                                     Color For articles with color allocation (variant) you can enter the quantity per
                                     color.

                                     Ident Box ID (manual booking or from receipt of goods).

                                     Storage location Storage place of the counted article.

                                        Storage location <n.e.>
                                        Even if you have defined your own storage locations, storage locations
                                        <n.e.> will remain and can be booked.

                                     Quantity Enter the counted quantities from the count list in this field. You can
                                     only enter the quantities after you have determined the target quantity.
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-177
                Inventory Management                                                              Software Reference




                                       Table
                                       The overview lists all the articles that are to be counted and valuated.
                                       •   Record no.:
                                           Sequential number on the inventory list.
                                       •   Art. no.:
                                           Product number according to the master data.
                                       •   Name:
                                           Product name from the master data.
                                       •   Content:
                                           Value 1 is shown for stock articles and stock sizes and the number of
                                           sheets for boxes.
                                       •   ID:
                                           Box ID (manual booking or from receipt of goods).
                                       •   Width, Height:
                                           Dimensions are only shown if the product has been defined as a stock size
                                           or box.
                                       •   Storage location:
                                           Storage location in the order of level 1 through 4.
                                       •   PP / PU:
                                           Purchase price (PP) per price unit. Depending on the settings, this is the
                                           lowest or the average PP.
                                       •   PU:
                                           Price unit of the purchase price.
                                       •   Category.:
                                           This function is used only for certain customers.
                                       •   Quantity:
                                           Value that has been entered as the counted quantity.
                                       •   QU:
                                           Quantity unit with which the product is kept in stock.
6.1 / 04-2020




                G-178                                                         A+W Business Inventory Management
                Software Reference                                                           Inventory Management




                                     Go to Product
                                     Stock management > Inventory > Management > Functions menu > Go to ar-
                                     ticle...




                                     Fig. G-92    Go to article


                                     In this dialog you can set a marking for the first document relating to the spec-
                                     ified article.

                                     Articles Number of the stock article on the list which you would like to go to.


                                     Value Correction
                                     Stock management > Inventory > Management > Category field > Folder icon




                                     Fig. G-93    Value correction


                                     Use this dialog to define the categories and percentages for correcting the
                                     stock value.
                                     This dialog is enabled for individual customers only.
6.1 / 04-2020




                A+W Business Inventory Management                                                             G-179
                Final Inventory                                                                Software Reference




                                  Final Inventory
                                  Stock management > Inventory > Finalization
                                  You conclude inventory taking with the final inventory. You can book stock
                                  again directly after counting.
                                  This chapter provides information on the following subjects:
                                  •   “Menus in Final Inventory” on page G-180
                                  •   “Finalization” on page G-181


                                  Menus in Final Inventory
                                  Stock management > Inventory > Finalization
                                  The menus can be used to define the standard settings or open other dialogs
                                  without closing this dialog.
                                  This chapter provides information on the following subjects:
                                  •   “Options menu” on page G-180
                                  •   “Functions menu” on page G-180


                                  Options menu
                                  Stock management > Inventory > Finalization
                                  The following entries are displayed:
                                  •   Do not print articles with stock on hand = 0:
                                      Only articles with stock on hand that is more than 0 will be printed. This set-
                                      ting is helpful if you have many articles without stock figures. This makes
                                      the printed list clearer.
                                  •   Check whether the stock for uncounted articles shall be set to 0:
                                      Use this function to define that the quantity of articles for which no stock
                                      has been entered is only then set to 0 when you have confirmed this for
                                      each article.


                                  Functions menu
                                  Stock management > Inventory > Finalization
                                  The following entries are displayed:
                                  •   Add supplementary inventory:
                                      Opens the dialog Select inventory list in order to print and analyze two dif-
                                      ferent inventories in one joint list.
                                       “Select Inventory List” on page G-183
6.1 / 04-2020




                G-180                                                      A+W Business Inventory Management
                Software Reference                                                                      Final Inventory




                                     Finalization
                                     Stock management > Inventory > Finalization




                                     Fig. G-94    Final inventory


                                     Use this dialog to finalize the inventory for each inventory list. With it, the en-
                                     tered values are adopted in the stock on hand (stock lists). Any goods issued
                                     or received in the meantime are taken into account. New stock articles from
                                     the inventory are automatically adopted in inventory management.
                                      Tutorial, “Finalize Inventory” on page G-150

                                        Per inventory list only one final inventory
                                        The final inventory can only be executed once per inventory list. Any entry
                                        errors can only be corrected in inventory management after the final inven-
                                        tory. Alternatively, a new inventory list can be created with the incorrectly
                                        entered articles.
6.1 / 04-2020




                A+W Business Inventory Management                                                                G-181
                Final Inventory                                                              Software Reference




                                  Booking

                                  Inventory date Date of the inventory that is to be finalized.

                                  Book by supply type as per production preparation If you work with or-
                                  der areas, stock may be allocated for a certain production preparation, e. g. for
                                  the production of LAMI. The field for selecting the production preparation is en-
                                  abled only if you have checked the checkbox.
                                  ☐ The counted stock is allocated to the standard storage place.
                                  ☑ The stocks shall be allocated to a production preparation.
                                   Master Data, “Order Areas” on page B-1014

                                  Record no. from ... to Displays the first and last record number of the load-
                                  ed inventory list.

                                  Overview
                                  •   Record no.:
                                      Sequential number on the inventory list.
                                  •   Art. no.:
                                      Product number according to the master data.
                                  •   Name:
                                      Product name from the master data.
                                  •   Content:
                                      Value 1 is shown for stock articles and stock sizes and the number of
                                      sheets for boxes.
                                  •   ID:
                                      Box ID (manual booking or from receipt of goods).
                                  •   Width, Height:
                                      Dimensions are only shown if the product has been defined as a stock size
                                      or box.
                                  •   Storage location:
                                      Storage location in the order of level 1 through 4.
                                  •   Quantity:
                                      Value that has been entered as the counted quantity.
                                  •   QU:
                                      Quantity unit with which the product is kept in stock.
                                  •   Status:
                                      The status is only shown if the record could not be booked. Use the logbook
                                      to check for the possible causes.
6.1 / 04-2020




                G-182                                                    A+W Business Inventory Management
                Software Reference                                                                      Final Inventory




                                     Select Inventory List
                                     Stock management > Inventory > Finalization > Functions menu > Add sup-
                                     plementary inventory




                                     Fig. G-95    Add supplementary inventory


                                     A supplementary inventory can only be added if both inventories have been
                                     finalized. Both inventories can then be printed on a joint list and be analyzed.
                                      Tutorial, “How to add a supplementary inventory” on page G-152
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-183
                Stock Management                                                            Software Reference




                                   Stock Management
                                   Stock management > Stock management
                                   Use the dialog Stock management to display all the stock articles that are
                                   managed.
                                   This chapter provides information on the following subjects:
                                   •   “Menus in Stock Management” on page G-184
                                   •   “Stock Management” on page G-185


                                   Menus in Stock Management
                                   Stock management > Stock management
                                   The menus can be used to define the standard settings of the dialog or open
                                   other dialogs without closing this dialog.
                                   This chapter provides information on the following subjects:
                                   •   “Functions menu” on page G-184
                                   •   “Options menu” on page G-185
                                   •   “Print menu” on page G-185


                                   Functions menu
                                   Stock management > Stock management > Functions menu
                                   This menu allows you to open other dialogs without closing stock manage-
                                   ment.
                                   The following entries are displayed:
                                   •   Stock History:
                                       Opens the dialog Stock History with the log of processes that have been
                                       booked in stock management.
                                        “Stock History” on page G-204
                                   •   Booking Journal:
                                       Opens the dialog Booking Journal with the log of stock bookings from or-
                                       ders and purchase orders.
                                        “Booking Journal” on page G-202
6.1 / 04-2020




                G-184                                                      A+W Business Inventory Management
                Software Reference                                                                 Stock Management




                                     Options menu
                                     Stock management > Stock management > Options menu
                                     This menu allows you to define the default settings for this dialog. The options
                                     can be enabled or disabled. The settings will not be reset when you close the
                                     dialog.
                                     The following entries are displayed:
                                     •   Do not print articles with stock on hand = 0:
                                         Only articles with stock on hand that is more than 0 will be printed. This set-
                                         ting is helpful if you have many boxes with an ID, but without stock. Usually,
                                         these have been delivered as boxes and were deleted from the stock. This
                                         setting applies only to printing; the dialog shows all the articles.
                                     •   Automatic ID allocation:
                                         The box ID can be allocated automatically even it has been booked as
                                         stock manually.


                                     Print menu
                                     Stock management > Stock management > Print menu
                                     Use this menu to start the printout of labels.
                                     The following entries are displayed:
                                     •   Box labels:
                                         Only labels for boxes will be printed. For this, the print point 973 must be
                                         created and the report boxlabel.qrp assigned in the form management.
                                     •   Standard:
                                         Labels for stock articles will be printed.


                                     Stock Management
                                     Stock management > Stock management
                                     In the Stock Management dialog you enter all the stock articles that are kept
                                     in the warehouse with stock on hand.
                                     Stock sizes are maintained in A+W Business even in product management.
                                     They are used to allocate price codes, product groups, etc.
                                     Dialog Stock Management offers the following tabs:
                                     •   Stock Management - Stock Articles
                                     •   Stock Management - Prices
                                     •   Stock Management - Supplement
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-185
                Stock Management                                                                    Software Reference




                                            Stock management at the level of bills of material
                                            In the warehouse, you can also manage products that are included as bill
                                            of material components in other products. For this purpose, the checkbox
                                            Stock keeping at BOM level must be enabled in the company data.

                                             Tutorial, “Stock control on BOM level” on page G-58
                                             Master Data, “Stock control on BOM level” on page B-958


                                         Stock Management - Stock Articles
                                         Stock management > Stock management > Stock articles tab




                Fig. G-96   Stock Management - Stock Articles


                                         Use this tab to check the articles that are managed in the warehouse. The
                                         shown stock is updated with each stock booking. You can add new articles and
                                         correct the different quantities.
                                         For ordering purposes, you furthermore define minimum quantities and pur-
                                         chase order quantities.
                                          Tutorial, “How to create a stock article” on page G-71

                                         Identification

                                         Articles Product number according to master data. If you want to enter a new
                                         stock article, you have to enter it in the master data first.
6.1 / 04-2020




                                         Stock ID Identification number, assigned on receipt of goods.



                G-186                                                             A+W Business Inventory Management
                Software Reference                                                               Stock Management




                                     Name Product names from the master data.

                                     Width x height / content Dimensions of the stock article in mm (only stock
                                     sizes) and content of box. For boxes, enter the number of sheets per box. For
                                     all other stock articles, a 1 is automatically shown.

                                     Variation If variations have been entered for an article, you will see the color
                                     here.

                                     Default storage location If you have defined storage locations, they will be
                                     offered for selection.
                                     If you keep one stock article at several storage locations, you can define a
                                     standard storage location.
                                     ☐ The shown storage location is not defined as standard for the stock article.
                                     ☑ The shown storage location is defined as standard for the stock article.
                                      Master Data, “Stock Definition” on page B-736

                                        Storage location <n.e.>
                                        Even if you have defined your own storage locations, storage locations
                                        <n.e.> will remain and can be booked.

                                     ID The box ID, is assigned on receipt of goods or manually.
                                     The ID is only shown if you have selected a box in the overview of stock arti-
                                     cles.

                                     Details

                                     Category If you have defined stock categories in the master data, you can
                                     use this field as a search criterion. When you enter new stock articles you can
                                     allocate a category.

                                     Del. ID The supplier's box ID is only shown if you have selected a box in the
                                     Stock articles section.

                                     Main product You can link stock articles with several dimensions by speci-
                                     fying a main product. The stock check (for the stock preview in the Stock info
                                     dialog) is then only executed for the main product and you only need to enter
                                     minimum stock for this main product.
                                     If you have also defined minimum stock for the allocated stock articles, they
                                     will be ignored for the check.
                                      Tutorial, “Main Stock Products” on page G-67

                                     Prod. batch / date Currently not being used.

                                     Date Date at which the stock article has been changed last time.
6.1 / 04-2020




                A+W Business Inventory Management                                                             G-187
                Stock Management                                                               Software Reference




                                   In production In connection with A+W Production you can determine
                                   whether the stock article has been allocated to production.
                                   ☐ The stock article is disposable.
                                   ☑ The stock article has been allocated to production (info only).

                                   Inventories

                                   Stock on hand Displays the current stock. The stock is updated with each
                                   booking of outgoing or incoming stock. For boxes with an ID, stock 1 is always
                                   shown.
                                   If you have created the stock article new, the field is enabled and you can enter
                                   the opening stock.

                                   Stock > 0 This checkbox is only available in the selection mode. Use it to de-
                                   fine as a search criterion whether articles should be shown without stock quan-
                                   tity.
                                   ☐ The search result also shows articles, the current stock of which is 0.
                                   ☑ The search result only shows articles, the current stock of which is at least 1.

                                   Min. stock The minimum stock forms the basis for automatic purchase order
                                   suggestions. They are created if stock falls below the minimum stock. Reser-
                                   vations and purchase orders are taken into account. You can check these au-
                                   tomatic purchase order suggestions in the dialog Stock P.O..
                                    “Stock P.O.” on page G-220

                                   Minimum stock level > 0 This checkbox is only available in the selection
                                   mode. You can use it to define as a search criterion whether the minimum
                                   stock must be more than 0.
                                   ☐ The search result shows all articles.
                                   ☑ The search result only shows articles, the minimum stock of which is more
                                   than zero.

                                   Purch. qty. This value specifies which quantity is ordered by default. This
                                   value is adopted for automatic stock ordering.

                                   Inventory < Min. Inventory This checkbox is only available in the selection
                                   mode. You can use it to define as a search criterion whether the minimum
                                   stock must be below the minimum inventory.
                                   ☐ The search result shows all articles.
                                   ☑ The search result only shows articles, the current stock of which is less than
                                   the minimum inventory.

                                   Maximum stock level By entering maximum quantities per stock article you
                                   can prevent the warehouse becoming overstocked. The entered value is only
                                   used for the manual check.

                                   Target quantity Currently not being used.
6.1 / 04-2020




                                   Inventory audit per stock location If you maintain stock per storage loca-
                                   tion you can check the stock per stock location.
                                   ☐ Stock is checked jointly for all storage locations.


                G-188                                                      A+W Business Inventory Management
                Software Reference                                                                Stock Management




                                     ☑ Stock is checked per storage location.

                                     Critical stock on hand For each stock article, you can specify the quantity
                                     starting with which a P.O. is absolutely necessary.
                                     So that the value entered is checked, the Inventory check per storage location
                                     option must be activated.
                                     In the stock management, the date is calculated on which the inventory of a
                                     stock article drops below this critical quantity. The date on which the stock ar-
                                     ticle reaches the critical quantity is used in the PO pool.
                                      Sales, “Order Transfer – Order Pool” on page C-654

                                     Stock articles
                                     The lists show stock articles that correspond to the search criteria. The top list
                                     shows all stock articles together. If you select one entry, the articles are shown
                                     per storage location in the bottom list. If the checkbox Stock > 0 has been ac-
                                     tivated, only storage locations with stock of more than 0 are listed.
                                     The following columns are displayed:
                                     •   Articles, Variation:
                                         Article number, name, and color from stock management.
                                     •   Width, Height:
                                         Dimensions from stock management.
                                     •   Content:
                                         Number of sheets in one box.
                                     •   Total stock:
                                         Total stock of the stock article at all storage locations.
                                     •   Min. stock level:
                                         Quantity of the defined minimum stock level.
                                     •   Purch. quantity:
                                         Defined purchasing quantity.

                                     Storage locations
                                     •   ID:
                                         Box ID (manual booking or from receipt of goods).
                                     •   Storage location:
                                         Storage location in the order of level 1 through 4.
                                     •   Stock level:
                                         Current stock level at the storage place.
                                     •   Del. ID:
                                         Supplier's box ID (only if it has been entered at goods receipt).
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-189
                Stock Management                                                                      Software Reference




                                        Stock Management - Prices
                                        Stock management > Stock management > Prices tab




                Fig. G-97   Stock management - Prices


                                        This tab shows the current prices for a stock article. During updates, orders,
                                        purchase orders and stock rebookings are taken into account.
                                         Tutorial, “Prices” on page G-48

                                            Prerequisite
                                            The average purchase price (average PP) is only calculated and shown if
                                            the checkbox Determine purchase price and the option Average PP has
                                            been enabled in the company data.

                                             Master Data, “Average PP: The average purchase price will be recalculated in
                                              the following cases:” on page B-955
                                        The fields in the lists are described in detail in connection with the Stock Article
                                        tab.
                                         “Stock Management - Stock Articles” on page G-186

                                        Purchase prices

                                        Lowest price The lowest price this article has been purchased at.
6.1 / 04-2020




                                        Max. price The highest price this article has been purchased at.

                                        Last price The latest price this article has been purchased at.


                G-190                                                            A+W Business Inventory Management
                Software Reference                                                                 Stock Management




                                     Stock value The current stock prices are shown in this column. They are the
                                     result from the respective price and the quantity.

                                     Calculation of the average price (average PP)
                                     By selecting an option, determine which stock sizes should be taken into ac-
                                     count on this list for the calculation. This setting only makes sense for lite with
                                     different stock sizes.
                                     •   Only this article:
                                         For the calculation only the displayed article in the selected dimension is
                                         taken into account. The PP history of the current article is displayed.
                                     •   All sizes:
                                         For the calculation all dimensions of the displayed glass are taken into ac-
                                         count. The PP history of all dimensions of the article is displayed.
                                     The average PP is calculated for each goods receipt, regardless of how it has
                                     been booked. Goods issued only reduce the stock. The list is reduced by ar-
                                     chiving and auditing.
                                     The first data record shows the opening stock and the original price. Under-
                                     neath you will find the goods received and issued (minus sign). If goods have
                                     been received as a result of a stock P.O., the P.O. number and the P.O. item
                                     is furthermore displayed.
                                     The average PP is updated during entering or changing purchase orders. It is
                                     determined by taking the total quantity into account.

                                         Example:

                                         100 pieces      in stock                each 15.00 €              1500.00 €

                                          40 pieces      new booking             each 18.00 €     +         720.00 €

                                                                                                  =        2200.00 €
                                                                                                           ========
                                         2200.00/140 pcs. = 15.86 €



                                     Automatic surcharges that are listed in the purchase orders, e. g. energy and
                                     transportation surcharge, are also included in the calculation.
6.1 / 04-2020




                A+W Business Inventory Management                                                                G-191
                Stock Management                                                                 Software Reference




                                   Overview The respective average prices are shown as history. This way, you
                                   can easily monitor price developments. Details displayed:
                                   •   Date:
                                       Date of the last update.
                                   •   Quantity [QU]:
                                       Quantity issued or received and quantity unit.
                                   •   Price/[PU]:
                                       Purchase price per price unit at the time of booking.
                                   •   Stock on hand [QU]:
                                       Stock on hand at the displayed date. If the average PP is shown for all di-
                                       mensions, the stock on hand is always shown in sqm.
                                   •   Average price / [PU]:
                                       Average price per price unit at the time of booking.
                                   •   P.O. / item.:
                                       Number of the purchase order and P.O. item.
                                   •   Stock value:
                                       Stock value at the displayed date (calculation: purchase price * stock on
                                       hand).
                                   •   Type:
                                       Type of booking that has caused the respective entry.

                                   Include in total PCH You can determine whether the article should be in-
                                   cluded in the calculation of the total average price of all variations of this arti-
                                   cle.
                                   ☐ The article will not be considered for calculating the average price.
                                   ☑ The article will be included in the calculation.

                                   Average price Current average price. Depending on the option for calculat-
                                   ing the average PPs, the display for the current article or the display for all di-
                                   mensions of the article applies.

                                       Updating the display
                                       The display of the average prices is updated for the respective stock article
                                       during archiving or auditing (invoice check). As a result, the display re-
                                       mains clearer.
                                       A+W Business assumes that the prices will not be changed anymore after
                                       these processes. However, if you still change prices after one of the pro-
                                       cesses, these changes are not included in the calculation of the average
                                       price.
6.1 / 04-2020




                G-192                                                       A+W Business Inventory Management
                Software Reference                                                                      Stock Management




                                         Stock Management - Supplement
                                         Stock management > Stock management > Supplement tab




                Fig. G-98   Stock management - table


                                         On this tab reservations for a selected stock article are shown.
                                         The fields in the lists are described in detail in connection with the Stock Article
                                         tab.
                                          “Stock Management - Stock Articles” on page G-186

                                         Reservation
                                         The fields in this area are enabled for individual customers only.

                                         Customer Number and name of customer for whom the selected stock arti-
                                         cle is reserved.

                                         Fully locked Currently not being used.

                                         Exclusive reservation Currently not being used.

                                         Supplier

                                         Supplier Number and name of supplier from whom the stock article is or-
                                         dered.
6.1 / 04-2020




                A+W Business Inventory Management                                                                    G-193
                Stock Management                                                            Software Reference




                                   Remark

                                   Product related, Storage location related You can enter additional infor-
                                   mation for each stock article and each storage location, e. g. when and from
                                   which supplier glass/boxes were supplied, so that older deliveries are used
                                   first.
6.1 / 04-2020




                G-194                                                   A+W Business Inventory Management
                Software Reference                                                                  Stock Movement




                                     Stock Movement
                                     Stock management > Stock movement
                                     You can manually book withdrawals and additions for stock articles, correct
                                     stock figures, rebook storage locations and resolve boxes.
                                     This chapter provides information on the following subjects:
                                     •   “Options Menu” on page G-195
                                     •   “Stock Movement” on page G-195


                                     Options Menu
                                     Stock management > Stock movement
                                     The following entries are displayed:
                                     •   Protocol at shut down:
                                         When exiting the dialog, the stock history is automatically shown.
                                          “Stock History” on page G-204
                                     •   Stock > 0:
                                         Only stock articles with a stock on hand of over 0 will be shown.


                                     Stock Movement
                                     Stock management > Stock movement
                                     Additions and dispatches of stock articles are automatically booked: for receipt
                                     of goods by delivery and for goods issued by orders. You can manually book
                                     additions or dispatches in the Stock Movement dialog, e. g to correct stock
                                     quantities.
                                     Dialog Stock Movement offers the following tabs:
                                     •   Stock Movement – Dispatch, Addition
                                     •   Stock Movement – Transfer
                                     •   Stock movement – Number of Sheets
                                     •   Stock Movement – Open Boxes
6.1 / 04-2020




                A+W Business Inventory Management                                                             G-195
                Stock Movement                                                               Software Reference




                                 Stock Movement – Dispatch, Addition
                                 Stock management > Stock movement > Dispatch tab, Addition tab




                                 Fig. G-99    Stock Movement – Dispatch, Addition


                                 You can manually book goods issued and received on the Dispatch and Addi-
                                 tion tabs. You can select a certain stock article and enter the corresponding
                                 data. If you have all stock articles displayed you can select the requested arti-
                                 cle on the Storage places list. The fields in the Change stock on hand section
                                 are then enabled.
                                  Tutorial, “Withdrawals and Additions” on page G-77
                                 If you have activated the option Protocol at shut down, the stock history is au-
                                 tomatically shown on the Table tab when you close the dialog.
                                  “Stock History – Table” on page G-208

                                    Manually enter addition of boxes
                                    Since every box is kept with its own ID, you can enter additions of boxes
                                    only via Goods Receipt or Stock Management. This process is explained in
                                    Box Management section.
6.1 / 04-2020




                G-196                                                      A+W Business Inventory Management
                Software Reference                                                                  Stock Movement




                                     Stock product

                                     Product Number and name of the stock article.

                                     ID no. You can only book stock dispatches via the ID no. Additions of boxes
                                     must be defined in Stock Management so that you can enter a new ID.

                                     Contents If you have selected a box, then its content is displayed. If a box
                                     with an ID no. that has already been allocated to an order is to be delivered or
                                     opened, a message is displayed. This prevents negative stock being created
                                     by the subsequent printing of the delivery note or invoice.

                                     Storage location Storage location that the stock article has been allocated
                                     to.

                                         Storage location <n.e.>
                                         Even if you have defined your own storage locations, storage locations
                                         <n.e.> will remain and can be booked.

                                     Average purch. price The average purchase price is only shown if the func-
                                     tion has been activated in the master data.
                                      Master Data, “Calculate purchase price” on page B-955

                                     Change stock on hand

                                     Quantity Enter the quantity that is to be booked out or in to stocks in pieces.
                                     If you go below the minimum stock when booking articles out of stock, a warn-
                                     ing message is displayed.

                                     Width / Height These fields are only filled with quantity unit sqm if it involves
                                     stock sizes.

                                     Assessment price Enter the purchase price at which the goods received
                                     were supplied.

                                     Booking date The current date is shown automatically. It can be changed if
                                     required.

                                     Remark You can enter a remark or select from the combo box. The remark
                                     will be displayed in the stock history.
                                      “Stock History – Table” on page G-208
                                     Use the button to add a new remark to the list.
                                      “Remark (Stock Movement)” on page G-201

                                     Storage locations
                                     •   Color:
                                         The color is only shown for variations.
                                     •   Width, Height:
6.1 / 04-2020




                                         Dimensions are only shown if the product has been defined as a stock size
                                         or box.



                A+W Business Inventory Management                                                              G-197
                Stock Movement                                                                 Software Reference




                                 •   Content:
                                     Value 1 is shown for stock articles and stock sizes and the number of
                                     sheets for boxes.
                                 •   Storage location:
                                     Storage location in the order of level 1 through 4.
                                 •   ID no.:
                                     Box ID (manual booking or from goods receipt).
                                 •   Stock on hand:
                                     Current stock
                                 •   QU:
                                     Quantity unit with which the product is kept in stock.
                                 •   Del. ID:
                                     Supplier's box ID.


                                 Stock Movement – Transfer
                                 Stock management > Stock movement > Transfer tab




                                 Fig. G-100    Stock movement – Transfer


                                 Use this tab to book a stock article to a different storage location. When you
                                 transfer a storage location, the entire stock of this storage location is always
                                 booked to the other storage location.
                                  Tutorial, “How to transfer the storage location” on page G-82
                                 The fields in sections Stock product and Storage locations are described under
                                 tab Dispatch.
6.1 / 04-2020




                                  “Stock Movement – Dispatch, Addition” on page G-196




                G-198                                                      A+W Business Inventory Management
                Software Reference                                                                    Stock Movement




                                     Storage location

                                     Storage location Displays the current storage place. You can allocate a dif-
                                     ferent storage place. The combo box lists all stored storage places.

                                        Storage location <n.e.>
                                        Even if you have defined your own storage locations, storage locations
                                        <n.e.> will remain and can be booked.


                                     Stock movement – Number of Sheets
                                     Stock management > Stock movement > No. of sheets tab




                                     Fig. G-101   Stock movement – Number of sheets


                                     Use this tab to correct the content of boxes.
                                      Kistenmanagement, “Kisteninhalt korrigieren (Blattanzahl)” auf Seite K-66
                                     The fields in sections Stock product and Storage locations are described under
                                     tab Dispatch.
                                      “Stock Movement – Dispatch, Addition” on page G-196

                                     Content change

                                     Contents The number of sheets that are supposed to be included in a box is
                                     only shown if you have selected a box with an ID no. You can correct this entry.
6.1 / 04-2020




                A+W Business Inventory Management                                                                  G-199
                Stock Movement                                                               Software Reference




                                 Stock Movement – Open Boxes
                                 Stock management > Stock movement > Open boxes tab




                                 Fig. G-102   Stock movement – Open boxes


                                 Use this tab to resolve boxes so that the individual sheets are available for pro-
                                 duction. During this process, the box is booked out of the inventory and the
                                 number of sheets is booked to the inventory of the stock size.
                                  Kistenmanagement, “Kisten aufbrechen (auflösen)” auf Seite K-67

                                    Book box content to a different storage location
                                    When you open a box, its content is booked to the same storage location
                                    of where the box is located. If you want to transfer the content, you must
                                    book it out of the previous storage location and subsequently, book it to the
                                    new storage location.

                                 The fields in sections Stock product and Storage locations are described under
                                 tab Dispatch.
                                  “Stock Movement – Dispatch, Addition” on page G-196

                                 Open box
                                 If a box with an ID no. that has already been allocated to an order is to be de-
                                 livered or opened, a message is displayed. This prevents that negative stock
                                 is created by the subsequent printing of the delivery note or invoice.

                                 No. of boxes Number of boxes that are to be opened.
6.1 / 04-2020




                                 Different contents The number of sheets is shown only if you have selected
                                 a box. You can correct this value.


                G-200                                                    A+W Business Inventory Management
                Software Reference                                                                 Stock Movement




                                     Remark (Stock Movement)
                                     Stock management > Stock Movement > [Remark]




                                     Fig. G-103   Remark concerning stock movement


                                     Use this dialog to store remarks that are offered for selection in the Stock
                                     movement dialog. If you leave the first line blank you can also delete an allo-
                                     cated remark.
6.1 / 04-2020




                A+W Business Inventory Management                                                            G-201
                Queries                                                                                Software Reference




                                          Queries
                                          Stock management > Queries
                                          Use the different queries to get a quick overview of stock on hand, movements
                                          and values in your stock.
                                          This chapter provides information on the following subjects:
                                          •    “Booking Journal” on page G-202
                                          •    “Stock History” on page G-204
                                          •    “Stock Statistics” on page G-209
                                          •    “Reserved Stock Products” on page G-215


                                          Booking Journal
                                          Stock management > Queries > Booking journal




                Fig. G-104   Booking Journal


                                          In this dialog you can select the criteria for the query. In the booking journal,
                                          all automatic order or purchase order processes that relate to the stock are
                                          logged, e. g. reservations, purchase orders, additions and dispatches.
                                           Tutorial, “Show Booking Journal” on page G-87
6.1 / 04-2020




                G-202                                                             A+W Business Inventory Management
                Software Reference                                                                           Queries




                                     Selection

                                     Booking type You can search the stock for the following booking types:
                                     • (No entry):
                                       If you do not enter any booking type, all articles are shown.
                                     • Reserved:
                                       Only the reserved articles are shown. An article remains reserved until the
                                       delivery note or invoice has been printed.
                                     • Delivered:
                                       Only delivered stock articles are shown. An article is marked as delivered
                                       after the delivery note or invoice has been printed.
                                     • Ordered:
                                       Only ordered stock articles are shown. The indicator is set as a result of a
                                       stock P.O.
                                     • Received:
                                       Only delivered stock articles are shown. An article is considered delivered
                                       or received once it has been booked in goods receipt.

                                     Booking date from ... to You can restrict the search to a date or time period
                                     during which the articles were booked in the stock. When you select the date,
                                     pay attention to the time at which the booking was executed.
                                     If you have not restricted the display any further, all bookings during the spec-
                                     ified time period are displayed.

                                     Storing place You can restrict the search to a storage place.

                                         Storage location <n.e.>
                                         Even if you have defined your own storage locations, storage locations
                                         <n.e.> will remain and can be booked.

                                     ID no. You can restrict the search to a box ID.

                                     Select by Choose an option to define what the search should refer to:
                                     • Articles:
                                        You can search for one or several articles. The entry in the fields Number
                                        from and to refers to the product numbers. If you have not selected a book-
                                        ing type, all booking types will be listed.
                                     • Order:
                                        You can search for articles that are included in orders. The entry in the
                                        fields Number from and to refers to the order numbers.

                                     Number from, to The search can be restricted to one number or a sequence
                                     of numbers.

                                     Table
                                     The result of the search is displayed on the list.
                                     •   Res. type:
6.1 / 04-2020




                                         Booking type in which the product has been booked.




                A+W Business Inventory Management                                                             G-203
                Queries                                                                Software Reference




                          •   Order No./P.O. No..:
                              Number of the order or purchase order from which the booking has been
                              created.
                          •   Item No..:
                              Number of the order or purchase order item.
                          •   Qty:
                              Item quantity.
                          •   Product, Name:
                              Product number and name as per master data.
                          •   Color:
                              The color is only shown for variations.
                          •   Width, Height:
                              Dimensions of the item.
                          •   ID:
                              Box ID (manual booking or from receipt of goods). If the entry is not a box,
                              a zero is displayed.
                          •   Del. ID:
                              Supplier's box ID.
                          •   Storage location:
                              Location at which the product has been booked out or in.
                          •   Booking date:
                              Date of goods receipt.
                          •   PP:
                              Purchasing price of item. Any change of the purchase price at the receipt
                              of goods, check of the delivery OC or invoice is updated in the P.O.


                          Stock History
                          Stock management > Queries > Stock history
                          In the stock history, all processes that refer to the stock are logged. In addition
                          to the booking types, this includes e. g. cut stock plates, corrections, new arti-
                          cles.
                          The Stock history dialog offers the following tabs:
                          •   Stock History – Selection
                          •   Stock History – Table
6.1 / 04-2020




                G-204                                             A+W Business Inventory Management
                Software Reference                                                                                 Queries




                                           Stock History – Selection
                                           Stock management > Queries > Stock history > Selection tab




                Fig. G-105   Stock history – Selection


                                           Select the criteria for the query on this tab. The result is automatically shown
                                           on the Table tab.
                                            Tutorial, “Show Booking Journal” on page G-87

                                           Booking type
                                           You can search the stock for the following booking types:
                                           •   (No entry):
                                               If you do not enter any booking type, all articles are shown.
                                           •   Reserved:
                                               Only the reserved articles are shown. An article remains reserved until the
                                               delivery note or invoice has been printed.
                                           •   Delivered:
                                               Only delivered stock articles are shown. An article is marked as delivered
                                               after the delivery note or invoice has been printed.
                                           •   Cut SS:
                                               This booking type is used by the A+W Optimizer report if an item has been
                                               cut from a stock size. The number of stock plates is analyzed.
                                           •   Ordered:
                                               Only ordered stock articles are shown. The indicator is set as a result of a
6.1 / 04-2020




                                               stock P.O.




                A+W Business Inventory Management                                                                   G-205
                Queries                                                                 Software Reference




                          •   Received:
                              Only delivered stock articles are shown. An article is considered delivered
                              or received once it has been booked in goods receipt.
                          •   Manual stock addition/stock dispatch:
                              Only manually booked stock additions or stock dispatches are displayed.
                          •   Stock transfer:
                              Only stock transfers are shown.
                          •   New entry:
                              Displays only articles that have been newly entered for the stock. The data
                              may have been created within the scope of an inventory or manually. All
                              new articles as of the last archiving process are included.
                          •   Correction:
                              Displays only articles the stock of which has been edited during inventory
                              taking. All corrections as of the last archiving process are included.
                          •   Transfer to Recycle Bin, Book back from Recycle Bin, Deleted from stock:
                              Internal booking types.

                          Program
                          You can restrict the search to articles that have been processed in a certain
                          dialog of stock management, e. g. Stock transfers.

                          Remarks
                          You can restrict the search to articles for which a certain remark has been
                          stored. The remark will be displayed underneath the input field.

                          Article/order no.
                          By selecting an option, you restrict the search to certain articles or orders:
                          •   By product from … to:
                              You can select one or several articles.
                          •   By document no. from … to:
                              You can select one or several orders or purchase orders.

                              Show daily activities
                              If you enter the same article or order number in both fields, all the activities
                              will be displayed that have been booked for an article or order during a cer-
                              tain time period. For this purpose, also enter the booking time.
6.1 / 04-2020




                G-206                                              A+W Business Inventory Management
                Software Reference                                                                         Queries




                                     Stock ID/serial no.

                                     Stock ID from ... to You can choose one or several stock IDs.

                                     ID No. / Del. ID from ... to You can choose one or several IDs. The ID no. re-
                                     fers to the box and the Del. ID to the supplier's box ID.

                                     Storage locations
                                     You can restrict the search to stock articles that have been transferred from
                                     one particular storage location to a different one.

                                     From storage location Displays only articles that have been booked out of
                                     the selected storage location and booked in to a selected storage location.

                                     To storage location Displays only articles that have been booked in to the
                                     selected storage location and booked out from a selected storage location.

                                     Employee/booking date

                                     Employee You can restrict the search to articles that have been processed
                                     by the selected employee.

                                     Booking date from ... to You can restrict the search to a booking time peri-
                                     od. Ensure that you also enter the time.
6.1 / 04-2020




                A+W Business Inventory Management                                                           G-207
                Queries                                                                            Software Reference




                                           Stock History – Table
                                           Stock management > Queries > Stock history > Table tab




                Fig. G-106   Stock history – Table


                                           The result of the query is displayed on this tab.

                                           Table
                                           •   Res. type:
                                               Booking type in which the product has been booked.
                                           •   Order/P.O. No..:
                                               Number of the order/purchase order and item from which the booking has
                                               been created.
                                           •   Qty:
                                               Item quantity.
                                           •   ID, Del. ID:
                                               Box ID (manual booking or from receipt of goods) and supplier's box ID.
                                           •   Product, Name:
                                               Product number and name as per master data.
                                           •   Color:
                                               The color is only shown for variations.
                                           •   Width, Height:
                                               Dimensions of the item.
                                           •   Contents:
6.1 / 04-2020




                                               Number of sheets in the case of boxes.
                                           •   PP / PU:
                                               Purchase price per price unit.


                G-208                                                             A+W Business Inventory Management
                Software Reference                                                                           Queries




                                     •   Total PP:
                                         Purchasing price of item.
                                     •   PU:
                                         Price unit of total PP.
                                     •   QU:
                                         Quantity unit of the item.
                                     •   Booking date:
                                         Booking date and time.
                                     •   Execution date:
                                         Date and time at which the process has been booked.
                                     •   From storage location, To storage location:
                                         Previous and new storage location for transfers.
                                     •   Employee, Program:
                                         Name of the employee who has booked the process and name of the dialog
                                         in which the booking was carried out.
                                     •   Remarks:
                                         For certain booking types, a remark is displayed, e. g. which corrections
                                         were carried out during inventory taking.


                                     Stock Statistics
                                     Stock management > Queries > Stock statistics
                                     Stock statistics inform you which ones of your stock articles are hits and which
                                     ones are slow sellers. The analyses show initial and end stocks and additions
                                     and dispatches of your stock articles per month. This will provide you with in-
                                     formation about the stock turnover, average storage duration and average
                                     stock on hand of your products.
                                     The Inventory statistics dialog includes the following tabs:
                                     •   Stock Statistics - Products
                                     •   Stock Statistics – Statistics
                                     •   Stock Statistics – FIFO/LIFO
6.1 / 04-2020




                A+W Business Inventory Management                                                             G-209
                Queries                                                                                   Software Reference




                                           Stock Statistics - Products
                                           Stock management > Queries > Stock statistics > Products tab




                Fig. G-107   Stock statistics - Products


                                           Define on this tab the criteria for the statistical analysis. If you mark an entry in
                                           the hit list, the corresponding details are displayed on the Statistics tab.
                                            Tutorial, “How to display the inventory statistics” on page G-91

                                           Selection

                                           Year Select the year from which data shall be analyzed. You can use it to
                                           compare one particular time period with the same time period in the previous
                                           year.

                                           Month from ... to The selection of the month always refers to the set year. If
                                           you want to analyze more than one year you must split the analysis. If you re-
                                           quire an analysis that stretches over the turn of the year, you must carry out
                                           two analyses consecutively.

                                           Product from ... to Select a product or a sequence of products. For each
                                           product number, all related stock articles are analyzed, e. g. all the stock sizes,
                                           boxes, storage places, etc. for product Float 4 mm.
6.1 / 04-2020




                G-210                                                                A+W Business Inventory Management
                Software Reference                                                                             Queries




                                     Overview
                                     The overview shows all stock articles matching the search criteria. If you mark
                                     an entry of the hit list, the corresponding details are displayed on the Statistics
                                     tab.
                                     •   Product:
                                         Product number according to the master data.
                                     •   Name:
                                         Name defined in the master data.
                                     •   Width, Height:
                                         Dimensions for stored stock sizes.
                                     •   Content:
                                         Number of sheets in a box.
                                     •   ID:
                                         Box ID (manual booking or from receipt of goods).
                                     •   Color:
                                         Only for variants that are kept on stock.
                                     •   Storage location:
                                         Storage location of stock article.

                                         Storage location <n.e.>
                                         Even if you have defined your own storage locations, storage locations
                                         <n.e.> will remain and can be booked.
6.1 / 04-2020




                A+W Business Inventory Management                                                                G-211
                Queries                                                                                 Software Reference




                                            Stock Statistics – Statistics
                                            Stock management > Queries > Stock statistics > Statistics tab




                Fig. G-108   Stock statistics – Statistics


                                            On this tab, details are shown for the entry that has been marked on the hit list
                                            on the Product tab.

                                            Stock article
                                            The data of the selected stock article is shown in this section.

                                            Product Product number and name according to the master data.

                                            Width / height Dimensions for stored stock sizes.

                                            Storage location Storage location of stock article.

                                            PP Average purchase price and quantity unit.

                                            Content Number of sheets in a box.
6.1 / 04-2020




                G-212                                                               A+W Business Inventory Management
                Software Reference                                                                          Queries




                                     Overview
                                     The overview displays the statistical values for the stock article per month.
                                     •   Month:
                                         Depending on the selection, individual months or the entire year are/is dis-
                                         played.
                                     •   Opening stock:
                                         The closing stock of the previous month is used as the opening stock.
                                     •   Addition:
                                         Total of all additions within the month.
                                         Additions are for example newly created stock articles, manual additions in
                                         stock movement and/or goods received from Purchasing.
                                     •   Dispatch:
                                         Total of all dispatches within the month.
                                         Dispatches are either automatically booked when the delivery note or in-
                                         voice is printed or in the form of manual stock movement.
                                     •   Closing stock:
                                         Calculation: opening stock + addition - dispatch (within a month).
                                     •   Stock turnover:
                                         Calculation: Stock dispatch ÷ average stock on hand
                                         The higher the value, the lower the storage time for products.
                                     •   Average time in storage (in days):
                                         Calculation: days of settlement period ÷ stock turnover
                                         Number of days required to reduce the current closing stock based on the
                                         current dispatch.
                                     •   Average stock on hand:
                                         Calculation: (opening stock + closing stock) ÷ 2.
                                     •   Initial value/Addition value/Dispatch value/End value:
                                         The stock values are determined on the basis of the purchase price.
                                     •   Sum of stock on hand:
                                         Calculation: (opening stock + (n * closing stock) / (n + 1), n = number of
                                         months.
6.1 / 04-2020




                A+W Business Inventory Management                                                            G-213
                Queries                                                                               Software Reference




                                           Stock Statistics – FIFO/LIFO
                                           Stock management > Queries > Stock Statistics > FIFO/LIFO tab




                Fig. G-109   Stock statistics – FIFO/LIFO


                                           On this tab, the articles kept in stock are displayed assessed according to the
                                           FIFO and/or LIFO process. You can select the desired display on the Options
                                           > Initial assessment by menu.
                                           The data is only displayed if you have started an assessment of the stock val-
                                           ues on the Stock assessment dialog.
                                            “Inventory Assessment” on page G-227

                                           Overview
                                           The overview displays the statistical values for the stock article per month.
                                           •   Date:
                                               Date of the assessment or the inventory.
                                           •   Receipt:
                                               Total of all receipts in the selected assessment period.
                                           •   QU:
                                               Quantity unit of the stock article.
                                           •   Price, PU:
                                               Price and price unit
                                           •   Residue qty FIFO:
6.1 / 04-2020




                                               Remaining quantity after the calculation.
                                           •   Price FIFO:
                                               Price of the remaining quantity after the FIFO calculation.


                G-214                                                             A+W Business Inventory Management
                Software Reference                                                                               Queries




                                     •   Residue qty LIFO:
                                         Remaining quantity after the calculation.
                                     •   Price LIFO:
                                         Price of the remaining quantity after the LIFO calculation.
                                     There is a calculation example in the Stock assessment section:
                                      “Inventory Assessment” on page G-226



                                     Reserved Stock Products
                                     Stock management > Queries > Reserved stock products




                                     Fig. G-110    Reserved stock products


                                     Use this dialog to display the orders of a Number Manager to check which
                                     stock articles have been reserved. The reserved articles are listed on the print-
                                     out.
                                      Tutorial, “Stock Control Mode and Reservation” on page G-28
                                      Tutorial, “How to print a list of reserved stock articles” on page G-89

                                     Selection

                                     Employee Name of the logged-in employee.

                                     Number Manager Choose the Number Manager, the orders of which shall
                                     be analyzed.
6.1 / 04-2020




                A+W Business Inventory Management                                                                G-215
                Queries                                                                 Software Reference




                          Table
                          •   Number:
                              Order number.
                          •   Number Cust./Suppl.:
                              Customer number.
                          •   Customer/Supplier:
                              Name of customer or supplier.
                          •   Status:
                              Status of the order.
                          •   Date Entry:
                              Date on which the order was entered.
                          •   Date Delivery:
                              Date when the order shall be delivered.
                          •   Date OC:
                              Date of the supplier's order confirmation
                          •   Lock code:
                              Lock code from the order.

                          Printed list




                          Fig. G-111   Reserved stock articles - output on the screen
6.1 / 04-2020




                          The reserved stock articles are listed per article number and storage place. If
                          there are several storage places the total amount is displayed.


                G-216                                             A+W Business Inventory Management
                Software Reference                                                                               Search




                                          Search
                                          Stock management > Search
                                          You can retrieve the stock on hand by individual stock articles or by product
                                          groups.

                                              Set filter
                                              If no filter is set, no data will be displayed.

                                          The dialog is described in detail in the Sales part.
                                           Sales, “Stock Info” on page C-736
                                          Dialog Stock search offers the following tabs:
                                          •   Stock Search – Stock Search
                                          •   Stock Search - Future Stock on Hand


                                          Stock Search – Stock Search
                                          Stock management > Search > Stock search tab




                Fig. G-112   Stock search – Stock search
6.1 / 04-2020




                A+W Business Inventory Management                                                                G-217
                Search                                                                                 Software Reference




                                          Use this tab to display the current stock on hand, reserved quantities and fu-
                                          ture stock on hand for stock articles.
                                           Tutorial, “Stock Control Mode and Reservation” on page G-28
                                           Tutorial, “Show Stock on Hand in Stock Search” on page G-98


                                          Stock Search - Future Stock on Hand
                                          Stock management > Search > Future stock on hand tab




                Fig. G-113   Stock search - Future stock on hand


                                          Use this tab to check whether the replacement times for a certain product are
                                          sufficient to delivery an order in accordance with the schedule. The color red
                                          shows that scheduled dates cannot be met. Yellow indicates that the replace-
                                          ment time is sufficient if the purchase orders are received on time.
                                           Tutorial, “Stock Information and Future Stock on Hand” on page G-96
                                          The replacement time results from the delivery time that has been defined in
                                          the supplier file for the article and the supplier's route days that are defined in
                                          route management.
6.1 / 04-2020




                G-218                                                              A+W Business Inventory Management
                Software Reference                                                                            Search




                                     In order to increase the performance you can restrict the preview display by
                                     the following settings:
                                     •   You can remove certain articles from the stock preview and availability
                                         check in dialog Product management > Stock/Purchasing > No availability
                                         check checkbox, by disabling the availability check for these articles.
                                     •   In the Company data dialog you can set the time period displayed in the
                                         preview.
                                          Tutorial, “Checking the setting” on page G-61
                                     •   You can link several stock sizes together in the dialog Stock management
                                         so that the stock check is only executed for the defined main stock article.
                                          “Main product” on page G-187
6.1 / 04-2020




                A+W Business Inventory Management                                                             G-219
                Stock P.O.                                                              Software Reference




                             Stock P.O.
                             Stock management > Stock P.O.
                             Use this dialog to check all suggested stock P.O.s and transfer them to Pur-
                             chasing.
                             This chapter provides information on the following subjects:
                             •   “Order Pool Menus” on page G-220
                             •   “Order Pool” on page G-223


                             Order Pool Menus
                             By using the menus you can have the date fields updated automatically and
                             open other dialogs additionally.
                             This chapter provides information on the following subjects:
                             •   “Functions Menu” on page G-220
                             •   “Options Menu” on page G-221


                             Functions Menu
                             Stock management > Stock P.O. > Functions menu
                             This menu can be used to open other dialogs without closing the P.O. transfer.
                             The following entries are displayed:
                             •   Change supplier/delivery date:
                                 Opens the dialog Change supplier and delivery date.
                                  “Change Supplier and Delivery Dates” on page C-657
                             •   Marking options:
                                 Opens dialog Marking options.
                                  “Marking Options” on page C-658
                             •   Supplier prices:
                                 Opens dialog Price comparison.
                                  “Price Comparison” on page C-659
6.1 / 04-2020




                G-220                                                A+W Business Inventory Management
                Software Reference                                                                          Stock P.O.




                                     Options Menu
                                     Stock management > Stock P.O. > Options menu
                                     This menu allows you to define the default settings for this dialog. The options
                                     can be enabled or disabled. The settings will not be reset when you close the
                                     dialog.

                                         Activated options after opening the dialog
                                         Please note that changed options will only become effective the next time
                                         you open the dialog.
                                         If an activated option has started a check, opening the document can be
                                         delayed. The extent of the delay depends on the performance of the com-
                                         puter.
                                         Activated options are described in the following.

                                     Transfer group
                                     •   Order-related transfer:
                                         Purchase orders are transferred by order. Collective P.O.s can be created
                                         if this option is disabled.
                                     •   P.O. number = order number:
                                         This option is only available if the option Order-related transfer has been
                                         enabled.
                                     •   Order pool by user:
                                         You can create separate order pools for every user.

                                     Delivery date group
                                     •   Check delivery date:
                                         The delivery date is checked automatically. The system will inform you if
                                         you have changed a delivery date to a date which is not a route day.
                                     •   Consider supplier's route:
                                         If the delivery date for the P.O. is not a route day, a message to that effect
                                         will be issued. This requires that supplier's routes have been defined in the
                                         master data.
                                          Master Data, “Routes” on page B-861
                                     •   Determine lead days based on PGR combinations:
                                         If lead days have been defined for PGR combinations, these shall be used
                                         to calculate the delivery date.
                                          Master Data, “Lead days” on page B-567
6.1 / 04-2020




                A+W Business Inventory Management                                                               G-221
                Stock P.O.                                                               Software Reference




                             Product name group
                             •   Product names as per supplier file:
                                 The names of the ordered products are adopted from the supplier file.
                             •   Product names as per master data (internal P.O.):
                                 For internal purchase orders, the names of the ordered products are load-
                                 ed from the product master data.

                             Other group
                             •   No saving of costs:
                                 Costs are not written back to the purchase prices of the order.
                             •   Consider size surcharges:
                                 Size surcharges shall be transferred with the P.O.
                             •   Always set print code for processing:
                                 On the P.O. processing steps shall always be printed. If this option is dis-
                                 abled, the print codes are adopted from the order into the P.O. without any
                                 changes.
                             •   Statistics PGR as per order:
                                 The statistics PGR information is adopted from the order if different statis-
                                 tics PGRs have been defined for order and P.O.
                             •   Business type as per order:
                                 The business type is adopted from the order if different business types
                                 have been defined for order and P.O.
                             •   Production preparation as per order:
                                 The production preparation is adopted from the order if different production
                                 preparations have been defined for order and P.O.
                             •   Consultant = user for new input:
                                 The P.O. automatically shows the name of the user logged on to
                                 A+W Business.
                             •   Check change of status:
                                 The query concerning the change of status is displayed.
                             •   Repeat transfer only up to lock status:
                                 Purchase orders can be transferred several times but only until lock status
                                 has been reached.

                             Further settings group
                             •   Settings:
                                 Opens the Further settings dialog in which you can define information con-
                                 cerning printing texts and file attachments.
6.1 / 04-2020




                G-222                                                A+W Business Inventory Management
                Software Reference                                                                             Stock P.O.




                                          Order Pool
                                          Stock management > Stock P.O.




                Fig. G-114   Order pool


                                          In this dialog you can view all suggested purchase orders for articles that fall
                                          short of the minimum stock. The order quantity is calculated by the quantity
                                          that has been defined in the dialog Stock management.
                                          After the transfer, the purchase orders are created and can be printed and
                                          sent.
                                           Tutorial, “Stock P.O. (automatic)” on page G-103
                                           Tutorial, “P.O. Quantity after Stocktaking” on page G-131

                                          Storing location

                                          Warehouse, Corridor, Shelf, Tray You can restrict the display to individual
                                          storage locations. Please remember that stock articles may be booked to stor-
                                          age location <n.e.>. If you do not restrict the selection, purchase order sug-
                                          gestions are displayed for all articles that fall short of the minimum stock.
                                          The name of the storage locations can be changed in the master data.
6.1 / 04-2020




                                           Tutorial, “Define Stock Levels” on page G-20




                A+W Business Inventory Management                                                                  G-223
                Stock P.O.                                                               Software Reference




                             Overview
                             The data relating to the purchase order suggestions is displayed in the over-
                             view. You can select a different supplier and view a price comparison.
                             •   Supplier:
                                 The supplier is adopted from the supplier file. You can change the name if
                                 no supplier has been entered or if your standard supplier has supply prob-
                                 lems.
                             •   Article/color:
                                 Number and - if applicable - variant of the product to be ordered.
                             •   ID no.:
                                 Box ID (manual booking or from receipt of goods)
                             •   Storage location:
                                 Storage location where the stock on hand of the stock article falls short.
                             •   Qty:
                                 Quantity to be ordered. The standard purchase order quantity is multiplied
                                 until the minimum stock on hand is exceeded. You can also change the val-
                                 ue directly on the list.
                             •   Width, Height:
                                 Size of the lite to be ordered.
                             •   Contents:
                                 Contents are only shown for boxes.
                             •   Deliv. supplier:
                                 The supplier's delivery date is determined based on the entries in the sup-
                                 plier file. You can change the date if your standard supplier has supply
                                 problems.
                              Sales, “Change Supplier and Delivery Dates” on page C-657
                              Sales, “Price Comparison” on page C-659

                             Item for The purchase order suggestions are displayed in different colors:
                             • Red: internal order:
                                Internal orders are production orders that are created to fill stock on hand.
                                The suggestion is automatically created if the corresponding option for the
                                product has been enabled in the supplier file.
                             • Blue: Inquiry:
                                Inquiry to a supplier e.g. to ask for prices and delivery times.
                             • Green: Delivery might not be on time:
                                The current date is automatically set as the delivery date. As a result, the
                                delivery is usually not possible on time. If you change the date the color for
                                the entry changes to black.
6.1 / 04-2020




                G-224                                                A+W Business Inventory Management
                Software Reference                                                                    Stock P.O.




                                     Target Number Manager

                                     Employee Name of the employee logged in to A+W Business or who has set
                                     up the Number Manager. If you create a new Number Manager you can allo-
                                     cate it to one particular employee.

                                     Name Name of the target Number Manager for the purchase orders. A new
                                     Number Manager will be created when you enter a new name.

                                     Target number area

                                     Client If you have set up separate number areas for your clients you can se-
                                     lect the requested client here.

                                     Production preparation If you work with production preparations, you can
                                     allocate the purchase order to a certain order area.
6.1 / 04-2020




                A+W Business Inventory Management                                                         G-225
                Inventory Assessment                                                                       Software Reference




                                       Inventory Assessment
                                       For the stock assessment, the stocks are assessed using the periodic pro-
                                       cess. For this, the stock removals for the whole period are totaled first. Then
                                       the stock removals are deducted from the stock receipts. This process de-
                                       pends on the process selected:
                                       •       LIFO: The last articles received are deducted first.
                                       •       FIFO: The first articles received are deducted first.
                                               The stock value is calculated from the quantity not used in each case. Here,
                                               the period from the last stock assessment to the assessment time is con-
                                               sidered.

                                       Example

                                           Stock         Article      Date          Value in €   Quantity        Value
                                                                                                 (according
                                                                                                 to LIFO)

                                           1             111          1.5.2016      8.50         15 (15)         15*8.50

                                           1             111          4.5.2016      8.70         20 (10)         15*8.50
                                                                                                                 +20*8.70

                                           1             111          5.5.2016      8.20         10 (0)          15*8.50
                                                                                                                 +20*8.70
                                                                                                                 +10*8.20

                                                                                 The LIFO value is (15*8.50+10*8.70) / 25 = 8.58

                                           Stock         Article      Date          Value in €   Quantity        Value
                                                                                                 (according
                                                                                                 to FIFO)

                                           1             111          1.5.2016      8.50         15 (15)         15*8.50

                                           1             111          4.5.2016      8.70         20 (10)         15*8.50
                                                                                                                 +20*8.70

                                           1             111          5.5.2016      8.20         10 (0)          15*8.50
                                                                                                                 +20*8.70
                                                                                                                 +10*8.20

                                                                                 The FIFO value is (15*8.70+10*8.20) / 25 = 8.50

                                       Tab. G-1          Calculation examples

                                               Stock article with flag
                                               Stock articles with flags cannot be assessed using FIFO/LIFO since these
                                               are uniquely identifiable. Either 1 or no pieces of this stock article is pres-
                                               ent. Therefore, there is no removal sequence.

                                       For the initial assessment, the stock may not be negative. The initial assess-
6.1 / 04-2020




                                       ment can only be done according to average PP or manual value. Starting
                                       from the time of initial assessment, it is then possible to calculate using the
                                       FIFO or LIFO process.


                G-226                                                                 A+W Business Inventory Management
                Software Reference                                                             Inventory Assessment




                                     Inventory Assessment
                                     Stock management > Stock assessment > Selection
                                     You start the calculation of the stock value on this dialog.
                                     The Stock assessment dialog includes the following tabs:
                                     •   Stock Assessment – Selection
                                     •   Stock Assessment – Assessment


                                     Options Menu
                                     Stock management > Stock assessment
                                     The following entries are displayed:
                                     •   Initial assessment according to:
                                         For the initial assessment of the inventory, you can select one of the follow-
                                         ing procedures:
                                         – FIFO, LIFO
                                         – Av. PP
                                         – Manual
6.1 / 04-2020




                A+W Business Inventory Management                                                              G-227
                Inventory Assessment                                                                Software Reference




                                          Stock Assessment – Selection
                                          Stock management > Stock assessment > Selection




                Fig. G-115   Stock assessment – Selection


                                          On this tab you set the criteria according to which the stock value should be
                                          calculated. In addition, you can specify in the company data how the PP
                                          should be calculated.
                                           “Inventory List” on page G-167

                                          Selection

                                          Not assessed since Specification of the last assessment date. You can se-
                                          lect any date in the past. Thus only the products are assessed whose last as-
                                          sessment was before this date.
                                          The assessment period is between this date and the date that you enter in the
                                          Assessment field.

                                          Product from ... to Selection of the products that should be assessed.

                                          Product type Selection of the product type whose products should be as-
                                          sessed.

                                          Stat. product group Selection of the statistics product group to which the
                                          product is assigned.
6.1 / 04-2020




                                          Warehouse, Corridor, Shelf, Tray Selection of the storage location whose
                                          products should be assessed.



                G-228                                                           A+W Business Inventory Management
                Software Reference                                                          Inventory Assessment




                                     Only valid inventory (no negative inventory) You can exclude products
                                     from the assessment whose inventory is negative due to reservations.
                                     ☐ All products are assessed that correspond to the selection criteria in the
                                     Product and Product type fields.
                                     ☑ Only the products are assessed whose inventory is not negative. This in-
                                     cludes products whose inventory = 0.

                                     No glass with dimensions 0x0 For the combined inventory, products with
                                     the dimensions 0x0 are created to which the reserved quantities up to the re-
                                     moval of the stock sheets used are booked.
                                     ☐ All products are assessed that correspond to the selection criteria in the
                                     Product and Product type fields.
                                     ☑ Products with the dimensions 0x0 are not assessed.

                                     Assessment Entry of the date on which the stock assessment should be cal-
                                     culated. Thus you can perform a stock assessment in the past. The inventories
                                     are assessed on this date.
6.1 / 04-2020




                A+W Business Inventory Management                                                          G-229
                Inventory Assessment                                                                  Software Reference




                                         Stock Assessment – Assessment
                                         Stock management > Stock assessment > Assessment tab




                Fig. G-116   Stock assessment – Assessment


                                         On this tab, first the articles are displayed that correspond to the selection cri-
                                         teria. If you have started the assessment using one of the buttons, the calcu-
                                         lated values are displayed.
                                         These values are then also displayed in the stock statistics:
                                          “Stock Statistics – FIFO/LIFO” on page G-214
                                         The values can be saved. Before saving, all set assessments will be checked
                                         again for their consistency. If here an error is determined, it is displayed and
                                         none of the records is saved. You must correct the error in order to be able to
                                         save the data records.
                                         Once you have saved the data, you can no longer change the assessment.

                                         Assessment

                                         Select all You can select individual products from the list. With multiple selec-
                                         tion, you can mark as many products as you wish. Using the buttons, you can
                                         select all products or undo the selection.

                                         [Calc. LIFO] Starts the assessment of the marked products according to the
                                         LIFO procedure.
6.1 / 04-2020




                                         [Calc. FIFO] Starts the assessment of the marked products according to the
                                         FIFO procedure.


                G-230                                                            A+W Business Inventory Management
                Software Reference                                                            Inventory Assessment




                                     [Calc. both] Starts the assessment of the marked products according to both
                                     procedures.

                                     Change assessment type Selection of the assessment type. The change of
                                     assessment type only affects the marked entries.

                                     Overview
                                     The following columns can be displayed:
                                     •   Product, Name:
                                         Number and name of the product.
                                     •   Width , Height:
                                         Dimensions of the sheet.
                                     •   Cont.:
                                         Contents of a box.
                                     •   Color:
                                         Color variant of the glass.
                                     •   Storage location:
                                         Complete storage location.
                                     •   PU:
                                         Price unit of the product.
                                     •   Stock on hand:
                                         Current stock without reservations.
                                     •   QU:
                                         Quantity unit with which the product is kept in the stock.
                                     •   Assessment:
                                         Type of assessment:
                                         – None:
                                             The inventory of this product was not calculated.
                                         – LIFO, FIFO:
                                             The stock value is calculated as LIFO, FIFO value.
                                         – Average PP:
                                             The stock value is an average PP value.
                                         – Manually:
                                             The stock value is entered manually.
                                     •   FIFO, LIFO:
                                         Calculated stock value of the product.
                                     •   Average PP:
                                         Average purchase price. This price is only calculated if the appropriate op-
                                         tion is activated in the company data.
                                     •   Manually:
                                         The value of the manual entry is entered as stock value.
6.1 / 04-2020




                A+W Business Inventory Management                                                            G-231
                Inventory Assessment                                                              Software Reference




                                       •   Remark FIFO/LIFO:
                                           Display of the status after assessment:
                                           – OK:
                                              The inventory of this product was calculated. This status is not possible
                                              on initial assessment.
                                           – Negative stock on hand:
                                              The inventory of this product cannot be calculated because the inven-
                                              tory contains negative values.
                                           – No initial inventory found:
                                              The inventory of this product can only be determined by average PP or
                                              manually.
                                           – Qty. must be greater than 0:
                                              The inventory of this product cannot be calculated because there is no
                                              inventory.
                                       •   Last assessment:
                                           Date of last assessment.
                                       •   Assessment:
                                           Value of the last assessment.
6.1 / 04-2020




                G-232                                                         A+W Business Inventory Management
Inventory Management            G

                       Section Index




                 A+W Business
                Section Index                                                                             Index




                Index
                A                                           – Create inventory list G-141
                Actual stock G-138                          – delete inventory list G-150
                Add supplementary inventory        G-151    – determine target inventory G-145
                Average PP G-50                             – enter article G-148
                Average price (stock) G-52                  – enter quantities counted G-147
                                                            – finalize G-149
                                                            – Print count list G-143
                B
                                                            – Product master data G-142
                BOM
                                                            – set stock on hand to zero G-148
                – Set up for stock control G-62
                                                            – sqm articles G-139
                Booking
                                                            – Value adjustment G-139
                – check for order item G-119
                                                            Inventory list
                Booking journal
                                                            – Add supplementary inventory G-151
                – Create for stock G-87
                                                            – complete G-144
                – Stock management G-86
                                                            – create G-141
                Booking type
                                                            – delete G-150
                – for stock booking G-43
                                                            – load G-144
                – stock G-76
                                                            – print G-143

                C                                           J
                Calculation
                                                            Journal
                – Purchase price calculation G-51
                                                            – show for stock booking   G-87
                – Waste G-40
                Combined stock control G-38
                Company data                                L
                – enable PP calculation G-54                Lock product master data   G-142
                – enable Stock control mode G-31
                – Settings G-29                             M
                                                            Master data
                D                                           – Check price lists for PP calculation G-56
                Determine target inventory G-145            – Check product G-41
                Display conventions G-11                    – define stock category G-25
                                                            – define stock level G-20
                                                            – define storage location G-23
                E
                                                            – Enter stock size G-45
                Enter quantities counted    G-147
                                                            – name stock level G-22
                                                            – prices for stock articles G-55
                F                                           – status allocation for stock booking G-34
                Final inventory   G-149                     – user status for stock booking G-33
                                                            Minimum quantity
                H                                           – stock on hand G-68
                History
                – Stock management        G-86              O
                                                            Order
                I                                           – Enter stock articles G-116
                Initial inventory G-153                     – Internal G-129
6.1 / 04-2020




                Inventory                                   – work order G-127
                – Actual stock, target inventory    G-138   Order item
                – box G-139                                 – check booking G-119


                A+W Business Inventory Management                                                    G-161
                Index                                                                            Section Index




                P                                             – define storage location G-23
                P.O.                                          – definition G-19
                – automatic G-104                             – forecast for stock on hand G-96
                – change date G-108                           – initial inventory G-153
                – Change supplier G-108                       – name level G-22
                – Price comparison G-110                      – show current stock on hand G-99
                – Proposal G-104                              stock
                – purchase quantity after stocktaking G-130   – locations G-19
                – Transfer P.O. proposal G-105                Stock addition
                – Transfer to Purchasing G-105                – by production order G-135
                Price                                         Stock article
                – Compare in P.O. proposal G-110              – enter at stocktaking G-148
                Price lists                                   – enter in Stock management G-71
                – for PP calculation G-56                     – in order G-115
                Print count list G-143                        – Main product G-67
                Print reserved stock articles G-89            – production order G-127
                Procurement type G-37                         – Stock size G-40, G-45
                Product                                       – transfer storage location G-82
                – Check master data for stock G-41            Stock articles G-67
                – Enter stock size G-45                       – print reservation G-89
                – Stock article G-37                          Stock booking
                Production order                              – Booking type G-76
                – Stock addition G-135                        – change storage location G-82
                – Supplier file G-129                         – Create journal G-87
                Purchase order                                – for BOM G-59
                – Minimum quantity and P.O. quantity G-104    – manual G-76, G-77
                Purchase price G-55                           – print reserved stock articles G-89
                – average PP G-50                             – Registration point G-135
                – Check settings G-54                         – select booking type G-43
                – combined stock mode G-50                    – Show journal G-87
                                                              – show statistics G-91
                                                              – status allocation G-34
                R
                                                              – user status G-33
                Receipt of goods
                                                              – Withdrawal and addition G-77
                – Stock booking G-77
                                                              stock booking
                Reservation
                                                              – combined stock control G-38
                – show in stock journal G-87
                                                              stock booking type G-37
                – Waste G-40
                                                              Stock code G-37
                Reservation for BOM G-59
                                                              Stock control
                reservations G-28
                                                              – Set up BOM G-62
                                                              – Stock codes G-37
                S                                             – storage location G-15
                Statistics                                    Stock control at BOM level G-59
                – show for stock movement G-91                Stock control mode G-28
                – Stock management G-86                       – enable in company data G-31
                Status                                        – PP calculation G-50
                – Allocations for stock booking G-33          Stock Management
                – Stock booking G-31                          – Main stock product G-67
                Stock                                         Stock management
                – Check prices in master data G-55            – Basic principles G-14
6.1 / 04-2020




                – Check product master data G-41              – booking journal G-86
                – define level G-20                           – enable PP calculation G-54
                – define stock category G-25                  – enter manual stock P.O. G-123


                G-162                                                   A+W Business Inventory Management
                Section Index                                          Index




                – enter stock articles G-71            W
                – history G-86                         waste   G-40
                – Menu overview G-12
                – Price development G-69
                – Processes G-15
                – statistics G-86
                – Stock value G-86
                Stock movement
                – manual G-76
                – Statistics G-91
                Stock on hand
                – future stock on hand G-96
                – Include in inventory G-138
                – Minimum quantity G-68
                – Replacement time G-97
                – show G-99
                Stock P.O.
                – Check if automatic order G-130
                – enter manually G-123
                Stock P.O. after stocktaking G-130
                Stock PO
                – surcharges G-70
                Stock query G-86
                Stock size
                – Enter in master data G-45
                – Master data, stock management G-40
                – Product management G-39
                – Stock article G-40, G-45
                Stock value
                – PP assessment G-49
                Stocking booking
                – Manual booking of additions/
                  withdrawals G-78, G-81
                storage location
                – stock on hand G-15
                – transfer article G-82
                Supplier
                – change in P.O. G-108
                Supplier file
                – Internal customer G-129
                – Production order G-129
                Surcharge
                – distribute to stock POs G-70

                T
                Target inventory   G-138

                V
                Value adjustment
6.1 / 04-2020




                – Inventory G-139




                A+W Business Inventory Management                     G-163
                Index                        Section Index
6.1 / 04-2020




                G-164   A+W Business Inventory Management

