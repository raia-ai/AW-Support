---
description: "EN AWBusiness Box Management 1.10"
---



# EN AWBusiness Box Management 1.10

Box Management            K




                           English




                 A+W Business
                                                                                                             Introduction




                                     Introduction
                                     This part of the documentation contains editorial notes.


                                     Revision Overview
                                     Section           Description
                                     Version/Date

                                     1.10/012-2019     Updating the settings in the master data. Transfer of box purchase
                                                       orders from Purchase part and stock bookings from Production
                                                       part.

                                     1.00/012-2018     Original version box management: Separation from Stock,
                                                       Purchase and Production parts.



                                     Editorial
                                     The editorial provides information on the following topics:
                                     •   Notes on this document
                                     •   Copyrights
                                     •   Trademarks
                                     •   Contact

                                     Notes on this document
                                     This document is intended for end users of A+W Business.
                                     The documentation and software described are licenses that must only be
                                     used or copied in accordance with the conditions of our license agreement.
                                     The contents of the documentation are only informative and are subject to
                                     changes without prior notice. The text and illustrations were compiled with the
                                     utmost care. Still, errors cannot be totally excluded. A+W Software GmbH can-
                                     not be held liable for errors or inaccuracies, unless they can be attributed to
                                     wilful or grossly negligent action.
                                     This document describes the full scope of A+W Business.

                                     Copyrights
                                     © 2020, A+W Software GmbH, all rights reserved, also those for reprinting, the
                                     making of copies and translation.
                                     The documentation may be copied, completely or in part, saved in an archiving
                                     system or transferred in any other form only in accordance with our license
                                     agreement. Transmission of the documentation is not allowed, neither elec-
                                     tronically, nor mechanically, nor by recording or in any other way, without 's pri-
1.10 / 12-2019




                                     or written approval.




                 A+W Business Box Management                                                                         K-3
                 Introduction




                                Trademarks
                                All hardware and software designations mentioned in the documentation can
                                also be registered trademarks or other industrial property rights of third parties.
                                Third party copyrights must be observed.

                                Contact
                                A+W Software GmbH

                                Am Pfahlgraben 4-10

                                D-35415 Pohlheim

                                    +49 6404 2051 0

                                    +49 6404 2051 877

                                aw.zentrale@a-w.com

                                http://www.a-w.com
1.10 / 12-2019




                 K-4                                                          A+W Business Box Management
                                                                                                                                                      Content




                                     Content
                                     Introduction ............................................................................................................. K-3
                                       Revision Overview ............................................................................................... K-3
                                       Editorial ............................................................................................................... K-3

                                     Tutorial                                                                                                             K-7
                                     Overview ................................................................................................................. K-9
                                       Documentation .................................................................................................. K-10
                                       Menu Overview ................................................................................................. K-11
                                     Basic Principles of Stock ...................................................................................... K-12
                                       Stock Sizes ........................................................................................................ K-13
                                       Stock Management ........................................................................................... K-14
                                     Basic Settings ....................................................................................................... K-16
                                       Prices ................................................................................................................ K-16
                                       Company Data .................................................................................................. K-18
                                       Status Changes due to Additions and Dispatches ............................................ K-21
                                       Stock Categories ............................................................................................... K-22
                                     Master Data for Boxes .......................................................................................... K-23
                                       Box Data ............................................................................................................ K-24
                                         Define stock sizes for boxes .......................................................................... K-25
                                         Creating stock articles for box ........................................................................ K-26
                                       Box with BOM .................................................................................................... K-29
                                         Master data for boxes with BOMs .................................................................. K-30
                                         BOM box in stock management ..................................................................... K-34
                                         BOM box at item entry ................................................................................... K-35
                                     Orders ................................................................................................................... K-36
                                       Sales Order with Box ......................................................................................... K-37
                                       Production Orders ............................................................................................. K-41
                                         Settings in Supplier File ................................................................................. K-42
                                         Enter production order ................................................................................... K-44
                                     Stock Management for Boxes ............................................................................... K-48
                                       Stock Management of Boxes ............................................................................ K-48
                                       Stock P.O. of boxes ........................................................................................... K-49
                                       Receipt of Goods via Barcode ........................................................................... K-54
                                       Shipping of Boxes ............................................................................................. K-55
                                         Withdrawal of boxes ....................................................................................... K-55
                                         Booking of issued goods ................................................................................ K-58
                                       Manual Stock Bookings ..................................................................................... K-60
                                         Manual input of addition ................................................................................. K-60
                                         Change storage location of a box .................................................................. K-64
                                         Correcting the box contents (number of sheets) ............................................ K-65
                                         Opening (resolving) boxes ............................................................................. K-66

                                     Software Reference                                                                                                K-69
                                     Overview ............................................................................................................... K-71
                                     Stock Management ............................................................................................... K-72
                                       Menus in Stock Management ............................................................................ K-72
                                         Functions Menu ............................................................................................. K-72
                                         Options Menu ................................................................................................. K-73
                                       Stock Management ........................................................................................... K-73
1.10 / 12-2019




                                         Stock Management - Stock Articles ............................................................... K-74
                                         Stock Management - Prices ........................................................................... K-78
                                         Stock Management - Supplement .................................................................. K-81
                                     Stock Movement ................................................................................................... K-83



                 A+W Business Box Management                                                                                                                 K-5
                 Content




                             Options Menu .................................................................................................... K-83
                             Stock Movement ................................................................................................ K-83
                               Stock Movement – Dispatch, Addition ........................................................... K-84
                               Stock Movement – Transfer ........................................................................... K-86
                               Stock Movement – Number of Sheets ........................................................... K-87
                               Stock Movement – Open Boxes .................................................................... K-88
                             Remark (Stock Movement) ................................................................................ K-89
                           Search .................................................................................................................. K-90
                             Stock Search – Stock Search ............................................................................ K-91
                             Stock Search - Future Stock on Hand ............................................................... K-94
                           Stock P.O. ............................................................................................................. K-96
                             Order Pool Menus ............................................................................................. K-96
                               Functions Menu ............................................................................................. K-96
                               Options Menu ................................................................................................. K-97
                             Order Pool ......................................................................................................... K-99
                           Receipt and Shipping of Boxes ........................................................................... K-102
                             Receipt of Goods (Boxes) ............................................................................... K-102
                               Receipt of Goods – Selection ...................................................................... K-103
                               Receipt of Goods –Complete ....................................................................... K-105
                               Receipt of Goods – by Item ......................................................................... K-107
                               Receipt of Goods – ID Numbers .................................................................. K-110
                               Receipt of Goods – Protocol (ID Numbers) ................................................. K-112
                             Settings (ID) .................................................................................................... K-113
                             Shipping of Boxes ........................................................................................... K-114

                           Part index                                                                                                     K-115
                           Index ................................................................................................................... K-117
1.10 / 12-2019




                 K-6                                                                              A+W Business Box Management
Box Management              K

                        Tutorial




                 A+W Business
                 Tutorial                                                                                     Overview




                                     Overview
                                     The box management tutorial discusses the settings for entering and booking
                                     boxes containing cut glass.

                                         The functions depend on the enabled modules
                                         Please note that the individual functions are only available if the corre-
                                         sponding modules and interfaces have been installed and enabled.

                                         If you detect functions in this description that are not available in your ver-
                                         sion, please contact A+W Software GmbH.

                                     Subjects
                                     This tutorial includes the following subjects:
                                     •   Basic Principles of Stock
                                     •   Basic Settings
                                     •   Master Data for Boxes
                                     •   Orders
                                     •   Stock Management for Boxes

                                     Required knowledge
                                     The tutorial is meant for those who work with boxes in A+W Business. The par-
                                     ticipants must be familiar with the concept of master data, sales, and purchas-
                                     ing in A+W Business.
1.10 / 12-2019




                 A+W Business Box Management                                                                       K-9
                 Overview                                                                               Tutorial




                            Documentation
                            The following documents are available for the Box Management module:

                            Format                    Volume

                            PDF                       Complete documentation
                                                      • Tutorial
                                                      • Software reference

                            Online help <F1>          Context-sensitive dialog help of A+W Business software
                                                      reference and tutorials.


                            Additional descriptions are available in the Stock, Purchasing, and Production
                            parts, each of which is available via the online help.

                            Tutorial Structure
                            The tutorial consists of subjects with several training modules each. Each
                            training module consists of the following elements:

                            Overview                  Each training module starts with an overview of the
                                                      major topics:

                            Concepts                  First, the concepts and terms of the corresponding
                                                      training module will be explained.

                            Instruction               The instructions are intended as examples to
                                                      demonstrate the flow. The names they contain are
                                                      fictitious.


                            Display Conventions
                            Certain parts of sentences are specially marked. The meanings are:

                            Italic                    marks character strings describing the software
                                                      elements, e. g. the Stock info dialog.

                            Bold                      marks character strings to be entered via the keyboard,
                                                      e.g.: Enter the value 0.

                            >                         The so-called breadcrumb trail marks the way to open a
                                                      dialog, e.g. Master data > Product > Article > Stock size.

                            []                        Square brackets mark buttons in a dialog, e. g. [OK] to
                                                      save the data.

                            <>                        Angle brackets refer to keys or shortcuts on the
                                                      keyboard, e. g. <F1> is used to open the online help.
1.10 / 12-2019




                 K-10                                                     A+W Business Box Management
                 Tutorial                                                                                      Overview




                                       Menu Overview
                                       This chapter provides a brief overview of the program sections that contain the
                                       dialogs that are displayed in this documentation.




                 Fig. K-1   Box management menu


                                       Master data
                                       •   Stock size:
                                           Use this dialog to enter the boxes with different price keys.

                                       Stock management
                                       •   Stock management:
                                           Use this dialog to enter and maintain data for stock articles.
                                       •   Stock movement:
                                           Use this dialog to book goods received and issued, changes of stock loca-
                                           tions and opening of boxes.
                                       •   Search:
                                           Use this dialog to check the product availability during a certain time period.

                                       Production
                                       •   Goods issues boxes:
                                           Use this dialog to enter stock issue of boxes that are assigned to an order.

                                       Documents
                                       •   Goods received:
                                           Use this dialog to enter the boxes that should be included in the inventory.
1.10 / 12-2019




                 A+W Business Box Management                                                                        K-11
                 Basic Principles of Stock                                                                                    Tutorial




                                             Basic Principles of Stock
                                             A+W Business's Stock Management module allows you to manage jumbo siz-
                                             es, stock sizes, residual plates, boxes, all-glass doors, fittings, frame parts and
                                             accessories, such as mirror mountings, sealing tape, etc.
                                             A detailed description of stock is in the Stock Management section. The most
                                             important points for box management will be summarized only briefly here.

                                             Stock control
                                             Before you set up your stock in A+W Business, you have to decide on the ba-
                                             sis of how your stocks should be managed: as an area (sqm) or in numbers of
                                             pieces. A third possibility is the combined stockkeeping, whereby the size-de-
                                             pendent stock mode is combined with the reports from the optimization so that
                                             in addition to the stock dimensions, the stock sizes cut can be booked out au-
                                             tomatically.
                                             After deciding about the mode, allocate the corresponding stock code per
                                             glass product and define the stockkeeping mode in the company data.

                                             Stock control mode and reservation
                                             When a product with procurement type Stock Withdrawal is entered in a (pro-
                                             duction) order, the corresponding quantity (plus waste in the case of fixed siz-
                                             es) of the stock article is marked as reserved. The reservation can optionally
                                             either be booked out of the current stock on hand or automatically when the
                                             delivery note or invoice is printed.
                                             These settings are shown in the stock quantities display in dialog Stock Info
                                             (stock preview) and the automatic purchase order suggestions that can be trig-
                                             gered when minimum quantities are reached.

                                             Consumption of BOM elements in production orders
                                             For production orders, the consumption of BOM elements in stock can be
                                             booked. Boxes then have a BOM if picture frame glass is packed in paper and
                                             these paper packages are on a pallet.

                                                Example

                                                In a production order, LAMI with 2xFloat 3 is entered. After reporting of the
                                                production order, the LAMI is booked to the stock, the Float 3 is booked out of
                                                the stock.

                                                If for the same LAMI a normal customer order is entered, only the LAMI is
                                                withdrawn from the stock. The Float 3 is not kept in the stock since it has
                                                already been withdrawn from the stock by the production order.


                                             Supplier list
                                             If a box with the identical dimensions is purchased, you must enter the supplier
1.10 / 12-2019




                                             in the supplier list. The supplier is found via the product group that is assigned
                                             to the box in the stock dimensions.



                 K-12                                                                         A+W Business Box Management
                 Tutorial                                                                          Basic Principles of Stock




                                             Stock Sizes
                                             The stock size Box is mandatory for stock bookings. For entering a box as an
                                             order or purchase order item, a stock article/size called Box must therefore
                                             have been created.
                                             If you have created a stock size in the master data, A+W Business provides
                                             you with the option to immediately switch to stock management.


                                                                                                   A


                                                                                                   B

                                                                                                   C
                                                                                                           D




                            F            E




                 A Product management – stock       C Stock sizes with different           E Allocation of price tables
                   sizes (master data)                dimensions                           F Determining the PP in the stock
                 B Product number pertaining to the D Stock articles relating to the stock
                   stock sizes                        sizes (stock management)
                 Fig. K-2       Stock sizes (product management) and related stock articles


                                             Each stock size can be allocated to a separate price table.
                                             If you work with the stock code size-related, you must create stock articles for
                                             all stock sizes.
1.10 / 12-2019




                 A+W Business Box Management                                                                            K-13
                 Basic Principles of Stock                                                                             Tutorial




                                              Stock Management
                                              Every (glass) product is related to a stock size and a stock article.
                                              Each stock article can be created in different variants, e. g. Float 5 mm in sev-
                                              eral sizes.


                                                 J                   I




                 A

                                                                                                                           H
                 B

                 C


                 D

                 E
                                                                                                                           G




                                                          F

                 A   Product number                                      F   Inventory audit for the stock preview
                 B   Stock article sizes                                 G   Defined stock articles
                 C   Standard storage location                           H   Main product
                 D   Stock category                                      I   Number of sheets in boxes
                 E   Main stock article code                             J   Storage place (4 levels)
                 Fig. K-3      Stock article definition


                                              In stock sizes (master data), a box can be defined for every product with the
                                              procurement type Stock withdrawal, e.g. one box per size.
                                              If there are boxes of the same size but with different numbers of sheets (I),
                                              separate stock articles must be defined for them. To define the exact box arti-
                                              cle, width and height (among others) are analyzed to determine the minimum
                                              stock.
1.10 / 12-2019




                                              A stock article is therefore required for every box variant, specifying the prod-
                                              uct number, the size, and the number of sheets.




                 K-14                                                                        A+W Business Box Management
                 Tutorial                                                                 Basic Principles of Stock




                                     You can link several stock sizes in stock management by defining a main stock
                                     product (H). The inventory check in Stock info dialog is executed only for the
                                     main stock product in this case; a minimum stock has to be defined only for
                                     this article.
                                     If the stock on hand is not checked for each storage location (F), a main prod-
                                     uct (E, H) must be allocated to determine the available square meters of the
                                     glass.
1.10 / 12-2019




                 A+W Business Box Management                                                                  K-15
                 Basic Settings                                                                                     Tutorial




                                           Basic Settings
                                           In addition to the products and the stock articles, additional setting must be
                                           specified so that the boxes can be managed correctly.
                                           This section provides information on the following basic settings:
                                           •   “Prices” on page K-16
                                           •   “Company Data” on page K-18
                                           •   “Status Changes due to Additions and Dispatches” on page K-21
                                           •   “Stock Categories” on page K-22


                                           Prices
                                           Via the price lists for boxes, the prices in purchasing and sales are calculated,
                                           e.g. also if individual sheets from a box are sold.
                                           If you want to calculate the glass in boxes with other prices, you must create
                                           appropriate price lists for sale and purchase. If you also want to use different
                                           glas prices depending on the quantity, additional price lists are also required
                                           for this.
                                           The prices are described in detail in the Master Data section.


                                  A                     B




                 A Price keys for boxes                               B Price per price key
                 Fig. K-4     Example of box prices


                                           In this example, you see that the prices for the glass in a box are calculated
                                           differently, e.g. for the whole box or for a single sheet from the box.
                                           The following conditions must be fulfilled to calculate the average purchase
                                           price:
                                           •   The product has to be defined also as a stock article.
1.10 / 12-2019




                                           •   The PP code must be set in company data.




                 K-16                                                                   A+W Business Box Management
                 Tutorial                                                                                Basic Settings




                                         Check price lists

                                          How to check the master data of your price lists
                                         1 Go to menu Master data > Prices and check the settings in the dialogs
                                           Year, Key, and Rate.
                                             You only need to check the entries used for the prices (and other internal
                                             calculations) for stock sizes and boxes.
                                         2 Select menu Master Data > Prices > Prices.




                    Fig. K-5   PP price tables


                                         3 Please check if all purchase and sales prices have been defined and are
                                           up to date, and complete or correct them as necessary.
                                         4 Go to the tab in which the price is defined, check if the purchase price has
                                           been entered correctly, and correct it if necessary.




                    Fig. K-6   Defined purchase prices


                                         5 Go to menu Start > Save to save the data.
                                             The data is saved.
1.10 / 12-2019




                 A+W Business Box Management                                                                      K-17
                 Basic Settings                                                                                    Tutorial




                                            Company Data
                                            In the company data, the settings for the receipt of boxes and stock receipts
                                            are specified through production orders. These settings are described in detail
                                            in the Stock management section.

                                            Checking settings for boxes

                                             How to check the settings for the stock
                                            1 Select menu Master Data > Company > Company Data.
                                                 Master Data, “Company Data” on page B-917
                                            2 Switch to the Parameter tab and check the settings for the virtual item num-
                                              bers.




                                                                                                                  A




                 A Virtual item numbers for receipt of boxes
                 Fig. K-7     Company data – parameters


                                                The virtual item number is necessary for booking the receipt of box items
                                                with a quantity of > 1 correctly.
1.10 / 12-2019




                                            3 Go to the Stock / PP / EDI tab.




                 K-18                                                                   A+W Business Box Management
                 Tutorial                                                                                        Basic Settings




                                               There are two ways of entering additions to stock based on production or-
                                               ders:
                                               •   If the status of the production order exceeds the defined status due to a
                                                   report from production, the addition to stock is booked automatically.
                                               •   If you do not use production reports, you can enter the addition to stock
                                                   by means of the manual status report in the Production module. If you
                                                   set the production order there to a status above the aforementioned lim-
                                                   it, the stock withdrawal of the material consumed and the addition of
                                                   produced stock articles to stock are booked automatically.
                                               If no other storage location has been defined, the order quantity is allocated
                                               to the standard storage location.




                 A




                 B


                 C
                 D

                                                                                                                             F

                 E




                 A Settings for determining the purchase price          D Stock bookings for production orders
                 B Setting to update the stock on hand                  E Number of preview days for dialog Stock Info
                 C Delete ID numbers                                    F Limit status for registration points (for production
                                                                          orders)
                 Fig. K-8     Company data - Stock / PP / EDI


                                            4 Select the settings for stock P.O.s (A).
                                               For the boxes, it is only important how the purchase price should be deter-
1.10 / 12-2019




                                               mined. The settings for determining the purchase price are described in the
                                               Master Data section.



                 A+W Business Box Management                                                                               K-19
                 Basic Settings                                                                           Tutorial




                                     All other settings in this area are described in detail in the Stock Manage-
                                     ment section.
                                  5 Select the functions that should be considered when updating the stock on
                                    hand in the Stock Control Mode (B).
                                     •   Reservation w/o stock update:
                                         Enable this option if reserved quantities should not be booked out of the
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
                                     •   Delete articles with ID if there is no stock on hand (C):Boxes with the
                                         stock = 0 are no longer present in stock. Enable this checkbox if in the
                                         stock management tbe boxes with the ident numbers from the overview
                                         should be deleted for which no inventory is displayed.
                                     •   Consumption of BOMs in production orders (D):
                                         If you are working with production orders, you can specify whether the
                                         consumption of BOM elements is booked out of stock automatically.
                                  6 Enter the number of workdays (E).
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
1.10 / 12-2019




                 K-20                                                          A+W Business Box Management
                 Tutorial                                                                             Basic Settings




                                     Status Changes due to Additions and
                                     Dispatches
                                     Goods dispatches and receipts can change the status of documents and result
                                     in stock changes due to the status change. If the status points and status allo-
                                     cations are defined correspondingly, this will also apply to partial deliveries.
                                     If you have enabled the option Execute stock booking before document print-
                                     out, the minimum, assigning and lock status must be organized in a manner
                                     that stock withdrawal bookings can be executed prior to printing. If the status
                                     allocation does not allow reversal of the order it may be possible that the stock
                                     withdrawal booking is not executed.

                                     Check Status Allocations
                                     A detailed description of stock sizes can be found in the Stock Management
                                     section:


                                      How to check the status management
                                     1 Go to menu Master data > Order > Status management.
                                     2 Check whether the user status for stock additions and stock dispatch ex-
                                       ists.
                                        Create them if necessary.
                                        Next, check the status allocations.
                                     3 Select menu Master Data > Order > Status allocation.
                                     4 Check whether the status allocations of stock addition and stock dispatch
                                       for document types Order and P.O. have been defined:
                                        •   Stock goods dispatch: Status Delivery note printed or Invoice printed
                                        •   Stock goods receipt: Status Goods receipt booked
                                     5 Create missing allocations and correct existing ones if necessary.
1.10 / 12-2019




                 A+W Business Box Management                                                                    K-21
                 Basic Settings                                                                         Tutorial




                                  Stock Categories
                                  The stock categories are allocated to stock articles in the Stock management
                                  dialog. The stock articles are summed up in groups (stock categories) that can
                                  be used as search criteria.

                                  Check stock category

                                   How to define a stock category
                                  1 Select menu Master data > Stock > Category.




                                     Fig. K-9     Stock categories


                                      Master Data, “Stock Categories” on page B-738
                                  2 Go to the menu Start > New to switch to the input mode.
                                  3 Enter an ID for the stock category, e. g. figures or names, such as raw ma-
                                    terial, boxes, production, etc.
                                  4 Go to the menu Start > Save to save the data.
                                     The data is saved.
1.10 / 12-2019




                 K-22                                                         A+W Business Box Management
                 Tutorial                                                                       Master Data for Boxes




                                     Master Data for Boxes
                                     This chapter contains information about how you create the data in order to
                                     differentiate the price calculation for boxes and manage boxes in stock. This
                                     includes the definition of the stock sizes and the definition of the stock articles.
                                     This section provides information on the following subjects:
                                     •   “Box Data” on page K-24
                                     •   “Box with BOM” on page K-29
1.10 / 12-2019




                 A+W Business Box Management                                                                       K-23
                 Master Data for Boxes                                                                                   Tutorial




                                         Box Data
                                         Objectives

                                         • Define stock sizes and stock articles for boxes.
                                         • Define products (articles) for boxes.


                                         Benefits

                                         • If the products are defined correctly, pieces and surfaces can be calculated and
                                           reserved.
                                         • The display of the actual stock on hand including reservations makes purchasing
                                           easier.


                                         Please note

                                         Products                     The products from the master data are used for entry
                                                                      and pricing in documents. They are not automatically
                                                                      kept as stock on hand; this is only the case as a result of
                                                                      additional settings and definitions.

                                         Stock articles              All products that are kept in the warehouse with stock
                                                                     quantities must be created as stock articles.

                                         Jumbo size                   Glass plate as delivered by the manufacturer. It is used
                                                                      to cut the glass pieces for sales.

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
1.10 / 12-2019




                 K-24                                                                     A+W Business Box Management
                 Tutorial                                                                               Master Data for Boxes




                                            Define stock sizes for boxes
                                            The stock size Box is mandatory for stock bookings. For entering a box as an
                                            order or purchase order item, a stock article/size called Box must therefore
                                            have been created.


                                             How to define stock sizes in master data
                                            1 Select menu Master data > Product > Products > Stock sizes
                                                The Stock sizes dialog opens.
                                            2 Go to menu Start > New and enter the stock size.




                 A




                 B

                 C




                 D




                 A Dimensions of the sheets and content of the box    C Pricing in stock
                 B Price tables for sales and purchasing              D Procurement type
                 Fig. K-10    Create stock size for pricing


                                                If you have already defined a corresponding stock article in stock manage-
                                                ment, enter the same values for width and height (A).
                                            3 Enter the number of sheets in the box in the Contents field.
                                            4 Enter the price code for sales and purchasing (B).
                                                You must create an individual stock dimension if you calculate different
1.10 / 12-2019




                                                prices, e.g. for the sale of the entire box, for individual sheets from the box,
                                                and/or for the cutting of individual sheets that are removed from the box.



                 A+W Business Box Management                                                                              K-25
                 Master Data for Boxes                                                                              Tutorial




                                         5 Check the checkbox Search stock PP (C) if the stock size is to be included
                                           in pricing.
                                         6 In addition, you can enter name and short name (matchcode), e.g. for bet-
                                           ter identification of stock articles.
                                         7 Enter the procurement type (D), e.g. Stock withdrawal for stock articles.
                                         8 Go to the menu Start > Save to save the data.
                                             The data is saved. Next, the system will want to know whether you want to
                                             define this stock size as a stock article as well.
                                         9 Choose [Yes] if the stock size is also to be managed as a stock article.
                                             The Stock management dialog opens.


                                         Creating stock articles for box
                                         For a stock article Box you have to define at least the following settings in order
                                         to manage the stock:
                                         •   Article number and name
                                         •   Sizes for stock sizes, sizes and contents for boxes
                                         •   Storage location and standard storage location (default storage location)
                                         •   Stock on hand

                                             Stock start-up
                                             If no stock articles have been entered at all, you can facilitate this task by
                                             running the so-called initial inventory. This function is described in the
                                             Stock management section.


                                          How to create a stock article
                                         1 Go to menu Stock management > Stock management.
                                             The Stock management dialog opens.
1.10 / 12-2019




                 K-26                                                                  A+W Business Box Management
                 Tutorial                                                                                Master Data for Boxes




                                            2 Go to the menu Start > New to switch to the input mode.
                                                 If you open the Stock management dialog from the master data, this step
                                                 can be omitted. The fields for articles and sizes are filled in already.




                 A


                 B

                 C




                 D




                 E




                                                     F
                 A Stock article number                                   D Main product
                 B Size and content of the box                            E Stock on hand
                 C Storage location                                       F Inventory audit
                 Fig. K-11    Fields for new stock articles are enabled


                                            3 Enter the number (A) the size and the content of the box (B).
                                            4 Choose a storage location (C).
                                                 If no storage location is selected, the storage location <n.e.> will be en-
                                                 tered. In stock management, this will be treated like the defined storage lo-
                                                 cations, e. g. for stocktaking purposes and queries.
                                                 If a stock article is kept in different storage locations, you have to define one
                                                 of them as the standard storage location.
                                            5 Check the Default storage location checkbox.
                                            6 Go to the Main product field (D) and select the article for which you want to
                                              enter the minimum stock for the inventory audit.
                                                 For boxes, this is the stock plate from which the sheets are cut.
1.10 / 12-2019




                 A+W Business Box Management                                                                                K-27
                 Master Data for Boxes                                                                                Tutorial




                                           7 Check the checkbox Inventory audit per stock location (F) if all storage lo-
                                             cations shall be evaluated separately when checking the inventory for this
                                             stock article.
                                           8 Change to the Prices tab and enter the quantity unit with which the average
                                             price is calculated.




                 A



                                                                B
                 A Average price                                       B Quantity unit
                 Fig. K-12   Average price for stock articles


                                           9 Change to the Supplement tab and check whether the supplier 0 is entered
                                             for the boxes from production.
                                               With this setting, you specify that you yourself are the supplier. This setting
                                               has no effect on the boxes that you can alternatively order from a supplier,
                                               for such boxes are not kept in stock.
                                           10 Go to the menu Start > Save to save the data.
                                               The data is saved.
                                           11 Repeat steps to for all fixed dimensions that can be entered as boxes.
                                               For boxes, you specify a stock article per glass, dimension, content, and
                                               price key.
                                               Thus all necessary information A+W Business needs for reservations and
1.10 / 12-2019




                                               booking have been defined.




                 K-28                                                                     A+W Business Box Management
                 Tutorial                                                                         Master Data for Boxes




                                     Box with BOM
                                     Objectives

                                     • Getting familiar with the product structure of boxes with BOMs (pallets).


                                     Benefits

                                     • Boxes with a deeply graduated BOM can be defined and entered as products.


                                     Please note

                                     Product structure           The article structure of boxes with a BOM is more
                                                                 complex than that of simple glass boxes.

                                     Default settings            Stock management
                                                                 Master data:
                                                                 • Product management
                                                                 • Supplier list
                                                                 Company data:
                                                                 • Parameters tab
                                                                 • Stock/ PP / EDI tab
1.10 / 12-2019




                 A+W Business Box Management                                                                         K-29
                 Master Data for Boxes                                                                           Tutorial




                                         Master data for boxes with BOMs
                                         Boxes with BOM are articles the structure of which is more complex than the
                                         glass boxes known so far. Picture frame glass can be wrapped in paper for ex-
                                         ample, and can then be put onto a pallet.
                                         The pallet is defined as the main product and the paper box with the sheets,
                                         as its BOM. Both the pallet and the paper box belong to the product type Box.

                                            Previous knowledge required for this unit
                                            This session is not about working on new dialogs or functions. Boxes with
                                            BOMs have a special product structure that is defined by means of the al-
                                            ready known tools. For information regarding the production BOMs, please
                                            see the Master Data section.

                                         BOM structure


                                                                                             A
                                                                                             B




                                         A Main product: pallet                  B BOM: box with glass sheets
                                         Fig. K-13    Product management – BOM with complex box


                                         The illustration shows the BOM structure of such a pallet. You will thus require
                                         a product for the pallet, a product for the box and the glass itself.

                                         Product type
                                         To make sure that A+W Business interprets the pallet and the box as boxes,
                                         product type 200 - Box must be set for both.




                                         Fig. K-14    Product management – Product tab
1.10 / 12-2019




                 K-30                                                                 A+W Business Box Management
                 Tutorial                                                                       Master Data for Boxes




                                     Procurement type and stock booking type
                                     To maintain both products on stock, the procurement type must be set to Stock
                                     withdrawal, and the stock booking type to size-dependent.




                                     Fig. K-15    Product management – tab Stock/Purchasing


                                        Define pallet with BOM
                                        When you define the pallet and the BOM please make sure that the correct
                                        procurement type is adopted.

                                     Standard sizes
                                     Product input at item entry becomes a bit easier if a standard width and a stan-
                                     dard height are entered for the product. After entering the article number, the
                                     matching box article will be automatically selected at item entry in this case.




                                     Fig. K-16    Product management – Product tab (optional)
1.10 / 12-2019




                 A+W Business Box Management                                                                   K-31
                 Master Data for Boxes                                                                                     Tutorial




                                          Price code
                                          Unlike for the boxes known already, the codes for Price-relevant SP/PP are
                                          analyzed for pricing on main product and BOM level.
                                          Previously, the box price used to be calculated and shown only in the box
                                          BOM. For boxes with BOMs, this can be configured by means of the Price-rel-
                                          evant codes. Depending on these codes, the sales price is thus determined by
                                          the price of the BOM element, the price of the main item, or both.
                                          If in our example, the price of the pallet shall consist only of the total prices of
                                          the boxes, i.e. the BOM, the main article's code must be disabled and that of
                                          the first BOM component, i.e. of the box, must be enabled.

                                           Product                      Price-relevant                Price calculation

                                           Pallet                       Yes                           Price per pallet and
                                                                                                      number of boxes
                                           Box                          Yes

                                           Pallet                       Yes                           Price per pallet
                                           Box                          No

                                           Pallet                       No                            Price based on the
                                                                                                      number of boxes
                                           Box                          Yes

                                          Tab. K-1      Pricing in connection with the setting of the 'price-relevant' code

                                          Price management
                                          Price management allows you to enter the box prices as usual.




                 Fig. K-17   Price management – Matrix tab


                                          A matrix with the two limit types Exact width and Exact height can be useful for
                                          example. This allows you to define unit prices for the different sizes.

                                          Stock sizes (product management)
                                          A stock size must be defined for every pallet and box variant in dialog Stock
                                          sizes. The variants are the glass sizes. The procurement type must be set to
1.10 / 12-2019




                                          Stock withdrawal so that the stock size can be kept on stock.




                 K-32                                                                      A+W Business Box Management
                 Tutorial                                                                                Master Data for Boxes




                                              Example

                                              The stock size Pallet with boxes shall consist of 80 boxes each, each of
                                              which again includes 25 sheets.
                                              It is essential that for every size, just one stock size is defined with unique
                                              contents. This means that you must not enter pallets of 50 and pallets with 80
                                              boxes for the size 600 x 700.




                 Fig. K-18   Product management stock sizes – Pallet of 80 boxes and box of 25 sheets


                                          You can define a diversion to other price keys for the stock sizes (as usual).
                                          When the new stock size is saved, you can directly switch from the query to
                                          stock management to define the related stock articles.
1.10 / 12-2019




                 A+W Business Box Management                                                                                K-33
                 Master Data for Boxes                                                                              Tutorial




                                          BOM box in stock management
                                          Stock articles are defined in the same way as product stock sizes. The article
                                          is entered with the same sizes and contents. Additionally, the current stock on
                                          hand and the storage location are defined.
                                          For the automatic creation of stock P.O.s, you also have to fill in the fields Min-
                                          imum stock and P.O. quantity.




                 Fig. K-19   Stock management – Pallets of 80 boxes, box of 25 sheets
1.10 / 12-2019




                 K-34                                                                   A+W Business Box Management
                 Tutorial                                                                            Master Data for Boxes




                                           BOM box at item entry
                                           If you enter the pallet in an item, first enter the article number as usual:
                                           •   If the standard width and height have been defined in product master data,
                                               the box will be automatically created from the product stock sizes.
                                           •   To enter the product with other sizes or if no standard size has been de-
                                               fined, use stock search to select the required pallet.
                                           On the BOM tab, the components are preset with the corresponding contents.




                                                                                                                     A




                                                                                                                            B




                 A Number of boxes on the pallet                      B Number of sheets per box
                 Fig. K-20    Document management – tab BOM: Pallet


                                           The box and its BOM can be entered like any other product. If kept as a stock
                                           article, it can also be used to replenish the stock on hand by means of produc-
                                           tion orders.


                                           Additional information
                                            Sales, “Order Header” on page C-38
                                            Sales, “Change P.O. Code” on page C-306
1.10 / 12-2019




                 A+W Business Box Management                                                                              K-35
                 Orders                                                                           Tutorial




                          Orders
                          Orders for boxes come in two forms:
                          •   Sales order for a customer.
                              If in addition to the boxes produced, you also sell boxes ordered, the set-
                              tings for the suppliers must also be specified on the Supplier tab.
                          •   Production order to fill up stock.
                          This section provides information on the following subjects:
                          •   “Sales Order with Box” on page K-37
                          •   “Production Orders” on page K-41
1.10 / 12-2019




                 K-36                                                  A+W Business Box Management
                 Tutorial                                                                                            Orders




                                          Sales Order with Box
                                          In a sales order, you enter a box for a customer. This box can be removed from
                                          your stock on hand or ordered from a supplier.


                                           How to enter a box as an order item
                                          1 Go to menu Documents > Order > Order and enter the order header.




                                                                                                                         A




                                                                                                                         B




                 A Order area                                        B Order type
                 Fig. K-21   Order header for sales order


                                              Pay attention to the settings for the order area and the order type.
                                          2 Save the data and change to the Items tab.
                                              Item entry opens.
                                          3 Go to the menu Start > New to enter a new item.
1.10 / 12-2019




                 A+W Business Box Management                                                                          K-37
                 Orders                                                                                           Tutorial




                 Fig. K-22   Enter product number of the glass in the box


                                           4 Enter the product number of the glass for which you want to enter an entire
                                             box.
                                           5 Go to the menu Start > Stock search to open the Stock info dialog.
1.10 / 12-2019




                 K-38                                                                 A+W Business Box Management
                 Tutorial                                                                                              Orders




                 A




                 B




                 A Product number of the glass                            B Box (without inventory)
                 Fig. K-23   Stock information on boxes


                                                 The Stock info dialog shows a list of all boxes and stock sizes available for
                                                 this product number. Boxes with the storage location <n.e.>-<n.e.>-<n.e.>
                                                 are boxes that are created as stock articles. Boxes with inventory generally
                                                 have an ID.
                                          6 Adopt the marked box with a double-click.
                                                 Pay attention to the specified dimensions if you are working with different
                                                 boxes for a product.
1.10 / 12-2019




                 A+W Business Box Management                                                                            K-39
                 Orders                                                                                              Tutorial




                                              The dialog is closed and you will find yourself back at item entry.




                 A




                 A Procurement type

                 Fig. K-24   Item with box entered


                                          7 Select the procurement type (A).
                                              •   Stock withdrawal:
                                                  The box will be withdrawn from stock.
                                              •   Order (complete):
                                                  The box will be ordered from the supplier who is entered on the Supplier
                                                  tab.
                                                  For this setting, the order must then be transferred to purchasing.
                                          8 If necessary, correct the quantity if you want to enter more than one box.
                                          9 Go to the menu Start > Save to save the data.
                                              The data is saved. You can now enter additional items and complete the
                                              order as usual.
                                              If you book the goods receipt of the box delivery by a supplier, the boxes
                                              delivered will be assigned to the order. There is a detailed description in the
                                              Purchasing section.
1.10 / 12-2019




                 K-40                                                                    A+W Business Box Management
                 Tutorial                                                                                        Orders




                                     Production Orders
                                     Production orders are used to replenish the stock on hand. All articles entered
                                     in such an order are automatically changed to procurement type Production.
                                     Unlike customer orders, the items are not reserved on stock but are marked
                                     as ordered.

                                     Manual and automatic stock P.O.


                                                                              Stock P.O.
                                                                           Storage location




                                                                           Below minimum
                                                                               stock?



                                                                                  yes




                                                                             Standard P.O.
                                                                               quantity?



                                                                                  yes




                                                                         Search in supplier file




                                                           Standard                                 Internal
                                                           supplier?                               customer



                                                              yes                                     yes




                                                         P.O. proposal                        Production order
                                                           Stock P.O.                      Document management



                                     Fig. K-25    Stock P.O. vs. production order


                                     This flow chart shows A+W Business's reactions to different presettings in the
1.10 / 12-2019




                                     supplier file.
                                     The program checks whether the current stock on hand plus the already or-
                                     dered quantities and minus the reserved quantities will fall below the minimum


                 A+W Business Box Management                                                                      K-41
                 Orders                                                                                               Tutorial




                                           stock on hand. If this is the case, the P.O. proposal shows the multiple of the
                                           (standard) P.O. quantity.


                                           Settings in Supplier File
                                           If a minimum stock and a (standard) order quantity have been defined for the
                                           stock article in dialog Stock management, the system can create automatic
                                           P.O. proposals. These are listed in dialog Stock P.O.
                                           This is how purchase orders of the type Stock P.O. are usually created. How-
                                           ever, if an internal customer is entered in the supplier file instead of a standard
                                           supplier, production orders can be created automatically.




                 Fig. K-26   Internal customer for production orders


                                           In the supplier file, an internal customer is defined for which the production or-
                                           der is entered automatically. The option Internal customer can be enabled on
                                           product group or product level. The product settings have priority over the
                                           product group settings.
1.10 / 12-2019




                 K-42                                                                    A+W Business Box Management
                 Tutorial                                                                                       Orders




                                     Purchase order quantity
                                     The multiplier will be calculated so that as a result of the P.O. proposal the min-
                                     imum stock is exceeded.




                                     Fig. K-27     Quantities for stock articles (dialog Stock management)


                                        Example

                                        Laminated glass with article number 107 is kept as a stock article.
                                        Current stock on hand: 10 pcs.
                                        Minimum stock: 30 pcs.
                                        P.O. quantity: 5 pcs.
                                        The P.O. quantity for laminated glass 107 is calculated as follows:
                                        Difference between current stock on hand and minimum stock on hand: 20
                                        pcs. This difference includes the P.O. quantity of 5 pcs. four times.
                                        P.O. quantity: 4 x 5 = 20 pcs.
                                        Current stock on hand plus ordered quantity: 10 + 20 = 30 pcs.


                                     The calculated quantity is adopted for the P.O. proposal. It can be amended in
                                     the Stock P.O. dialog. How you edit and transfer is described in the Purchasing
                                     section.
                                     The production order is created by the transfer, in the last active order Number
                                     Manager. The production order can be edited and transferred to production.
1.10 / 12-2019




                 A+W Business Box Management                                                                      K-43
                 Orders                                                                          Tutorial




                          Enter production order
                          If you enter production orders manually, you can enter a previously entered or-
                          der by copying it and transferring it to production.

                              Labels for receipt of goods
                              In order to enter a self-produced box in receipt of goods via PDC, a label/
                              barcode is required. For this, the print item 973 must be assigned.

                          This section provides information on the following action sequences:
                          •   “Entering header data for a production order” on page K-44
                          •   “How to enter the glass for the box” on page K-46
                          •   “How to enter a production order by copying” on page K-47


                           Entering header data for a production order
                          1 Go to Documents > Order > Order.
                              The dialog Document management opens. In this description it is the Edit
                              mode.
                          2 Go to the menu Functions > Document > Select NM and check if the correct
                            number manager has been set, and correct the setting if necessary.
                              The allocation of the order to a number manager is also shown in the order
                              header.
                          3 Go to the menu Start > New to switch to the input mode.
1.10 / 12-2019




                 K-44                                                  A+W Business Box Management
                 Tutorial                                                                                        Orders




                                                                                                                       A




                                                                                                                       B




                 A Order area:                                      B Production order
                 Fig. K-28   Header data for production order


                                          4 Enter the required header data.
                                          5 If necessary, enter an explanation for the order in the fields under the
                                            name; for example, that the sheets should be packed in boxes.
                                          6 Choose the order type (B) Production order.
                                          7 Check the other details.
                                          8 Go to the menu Start > Save to save the data.
                                              The header data will be saved. Now you can go to the Items tab and enter
                                              the order items.
                                              The Items tab will be locked again if you change data in the order header.
                                              You have to save the changes to enable the Items tab again.
1.10 / 12-2019




                 A+W Business Box Management                                                                       K-45
                 Orders                                                                                           Tutorial




                                            How to enter the glass for the box
                                           1 Select Documents > Order > Select order > Items tab or <F9>.
                                              Item entry opens.
                                           2 Go to the menu Start > New to enter a new item.
                                           3 Enter the product number of the glass that should be produced as box.




                 Fig. K-29   Enter product number of the glass in the box


                                           4 Set the quantity to the content of the box or a multiple of the content.
                                           5 Select in the menu Start > Save to save the data.
                                              The data is saved. It is transferred to production.
                                              If you enter production orders on a regular basis, you can copy the previ-
                                              ously entered order to make this task easier.
                                              For a detailed description, please see the Sales chapter.
                                              •   Before copying, you have to set the document type of the target docu-
                                                  ment to Production Order.
                                              •   If only certain items shall be adopted from the order, you can select
1.10 / 12-2019




                                                  them.
                                              •   You can amend the data in the new document.




                 K-46                                                                   A+W Business Box Management
                 Tutorial                                                                                            Orders




                                               How to enter a production order by copying
                                              1 Select Documents > Order > Select Order.
                                                 The order entry opens.
                                              2 Select menu Functions > Copy documents.




                 A


                                                                                                                         B




                 A Copy from order to order                                    B Document type of the target order
                 Fig. K-30    Create production order by copying


                                              3 Change to the Copy by item tab and mark the item(s) that should be copied.
                                              4 Correct the target quantity if necessary.
                                              5 To generate the copy, go to the menu Start > Execute.
1.10 / 12-2019




                 A+W Business Box Management                                                                          K-47
                 Stock Management for Boxes                                                                   Tutorial




                                       Stock Management for Boxes
                                       For stock articles, both the goods receipt as well as the goods removal are en-
                                       tered so that you can manage inventories.
                                       The receipt and withdrawal of boxes can be entered using barcodes (PDC) or
                                       manually.
                                       This section provides information on the following subjects:
                                       •   “Stock Management of Boxes” on page K-48
                                       •   “Stock P.O. of boxes” on page K-49
                                       •   “Receipt of Goods via Barcode” on page K-54
                                       •   “Manual Stock Bookings” on page K-60
                                       •   “Shipping of Boxes” on page K-55

                                       Scanning
                                       In connection with AWPort, stock bookings can also be entered via barcode.
                                       This does not only include receipt and withdrawal of goods but also opening
                                       of boxes and other reallocation actions.
                                       By scanning, entire boxes can be allocated to a certain order or order item, or
                                       can be registered for the inventory including the sheets it contains.
                                        “Receipt of Goods via Barcode” on page K-54
                                       For more information on barcodes and barcode formats, please refer to the
                                       documentation on AWPort.


                                       Stock Management of Boxes
                                       Delivered boxes generally have an ID from the supplier with which they are en-
                                       tered when received.
                                       Every box is booked with its own box ID by which it is kept on stock. The
                                       checkbox for assigning virtual item numbers must be checked in the company
                                       data.
                                        “Company Data” on page K-18
                                        “Receipt of Goods via Barcode” on page K-54

                                       Open boxes
                                       To register individual sheets of a box you have to open the box. First, a box
                                       (with ID) is removed from the stock on hand. The number of sheets is then
                                       added to the stock on hand for the corresponding stock article (stock size).
1.10 / 12-2019




                 K-48                                                              A+W Business Box Management
                 Tutorial                                                                  Stock Management for Boxes




                                          Stock P.O. of boxes
                                          The inventory of boxes can either be filled up with an automatically or manually
                                          generated production order.
                                          Stock P.O.s can also be created manually, via document management.
                                           “How to enter a stock P.O. with boxes” on page K-51

                                          P.O. proposals
                                          Purchase orders are usually created through stock management in order to
                                          keep the stock on hand on the required level.




                 A
                 B




                 A Minimum stock                                     B Quantity for P.O. proposal
                 Fig. K-31   Stock management - Stock on hand figures


                                          If you have defined minimum quantities (A) for a stock article in dialog Stock
                                          management, P.O. proposals are created automatically with the stored P.O.
                                          quantity (B). You can check these before they are transferred to Purchasing,
                                          and change the supplier and date if necessary. Transfer to Purchasing turns
                                          the proposal into a stock P.O.
1.10 / 12-2019




                 A+W Business Box Management                                                                        K-49
                 Stock Management for Boxes                                                                       Tutorial




                                       Stock Addition based on Production Order
                                       On tab Stock / PP / EDI in company data, set the limit status for registration
                                       points to define from which point on an order counts as produced. The limit sta-
                                       tus is the status defined for the selected registration point.




                                       Fig. K-32    Company data – Stock / PP / EDI: Registration point for status change


                                       There are two ways of entering additions to stock based on production orders:
                                       •   If the status of the production order exceeds the defined status due to a re-
                                           port from production, the addition to stock is booked automatically.
                                       • If you do not use production reports, you can enter the addition to stock by
                                           means of the manual status report in the Production module. If you set the
                                           production order there to a status above the aforementioned limit, the stock
                                           withdrawal of the material consumed and the addition of produced stock ar-
                                           ticles to stock are booked automatically.
                                       If no other storage location has been defined, the order quantity is allocated to
                                       the standard storage location.
                                       The booking of production orders is described in detail in section Production.


                                       Additional information
                                        Master Data, “Company Data – Stock/Purchasing/EDI” on page B-955
                                        Sales, “Order Header” on page C-38
                                        Sales, “Change P.O. Code” on page C-306
                                        Production, “Production Orders” on page E-128
1.10 / 12-2019




                 K-50                                                                A+W Business Box Management
                 Tutorial                                                            Stock Management for Boxes




                                     Entering manual stock P.O. of boxes
                                     The following guideline shows how to enter a stock P.O. for boxes.
                                     Manual P.O.s are described in detail in the Purchasing section.
                                      Purchasing, “Manual purchase order” on page D-77


                                      How to enter a stock P.O. with boxes
                                     1 Go to the menu Documents > P.O. > P.O.
                                        The dialog Document management opens.
                                     2 Go to field Type and select the entry Stock P.O.




                                        If you set the type to <n.s.>, goods received cannot be automatically added
                                        to stock.
                                     3 Go to the Items tab.
                                     4 Enter the product number, e.g. 1005.
                                        You can specify the number after selecting the stock article. You do not
                                        need to enter sizes as they are taken from the stock article.
                                     5 Go to the menu Start > Stock search to open the Stock info dialog.
                                        You can also open this dialog by pressing <F3>.
1.10 / 12-2019




                 A+W Business Box Management                                                                 K-51
                 Stock Management for Boxes                                                                          Tutorial




                    A




                    B




                   A Product number of glass type                        B Box (without ID)
                   Fig. K-33   Stock info – stock search


                                             The Stock info dialog opens providing a list of all boxes and stock sizes. For
                                             boxes, the entry in column Cont. is greater than 1.
                                         6 Select the required box without box ID and accept it by a double click.
                                             The dialog is closed and you will find yourself back at item entry. In the input
                                             line, you will find that all fields from Quantity onwards are locked for boxes.
                                             The price fields are updated.
1.10 / 12-2019




                 K-52                                                                   A+W Business Box Management
                 Tutorial                                                                   Stock Management for Boxes




                                       A                B
                    A Quantity                                              B Quantity
                    Fig. K-34    Box at item entry


                                           7 Enter the amount required.
                                               The display of details is updated.
                                           8 Repeat steps 4 to 7 to enter all P.O. items.
                                           9 Go to the menu Start > Save to save the data.
                                               The data is saved.
                                           10 Print and send the purchase order.
1.10 / 12-2019




                 A+W Business Box Management                                                                     K-53
                 Stock Management for Boxes                                                                        Tutorial




                                          Receipt of Goods via Barcode
                                          In general, all stock bookings are entered via PDC (plant data collection). For
                                          this, the boxes much each have their own barcode label.

                                              Labels for receipt of goods
                                              In order to enter a self-produced box in receipt of goods via PDC, a label/
                                              barcode is required. For this, the print item 973 must be assigned.


                                           How to enter a box via barcode
                                          1 Go to the menu Documents > P.O.> Receipt of goods > Receipt of goods.
                                          2 Select the Scanner option and scan the box's label.
                                          3 Go to menu Start > Execute.
                                              If you have a barcode for the receipt booking, you can scan it. This way, the
                                              box is included in the inventory in the default stock location.
                                              You can scan and then book all produced boxes one after another.
                                          4 Change to the Item-by-item tab and check the Book complete checkbox for
                                            the box.




                 Fig. K-35   Booking item by item


                                          5 Go to menu Start > Execute.
1.10 / 12-2019




                                              Thus the box is booked and present in the inventory.




                 K-54                                                                   A+W Business Box Management
                 Tutorial                                                                        Stock Management for Boxes




                 Fig. K-36   Warehouse search - box with ID in inventory



                                          Shipping of Boxes
                                          Boxes are usually withdrawn from stock when the delivery note is printed.
                                          Printing of the invoice can also be used as a trigger for the withdrawal.


                                          Withdrawal of boxes
                                          Boxes are usually withdrawn from stock when the delivery note is printed.
                                          Printing of the invoice can also be used as a trigger for the withdrawal.
                                          As the person who enters the order will not know which box is actually going
                                          to be shipped, he first enters a dummy box with the required sizes. The stock
                                          on hand can only be updated after the ID of the real box is entered and with-
                                          drawn from stock.

                                          Example
                                          A dummy box (without ID) with the required sizes is entered in the order. 3 is
                                          specified as the quantity. This reserves three of the dummy boxes.

                                                                                  Withdrawal

                                              Before printing the delivery note          After printing the delivery note

                                              • The real box IDs are scanned in the      • The delivery note is printed.
                                                issuing area.                            • The reserved dummy boxes will be
                                              • Reservation of the dummy box is            withdrawn.
                                                canceled.                                • When the boxes are issued, the
                                              • The three boxes with IDs are marked        three real box IDs are scanned.
                                                as reserved.                             • Reservation of the dummy boxes is
                                              • The delivery note is printed. Three        canceled.
                                                boxes are booked upon issue of           • The three boxes are withdrawn.
                                                goods.

                                          Tab. K-2        Withdrawal of boxes before or after printing the delivery note

                                          The following steps have usually been taken already:
                                          •     The product was entered in the customer order:
1.10 / 12-2019




                 A+W Business Box Management                                                                                K-55
                 Stock Management for Boxes                                                                    Tutorial




                   Fig. K-37   Product 1005 entered


                                         •   [F1] in the Stock info dialog was used to select the dummy box:




                                                                                                                 A




                                                                                           B

                   A Dummy box without ID              B Reservation of dummy box
                   Fig. K-38   Selection of the dummy box


                                         •   The box was added to the order and saved, e.g with an item quantity of 3:




                   Fig. K-39   Item quantity 3 saved
1.10 / 12-2019




                                         •   3 additional reservations were booked for the dummy box on stock:



                 K-56                                                               A+W Business Box Management
                 Tutorial                                                                 Stock Management for Boxes




                                                                                            A
                    A Reservation of dummy box increased by 3
                    Fig. K-40   Reservation


                                          •   The booking journal (stock management) shows the item quantity as re-
                                              served:




                                          Fig. K-41    Order item reserved


                                          Next, boxes with IDs are allocated and withdrawn after printing the delivery
                                          note.
1.10 / 12-2019




                 A+W Business Box Management                                                                      K-57
                 Stock Management for Boxes                                                                  Tutorial




                                         Booking of issued goods

                                          How to book the issue of boxes
                                         1 Go to the menu Production > Dispatch > Issue of boxes.




                   Fig. K-42   Issue of boxes – load customer order


                                         2 Select the option By scanner.
                                         3 Enter the barcode of the order number and item number.
                                            The numbers appear in the Document fields.
                                            If you are not using a scanner, choose the option By order number and en-
                                            ter the number.
                                         4 To import order data, select Start > Execute.
                                            The display switches to the ID tab.
1.10 / 12-2019




                 K-58                                                              A+W Business Box Management
                 Tutorial                                                                 Stock Management for Boxes




                    Fig. K-43   Order item with sub-items


                                             Each box is shown in a separate line as a virtual item. The fields in column
                                             ID are empty as no box with an ID has been allocated.
                                          5 Scan the box ID of the first box to be reserved.
                                             If you do not use a scanner, go to field ID and select one of the displayed
                                             IDs. The list only shows box IDs of the defined type.
                                          6 To alocate the boxes, go to the menu Start > Execute.
                                          7 Repeat steps 5 and 6 to allocate more boxes with IDs.


                                          Additional information
                                           Master Data, “Company Data – Parameters” on page B-934
                                           Master Data, “Use virtual item numbers” on page B-940
                                           Sales, “Stock Info” on page C-736
                                           Software Reference, “Issue of Goods” on page E-236
1.10 / 12-2019




                 A+W Business Box Management                                                                       K-59
                 Stock Management for Boxes                                                                  Tutorial




                                       Manual Stock Bookings
                                       If you are not working with PDC, you also start all stock bookings manually.
                                       This section provides information on the following subjects:
                                       •   “Manual input of addition” on page K-60
                                       •   “Change storage location of a box” on page K-64
                                       •   “Correcting the box contents (number of sheets)” on page K-65
                                       •   “Opening (resolving) boxes” on page K-66


                                       Manual input of addition
                                       You can receive boxes manually into inventory or withdraw them from inven-
                                       tory.

                                           Prerequisite
                                           The checkbox for the virtual assignment of item numbers must be checked
                                           in company data.

                                            “Company Data” on page K-18
                                       The following instructions exist for this training module:
                                       •   “How to set the ID for boxes” on page K-60
                                       •   “How to create a new box in inventory” on page K-60
                                       •   “How to book the dispatch of goods manually” on page K-62


                                        How to set the ID for boxes
                                       1 Go to the menu Documents > P.O.> Receipt of goods > Receipt of goods.
                                       2 Go to the menu Options > Group > ID number allocation > Settings.




                                       3 Replace the sequence of letters with the desired ID.
                                           Please avoid overwriting the placeholders for the numbers.
                                       4 Click on [OK] to save the changes.
1.10 / 12-2019




                                        How to create a new box in inventory
                                       1 Go to menu Stock management > stock management.


                 K-60                                                               A+W Business Box Management
                 Tutorial                                                                 Stock Management for Boxes




                                           The Stock management dialog is displayed.
                                        2 From the menu, select Options > Assign ID number automatically.
                                           This way, the automatic ID is assigned for boxes with the new ID. Counting
                                           begins with each new ID at 1 and is incremented by 1 each time.
                                           The Ident field on the Stock article tab is locked.
                                        3 In the Article field, enter the product number of the glass for which a box
                                          should be booked.
                                        4 Go to menu Start > Search.




                                                                                                                   C



                 A




                                                                                                                   D



                 B




                 A Storage location                               C Box
                 B Stock on hand                                  D Stock article without ID
                 Fig. K-44   Box data


                                        5 Mark the box (C, D) for which you want to enter the stock on hand.
                                           Thus, all required data will be taken over and you can create a new box in
                                           the stock on hand.
                                        6 Go to the menu Start > New.
                                           The fields will be enabled.
                                        7 Select the storage location (A) where the new box is located.
                                        8 Enter the number 1 in the Stock on hand field.
1.10 / 12-2019




                                           Since each box should have its own ident number, you may only enter 1.
                                        9 Go to the menu Start > Save to save the data.


                 A+W Business Box Management                                                                     K-61
                 Stock Management for Boxes                                                                    Tutorial




                                          In the field for the stock on hand, a new box is displayed with an ID.
                                       10 Repeat steps 6 and 9 until you have included all boxes in the stock on
                                          hand.
                                          Pay attention here whether all boxes should be booked to the same stor-
                                          age location. You don't need to change any other values until you have
                                          booked all boxes.


                                        How to book the dispatch of goods manually
                                       1 Go to menu Stock management > Stock movement > tab Dispatch
                                       2 Enter the either the product number or the ident number of the box and se-
                                         lect Start > Search in the menu.
                                          The search will be restricted to this box in that case.
                                          Alternatively, you can restrict the search to a product code and the storage
                                          place.
                                          Section Storage locations lists all stock articles matching the search crite-
                                          rion.
1.10 / 12-2019




                 K-62                                                               A+W Business Box Management
                 Tutorial                                                             Stock Management for Boxes




                                        Fig. K-45    Manual stock dispatch of boxes


                                     3 Mark the box that you want to withdraw.
                                     4 Enter a 1 in the Quantity field in order to reduce the stock on hand by the
                                       marked box.
                                     5 If necessary, change the booking date and enter a note.
                                     6 Go to menu Start > Save to save the data.
                                        Data will be saved, and the stock on hand set to 0.
1.10 / 12-2019




                 A+W Business Box Management                                                                 K-63
                 Stock Management for Boxes                                                                    Tutorial




                                       Change storage location of a box
                                       This module will show you how to move a box from one storage location to an-
                                       other. This movement will be entered with a rebooking. This way, the stock ar-
                                       ticle will be booked from the old storage location as a withdrawal and as an
                                       addition to the new one.


                                        How to transfer the storage location
                                       1 Go to menu Stock management > Stock movements.
                                          Dialog Stock movement opens.
                                       2 Go to tab Transfer.
                                       3 Enter the product number in the Product field or the (box) ID.
                                       4 To start the search, go to the menu Start > Search.

                                                                              A                       B




                                          A Current storage location               B Select new storage location
                                          Fig. K-46    Stock movement – Transfer


                                       5 Mark the box that you want to transfer to another storage location.
                                       6 Choose the new storage location in section storage location (B).
                                       7 Go to menu Start > Save to save the data.
                                          The box is withdrawn from the old storage location, and added to the new
                                          one.
1.10 / 12-2019




                                          If you have activated the Log when finished option, the Stock history dialog
                                          opens. You can then print out all stock movements as a log.



                 K-64                                                               A+W Business Box Management
                 Tutorial                                                            Stock Management for Boxes




                                     Correcting the box contents (number of sheets)
                                     If you find out in the warehouse that the content of a box does not match the
                                     quantity shown on the delivery note, the number of sheets needs correcting.
                                     This module will show you how to correct the contents of a box.

                                        Only boxes with ID
                                        The content of a box can be changed only if the box has been entered with
                                        its own box ID.


                                      How to correct the number of sheets in a box
                                     1 Go to menu Stock management > Stock movements.
                                        Dialog Stock movement opens.
                                     2 Go to tab No, of sheets.
                                     3 Enter the product number in the Product field or the (box) ID.
                                     4 To start the search, go to the menu Start > Search.

                                                                                A                            B




                                        A Box                                   B Number of sheets
                                        Fig. K-47    Correct the number of sheets


                                     5 Select the required box (A).
                                        Field Contents is enabled.
1.10 / 12-2019




                                     6 Enter the new number of sheets (B).




                 A+W Business Box Management                                                                 K-65
                 Stock Management for Boxes                                                                   Tutorial




                                       7 Go to menu Start > Save to save the data.
                                          The data is saved.


                                       Opening (resolving) boxes
                                       You can open boxes in order to make the sheets available for production or
                                       enter them individually in the order. You can only open boxes with an ID.

                                          Stock articles with sheet dimensions must be created
                                          If you break up a box, the sheets are booked to the stock on hand. The
                                          stock sizes for the sheets are created automatically if necessary. IN this
                                          case, the sheets are booked to the storage location of the opened box.


                                        How to open a box
                                       1 Go to menu Stock management > Stock movements.
                                          Dialog Stock movement opens.
                                       2 Go to tab Open boxes.
                                       3 Enter the product number in the Product field or the (box) ID.
                                       4 To start the search, go to the menu Start > Search.

                                                                                   A                   B        C




                                          A Box shall be opened                  B Content
                                                                                 C Number of boxes
                                          Fig. K-48    Stock movement – Open box
1.10 / 12-2019




                                       5 Select the required box.



                 K-66                                                              A+W Business Box Management
                 Tutorial                                                              Stock Management for Boxes




                                        CThe fields Number of boxes and Different contents are enabled.
                                     6 Enter 1 in field Number of boxes and check if the contents of the box are
                                       correct.
                                        If necessary, correct the entry in field Different contents.
                                     7 Go to menu Start > Save to save the data.
                                        The box will be booked out and the lite as stock articles.
                                     8 If necessary, update the view of storage locations by reloading them.
                                     9 If necessary, delete the empty box from the stock on hand manually.
1.10 / 12-2019




                 A+W Business Box Management                                                                 K-67
                 Stock Management for Boxes                        Tutorial
1.10 / 12-2019




                 K-68                         A+W Business Box Management
Box Management                  K

                 Software Reference




                  A+W Business
                 Software Reference                                                                     Overview




                                      Overview
                                      Use the module Stock Management to maintain and analyze all data concern-
                                      ing stock. Furthermore, use this module to carry out the inventory and book
                                      stock movements.
                                      The Software Reference provides information on the following subjects:
                                      •   “Stock Management” on page K-72
                                      •   “Stock Movement” on page K-83
                                      •   “Search” on page K-90
                                      •   “Stock P.O.” on page K-96
                                      •   “Receipt and Shipping of Boxes” on page K-102
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                 K-71
                 Stock Management                                                             Software Reference




                                    Stock Management
                                    Stock management > Stock management
                                    Use the dialog Stock management to display all the stock articles that are
                                    managed.
                                    This section provides information on the following subjects:
                                    •   “Menus in Stock Management” on page K-72
                                    •   “Stock Management” on page K-73


                                    Menus in Stock Management
                                    Stock management > Stock management
                                    The menus can be used to define the standard settings of the dialog or open
                                    other dialogs without closing this dialog.
                                    This section provides information on the following subjects:
                                    •   “Functions Menu” on page K-72
                                    •   “Options Menu” on page K-73


                                    Functions Menu
                                    Stock management > Stock management > Functions menu
                                    This menu allows you to open other dialogs without closing stock manage-
                                    ment.
                                    The following entries are displayed:
                                    •   Stock History:
                                        Opens the dialog Stock History with the log of processes that have been
                                        booked in stock management.
                                    •   Booking Journal:
                                        Opens the dialog Booking Journal with the log of stock bookings from or-
                                        ders and purchase orders.
1.10 / 12-2019




                 K-72                                                         A+W Business Kistenmanagement
                 Software Reference                                                                 Stock Management




                                      Options Menu
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

                                          Stock management at the level of bills of material
                                          In the warehouse, you can also manage products that are included as bill
                                          of material components in other products. For this purpose, the checkbox
                                          Stock keeping at BOM level must be enabled in the company data.

                                           Master Data, “Stock control on BOM level” on page B-958
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                     K-73
                 Stock Management                                                                    Software Reference




                                          Stock Management - Stock Articles
                                          Stock management > Stock management > Stock articles tab




                 Fig. K-49   Stock management - stock articles


                                          Use this tab to check the articles that are managed in the warehouse. The
                                          shown stock is updated with each stock booking. You can add new articles and
                                          correct the different quantities.
                                          For ordering purposes, you furthermore define minimum quantities and pur-
                                          chase order quantities.
                                           Tutorial, “How to create a stock article” on page K-26

                                          Articles

                                          Articles Product number according to master data. If you want to enter a new
                                          stock article, you have to enter it in the master data first.

                                          Stock ID Identification number, assigned on receipt of goods.

                                          Name Product names from the master data.

                                          Width x height / content Dimensions of the stock article in mm (only stock
                                          sizes) and content of box. For boxes, enter the number of sheets per box. For
1.10 / 12-2019




                                          all other stock articles, a 1 is automatically shown.




                 K-74                                                                  A+W Business Kistenmanagement
                 Software Reference                                                               Stock Management




                                      Variant If variations have been entered for an article, you will see the color
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

                                      ID The box ID, is assigned on receipt of goods or manually. The ID is only
                                      shown if you have selected a box in the overview of stock articles.

                                      Details

                                      Category If you have defined stock categories in the master data, you can
                                      use this field as a search criterion. When you enter new stock articles you can
                                      allocate a category.

                                      Del. ID The supplier's box ID is only shown if you have selected a box in the
                                      Stock articles section.

                                      Main article You can link stock articles with several dimensions by specify-
                                      ing a main product. The stock check (for the stock preview in the Stock info
                                      dialog) is then only executed for the main product and you only need to enter
                                      minimum stock for this main product.
                                      If you have also defined minimum stock for the allocated stock articles, they
                                      will be ignored for the check.
                                       Tutorial, “Stock Management” on page K-14

                                      Prod. batch / date Not currently used.

                                      Date Date at which the stock article has been changed last time.

                                      In production In connection with A+W Production you can determine wheth-
                                      er the stock article has been allocated to production.
                                      ☐ The stock article is disposable.
                                      ☑ The stock article has been allocated to production (info only).

                                      Stock on hand

                                      Stock on hand Displays the current stock. The stock is updated with each
                                      booking of outgoing or incoming stock. For boxes with an ID, stock 1 is always
1.10 / 12-2019




                                      shown.
                                      If you have created the stock article new, the field is enabled and you can enter
                                      the opening stock.


                 A+W Business Kistenmanagement                                                                   K-75
                 Stock Management                                                               Software Reference




                                    Stock > 0 This checkbox is only available in the selection mode. Use it to de-
                                    fine as a search criterion whether articles should be shown without stock quan-
                                    tity.
                                    ☐ The search result also shows articles, the current stock of which is 0.
                                    ☑ The search result only shows articles, the current stock of which is at least 1.

                                    Min. stock The minimum stock forms the basis for automatic purchase order
                                    suggestions. They are created if stock falls below the minimum stock. Reser-
                                    vations and purchase orders are taken into account. You can check these au-
                                    tomatic purchase order suggestions in the dialog Order pool.
                                     “Stock P.O.” on page K-96

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

                                    Target quantity Not currently used.

                                    Inventory audit per stock location If you maintain stock per storage loca-
                                    tion you can check the stock per stock location.
                                    ☐ Stock is checked jointly for all storage locations.
                                    ☑ Stock is checked per storage location.

                                    Stock articles
                                    The lists show stock articles that correspond to the search criteria. The top list
                                    shows all stock articles together. If you select one entry, the articles are shown
                                    per storage location in the bottom list. If the checkbox Stock > 0 has been ac-
                                    tivated, only storage locations with stock of more than 0 are listed.
                                    The following columns are displayed:
1.10 / 12-2019




                                    •   Articles, Quantity unit - Variation:
                                        Article number, name, quantity unit and color from stock management.
                                    •   Width, Height:
                                        Dimensions from stock management.

                 K-76                                                           A+W Business Kistenmanagement
                 Software Reference                                                                    Stock Management




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
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                    K-77
                 Stock Management                                                                       Software Reference




                                          Stock Management - Prices
                                          Stock management > Stock management > Prices tab




                 Fig. K-50   Stock management - prices


                                          This tab shows the current prices for a stock article. During updates, orders,
                                          purchase orders and stock rebookings are taken into account.

                                             Prerequisite
                                             The average purchase price (average PP) is only calculated and shown if
                                             the checkbox Determine average purchase price has been enabled in the
                                             company data.

                                              Master Data, “Average PP: The average purchase price will be recalculated in
                                               the following cases:” on page B-955
                                          The fields in the lists are described in detail in connection with the Stock Article
                                          tab.
                                           “Stock Management - Stock Articles” on page K-74

                                          Purchase prices

                                          Lowest price The lowest price this article has been purchased at.
1.10 / 12-2019




                                          Max. price The highest price this article has been purchased at.

                                          Last price The latest price this article has been purchased at.


                 K-78                                                                  A+W Business Kistenmanagement
                 Software Reference                                                                 Stock Management




                                      Stock value The current stock prices are shown in this column. They are the
                                      result from the respective price and the quantity.

                                      Calculation of the average price (average PP)
                                      By selecting an option, determine which stock sizes should be taken into ac-
                                      count on this list for the calculation. This setting only makes sense for lite with
                                      different stock sizes.
                                      •   Only this article:
                                          For the calculation only the displayed article in the selected size is taken
                                          into account. The PP history of the current article is displayed.
                                      •   All sizes:
                                          For the calculation all dimensions of the displayed glass are taken into ac-
                                          count. The PP history of all dimensions of the article is displayed.
                                      The average PP is calculated for each goods receipt, regardless of how it has
                                      been booked. Goods issued only reduce the stock. The list is reduced by ar-
                                      chiving and auditing.
                                      The first data record shows the opening stock and the original price. Under-
                                      neath you will find the goods received and issued (minus sign). If goods have
                                      been received as a result of a stock P.O., the P.O. number and the P.O. item
                                      are furthermore displayed.
                                      The average PP is updated during entering or changing purchase orders. It is
                                      determined by taking the total quantity into account.

                                          Example:

                                          100 pieces      on stock                each 15.00 €              1500.00 €

                                           40 pieces      new booking             each 18.00 €     +         720.00 €

                                                                                                   =        2200.00 €
                                                                                                            ========
                                          2200.00/140 pcs. = 15.86 €



                                      Automatic surcharges that are listed in the purchase orders, e. g. energy and
                                      transportation surcharge, are also included in the calculation.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                     K-79
                 Stock Management                                                                 Software Reference




                                    Overview The respective average prices are shown as history. This way, you
                                    can easily monitor price developments. Details displayed:
                                    •   Date:
                                        Date of the last update.
                                    •   Quantity [QU]:
                                        Quantity issued or received and quantity unit.
                                    •   Price/PU:
                                        Purchase price per price unit at the time of booking.
                                    •   Stock on hand [QU]:
                                        Stock on hand at the displayed date. If the average PP is shown for all di-
                                        mensions, the stock on hand is always shown in sqm.
                                    •   Average price / PU:
                                        Average price per price unit at the time of booking.
                                    •   P.O. / item:
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
                                        during archiving or invoice check. As a result, the view remains clearer.
                                        A+W Business assumes that the prices will not be changed anymore after
                                        these processes. However, if you still change prices after one of the pro-
                                        cesses, these changes are not included in the calculation of the average
                                        price.
1.10 / 12-2019




                 K-80                                                            A+W Business Kistenmanagement
                 Software Reference                                                                     Stock Management




                                         Stock Management - Supplement
                                         Stock management > Stock management > Supplement tab




                 Fig. K-51   Stock management - supplement


                                         On this tab reservations for a selected stock article are shown.
                                         The fields in the lists are described in detail in connection with the Stock Article
                                         tab.
                                          “Stock Management - Stock Articles” on page K-74

                                         Reservation
                                         The fields in this area are enabled for individual customers only.

                                         Customer Number and name of customer for whom the selected stock article
                                         is reserved.

                                         Fully locked Not currently used.

                                         Exclusive reservation Not currently used.

                                         Supplier
1.10 / 12-2019




                                         Supplier Number and name of supplier from whom the stock article is or-
                                         dered.




                 A+W Business Kistenmanagement                                                                         K-81
                 Stock Management                                                            Software Reference




                                    Remark

                                    Product related, Storage location related You can enter additional infor-
                                    mation for each stock article and each storage location, e. g. when and from
                                    which supplier glass/boxes were supplied, so that older deliveries are used
                                    first.
1.10 / 12-2019




                 K-82                                                        A+W Business Kistenmanagement
                 Software Reference                                                                  Stock Movement




                                      Stock Movement
                                      Stock management > Stock movement
                                      You can manually book withdrawals and additions for stock articles, correct
                                      stock figures, rebook storage locations and resolve boxes.
                                      This section provides information on the following subjects:
                                      •   “Options Menu” on page K-83
                                      •   “Stock Movement” on page K-83


                                      Options Menu
                                      Stock management > Stock movement
                                      The following entries are displayed:
                                      •   Protocol at shut down:
                                          When exiting the dialog, the stock history is automatically shown.
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
                                      •   Stock Movement – Number of Sheets
                                      •   Stock Movement – Open Boxes
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-83
                 Stock Movement                                                               Software Reference




                                  Stock Movement – Dispatch, Addition
                                  Stock management > Stock movement > Dispatch tab, Addition tab




                                  Fig. K-52    Stock movement – dispatch, addition


                                  You can manually book goods issued and received on the Dispatch and Addi-
                                  tion tabs. You can select a certain stock article and enter the corresponding
                                  data. If you have all stock articles displayed you can select the requested arti-
                                  cle on the Storage places list. The fields in the Change stock on hand section
                                  are then enabled.
                                   Tutorial, “Stock Management for Boxes” on page K-48
                                  If you have activated the option Protocol at shut down, the stock history is au-
                                  tomatically shown on the Table tab when you close the dialog.

                                     Manually enter addition of boxes
                                     Since every box is kept with its own ID, you can enter additions of boxes
                                     only via Goods Receipt or Stock Management. In Stock Management, you
                                     create the box as a new stock article.
1.10 / 12-2019




                 K-84                                                        A+W Business Kistenmanagement
                 Software Reference                                                                  Stock Movement




                                      Stock product

                                      Product Number and name of the stock article.

                                      ID no. You can only book stock dispatches via the ID no. Additions of boxes
                                      must be defined in Stock Management so that you can enter a new ID. Boxes
                                      added have to be defined in inventory management in order to enter a new ID.

                                      Content If you have selected a box, then its content is displayed. If a box with
                                      an ID no. that has already been allocated to an order is to be delivered or
                                      opened, a message is displayed. This prevents that negative stock is created
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

                                      Width, height These fields are only filled with quantity unit sqm if it involves
                                      stock sizes.

                                      Assessment price Enter the purchase price at which the goods received
                                      were supplied.

                                      Booking date The current date is shown automatically. It can be changed if
                                      required.

                                      Remark You can enter a remark or select from the combo box. The remark
                                      will be displayed in the stock history.
                                      Use the button to add a new remark to the list.
                                       “Remark (Stock Movement)” on page K-89

                                      Storage locations
                                      •   Color:
                                          The color is only shown for variations.
                                      •   Width, Height:
1.10 / 12-2019




                                          Dimensions are only shown if the product has been defined as a stock size
                                          or box.




                 A+W Business Kistenmanagement                                                                  K-85
                 Stock Movement                                                                 Software Reference




                                  •   Contents:
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




                                  Fig. K-53     Stock movement – transfer


                                  Use this tab to book a stock article to a different storage location. When you
                                  transfer a storage location, the entire stock of this storage location is always
                                  booked to the other storage location.
                                   Tutorial, “How to transfer the storage location” on page K-64
                                  The fields in sections Stock product and Storage locations are described under
                                  tab Dispatch.
1.10 / 12-2019




                                   “Stock Movement – Dispatch, Addition” on page K-84




                 K-86                                                          A+W Business Kistenmanagement
                 Software Reference                                                                    Stock Movement




                                      Storage location

                                      Storage location Displays the current storage place. You can allocate a dif-
                                      ferent storage place. The combo box lists all stored storage places.

                                         Storage location <n.e.>
                                         Even if you have defined your own storage locations, storage locations
                                         <n.e.> will remain and can be booked.


                                      Stock Movement – Number of Sheets
                                      Stock management > Stock movement > No. of sheets tab




                                      Fig. K-54    Stock movement – number of sheets


                                      Use this tab to correct the content of boxes.
                                       Tutorial, “How to correct the number of sheets in a box” on page K-65
                                      The fields in sections Stock product and Storage locations are described under
                                      tab Dispatch.
                                       “Stock Movement – Dispatch, Addition” on page K-84

                                      Content change

                                      Content Only if a box with an ID has been selected, the number of sheets
                                      that should in the box, is displayed. You can correct this value.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-87
                 Stock Movement                                                               Software Reference




                                  Stock Movement – Open Boxes
                                  Stock management > Stock movement > Open boxes tab




                                  Fig. K-55    Stock movement – open boxes


                                  Use this tab to resolve boxes so that the individual sheets are available for pro-
                                  duction. During this process, the box is booked out of the inventory and the
                                  number of sheets is booked to the inventory of the stock size.
                                   Tutorial, “How to open a box” on page K-66

                                     Book box content to a different storage location
                                     When you open a box, its content is booked to the same storage location
                                     of where the box is located. If you want to transfer the content, you must
                                     book it out of the previous storage location and subsequently, book it to the
                                     new storage location.

                                  The fields in sections Stock product and Storage locations are described under
                                  tab Dispatch.
                                   “Stock Movement – Dispatch, Addition” on page K-84

                                  Open box
                                  If a box with an ID no. that has already been allocated to an order is to be de-
                                  livered or opened, a message is displayed. This prevents that negative stock
                                  is created by the subsequent printing of the delivery note or invoice.
1.10 / 12-2019




                                  No. of boxes Number of boxes that are to be opened.

                                  Different contents The number of sheets is shown only if you have selected
                                  a box. You can correct this value.


                 K-88                                                         A+W Business Kistenmanagement
                 Software Reference                                                                 Stock Movement




                                      Remark (Stock Movement)
                                      Stock > Stock movement > [Remark]




                                      Fig. K-56    Remark concerning stock movement


                                      Use this dialog to store remarks that are offered for selection in the Stock
                                      movement dialog. If you leave the first line blank you can also delete an allo-
                                      cated remark.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                 K-89
                 Search                                                              Software Reference




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
1.10 / 12-2019




                 K-90                                                    A+W Business Kistenmanagement
                 Software Reference                                                                              Search




                                          Stock Search – Stock Search
                                          Stock management > Search > Stock search tab




                 Fig. K-57   Stock search – stock search


                                          Use this tab to display the current stock on hand, reserved quantities and fu-
                                          ture stock on hand for stock articles.
                                           Tutorial, “Stock control mode and reservation” on page K-12

                                          Selection
                                          The fields are only enabled in selection mode.

                                          Product Product number by which the product has been entered in the mas-
                                          ter data.

                                          Type Product type this product has been assigned to in the master data.

                                          Group Product group this product has been assigned to in the master data.

                                          ID Identification number by which the stock article has been entered in the
                                          stock, e. g. for a box.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                     K-91
                 Search                                                                  Software Reference




                          Category If you have defined stock categories in your company, these can
                          be used as filters.
                           Master Data, “Stock Categories” on page B-738

                          Color (Color) variations that have been defined for the selected product.

                          from, to PGR You can also enter product groups or product group areas.
                          The overview then displays all the products of the selected product groups.

                          Thickness / width / height These details are transferred from stock man-
                          agement. Width and height are only displayed if the selected item has been
                          entered as a stock size or box, including the corresponding details.

                          Storage location If you are using different storage locations, the storage lo-
                          cation of the selected item will be shown, including all defined levels.
                           Master Data, “Stock Definition” on page B-736

                          Del. ID Identification number of the shipment from stock management. It is
                          not identical with the entry in the ID column.

                          Remark Information stored for the selected item when delivered.

                          Contents from, to You can use the contents as a search criterion in the se-
                          lection mode, e.g. all boxes with a content of 50 pieces. Contents = 1 always
                          means stock size.

                          Availability Displays the available pieces.

                          Filter options
                          If no filter is set, no stock will be displayed. A filter is set if the corresponding
                          checkbox is ticked. The following filters are available:
                          •   Stock articles:
                              Stock articles will be displayed.
                          •   Boxes (contents > 1):
                              Boxes with a content of > 1 will be displayed.
                          •   Stock sizes (contents = 1):
                              Stock sizes will be shown. Display of the quantity (= 1) helps to distinguish
                              boxes of identical sizes.
                          •   Group boxes by storage location and supplier:
                              Only one line is displayed per storage location and supplier.
                          •   Articles without sizes:
                              Even stock articles for which no sizes have been entered will be shown.
                          •   No boxes with ID:
                              Boxes entered with an ID at receipt of goods shall not be shown.
                          •   Minimum qty > 0:
                              Only stock articles with a minimum quantity of over 0 should be displayed.
                          •   Stock > 0:
1.10 / 12-2019




                              Only stock articles with actual stock should be displayed.
                          •   Stock = 0:
                              Only stock articles without stock should be displayed.


                 K-92                                                   A+W Business Kistenmanagement
                 Software Reference                                                                          Search




                                      •   Stock < 0:
                                          Only stock articles that have been reserved, but are without stock, should
                                          be displayed.

                                      Print options
                                      You can define the sorting of the list for printing purposes. The appropriate
                                      checkboxes will be enabled with the selected option. You can then additionally
                                      define where a subtotal will be printed.
                                      The following entries are displayed:
                                      •   Group by product no.:
                                          The checkbox Subtotal by product group is enabled.
                                      •   Group by product type/group:
                                          The Subtotal by superior product group checkbox is enabled.
                                      •   Group by product group:
                                          The Subtotal by main product group checkbox is enabled.

                                      Overview
                                      The overview lists all products that have been selected by means of the
                                      search. The columns provide details on the stored products.
                                      The reserved quantities will be updated as soon as a corresponding item has
                                      been saved in the order. The details in column Stock on hand will be updated
                                      when a delivery note is issued.
                                      The entries in the hit list are identified with the following colors:
                                      • Black:
                                         Quantity-based stock article
                                      • Blue:
                                         Stock article not quantity-based
                                      • Red:
                                         – No stock article: articles that are not kept on stock.
                                         – This applies also to products which are no longer available, or which
                                            show negative quantities. Negative quantities occur if the stock on hand
                                            and the order quantity minus the reserved quantity <= 0.

                                      Totals
                                      The totals of the selected products are shown. If you have selected a PGR with
                                      different products, the totals of the selected product are shown.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-93
                 Search                                                                                 Software Reference




                                           Stock Search - Future Stock on Hand
                                           Stock management > Search > Future stock on hand tab




                 Fig. K-58   Stock search - future stock on hand


                                           Use this tab to check whether the replacement times for a certain product are
                                           sufficient to delivery an order in accordance with the schedule. The color red
                                           shows that scheduled dates cannot be met. Yellow indicates that the replace-
                                           ment time is sufficient if the purchase orders are received on time.
                                           The replacement time results from the delivery time that has been defined in
                                           the supplier file for the article and the supplier's route days that are defined in
                                           route management.

                                           Preview up to
                                           The preview always starts with the current date. Set the number of days for the
                                           preview in the company data, e. g. 14 days.
                                           • The list at the top shows the data for each selected product in one line.
                                           • The list in the center shows the stock on hand per day.
                                           • The list at the bottom displays details on the selected product.
1.10 / 12-2019




                                           The lines are red if production is impossible because the reservations exceed
                                           the stock on hand.




                 K-94                                                                   A+W Business Kistenmanagement
                 Software Reference                                                                              Search




                                      In order to increase the performance you can restrict the preview display by
                                      the following settings:
                                      •   You can remove certain articles from the stock preview and availability
                                          check in dialog Product management > tab Stock/Purchasing > No avail-
                                          ability check checkbox, by disabling the availability check for these articles.
                                      •   In the Company data dialog you can set the time period displayed in the
                                          preview.
                                      •   You can link several stock sizes together in the dialog Stock management
                                          so that the stock check is only executed for the defined main stock article.
                                           “Main article” on page K-75
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                     K-95
                 Stock P.O.                                                              Software Reference




                              Stock P.O.
                              Stock management > Stock P.O.
                              Use this dialog to check all suggested stock P.O.s and transfer them to Pur-
                              chasing.
                              This section provides information on the following subjects:
                              •   “Order Pool Menus” on page K-96
                              •   “Order Pool” on page K-99


                              Order Pool Menus
                              By using the menus you can have the date fields updated automatically and
                              open other dialogs additionally.
                              This section provides information on the following subjects:
                              •   “Functions Menu” on page K-96
                              •   “Options Menu” on page K-97


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
1.10 / 12-2019




                 K-96                                                   A+W Business Kistenmanagement
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
                                          puter. The following descriptions represent the activated option.

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
                                          If lead days have been defined for PGR combinations, these will be used
                                          to calculate the delivery date.
                                           Master Data, “Lead days” on page B-567
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                    K-97
                 Stock P.O.                                                               Software Reference




                              Product name group
                              •   Product names as per the supplier file:
                                  The names of the ordered products are adopted from the supplier file.
                              •   Product names as per master data (internal P.O.):
                                  For internal purchase orders, the names of the ordered products are load-
                                  ed from the product master data.

                              Other group
                              •   No saving of costs:
                                  Costs are not written back to the purchase prices of the order.
                              •   Consider size surcharges:
                                  Size surcharges will be transferred with the P.O.
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
                                  The P.O. automatically shows the name of the user logged on to A+W Busi-
                                  ness.
                              •   Check change of status:
                                  The query concerning the change of status is displayed.
                              •   Repeat transfer only up to lock status:
                                  Purchase orders can be transferred several times but only until lock status
                                  has been reached.

                              Further settings group
                              •   Settings:
                                  Opens the Further settings dialog in which you can define information con-
                                  cerning printing texts and file attachments.
1.10 / 12-2019




                 K-98                                                    A+W Business Kistenmanagement
                 Software Reference                                                                            Stock P.O.




                                          Order Pool
                                          Stock management > Stock P.O.




                 Fig. K-59   Order pool


                                          In this dialog you can view all suggested purchase orders for articles that fall
                                          short of the minimum stock. The order quantity is calculated by the quantity
                                          that has been defined in the dialog Stock management.
                                          After the transfer, the purchase orders are created and can be printed and
                                          sent.
                                           Tutorial, “Stock P.O. of boxes” on page K-49
                                           Tutorial, “Manual and automatic stock P.O.” on page K-41

                                          Storage location

                                          Warehouse, Corridor, Shelf, Tray You can restrict the display to individual
                                          storage locations. Please remember that stock articles may be booked to stor-
                                          age location <n.e.>. If you do not restrict the selection, purchase order sug-
                                          gestions are displayed for all articles that fall short of the minimum stock.
                                          The name of the storage locations can be changed in the master data.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                       K-99
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

                              Target Number Manager

                              Employee Name of the employee logged in to A+W Business or who has set
                              up the Number Manager. If you create a new Number Manager you can allo-
                              cate it to one particular employee.
1.10 / 12-2019




                              Name Name of the target Number Manager for the purchase orders. A new
                              Number Manager will be created when you enter a new name.




                 K-100                                                   A+W Business Kistenmanagement
                 Software Reference                                                                    Stock P.O.




                                      Target number area

                                      Client If you have set up separate number areas for your clients you can se-
                                      lect the requested client here.

                                      Production preparation If you work with production preparations, you can
                                      allocate the purchase order to a certain order area.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                             K-101
                 Receipt and Shipping of Boxes                                                      Software Reference




                                         Receipt and Shipping of Box-
                                         es
                                         You will find the complete descriptions of goods receipt and shipping of goods
                                         in the Production and Purchasing sections.
                                         This section provides information on the following subjects:
                                         •   “Receipt of Goods (Boxes)” on page K-102
                                         •   “Settings (ID)” on page K-113
                                         •   “Shipping of Boxes” on page K-114


                                         Receipt of Goods (Boxes)
                                         Documents > P.O. > Receipt of goods > Receipt of goods
                                         This dialog serves to enter the goods received for individual purchase orders
                                         or for the purchase orders in a Number Manager.
                                         For booking stock on hand, you can define ID numbers to be automatically as-
                                         signed if the stock P.O. includes items with a quantity of larger than 1. The ID
                                         numbers are assigned for boxes and glass (stockplates).

                                             Prerequisite
                                             The checkbox for the virtual assignment of item numbers must be ticked in
                                             company data.

                                              “Company Data” on page K-18
                                         This dialog offers the following tabs:
                                         •   “Receipt of Goods – Selection” on page K-103
                                         •   “Receipt of Goods –Complete” on page K-105
                                         •   “Receipt of Goods – by Item” on page K-107
                                         •   “Receipt of Goods – ID Numbers” on page K-110
                                         •   “Receipt of Goods – Protocol (ID Numbers)” on page K-112
1.10 / 12-2019




                 K-102                                                              A+W Business Kistenmanagement
                 Software Reference                                                         Receipt and Shipping of Boxes




                                           Receipt of Goods – Selection
                                           Documents > P.O. > Receipt of goods > Receipt of goods > Selection tab




                 Fig. K-60   Receipt of goods – selection


                                           This tab is used to filter the selection and display of documents for which re-
                                           ceipt of goods shall be checked and/or entered.
                                            Tutorial, “Receipt of goods” on page D-118

                                           Selection
                                           By choosing the option, you define how the purchase orders shall be filtered.
                                           Open purchase orders are displayed after the search in the Complete tab so
                                           that receipt of goods can be booked.
                                           •   By P.O. number:
                                               The input field for the P.O. number can be accessed. Tab Complete shows
                                               the required purchase order and all reference orders.
                                           •   By order number:
                                               The input field for the order number is released. The Complete tab shows
                                               all purchase orders issued for the defined order number.
                                           •   By supplier:
                                               The input field for the supplier number is accessible. Tab Complete shows
                                               all purchase orders placed with the selected supplier.
                                           •   By delivery note number/notification, total quantity delivered:
1.10 / 12-2019




                                               The input field for the delivery note number or notification number and the
                                               field for entering the total quantity can be accessed. If a dispatch notifica-
                                               tion has been imported, the actually received quantities must be entered.



                 A+W Business Kistenmanagement                                                                        K-103
                 Receipt and Shipping of Boxes                                                     Software Reference




                                         •   By supplier delivery date:
                                             The input field for the delivery date is accessible. Tab Complete shows all
                                             purchase orders to be delivered on the selected date.
                                         •   By number manager:
                                             The combo box for selecting the number manager is accessible. Tab Com-
                                             plete shows all purchase orders in the selected number manager.
                                         •   By scanner / document:
                                             The fields for the barcode of the P.O. number or a P.O. item are released.

                                         Target Number Manager

                                         Target Number Manager After booking the receipt of goods, the stock P.O.s
                                         can be automatically transferred to a different Number Manager.
                                         ☐ The stock P.O.s are not moved to a different Number Manager.
                                         ☑ The fields in the Target number manager section are accessible. The orders
                                         are moved to the selected number manager.

                                         Employee Name of the employee allocated to the target Number Manager.

                                         Number Manager Number Manager to which the stock P.O.s with (com-
                                         plete) receipt of goods should be moved.
1.10 / 12-2019




                 K-104                                                             A+W Business Kistenmanagement
                 Software Reference                                                        Receipt and Shipping of Boxes




                                          Receipt of Goods –Complete
                                          Documents > P.O.> Receipt of goods > Receipt of goods > Complete tab




                 Fig. K-61   Receipt of goods – complete


                                          This tab shows all purchase orders matching the search criteria. Select a pur-
                                          chase order to list all reference orders.
                                           Tutorial, “Enter receipt of goods” on page D-125

                                          Delivery date

                                          Supplier's delivery date Shows the current date. You can change it to enter
                                          a delivery received before that date. The date will be adopted only for the doc-
                                          uments selected in the list.

                                          OC supplier You can also enter the supplier's order confirmation number for
                                          the goods received.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                     K-105
                 Receipt and Shipping of Boxes                                                      Software Reference




                                         Documents
                                         You can use these buttons to select some documents or cancel the selection.
                                         The list shows all purchase orders matching the search criteria on the Selec-
                                         tion tab. Complete receipt of goods is entered for the documents for which the
                                         Book Complete checkbox is ticked.
                                         •   P.O. no.:
                                             Purchase order number.
                                         •   Book as complete:
                                             A purchase order can be booked as complete when all items were deliv-
                                             ered.
                                             ☐ Receipt of goods is incomplete. Some deliveries have yet to be made.
                                             ☑ Receipt of goods is incomplete; the purchase order will be booked as
                                             complete.
                                         •   Status:
                                             Current status. The status is changed after receipt of goods has been en-
                                             tered.
                                         •   Supplier:
                                             Supplier number and name.
                                         •   Supplier's delivery date:
                                             Delivery date stated by the supplier. This date is adopted from the purchase
                                             order or order confirmation. When you have entered the receipt of goods,
                                             the date is changed to the present date or to the date you have selected.
                                         •   Contains boxes:
                                             Shows the purchase orders which include boxes. This checkbox cannot be
                                             selected.

                                         Appended orders
                                         This list shows only the reference orders for the selected purchase order. If
                                         several purchase orders are selected, this list remains empty.

                                         Delivery at the customer's site This date is adopted from the reference or-
                                         der. You can change it if the originally scheduled date cannot be adhered to.
1.10 / 12-2019




                 K-106                                                              A+W Business Kistenmanagement
                 Software Reference                                                      Receipt and Shipping of Boxes




                                          Receipt of Goods – by Item
                                          Documents > P.O. > Receipt of goods > Receipt of boxes > By item tab




                 Fig. K-62   Receipt of goods – by item


                                          This tab serves to enter the receipt of goods by item for a purchase order se-
                                          lected on the Complete tab.

                                          Goods received/issued

                                          Quantity received Quantity already delivered for the selected item.

                                          Quantity ordered, already delivered, quantity announced These fields
                                          show the corresponding quantities for the item selected. The fields are updat-
                                          ed after input.

                                          Storage location You can select a storage place for the item, for booking the
                                          stock article to. Please note that stock articles can also be booked to storage
                                          place <n.e.>. The storage location from the purchase order can be shown via
                                          the Options menu.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                    K-107
                 Receipt and Shipping of Boxes                                                          Software Reference




                                         Accept surplus or shortfall The quantity delivered can differ from the
                                         quantity ordered. You can accept deviating quantities and thus declare deliv-
                                         ery of the item as complete.
                                         ☐ Do not accept surplus or shortfall.
                                         ☑ The quantity entered is accepted; the item is booked as complete. If a stock
                                         article has been delivered, the stock on hand is updated based on the quantity
                                         delivered. The changed quantity is saved in the purchase order.

                                         Confirmation

                                         OC supplier Supplier's order confirmation number for the selected item.

                                         OC delivery date Delivery date for the item.

                                         Items
                                         List of items included in the selected purchase order.
                                         •   Item:
                                             P.O. item number.
                                         •   Book as complete:
                                             An item can be booked as complete when the entire quantity has been de-
                                             livered.
                                             ☐ Receipt of goods is incomplete.
                                             ☑ The item is to be booked as complete.
                                         •   Order no.:
                                             Order number.
                                         •   Article:
                                             Name of the ordered product.
                                         •   Color:
                                             (Color) variations that have been defined for the selected product.
                                         •   Width / Height:
                                             Dimensions of the ordered item.
                                         •   Ordered:
                                             Quantity ordered for this item.
                                         •   Announced:
                                             Quantity announced for the item.
                                         •   Delivered:
                                             Quantity already delivered for this item. For partial deliveries, this is the to-
                                             tal of the quantities delivered so far for this purchase order.
                                         •   Receipt:
                                             Quantity already delivered for the selected item.
1.10 / 12-2019




                 K-108                                                                A+W Business Kistenmanagement
                 Software Reference                                                     Receipt and Shipping of Boxes




                                      •   Accept:
                                          If the quantity delivered is higher or lower than the quantity ordered, this
                                          quantity can be accepted. Lites that have not been ordered will only be
                                          booked on stock if they are stock articles ordered by means of a stock P.O.
                                          If the purchase order was created from an order, the stock on hand will not
                                          be updated.
                                          ☐ The quantity delivered matches the quantity ordered and does not have
                                          to be marked in a special way.
                                          ☑ The quantity delivered is lower or higher than the quantity ordered and
                                          is accepted. The quantity delivered is saved in the purchase order. The ref-
                                          erence order will not be changed. Excess lites can be booked as stock on
                                          hand if required.
                                      •   Contains boxes:
                                          Shows the purchase orders which include boxes. This checkbox cannot be
                                          selected.
                                      •   OC supplier:
                                          Supplier's order confirmation number.
                                      •   OC delivery date:
                                          Delivery date as per the supplier's order confirmation.
                                      •   Storage place:
                                          Standard storage place for this stock article. Please note that articles can
                                          also be booked to storage location <n.e.>.
                                      •   Article description 2 + 3:
                                          Descriptions of the ordered product that are stored in the master data. For
                                          float glass, usually only description 1 is stored, which is displayed in the Ar-
                                          ticle column.

                                      Appended orders
                                      The list shows the reference orders for the items. The fields are explained in
                                      connection with the Complete tab.
                                       “Receipt of Goods –Complete” on page K-105
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                    K-109
                 Receipt and Shipping of Boxes                                                         Software Reference




                                          Receipt of Goods – ID Numbers
                                          Documents > P.O.> Receipt of goods > Receipt of goods > ID numbers tab




                 Fig. K-63   Receipt of goods – ID numbers


                                          This tab shows the items belonging to a purchase order that includes boxes.
                                          For every box in a P.O. item, a sub-item (virtual item number) is created which
                                          can be assigned a box with a special ID number (identification number). You
                                          can define the default for the ID.
                                           “Settings (ID)” on page K-113

                                             Prerequisite
                                             The checkbox for assigning virtual item numbers must be ticked in the com-
                                             pany data.

                                              Master Data, “Use virtual item numbers” on page B-940

                                          Box data

                                          Supplier ID number Box ID assigned to the delivery item by the supplier.
                                          When you enter the number, the ID numbers filed shows the automatic box ID.
1.10 / 12-2019




                 K-110                                                              A+W Business Kistenmanagement
                 Software Reference                                                   Receipt and Shipping of Boxes




                                      ID numbers The automatic box ID appears when you enter the supplier ID.
                                      For every box in a P.O. item, a separate box ID is created when you enter the
                                      receipt of goods. If e.g. 5 boxes of Float 5, size 1200 x 800 mm have been or-
                                      dered and delivered, the IDs XXXX00001, XXXX00002, …, XXXX00005 will
                                      be assigned. You can define the presetting for XXXX.
                                       “Settings (ID)” on page K-113

                                      Storage location Each item can be assigned a separate storage location.
                                      Please note you can also assign storage location <n.s.>.

                                      Remark Comments can be entered here in case of peculiarities, e.g. regard-
                                      ing the allocation of storage locations or in connection with reservations.

                                      Content Contents of the box selected in the list. This entry can be changed
                                      if required.

                                      Prod. date Date by which the production of the ordered goods should be fin-
                                      ished. This date is important for the stock withdrawal in accordance with the
                                      FiFo principle, e.g. for coated glass.

                                      PP / QU Purchase price and price unit of the ordered item. If you change the
                                      price, the amendment will be saved in the purchase order.

                                      Box items
                                      •   Item:
                                          Item number stated in the purchase order. An item sub-number is automat-
                                          ically assigned at booking if the quantity of the P.O. item is higher than 1,
                                          e.g. 1.1, 1.2, etc.
                                      •   Description:
                                          Description shown in the purchase order.
                                      •   Width / height:
                                          Stock sizes of the lites in the box.
                                      •   Supplier ID:
                                          Supplier's box ID as entered in the Box data section.
                                      •   Contents:
                                          Contents of the box as defined in the Box data section.
                                      •   ID number:
                                          (Automatic) ID as defined in the Box data section.
                                      •   Storage location:
                                          Storage location as defined in the Box data section.
                                      •   Prod. date:
                                          Production date as defined in section Box data.
                                      •   Pr./QU:
                                          Purchase price per quantity unit as defined in the Box data section.
                                      •   Pr. unit:
                                          Price unit that applies to the displayed price.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                  K-111
                 Receipt and Shipping of Boxes                                                       Software Reference




                                          Receipt of Goods – Protocol (ID Numbers)
                                          Documents > P.O.> Receipt of goods > Receipt of goods > Protocol tab (ID
                                          numbers)




                 Fig. K-64   Receipt of goods – Protocol (ID numbers)


                                          This tab gives you an overview of the allocated box IDs.
1.10 / 12-2019




                 K-112                                                             A+W Business Kistenmanagement
                 Software Reference                                                    Receipt and Shipping of Boxes




                                      Settings (ID)
                                      Documents > P.O. > Receipt of goods > Receipt of goods > Options menu >
                                      ID allocation group > Settings




                                      Fig. K-65    Settings


                                      This dialog is used to define the ID numbers for boxes. This setting is neces-
                                      sary to automatically allocate individual box IDs.
                                      If a delivery includes, e.g. an item with 5 boxes, 5 (virtual) sub-numbers will be
                                      assigned when you enter the receipt of goods. These numbers must be given
                                      a code so that, e.g. instead of the scanned box number 12345, the sub-num-
                                      bers SupplierA00001, SupplierA00002, ..., SupplierA00005 are assigned.
                                       Tutorial, “Dealing with boxes” on page D-134

                                         Prerequisite
                                         The checkbox for the virtual assignment of item numbers must be ticked in
                                         company data.

                                          Master Data, “Use virtual item numbers” on page B-940

                                      Stock ID number

                                      Default You can enter text (or numbers) of max. 15 characters which is com-
                                      pleted by XXXXX. XXXXX represents the automatically assigned number. The
                                      text is retained until you change it.
                                      If you buy boxes from different suppliers and want to mark them separately,
                                      you have to amend the default before entering the receipt of goods.
1.10 / 12-2019




                 A+W Business Kistenmanagement                                                                   K-113
                 Receipt and Shipping of Boxes                                                     Software Reference




                                          Shipping of Boxes
                                          Production > Logistics > Shipping boxes > ID tab




                 Fig. K-66   Shipping of boxes – withdraw box


                                          This tab can be used to reserve a box or withdraw it from stock. You can only
                                          reserve boxes which were added to stock with a box ID.
                                           Tutorial, “Issue of Boxes” on page E-146
1.10 / 12-2019




                 K-114                                                                 A+W Business Kistenmanagement
Box Management              K

                      Part Index




                 A+W Business
                 Part Index                                                                             Index




                 Index
                 B                                             – Options (P.O. transfer) K-97
                 BOM
                 – Box at item entry K-35                      N
                 – Box in stock management K-34                Number of sheets in a box   K-87
                 Box
                 – Box ID K-110
                                                               O
                 – Check reservation K-55
                                                               Opening a box K-88
                 – Complex structure K-30
                                                               Options
                 – correct booking of contents K-65
                                                               – Stock movement K-83
                 – Enter in issue of goods K-55
                                                               Order
                 – Issue of goods K-58
                                                               – Allocate dummy box K-55
                 – open K-66
                                                               – BOM box K-35
                 – Receipt of goods K-103
                                                               – Internal K-42
                 – Reservation K-55
                 – resolve K-88
                 – Virtual item number K-111                   P
                 Box as pallet K-30                            P.O.
                 Box ID K-55                                   – automatic K-49
                 – Settings K-113                              – Proposal K-49
                                                               – purchase quantity after stocktaking K-41
                                                               P.O. transfer
                 C
                                                               – Functions menu K-96
                 Company data
                                                               – Options menu K-97
                 – enable Stock control mode K-20
                                                               Pallet as box K-30
                 – Settings K-18
                                                               Price lists
                 Correct number of sheets K-65
                                                               – for PP calculation K-16
                                                               Prices
                 D                                             – Stock management K-78
                 Delivery                                      Product
                 – Partial quantity K-108                      – Enter stock size K-25
                 Display conventions K-10                      Production order
                                                               – Stock addition K-18, K-50
                 I                                             – Supplier file K-42
                 ID number                                     Purchase order
                 – Box ID K-110                                – Enter box K-51
                 – Settings K-113                              – Minimum quantity and P.O. quantity K-49
                 Inventory management K-71                     – Stock K-96
                 Issue of goods
                 – Allocate box to item K-58                   R
                 – Withdraw box K-55                           Receipt of goods
                                                               – Box K-103
                 M                                             – Complete K-106
                 Master data                                   – ID for box K-110
                 – Check price lists for PP calculation K-16   – Partial quantity K-108
                 – define stock category K-22                  – Sub-item (boxes) K-110
                                                               Remark on stock movement     K-89
1.10 / 12-2019




                 – Enter stock size K-25
                 – user status for stock booking K-21          Reservation
                 Menu                                          – Box K-55
                 – Functions (P.O. transfer) K-96              – Check K-55


                 A+W Business Box Management                                                           K-117
                 Index                                                                                  Part Index




                 reservations   K-12                                Stock size
                                                                    – Enter in master data K-25
                 S                                                  – Product management K-13
                 Search (stock info) K-90                           – Stock article K-25
                 Settings                                           storage location
                 – Box ID K-113                                     – transfer article K-64
                 Status                                             Sub-item
                 – Allocations for stock booking K-21               – Receipt of boxes K-110
                 – Stock booking K-20                               Supplement
                 Stock                                              – Stock management K-81
                 – define stock category K-22                       Supplier file
                 Stock addition K-84                                – Internal customer K-42
                 – by production order K-18, K-50                   – Production order K-42
                 Stock article                                      Supplier list K-12
                 – enter in Stock management K-26
                 – Stock size K-25                                  T
                 – transfer storage location K-64                   Transfer of stock articles   K-86
                 Stock booking
                 – box K-48                                         V
                 – Change stock on hand manually K-60               Virtual item number    K-111
                 – change storage location K-64
                 – correct box contents K-65
                 – Manual booking of additions/withdrawals   K-62
                 – Open box K-66
                 – Registration point K-18, K-50
                 – user status K-21
                 Stock control mode K-12
                 – enable in company data K-20
                 Stock dispatch K-84
                 Stock management K-73
                 – Basic principles K-12
                 – BOM box K-34
                 – enter stock articles K-26
                 – Menu overview K-11
                 – Prices K-78
                 – Stock articles K-74
                 – Supplement K-81
                 Stock Movement
                 – Dispatch, Addition K-84
                 Stock movement K-83
                 – Number of sheets K-87
                 – Open boxes K-88
                 – Options (menu) K-83
                 – Remark K-89
                 – Transfer K-86
                 Stock on hand
                 – Reservation K-55
                 Stock P.O.
                 – Box K-103
1.10 / 12-2019




                 – Check if automatic order K-41
                 – Order pool K-96
                 Stock P.O. after stocktaking K-41



                 K-118                                                              A+W Business Box Management

