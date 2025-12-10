---
description: "EN AWEnterprise Stock 1.01"
---



# EN AWEnterprise Stock 1.01

Stock              E




                   english




        A+W Enterprise
                                                                                                            Introduction




                                        Introduction
                                        This section of the documentation contains editorial notes.


                                        Revision overview
                                        Section
                                        Version / Date

                                        1.00 / 01-2016             English edition.

                                        1.01 / 01-2017             Product and company names adjusted.



                                        Editorial
                                        The editorial provides information on the following topics:
                                        •   Notes on this document
                                        •   Copyrights
                                        •   Trademarks
                                        •   Contacts

                                        Notes on this document
                                        This publication is written exclusively for end users of A+W Enterprise.
                                        The documentation and software described therein are licensed only and must
                                        be used or copied only in accordance with the terms of our license agreement.
                                        The contents of the documentation are for information purposes only and are
                                        subject to changes without prior notice.
                                        The text and illustrations were compiled with the utmost care. In spite of this,
                                        we cannot rule out all mistakes. A+W Software GmbH assumes no liability for
                                        errors or omissions unless these are based on intentional or grossly negligent
                                        behavior.
                                        The descriptions in this documentation rely on the full version of A+W Enter-
                                        prise.

                                        Copyrights
                                        © 2017, A+W Software GmbH, all rights reserved, including the right of reprint,
                                        the production of copies and of the translation.
                                        The documentation may be copied, completely or in part, saved in an archiving
                                        system, or transferred in any other form only in accordance with our license
                                        agreement. Transmission of the documentation is not allowed, neither elec-
                                        tronically, nor mechanically, nor by recording or in any other way, without prior
                                        written approval from A+W Software GmbH.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                E-3
                 Introduction




                                Trademarks
                                All hardware and software names mentioned in this documentation might also
                                be registered trademarks or other property rights of third parties. Copyrights of
                                third parties must be complied with.

                                Contacts
                                A+W Software GmbH


                                Am Pfahlgraben 4-10

                                35415 Pohlheim

                                   +49 6404 2051-0

                                   +49 6404 2051 877

                                Zentrale@a-w.com

                                http://www.a-w.com
1.01 / 01-2017




                 E-4                                                                     A+W Enterprise Stock
                                                                                                                                                        Contents




                                        Contents
                                        Introduction ............................................................................................................. E-3
                                          Revision overview ............................................................................................... E-3
                                          Editorial ............................................................................................................... E-3

                                        Software Reference
                                        Overview ................................................................................................................. E-9
                                          Menus in the Stock module ................................................................................. E-9
                                             Booking menu .................................................................................................. E-9
                                             Master data menu .......................................................................................... E-10
                                             Inventory menu .............................................................................................. E-10
                                             Evaluation menu ............................................................................................ E-11
                                             Info system menu ........................................................................................... E-11
                                             Print menu ...................................................................................................... E-12
                                             System menu ................................................................................................. E-12
                                             Additional menu ............................................................................................. E-12
                                        Search Functions .................................................................................................. E-14
                                        Stock Management ............................................................................................... E-15
                                          Warehouse in ................................................................................................... E-16
                                             Warehouse in – Pieces .................................................................................. E-16
                                             Warehouse in – Quantity ............................................................................... E-20
                                          Warehouse out ................................................................................................. E-22
                                          Box warehouse in ............................................................................................. E-23
                                             Box warehouse in – Pieces ............................................................................ E-23
                                             Box warehouse in – Quantity ......................................................................... E-26
                                          Box warehouse out ........................................................................................... E-28
                                          Slot warehouse in ............................................................................................. E-29
                                             Slot warehouse in – Pieces ............................................................................ E-29
                                             Slot warehouse in – Quantity ......................................................................... E-32
                                          Slot warehouse out ........................................................................................... E-34
                                          Stack warehouse in ........................................................................................... E-35
                                          Modify stack warehouse .................................................................................... E-36
                                          Rack storage receipt ......................................................................................... E-38
                                          Rack storage exit ............................................................................................... E-40
                                             Rack storage exit – Order related .................................................................. E-40
                                             Rack storage exit – Transfer .......................................................................... E-42
                                          Outgoing stocks (order-related) ........................................................................ E-44
                                          Correction – Overview ....................................................................................... E-46
                                          Booking correction – Details .............................................................................. E-47
                                        Master Data Management .................................................................................... E-49
                                          Stock room administration ................................................................................ E-50
                                          Article master data stock .................................................................................. E-51
                                        Inventory Management ......................................................................................... E-53
                                          Inventory – Standard stock ................................................................................ E-54
                                          Inventory – Box stock ........................................................................................ E-57
                                          Inventory – Slots ................................................................................................ E-59
                                          Inventory – Stack stock ..................................................................................... E-60
                                          Inventory – Rack stock ...................................................................................... E-61
                                        Evaluation ............................................................................................................. E-64
                                          Evaluation – Standard stock .............................................................................. E-65
                                          Evaluation – Box stock ...................................................................................... E-67
1.01 / 01-2017




                                          Evaluation – Slot stock ...................................................................................... E-68
                                          Evaluation – Stack stock ................................................................................... E-69
                                          Rack stock evaluation ....................................................................................... E-70
                                        Information System ............................................................................................... E-71


                 A+W Enterprise Stock                                                                                                                           E-5
                 Contents




                              Info: Stock products ........................................................................................... E-72
                                Info: Stock products – Filter dialog ................................................................. E-72
                                Info: Stock products – Hit list ......................................................................... E-73
                                Info: Stock products – Hit list details .............................................................. E-74
                              Info: Stock variants ............................................................................................ E-75
                                Info: Stock variants – Filter dialog .................................................................. E-75
                                Info: Stock variants – Hit list ........................................................................... E-76
                                Info: Stock variants – Hit list details ............................................................... E-78
                              Info: Stock slots ................................................................................................. E-80
                                Info: Stock slots .............................................................................................. E-80
                                Info: Stock slots – Hit list ................................................................................ E-81
                                Info: Stock slots – Hit list details .................................................................... E-82
                              Info: Stock racks ................................................................................................ E-83
                                Info: Stock racks – Filter dialog ...................................................................... E-83
                                Info: Stock racks – Hit list details – General .................................................. E-84
                                Info: Stock racks – Hit list details ................................................................... E-85
                              Info: Stock stacks .............................................................................................. E-87
                                Info: Stock stacks – Filter dialog .................................................................... E-87
                                Info: Stock stacks – Hit list ............................................................................. E-88
                                Info: Stock stacks – Hit list details .................................................................. E-89
                              Info: Stock sheets .............................................................................................. E-90
                                Info: Stock sheets – Filter dialog .................................................................... E-90
                                Info: Stock sheets – Hit list ............................................................................. E-92
                              Info: Stock history .............................................................................................. E-93
                                Info: Stock history – Filter dialog .................................................................... E-93
                                Info: Stock history – Hit list ............................................................................. E-94
                                Info: Stock history – Hit list details ................................................................. E-96
                              Orders/Purchase Orders ................................................................................... E-98
                                Orders/Purch. Orders – Filter dialog .............................................................. E-98
                                Orders/Purch. Orders – Hit list ....................................................................... E-99
                                Orders/Purch. Orders – Hit list details ......................................................... E-100
                              Booking Status ............................................................................................... E-102
                                Booking Status – Unbooked ........................................................................ E-102
                                Booking Status – Error ................................................................................. E-104
                                Booking Status – Inventory .......................................................................... E-105
                                Booking Status – Correction ........................................................................ E-106
                              Stock Information – Pick list ............................................................................ E-108
                              Stock Information – Hit list ............................................................................... E-109
                              LVR Status ...................................................................................................... E-110
                              Range – Stock Forecast .................................................................................. E-110
                              Range – Hit list ................................................................................................ E-111
                              Available stock ................................................................................................ E-112
                              Stock forecast .................................................................................................. E-113
                            Print .................................................................................................................... E-115
                              Print labels for boxes ...................................................................................... E-116
                              List printing ...................................................................................................... E-117
                            System Administration ........................................................................................ E-118
                              Delete stock log .............................................................................................. E-119
                              Stock price correction ..................................................................................... E-119
                            Service Functions ............................................................................................... E-120

                            Section index
                            Index ................................................................................................................... E-123
1.01 / 01-2017




                 E-6                                                                                                  A+W Enterprise Stock
Stock                  E

        Software Reference




        A+W Enterprise
                 Software Reference                                                                           Overview




                                        Overview
                                        In the Stock module, you have all functions that are required for successful
                                        stock management, e.g. stock maintenance, stock bookings, inventories, as
                                        well as the planning of incoming and outgoing articles. All prices are specified
                                        as net prices in this module.
                                        The Stock section covers the following topics:
                                        •   “Stock Management” on page E-15
                                        •   “Master Data Management” on page E-49
                                        •   “Inventory Management” on page E-53
                                        •   “Evaluation” on page E-64
                                        •   “Information System” on page E-71
                                        •   “Print” on page E-115
                                        •   “System Administration” on page E-118
                                        •   “Service Functions” on page E-120


                                        Menus in the Stock module
                                        The dialogs of the Stock module have the following menus:
                                        •   “Booking menu” on page E-9
                                        •   “Master data menu” on page E-10
                                        •   “Inventory menu” on page E-10
                                        •   “Evaluation menu” on page E-11
                                        •   “Info system menu” on page E-11
                                        •   “Print menu” on page E-12
                                        •   “System menu” on page E-12


                                        Booking menu
                                        The first level of the Booking menu includes the following entries:
                                        •   Warehouse in:
                                             “Warehouse in” on page E-16
                                        •   Warehouse out:
                                             “Warehouse out” on page E-22
                                        •   Boxes in:
                                             “Box warehouse in” on page E-23
                                        •   Boxes out:
                                             “Box warehouse out” on page E-28
                                        •   Slots in:
                                             “Slot warehouse in” on page E-29
                                        •   Slots out:
1.01 / 01-2017




                                             “Slot warehouse out” on page E-34
                                        •   Stack management:
                                            Customer-specific functions will be explained in detail in a separate sec-
                                            tion.


                 A+W Enterprise Stock                                                                               E-9
                 Overview                                                              Software Reference




                            •   Stack in:
                                 “Stack warehouse in” on page E-35
                            •   Stack modification:
                                 “Modify stack warehouse” on page E-36
                            •   Rack receipt:
                                 “Rack storage receipt” on page E-38
                            •   Rack shipment:
                                 “Rack storage exit” on page E-40
                            •   Stack booking (doc.rel.):
                                Customer-specific functions will be explained in detail in a separate sec-
                                tion.
                            •   Outg. Stocks (order-rel.):
                                 “Outgoing stocks (order-related)” on page E-44
                            •   Correction:
                                 “Correction – Overview” on page E-46


                            Master data menu
                            The Master data menu includes the following entries:
                            •   Location:
                                 “Stock room administration” on page E-50
                            •   Article:
                                 “Article master data stock” on page E-51
                            •   Slots:
                                Customer-specific functions will be explained in detail in a separate sec-
                                tion.
                            •   Stack types:
                                Customer-specific functions will be explained in detail in a separate sec-
                                tion.


                            Inventory menu
                            The Inventory menu includes the following entries:
                            •   Stock:
                                 “Inventory – Standard stock” on page E-54
                            •   Box stock:
                                 “Inventory – Box stock” on page E-57
                            •   Slot stock:
                                 “Inventory – Slots” on page E-59
                            •   Stack stock:
                                 “Inventory – Stack stock” on page E-60
                            •   Rack stock:
                                 “Inventory – Rack stock” on page E-61
1.01 / 01-2017




                 E-10                                                               A+W Enterprise Stock
                 Software Reference                                                                           Overview




                                        Evaluation menu
                                        The Evaluation menu includes the following entries:
                                        •   Stock:
                                             “Evaluation – Standard stock” on page E-65
                                        •   Box stock:
                                             “Evaluation – Box stock” on page E-67
                                        •   Slot stock:
                                             “Evaluation – Slot stock” on page E-68
                                        •   Stack stock:
                                             “Evaluation – Stack stock” on page E-69
                                        •   Rack stock:
                                             “Rack stock evaluation” on page E-70


                                        Info system menu
                                        The first level of the Info system menu includes the following entries:
                                        •   Article:
                                             “Info: Stock products – Filter dialog” on page E-72
                                        •   Variant:
                                             “Info: Stock variants – Filter dialog” on page E-75
                                        •   Slot:
                                             “Info: Stock slots” on page E-80
                                        •   Rack:
                                             “Info: Stock racks – Filter dialog” on page E-83
                                        •   Stack:
                                             “Info: Stock stacks – Filter dialog” on page E-87
                                        •   Sheet:
                                             “Info: Stock sheets – Filter dialog” on page E-90
                                        •   History:
                                             “Info: Stock history – Filter dialog” on page E-93
                                        •   Orders/Purchase orders:
                                             “Orders/Purch. Orders – Filter dialog” on page E-98
                                        •   Booking status:
                                             “2nd level menu - Booking status” on page E-12
                                        •   Order list:
                                             “Stock Information – Pick list” on page E-108
                                        •   Status:
                                            At present, this dialog is not used.
                                        •   Range:
                                             “Range – Stock Forecast” on page E-110
                                        •   Available stock:
                                             “Available stock” on page E-112
                                        •   Forecast:
1.01 / 01-2017




                                             “Stock forecast” on page E-113




                 A+W Enterprise Stock                                                                             E-11
                 Overview                                                            Software Reference




                            2nd level menu - Booking status
                            •   No booking:
                                 “Booking Status – Unbooked” on page E-102
                            •   Error:
                                 “Booking Status – Error” on page E-104
                            •   Inventory:
                                 “Booking Status – Inventory” on page E-105


                            Print menu
                            The Print menu includes the following entries:
                            •   Labels:
                                 “Print labels for boxes” on page E-116
                            •   List printing:
                                This dialog is described in the Sales section.
                                 Sales, “List printing” on page D-162


                            System menu
                            The System menu includes the following entries:
                            •   Delete stock transcript:
                                 “Delete stock log” on page E-119
                            •   Price correction:
                                 “Stock price correction” on page E-119


                            Additional menu
                            <F4>
                            The Additional menu includes the following entries:

                            1st menu level
                            •   PCD prices:
                                In the warehouse ins, you can assign articles pre-defined prices via price
                                codes. You can select the price codes from a pre-defined list.
                            •   Booking - no Price:
                                In the warehouse ins, you can assign articles the price = 0.
                            •   Trans.bookings:
                                Transfer selected data record to another stock. The booking must be com-
                                pleted with [OK].
                            •   Contract book.:
                                Assign selected data record to an object (e.g. construction site).
                            •   Boxes:
                                 “2nd level menu - Boxes” on page E-13
1.01 / 01-2017




                 E-12                                                              A+W Enterprise Stock
                 Software Reference                                                                          Overview




                                        2nd level menu - Boxes
                                        •   Book box:
                                            Removes the box of the current data record from the box stock and books
                                            the articles of the box automatically into the normal stock. The booking
                                            must be completed with [OK].
                                        •   Resolve box:
                                            Removes the box of the current data record from the box stock and books
                                            the articles into a target stock. The booking must be completed with [OK].
                                        •   Single sheet information:
                                             “3rd level menu - Individual sheet information” on page E-13

                                        3rd level menu - Individual sheet information
                                        •   Display:
                                             “Footer area – individual sheet information” on page E-25
                                        •   Edit:
                                             “Footer area – individual sheet information” on page E-25
1.01 / 01-2017




                 A+W Enterprise Stock                                                                            E-13
                 Search Functions                                                             Software Reference




                                    Search Functions
                                    You can search for information via the search functions, e.g. about articles,
                                    stock types, orders or purchase orders.
                                     “Information System” on page E-71
1.01 / 01-2017




                 E-14                                                                      A+W Enterprise Stock
                 Software Reference                                                               Stock Management




                                        Stock Management
                                        In the stock management, you record and edit the bookings for the goods
                                        warehouse, e.g. warehouse in receipts for articles or booking corrections.
                                        This section explains the following dialogs:
                                        •   “Warehouse in” on page E-16
                                        •   “Warehouse out” on page E-22
                                        •   “Box warehouse in” on page E-23
                                        •   “Box warehouse out” on page E-28
                                        •   “Slot warehouse in” on page E-29
                                        •   “Slot warehouse out” on page E-34
                                        •   “Stack warehouse in” on page E-35
                                        •   “Modify stack warehouse” on page E-36
                                        •   “Rack storage receipt” on page E-38
                                        •   “Rack storage exit” on page E-40
                                        •   “Outgoing stocks (order-related)” on page E-44
                                        •   “Correction – Overview” on page E-46
                                        •   “Booking correction – Details” on page E-47
1.01 / 01-2017




                 A+W Enterprise Stock                                                                           E-15
                 Stock Management                                                                   Software Reference




                                         Warehouse in
                                         Booking > Warehouse in
                                         On this dialog, you record and book the stock receipts for the stock articles of
                                         the selected stock.
                                         This dialog offers the following tabs:
                                         •   “Warehouse in – Pieces” on page E-16
                                         •   “Warehouse in – Quantity” on page E-20


                                         Warehouse in – Pieces
                                         Booking > Warehouse in > Pieces




                 Fig. E-1   Warehouse in – pieces


                                         On this dialog, you record and book the warehouse ins in the pieces of the cur-
                                         rent type of article. You can select another stock by entering another stock
                                         number. This also applies for stock of another stock type.
                                         The warehouse ins for boxes, slots, stacks and racks are booked in the follow-
                                         ing place:
                                          “Box warehouse in” on page E-23
                                          “Slot warehouse in” on page E-29
                                          “Stack warehouse in” on page E-35
                                          “Rack storage receipt” on page E-38
1.01 / 01-2017




                 E-16                                                                            A+W Enterprise Stock
                 Software Reference                                                                    Stock Management




                                        You can execute the following keyboard commands:
                                        •   With <Ctrl> + <F8>, you can change in the first field between the Ware-
                                            house in and Warehouse out dialogs.
                                        •   With <F5>, you can change from one column in the variant-related details
                                            into the footer area.
                                        •   With <Home>, you discard your entry in the footer area.
                                        •   With <End>, you can save your entry in the footer area and change back
                                            to the rump area.
                                        •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                            cord.

                                        Header area

                                        Article Article number and name.

                                        Stock Stock number and name.

                                        Supplier Supplier number and name.

                                        Total stock Total stock of the article, including all article variants.

                                        Total value Total value of the stock article.

                                        Booking status Status of the bookings in the stock.

                                        Booking status with        Meaning
                                        colored markings

                                            Gray                   In warehouse in, all booking articles are booked by the
                                                                   process (program).

                                            Red                    In warehouse in, at least one booking article has not or
                                                                   not yet been booked by the process (program).

                                        Tab. E-1     Booking status of the stock

                                        Last change on, frm Date of the last change to the booking record and
                                        name of the user who made the last booking.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                  E-17
                 Stock Management                                                                  Software Reference




                                    Rump area
                                    In this area, you book the inventories and prices of the article variant in pieces.
                                    •   Variant:
                                        Dimensional variant of the article. With <F9>, you can call up the variant
                                        selection. Here only the variants are displayed that are assigned to the cur-
                                        rent article in the master data.
                                    •   Stock desc:
                                        Stock designation.

                                    Stock HD (Piece) Stock of the variant in pieces.
                                    •   Old:
                                        Old article stock in the stock before booking.
                                    •   Booking:
                                        Article stock that is booked.
                                    •   New:
                                        Newly-calculated stock. This stock is taken over when the new article is
                                        booked. If you exit the dialog with <Home>, the old stock is retained.

                                    Prices The display of the current depends on the own currency that was
                                    specified during installation.
                                    • € / qm:
                                       Article price of the supplier in own currency per quantity unit.
                                    • Price:
                                       Total price of the article.
                                    • (Column without designation):
                                       Booking status of the article item.

                                    Booking status with         Meaning
                                    colored markings

                                        Gray                    Article item has been booked by the process
                                                                (program).

                                        Red                     Article item has not or not yet been booked by the
                                                                process (program).

                                    Tab. E-2      Booking status of the article item

                                    Footer area – variant-related details

                                    Object Designation of the object for order-related stock articles, e.g. custom-
                                    er’s construction site.

                                    Cost center Designation of the cost center for statistical evaluations.

                                    Remark Text field for additional information.

                                    Minimum stock Minimum permissible stock of the article to prevent produc-
1.01 / 01-2017




                                    tion bottlenecks.




                 E-18                                                                          A+W Enterprise Stock
                 Software Reference                                                                    Stock Management




                                        Alarm stock Quantity of the article stock that creates a P.O. proposal in pur-
                                        chasing. Alarm stocks can prevent a material shortage in the stock.

                                        Maximum stock Maximum permissible stock of the article to minimize stock
                                        costs.

                                           Automatic P.O. proposals by the stock
                                           If the defined alarm stock is underrun with a warehouse out booking, P.O.
                                           proposals are created in purchasing automatically by the stock. Automatic
                                           P.O. proposals are also created by the nightly booking routine in purchas-
                                           ing if the article stock falls below the minimum stock in the long term. The
                                           quantity in the P.O. proposal depends on the defined maximum stock.
                                           These P.O. proposals are enabled by purchasing and transferred into pur-
                                           chase orders.

                                        Total Total price of the article variant.

                                        Average price Average purchase price of the article variant in the stock.

                                        Maximum price Maximum purchase price of the article variant in the stock.

                                        Minimum price Minimum purchase price of the article variant in the stock.

                                        LIFO total price Total price of the article variant in the stock if the last re-
                                        ceived stock articles are sent out as the first articles.

                                        FIFO total price Total price of the article variant in the stock if the first re-
                                        ceived stock articles are sent out as the first articles.

                                           Example

                                           1st warehouse in 10 pieces at € 10 = € 100
                                           2nd warehouse in 10 pieces at € 15 = € 150
                                           Total value of both warehouse ins = € 250

                                           Warehouse out 10 pieces according to LIFO = - € 150
                                           LIFO total price = € 100

                                           Warehouse out 10 pieces according to FIFO = - € 100
                                           FIFO total price = € 150
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                 E-19
                 Stock Management                                                                    Software Reference




                                         Warehouse in – Quantity
                                         Booking > Warehouse in > Quantity




                 Fig. E-2   Warehouse in – Quantity


                                         On this tab, you record and book the warehouse receipts in the pieces of the
                                         current article variant.
                                         The Quantity tab is structured like the Pieces tab.
                                          “Header area” on page E-17
                                          “Footer area – variant-related details” on page E-18

                                         Rump area
                                         In this area, you book the inventories and prices of the article variant in quan-
                                         tity units.
                                         •   Variant:
                                             Dimensional variant of the article. With <F9>, you can call up the variant
                                             selection. Here only the variants are displayed that are assigned to the cur-
                                             rent article in the master data.
                                         •   Color:
                                             Color of the dimensional variant of the article.

                                         Stock HD (Unit) Stock of the variant in the quantity that is defined for this ar-
                                         ticle variant in the master data.
                                         •   Old:
1.01 / 01-2017




                                             Old article stock in the stock before booking.
                                         •   Booking:
                                             Article stock that is booked.


                 E-20                                                                             A+W Enterprise Stock
                 Software Reference                                                                   Stock Management




                                        •   New:
                                            Newly-calculated stock. This stock is taken over when the new article is
                                            booked. If you exit the dialog with <Home>, the old stock is retained.

                                        Prices The display of the current depends on the own currency that was
                                        specified during installation.
                                        • € / qm:
                                           Article price of the supplier in own currency per quantity unit.
                                        • Price:
                                           Total price of the article.
                                        • (Column without designation):
                                           Booking status of the article item.

                                        Booking status with        Meaning
                                        colored markings

                                            Gray                   Article item has been booked by the process
                                                                   (program).

                                            Red                    Article item has not or not yet been booked by the
                                                                   process (program).

                                        Tab. E-3     Booking status of the article item
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                   E-21
                 Stock Management                                                                 Software Reference




                                        Warehouse out
                                        Booking > Warehouse out




                 Fig. E-3   Warehouse out


                                        On this dialog, you record and book the warehouse outs, e.g. if stock articles
                                        are delivered to production. The warehouse outs for boxes, slots, stacks,
                                        racks, and order-related warehouse outs are booked in the following place:
                                         “Box warehouse out” on page E-28
                                         “Slot warehouse out” on page E-34
                                         “Modify stack warehouse” on page E-36
                                         “Rack storage exit” on page E-40
                                         “Outgoing stocks (order-related)” on page E-44
                                        You can execute the following keyboard commands:
                                        •   With <Ctrl> + <F8>, you can change in the first field between the Ware-
                                            house in and Warehouse out dialogs.
                                        •   With <F5>, you can change from one column in the variant-related details
                                            into the footer area.
                                        •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                            cord.
                                        The tabs, fields, and columns are described here:
                                         “Warehouse in” on page E-16
                                        The values in the fields display the quantities to be removed.
1.01 / 01-2017




                 E-22                                                                          A+W Enterprise Stock
                 Software Reference                                                                     Stock Management




                                          Box warehouse in
                                          Booking > Box warehouse in
                                          On this dialog, you book the warehouse ins for complete boxes, e.g. pallet
                                          cages with 50 identical panes.
                                          This dialog offers the following tabs:
                                          •   “Box warehouse in – Pieces” on page E-23
                                          •   “Box warehouse in – Quantity” on page E-26


                                          Box warehouse in – Pieces
                                          Booking > Box warehouse in > Pieces




                 Fig. E-4   Box warehouse in -- pieces, box stock, and single sheet box stock


                                          On this tab, you book the warehouse ins for complete boxes. Using the selec-
                                          tion of the stock type in the Stock field, you can select whether you book the
                                          warehouse ins into the box stock or into the single sheet box stock.
                                          If you select a single sheet box stock, you can book the sheets individually into
1.01 / 01-2017




                                          boxes.
                                           “Footer area – individual sheet information” on page E-25



                 A+W Enterprise Stock                                                                                E-23
                 Stock Management                                                                 Software Reference




                                    You can execute the following keyboard commands:
                                    •   With <Ctrl> + <F8>, you can change in the first field between the Box ware-
                                        house in and Box warehouse out dialogs.
                                    •   With <F5>, you can change from one column in the box-related details into
                                        the footer area (left side).
                                    •   With <Shift> + <F8>, you can change from one column in the variant-relat-
                                        ed details into the footer area (right side).
                                    •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                        cord.

                                    Header area
                                    The fields are described in the following section:
                                     “Warehouse in” on page E-16
                                    In addition, the following field is described:

                                    Stock Stock number and name. If you enter the number for a single sheet box
                                    stock, you can record the sheets individually for each box.
                                     “Footer area – individual sheet information” on page E-25

                                    Rump area
                                    In this area, you book the inventories and prices of the articles in pieces.
                                    •   Variant:
                                        Dimensional variant of the article. With <F9>, you can call up the variant
                                        selection. Here only the variants are displayed that are assigned to the cur-
                                        rent article in the master data.
                                    •   Box:
                                        Box number.
                                    •   Box description:
                                        Designation of the box.
                                    •   Supplier:
                                        Supplier number.
                                    •   Packing type:
                                        Identification of the packing type, e.g. 13 = small wooden box.
                                    •   New:
                                        Newly-calculated stock. This stock is taken over when the new article is
                                        booked. If you exit the dialog with <Home>, the old stock is retained.

                                    Stocks Stock of the variant in pieces. With <F2>, you can change through
                                    the following displays:
                                    •   Old:
                                        Old article stock in the stock before booking.
                                    •   Booking:
                                        Article stock that is booked.
                                    •   New:
1.01 / 01-2017




                                        Newly-calculated stock. This stock is taken over when the new article is
                                        booked. If you exit the dialog with <Home>, the old stock is retained.




                 E-24                                                                         A+W Enterprise Stock
                 Software Reference                                                                   Stock Management




                                        Prices The display of the current depends on the own currency that was
                                        specified during installation.
                                        • € / qm:
                                           Article price of the supplier in own currency per quantity unit.
                                        • Price:
                                           Total price of the article.
                                        • (Column without designation):
                                           Booking status of the article item.

                                        Booking status with        Meaning
                                        colored markings

                                            Gray                   Article item has been booked by the process
                                                                   (program).

                                            Red                    Article item has not or not yet been booked by the
                                                                   process (program).

                                        Tab. E-4     Booking status of the article item

                                        Footer area – box-related details
                                        The fields are described in the following section:
                                         “Warehouse in” on page E-16
                                        In addition, the following fields are described:

                                        Supplier Supplier number and name.

                                        Packing type Identification of the packing type.

                                        Reserved Order number for which the box was reserved.

                                        Label Display of the label printing.
                                        • Y = print labels.
                                        • N = do not print labels.

                                        Footer area – individual sheet information
                                        You can only call up the individual sheet information if you have selected a sin-
                                        gle sheet box stock in the Stock field.
                                        •   With <Shift> + <F12>, you can display the single sheet information.
                                        •   With <Shift> + <E>, you can edit the single sheet information.
                                        On the dialog at the bottom right, the table for the single sheet information is
                                        displayed with the following columns:
                                        •   Sheet:
                                            Number of the sheet.
                                        •   Description:
                                            Designation of the sheet.
1.01 / 01-2017




                                        •   €/piece:
                                            Piece price of the sheet.



                 A+W Enterprise Stock                                                                                   E-25
                 Stock Management                                                                   Software Reference




                                         •   Yield:
                                             Yield in percent.
                                         •   Reserved:
                                             Reservation code.
                                             – Y = Variant is reserved for a process.
                                             – N = Variant is not reserved for a process.


                                         Box warehouse in – Quantity
                                         Booking > Box warehouse in > Quantity




                 Fig. E-5   Box warehouse in – Quantity


                                         On this tab, you book the inventories and prices of the articles in quantity.
                                         The Quantity tab is structured like the Pieces tab.
                                          “Header area” on page E-24
                                          “Footer area – box-related details” on page E-25
1.01 / 01-2017




                 E-26                                                                             A+W Enterprise Stock
                 Software Reference                                                                    Stock Management




                                        Rump area
                                        On this tab, you book the inventories and prices of the articles in quantity unit.
                                        •   Variant:
                                            Dimensional variant of the article. With <F9>, you can call up the variant
                                            selection. Here only the variants are displayed that are assigned to the cur-
                                            rent article in the master data.
                                        •   Box:
                                            Box number.
                                        •   Box description:
                                            Designation of the box.
                                        •   Supplier:
                                            Supplier number.
                                        •   Packing type:
                                            Identification of the packing type, e.g. 13 = small wooden box.
                                        •   New:
                                            Newly-calculated stock. This stock is taken over when the new article is
                                            booked. If you exit the dialog with <Home>, the old stock is retained.

                                        Stock Stock of the variant in the quantity unit that is defined in the master da-
                                        ta.
                                        •   UQ:
                                            Newly-calculated article stock in quantity units. This stock is taken over
                                            when the new article is booked. If you exit the dialog with <Home>, the old
                                            stock is retained.

                                        Prices The display of the current depends on the own currency that was
                                        specified during installation.
                                        • € / qm:
                                           Article price of the supplier in own currency per quantity unit.
                                        • Price:
                                           Total price of the article.
                                        • (Column without designation):
                                           Booking status of the article item.

                                        Booking status with         Meaning
                                        colored markings

                                            Gray                    Article item has been booked by the process
                                                                    (program).

                                            Red                     Article item has not or not yet been booked by the
                                                                    process (program).

                                        Tab. E-5      Booking status of the article item
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                    E-27
                 Stock Management                                                                  Software Reference




                                        Box warehouse out
                                        Booking > Box warehouse out




                 Fig. E-6   Box warehouse out


                                        On this tab, you book the warehouse outs for complete boxes. If you would like
                                        to remove only one part of the articles from a box, you must first resolve the
                                        box and book the articles of the box to another stock.
                                        You can execute the following keyboard commands:
                                        •   With <Ctrl> + <F8>, you can change in the first field between the Box ware-
                                            house in and Box warehouse out dialogs.
                                        •   With <F5>, you can change from one column in the box-related details into
                                            the footer area (left side).
                                        •   With <Shift> + <F8>, you can change from one column in the variant-relat-
                                            ed details into the footer area (right side).
                                        •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                            cord.
                                        •   With <Ctrl> + <F12>, you can book complete boxes. Thus the entire box is
                                            removed.
                                        •   With <Ctrl> + <F8>, you can resolve boxes and book the articles from the
                                            box to a target stock. Thus the individual sheets of the box are booked into
                                            the target stock.
                                        The tabs, fields, and columns are described here:
                                         “Box warehouse in” on page E-23
1.01 / 01-2017




                 E-28                                                                           A+W Enterprise Stock
                 Software Reference                                                                   Stock Management




                                         Slot warehouse in
                                         Booking > Slot stock
                                         On this dialog, you can book articles to slots of a slot stock.
                                         This dialog offers the following tabs:
                                         •   “Slot warehouse in – Pieces” on page E-29
                                         •   “Slot warehouse in – Quantity” on page E-32


                                         Slot warehouse in – Pieces
                                         Booking > Slot warehouse in > Pieces




                 Fig. E-7   Slot warehouse in – Pieces


                                         On this tab, you record and book the inventories and prices of the current ar-
                                         ticle variant in pieces.
                                         You can execute the following keyboard commands:
                                         •   With <Ctrl> + <F8>, you can change in the first field between the Slot ware-
                                             house in and Slot warehouse out dialogs.
                                         •   With <F5>, you can change from one column in the variant-related details
                                             into the footer area.
                                         •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                             cord.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                              E-29
                 Stock Management                                                                  Software Reference




                                    Header area
                                    The fields are described in the following section:
                                     “Warehouse in” on page E-16

                                    Rump area
                                    On this tab, you book the inventories and prices of the articles in pieces.
                                    •   Variant:
                                        Dimensional variant of the article. With <F9>, you can call up the variant
                                        selection. Here only the variants are displayed that are assigned to the cur-
                                        rent article in the master data.
                                    •   Slot:
                                        Designation of the slot.

                                    Stock HD (Piece) Stock of the variant in pieces.
                                    •   Old:
                                        Old article stock in the stock before booking.
                                    •   Booking:
                                        Article stock that is booked.
                                    •   New:
                                        Newly-calculated stock. This stock is taken over when the new article is
                                        booked. If you exit the dialog with <Home>, the old stock is retained.

                                    Prices The display of the current depends on the own currency that was
                                    specified during installation.
                                    • € / qm:
                                       Article price of the supplier in own currency per quantity unit.
                                    • Price:
                                       Total price of the article.
                                    • (Column without designation):
                                       Booking status of the article item.

                                    Booking status with         Meaning
                                    colored markings

                                        Gray                    Article item has been booked by the process
                                                                (program).

                                        Red                     Article item has not or not yet been booked by the
                                                                process (program).

                                    Tab. E-6      Booking status of the article item
1.01 / 01-2017




                 E-30                                                                          A+W Enterprise Stock
                 Software Reference                                                                    Stock Management




                                        Footer area – variant-related details

                                        Object Designation of the object for order-related stock articles, e.g. custom-
                                        er’s construction site.

                                        Cost center Designation of the cost center for statistical evaluations.

                                        Remark Text field for additional information.

                                        Minimum stock Minimum permissible stock of the article to prevent produc-
                                        tion bottlenecks.

                                        Alarm stock Quantity of the article stock that creates a P.O. proposal in pur-
                                        chasing. Alarm stocks can prevent a material shortage in the stock.

                                        Maximum stock Maximum permissible stock of the article to minimize stock
                                        costs.

                                        Total Total price of the article variant.

                                        Average price Average purchase price of the article variant in the stock.

                                        Maximum price Maximum purchase price of the article variant in the stock.

                                        Minimum price Minimum purchase price of the article variant in the stock.

                                        LIFO total price Total price of the article variant in the stock if the last re-
                                        ceived stock articles are sent out as the first articles.

                                        FIFO total price Total price of the article variant in the stock if the first re-
                                        ceived stock articles are sent out as the first articles.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                 E-31
                 Stock Management                                                                    Software Reference




                                         Slot warehouse in – Quantity
                                         Booking > Slot warehouse in > Quantity




                 Fig. E-8   Slot warehouse in – Quantity


                                         On this tab, you record and book the inventories and prices of the current ar-
                                         ticle variant in quantity unit.
                                         The Quantity tab is structured like the Pieces tab.
                                          “Header area” on page E-30
                                          “Footer area – variant-related details” on page E-31

                                         Rump area
                                         On this tab, you book the inventories and prices of the articles in quantity unit.
                                         •   Variant:
                                             Dimensional variant of the article. With <F9>, you can call up the variant
                                             selection. Here only the variants are displayed that are assigned to the cur-
                                             rent article in the master data.
                                         •   Slot:
                                             Designation of the slot.

                                         Stock HD (Unit) Stock of the variant in quantity unit.
                                         •   Old:
                                             Old article stock in the stock before booking.
                                         •
1.01 / 01-2017




                                             Booking:
                                             Article stock that is booked.




                 E-32                                                                             A+W Enterprise Stock
                 Software Reference                                                                   Stock Management




                                        •   New:
                                            Newly-calculated stock. This stock is taken over when the new article is
                                            booked. If you exit the dialog with <Home>, the old stock is retained.

                                        Prices The display of the current depends on the own currency that was
                                        specified during installation.
                                        • € / qm:
                                           Article price of the supplier in own currency per quantity unit.
                                        • Price:
                                           Total price of the article.
                                        • (Column without designation):
                                           Booking status of the article item.

                                        Booking status with        Meaning
                                        colored markings

                                            Gray                   Article item has been booked by the process
                                                                   (program).

                                            Red                    Article item has not or not yet been booked by the
                                                                   process (program).

                                        Tab. E-7     Booking status of the article item
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                   E-33
                 Stock Management                                                                   Software Reference




                                         Slot warehouse out
                                         Booking > Slot warehouse out




                 Fig. E-9   Slot warehouse out


                                         On this dialog, you can remove articles from the slot stock.
                                         You can execute the following keyboard commands:
                                         •   With <Ctrl> + <F8>, you can change in the first field between the Slot ware-
                                             house in and Slot warehouse out dialogs.
                                         •   With <F5>, you can change from one column in the variant-related details
                                             into the footer area.
                                         •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                             cord.
                                         The tabs, fields, and columns are described here:
                                          “Slot warehouse in” on page E-29
1.01 / 01-2017




                 E-34                                                                            A+W Enterprise Stock
                 Software Reference                                                                  Stock Management




                                        Stack warehouse in
                                        Booking > Stack in




                                        Fig. E-10    Stack warehouse in


                                        On this dialog, you can book articles to a stack. You can book different articles
                                        with different dimensions to a stack.
                                        You can execute the following keyboard commands:
                                        •   With <Ctrl> + <F8>, you can change in the first field between the Stack
                                            warehouse in and Modify stack warehouse dialogs.
                                        •   With <F2>, you can switch the display between articles in pieces and arti-
                                            cles in quantity unit.
                                        •   With <Shift> + <F8>, you can have the system assign a new stack number.
                                        •   With <Shift> + <F9>, you can copy all stack rows and assign a new stack
                                            number.
                                        •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                            cord.
                                        •   With <Ctrl> + <F12>, you can book a stack.
                                        •   With <End>, you can book the stack booking.

                                        Header area

                                        Stock Stock number and name.

                                        Supplier Supplier number and name.
1.01 / 01-2017




                                        Last change on, frm Date of the last change to the booking record and
                                        name of the user who made the last booking.




                 A+W Enterprise Stock                                                                              E-35
                 Stock Management                                                                Software Reference




                                    Rump area
                                    •   Stack:
                                        Number of the stack location.
                                    •   Description:
                                        Description of the stack location.
                                    •   Article:
                                        Article number of the article that is booked to the stack location.
                                    •   Variant:
                                        Designation of the article variant.
                                    •   Quantity:
                                        Quantity of the article.
                                        With <F2>, you can switch to articles in quantity unit.
                                    •   Quantity / qm:
                                        Quantity in square meters.
                                    •   Price / qm:
                                        Price per square meter.


                                    Modify stack warehouse
                                    Booking > Stack modification




                                    Fig. E-11     Modify stack warehouse


                                    On this dialog, you can search for articles that are in the stack in order to book
                                    them into another stock.
1.01 / 01-2017




                 E-36                                                                         A+W Enterprise Stock
                 Software Reference                                                                 Stock Management




                                        You can execute the following keyboard commands:
                                        •   With <Ctrl> + <F8>, you can change in the header area between the Stack
                                            warehouse in and Modify stack warehouse dialogs.
                                        •   With <Ctrl> + <F8>, you can resolve the selected stack in the rump area.
                                            When a stack is resolved, the articles from the resolved stack must be
                                            booked to another stock. You specify the stock for the articles in the Target
                                            stock column.
                                        •   With <Shift> + <F9>, you can copy the selected data record in the rump ar-
                                            ea.
                                        •   With <F2>, you can switch the display between articles in pieces and arti-
                                            cles in quantity unit.
                                        •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                            cord.
                                        •   With <Ctrl> + <F12>, you can remove a stack.
                                        •   With <End>, you can book the stack change.
                                        The fields and columns are described here:
                                         “Stack warehouse in” on page E-35
                                        In addition, the following fields are displayed:

                                        Header area

                                        Article 1, Article 2 Search across a sequence of article numbers.

                                        Rump area
                                        •   Target stock:
                                            Number of the target stock.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                              E-37
                 Stock Management                                                                      Software Reference




                                          Rack storage receipt
                                          Booking > Rack storage receipt




                 Fig. E-12   Rack storage receipt


                                          On this dialog, you can book articles on racks into a rack stock.
                                          You can execute the following keyboard commands:
                                          •   With <Ctrl> + <F8>, you can change in the first field between the Rack stor-
                                              age receipt and Rack storage exit dialogs.
                                          •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                              cord.

                                          Header area
                                          In the header area, you must either specify the article and the stock or the rack.

                                          Article Article number and name.

                                          Stock Stock number and name.

                                          Rack External designation of the stock rack.

                                          Total stock Total stock of the article, including all article variants.

                                          Total value Total value of the stock article.
1.01 / 01-2017




                                          Booking status Status of the bookings in the stock.




                 E-38                                                                               A+W Enterprise Stock
                 Software Reference                                                                     Stock Management




                                        Booking status with         Meaning
                                        colored markings

                                            Gray                    In warehouse in, all booking articles are booked by the
                                                                    process (program).

                                            Red                     In warehouse in, at least one booking article has not or
                                                                    not yet been booked by the process (program).

                                        Tab. E-8      Booking status of the stock

                                        Last change on, frm Date of the last change to the booking record and
                                        name of the user who made the last booking.

                                        Rump area
                                        •   Variant:
                                            Dimensional variant of the article. With <F9>, you can call up the variant
                                            selection. Variants of an article are only displayed if the variants are created
                                            in the master data module.
                                        •   Rack:
                                            External rack designation of the stock rack.
                                        •   M:
                                            Article variants that are on the rack.
                                             Various article variants are on one rack.
                                             Only the same article variants are on one rack.
                                        •   Slot:
                                            Designation of the slot.
                                        •   FIFO date:
                                            Date for the rack booking according to the FIFO principle.
                                        •   Quantity:
                                            Current quantity of the article on the stock rack.
                                        •   Booking:
                                            Article stock that is booked.
                                        •   € / qm:
                                            Article price of the supplier in own currency per quantity unit.
                                        •   Price:
                                            Total price of the article.
                                        •   Booking status:
                                            Status of the bookings in the rack storage.

                                        Booking status with         Meaning
                                        colored markings

                                            Gray                    Booking item has been booked by the process
                                                                    (program).

                                            Red                     Booking item has not or not yet been booked by the
                                                                    process (program).
1.01 / 01-2017




                                        Tab. E-9      Booking status of the rack storage receipt




                 A+W Enterprise Stock                                                                                   E-39
                 Stock Management                                                                     Software Reference




                                           Rack storage exit
                                           Booking > Rack storage exit
                                           On this dialog, you can book rack-related stock exits or rebook articles be-
                                           tween racks.
                                           This dialog offers the following tabs:
                                           •   “Rack storage exit – Order related” on page E-40
                                           •   “Rack storage exit – Transfer” on page E-42


                                           Rack storage exit – Order related
                                           Booking > Rack storage exit > Order related




                 Fig. E-13   Rack storage exit – Order related


                                           This tab is used to book order-related stock exits.
                                           You can execute the following keyboard commands:
                                           •   With <Ctrl> + <F8>, you can change in the first field between the Rack stor-
                                               age receipt and Rack storage exit dialogs.
                                           •   With <F2>, you can switch between the tabs Order related and Transfer.
                                           •   With <F5>, you can change to the variant-related details in the footer area.
                                           •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                               cord.
                                           •   With <Ctrl> + <F8>, you can resolve an item.
1.01 / 01-2017




                                           [Reset] Discards the changes entered.



                 E-40                                                                              A+W Enterprise Stock
                 Software Reference                                                                       Stock Management




                                        Header area
                                        In the header area, you must either specify the article and the stock or the rack.
                                        The fields are described in the following section:
                                         “Rack storage receipt” on page E-38

                                        Rump area
                                        •   Variant:
                                            Dimensional variant of the article. With <F9>, you can call up the variant
                                            selection. Variants of an article are only displayed if the variants are created
                                            in the master data module.
                                        •   Rack:
                                            External rack designation of the stock rack.
                                        •   G:
                                            Article variants that are on the rack.
                                             Various article variants are on one rack.
                                             Only the same article variants are on one rack.
                                        •   Slot:
                                            Designation of the slot.
                                        •   FIFO date:
                                            Date for the rack booking according to the FIFO principle.
                                        •   Quantity:
                                            Current quantity of the article on the stock rack.
                                        •   Booking:
                                            Article stock that is booked.
                                        •   Order:
                                            Order number for the order-related rack booking.
                                        •   Item:
                                            Number of the rack item in the rack stock.
                                        •   Booking status:
                                            Status of the bookings in the stock.

                                        Booking status with          Meaning
                                        colored markings

                                            Gray                     Booking item has been booked by the process
                                                                     (program).

                                            Red                      Booking item has not or not yet been booked by the
                                                                     process (program).

                                            Yellow                   Rack data was changed: For the order-related booking,
                                                                     a quantity or partial quantity from this rack was planned
                                                                     for the booking.

                                            Half yellow/half gray    Reworking is required: A new record was created with
                                                                     the remaining rack quantity for the subpart of the order
                                                                     item.
1.01 / 01-2017




                                        Tab. E-10      Booking status of the rack storage exit




                 A+W Enterprise Stock                                                                                     E-41
                 Stock Management                                                                      Software Reference




                                           Rack storage exit – Transfer
                                           Booking > Rack storage exit > Transfer




                 Fig. E-14   Rack storage exit – Transfer


                                           On this tab, you can transfer the article to a new rack or a new slot.
                                           You can execute the following keyboard commands:
                                           •   With <Ctrl> + <F8>, you can change in the first field between the Rack stor-
                                               age receipt and Rack storage exit dialogs.
                                           •   With <F2>, you can switch between the tabs Order related and Transfer.
                                           •   With <F5>, you can change to the variant-related details in the footer area.
                                           •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                               cord.
                                           •   With <Ctrl> + <F8>, you can resolve an item.

                                           [Reset] Discards the changes entered.

                                           Header area
                                           In the header area, you must either specify the article and the stock or the rack.
                                           The fields are described in the following section:
                                            “Rack storage receipt” on page E-38
1.01 / 01-2017




                 E-42                                                                               A+W Enterprise Stock
                 Software Reference                                                                       Stock Management




                                        Rump area
                                        •   Variant:
                                            Dimensional variant of the article. With <F9>, you can call up the variant
                                            selection. Variants of an article are only displayed if the variants are created
                                            in the master data module.
                                        •   Rack:
                                            External rack designation of the stock rack.
                                        •   G:
                                            Article variants that are on the rack.
                                             Various article variants are on one rack.
                                             Only the same article variants are on one rack.
                                        •   Slot:
                                            Designation of the slot.
                                        •   FIFO date:
                                            Date for the rack booking according to the FIFO principle.
                                        •   Qty:
                                            Current quantity of the article on the stock rack.
                                        •   Booking:
                                            Article stock that is booked.
                                        •   New rack:
                                            Number of the rack to which the article is transferred.
                                        •   New slot:
                                            Designation of the slot to which the rack is transferred.
                                        •   Booking status:
                                            Status of the bookings in the stock.

                                        Booking status with          Meaning
                                        colored markings

                                            Gray                     Booking item has been booked by the process
                                                                     (program).

                                            Red                      Booking item has not or not yet been booked by the
                                                                     process (program).

                                            Yellow                   Rack data was changed: For the order-related booking,
                                                                     a quantity or partial quantity from this rack was planned
                                                                     for the booking.

                                            Half yellow/half gray    Reworking is required: A new record was created with
                                                                     the remaining rack quantity for the subpart of the order
                                                                     item.

                                        Tab. E-11      Booking status of the rack storage exit
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                     E-43
                 Stock Management                                                            Software Reference




                                    Outgoing stocks (order-related)
                                    Booking > Outgoing stock (order related)




                                    Fig. E-15    Outgoing stocks (order-related)


                                    On this dialog, you can book the order-related outgoing stocks manually. It is
                                    defined in the article master data whether an article can only be booked man-
                                    ually.
                                    You can execute the following keyboard commands:
                                    •   With <F2>, you can display the Date column for the delivery date of the
                                        item.
                                    •   With <F3>, you can trigger the booking.
                                    •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                        cord.

                                    Header area

                                    Order Order number.

                                    Journey Delivery date on which the order is delivered to the customer.

                                    Customer Customer number and name.

                                    Ent’rd on, frm Date of the order entry and name of the person who entered
                                    the order.

                                    Book on, frm Date of the stock exit booking and name of the employee who
                                    make the stock exit booking.
1.01 / 01-2017




                 E-44                                                                      A+W Enterprise Stock
                 Software Reference                                                               Stock Management




                                        Rump area
                                        •   Itm.:
                                            Number of the order item.
                                        •   Article:
                                            Product code.
                                        •   Description:
                                            Article description.
                                        •   Variant:
                                            Dimensional variant of the item.
                                        •   Total:
                                            Total quantity per item.
                                        •   Booked:
                                            Quantity of the item that was already removed.
                                        •   Book:
                                            Quantity of the item that should be removed from the stock.
                                        With <F2>, you can display the Date column for the delivery date of the item.
                                        •   Date:
                                            Delivery date of the item.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                          E-45
                 Stock Management                                                              Software Reference




                                    Correction – Overview
                                    Booking > Correction




                                    Fig. E-16    Correction – Overview


                                    On this dialog, you can specify the search criteria for having bookings dis-
                                    played and correcting them.
                                    In order to be able to correct bookings, stock data must first have been created
                                    through the stock booking system. Back-up stock data is only created if times
                                    for automatic saving of the stock data are defined, e.g. on the 15th of each
                                    month. Flawed booking records may not be present in the booking system.
                                    You can display the details of the overview on the detail view.
                                     “Booking correction – Details” on page E-47
                                    You can execute the following keyboard commands:
                                    •   With <F5>, you change between the overview and the detail view of the se-
                                        lected item.
                                    •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                        cord.

                                    Header area

                                    Article Article number and name.

                                    Stock Stock number and name.

                                    From date, to date Time period for which the bookings are listed.
1.01 / 01-2017




                 E-46                                                                       A+W Enterprise Stock
                 Software Reference                                                                  Stock Management




                                        Rump area
                                        •   Variant:
                                            Article variant.
                                        •   Color:
                                            Color variant of the article.
                                        •   Supplier:
                                            Supplier number.
                                        •   Quantity:
                                            Quantity unit of the article in the booking to be corrected.
                                        •   Quantity:
                                            Quantity of the booking to be corrected.
                                        •   Price:
                                            Piece price of the variant.
                                        •   Stat.:
                                            Designation of the booking status, e.g. warehouse in.
                                        •   Date:
                                            Date on which the booking was corrected.


                                        Booking correction – Details
                                        Booking > Correction > Filter > <F5>




                                        Fig. E-17     Booking correction – Details


                                        On this dialog, the details of a booking correction from the overview are dis-
                                        played and corrected.
                                        You can execute the following keyboard commands:
                                        •   With <F5>, you change between the overview and the detail view of the se-
                                            lected item.
1.01 / 01-2017




                                        •   With <Shift> + <F12>, you can enter a new date for the current booking re-
                                            cord.




                 A+W Enterprise Stock                                                                            E-47
                 Stock Management                                                             Software Reference




                                    Header area
                                    The fields are described in the following section:
                                     “Header area” on page E-46

                                    Rump area

                                    Box Box number.

                                    Slot Designation of the slot.

                                    Variant Article variant.

                                    Color Color variant of the article.

                                    Supplier Supplier number.

                                    Order Order number for order-related stock bookings.

                                    Item Number of the order item.

                                    Quantity Quantity unit of the article in the booking to be corrected.

                                    Pieces Number of pieces of the booking to be corrected.

                                    Price Piece price of the variant.

                                    Status Designation of the booking status, e.g. warehouse in.

                                    Date Date on which the booking was corrected.
1.01 / 01-2017




                 E-48                                                                      A+W Enterprise Stock
                 Software Reference                                                        Master Data Management




                                        Master Data Management
                                        In the master data, you manage the stock room and the stock limits for stock
                                        articles, e.g. you create new storage spaces in the warehouse. You also define
                                        the stock articles and their stock limits.
                                        This section explains the following dialogs:
                                        •   “Stock room administration” on page E-50
                                        •   “Article master data stock” on page E-51
1.01 / 01-2017




                 A+W Enterprise Stock                                                                           E-49
                 Master Data Management                                                           Software Reference




                                      Stock room administration
                                      Master data > Room




                                      Fig. E-18     Stock room administration


                                      On this dialog, you can create new stock rooms. The specified assignment of
                                      stock number, stock designation, stock type, and inventory type can no longer
                                      be changed after saving. For a stock room, you must always specify the type
                                      of stock and inventory.
                                      You save the data for the stock room with <End>.

                                      Header area

                                      Stock Number and designation of the stock.

                                      Name Name of the stock.

                                      In Site Number and designation of the company or site.

                                      Rump area

                                      Inventory type Type of stock control.
                                      •   Permanent = Permanent inventory.
                                      •   Cyclical = Cyclical inventory on the balance sheet date
                                       “Inventory – Standard stock” on page E-54

                                      StockTyp Type of the stock:
                                      •   Normal stock = stock for all articles without restrictions.
                                      •   Box stock = stock for complete boxes. Boxes that are broken open must be
                                          resolved and booked to another stock.
                                      •   Slot stock = stock for all articles with assigned designation of the slot.
                                      •   Rack stock = stock with storage spaces on high racks.
                                      •   Stack stock = stock for sheets with uniform dimensions.
                                      •   Single sheet box stock = stock for booking of individual glass sheets in box-
1.01 / 01-2017




                                          es.
                                      •   Rack stock = stock with storage spaces on racks.



                 E-50                                                                          A+W Enterprise Stock
                 Software Reference                                                          Master Data Management




                                        Interface Specification of the software interface. Selection for a customer-
                                        side connected stock management system.

                                        Size Storage space in quantity unit.

                                        Fixed costs Fixed costs of the storage space in own currency per square
                                        meter.

                                        Variable costs Variable costs of the storage space in own currency per
                                        square meter.

                                        GR stock Number of the warehouse incoming stock.


                                        Article master data stock
                                        Master data > Article




                                        Fig. E-19    Article master data stock


                                        On this dialog, you can specify the stock limits of the stock articles. The stock
                                        limits of the stock articles are specified by the minimum stock, alarm stock, and
                                        maximum stock.
                                        You can execute the following keyboard commands:
                                        •   If you are in a column in the rump area, you can save the specification of
                                            the stock limits with <End>.
                                        •   With <F5>, you can change to the footer area.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                              E-51
                 Master Data Management                                                        Software Reference




                                      Header area

                                      Article Article number and name.

                                      Stock Stock number and name.

                                      Order variant Article variant for reorders.

                                      Color Color variant of the article for reorders.

                                      Stock limits

                                      Minimum stock Minimum permissible stock of the article to prevent produc-
                                      tion bottlenecks.

                                      Alarm stock Quantity of the article stock that creates a P.O. proposal in pur-
                                      chasing. Alarm stocks can prevent a material shortage in the stock.

                                      Maximum stock Maximum permissible stock of the article to minimize stock
                                      costs.

                                      Rump area
                                      With <F2>, you can switch the display between articles in pieces and articles
                                      in quantity unit.

                                      Variant Dimensional variant of the article.

                                      Color Color variant of the article.

                                      Footer area

                                      Remark With <F5>, you can change to the text field for remarks about the
                                      article variant.
1.01 / 01-2017




                 E-52                                                                       A+W Enterprise Stock
                 Software Reference                                                        Inventory Management




                                        Inventory Management
                                        With inventory management, you compare the stocks counted with the stocks
                                        booked by the system and correct the numbers in the system accordingly.
                                        This section explains the following dialogs:
                                        •   “Inventory – Standard stock” on page E-54
                                        •   “Inventory – Box stock” on page E-57
                                        •   “Inventory – Slots” on page E-59
                                        •   “Inventory – Stack stock” on page E-60
                                        •   “Inventory – Rack stock” on page E-61
1.01 / 01-2017




                 A+W Enterprise Stock                                                                       E-53
                 Inventory Management                                                                 Software Reference




                                           Inventory – Standard stock
                                           Inventory > Stock




                 Fig. E-20   Inventory – standard stock


                                           On this dialog, you can perform and complete the inventory for the standard
                                           stock.

                                               Stock in inventory
                                               If a stock is enabled for the inventory, a copy of the stock with negative
                                               stock numbers is generated, the so-called inventory stock. The stocks
                                               counted are entered in this inventory stock.
                                               During the inventory, the warehouse ins and outs are still booked to the
                                               positive stock number. This guarantees that during the inventory, ware-
                                               house in and out bookings for this stock can be recorded.
                                               After an inventory completion, the changed stocks are updated from the in-
                                               ventory stock with the incoming and outgoing bookings that were recorded
                                               during the inventory.

                                           The dialogs for the inventory in the various stock types are structured identi-
                                           cally and are therefore described for the standard stock. The description there-
                                           fore applies for:
                                           •   Box stock
                                           •   Slot stock
1.01 / 01-2017




                                           •   Stack stock
                                           •   Rack stock




                 E-54                                                                              A+W Enterprise Stock
                 Software Reference                                                              Inventory Management




                                        You can execute the following keyboard commands:
                                        •   With <F2>, you can switch the display between articles in pieces and arti-
                                            cles in quantity unit.
                                        •   With <Shift> + <F8>, you can complete the inventory.
                                        •   With <Shift> + <F12>, you can discard the inventory.

                                        Header area

                                        from Article, to Article Value range of the article numbers in order to filter
                                        the inventory list.

                                        from Stock, to Stock Input of the stock numbers:
                                        •   If in the from Stock, to Stock fields you enter the same stock number, the
                                            stock is enabled for the inventory.
                                        •   If in the from Stock, to Stock fields you enter a range of stock numbers, the
                                            data records are loaded into the dialog for viewing.

                                        Inventory/assessment at Date of the inventory.

                                        Rump area
                                        The following columns are displayed:
                                        •   Article:
                                            Product code.
                                        •   Stock:
                                            Stock number.
                                        •   Variant:
                                            Dimensional variant of the item.
                                        •   C:
                                            Cancellation of the article.
                                            – N = No cancellation of the article.
                                            – Y = Article was canceled.
                                        •   Def.qty.:
                                            Display of target quantity of the article in the stock.
                                        •   Actual qty.:
                                            Display of actual quantity of the counted article in the stock.
                                        •   Price:
                                            Total price of the actual stock of the article.
                                        •   QU:
                                            Average price per quantity unit for the actual stock, e.g. € 75.00 per square
                                            m.
                                        •   Remark:
                                            Inventory remark for statistical evaluations.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                              E-55
                 Inventory Management                                                                 Software Reference




                                        With <F2>, you can display the following columns:
                                        •   Target stock:
                                            Display of target value of the quantity unit of the article stock in the stock.
                                        •   Actual stock:
                                            Input for actual value of the counted quantity unit of the article stock in the
                                            stock.

                                        Footer area

                                        Article Article designation of the selected article.

                                        A-Price Average price of the selected article for the actual stock.

                                        TotPrice Total price of the selected article for the actual stock.

                                        Stock Stock designation of the selected stock.

                                        LIFO price Article price in the stock if booking and calculation are done ac-
                                        cording to the LIFO booking method.

                                        FIFO price Article price in the stock if booking and calculation are done ac-
                                        cording to the FIFO booking method.
1.01 / 01-2017




                 E-56                                                                              A+W Enterprise Stock
                 Software Reference                                                              Inventory Management




                                           Inventory – Box stock
                                           Inventory > Box stock




                 Fig. E-21   Inventory - box stock


                                           On this dialog, you can perform and complete the inventory for the box stock.
                                           A description of the fields is found here:
                                            “Header area” on page E-55

                                           Rump area
                                           •   Box:
                                               Box number.
                                           •   Stock:
                                               Stock number.
                                           •   Article:
                                               Product code.
                                           •   Variant:
                                               Dimensional variant of the item.
                                           •   C:
                                               Cancellation of the article.
                                               – N = No cancellation of the article.
                                               – Y = Article was canceled.
                                           •   Quantity:
1.01 / 01-2017




                                               Total sheet area in a box.




                 A+W Enterprise Stock                                                                              E-57
                 Inventory Management                                                               Software Reference




                                        •   Pieces:
                                            Number of sheets in the box.
                                        •   DT:
                                            Identification of the packing type.
                                        •   Supp.No:
                                            Supplier number.
                                        •   QU:
                                            Average price per quantity unit for the actual stock, e.g. € 75.00 per square
                                            m.
                                        •   Remark:
                                            Inventory remark for statistical evaluations.

                                        Footer area

                                        Article Article description.

                                        Stock Stock designation.

                                        Box Box description.

                                        Pack type Identification of the packing type.

                                        Supplier Supplier name.
1.01 / 01-2017




                 E-58                                                                            A+W Enterprise Stock
                 Software Reference                                                              Inventory Management




                                           Inventory – Slots
                                           Inventory > Slot stock




                 Fig. E-22   Inventory - slot stock


                                           On this dialog, you can perform and complete the inventory for the slot stock.
                                           A description of the fields is found here:
                                            “Header area” on page E-55
                                            “Footer area” on page E-56

                                           Rump area
                                           •   Stock:
                                               Stock number.
                                           •   Article:
                                               Product code.
                                           •   Variant:
                                               Dimensional variant of the item.
                                           •   C:
                                               Cancellation of the article.
                                               – N = No cancellation of the article.
                                               – Y = Article was canceled.
                                           •   Slot:
                                               Designation of the slot.
1.01 / 01-2017




                                           •   Qty:
                                               Quantity of the article in quantity unit.



                 A+W Enterprise Stock                                                                               E-59
                 Inventory Management                                                                   Software Reference




                                           •   Pieces:
                                               Display of actual quantity of the counted article in the stack.
                                           •   Price:
                                               Total price of the actual stock of the article.
                                           •   Remark:
                                               Inventory remark for statistical evaluations.


                                           Inventory – Stack stock
                                           Inventory > Stack stock




                 Fig. E-23   Inventory - Stack stock


                                           On this dialog, you can perform and complete the inventory for the stack stock.
                                           A description of the fields is found here:
                                            “Header area” on page E-55
                                            “Footer area” on page E-56

                                           Rump area
                                           •   Stock:
                                               Stock number.
                                           •   Article:
                                               Product code.
1.01 / 01-2017




                                           •   Variant:
                                               Dimensional variant of the item.




                 E-60                                                                                A+W Enterprise Stock
                 Software Reference                                                                 Inventory Management




                                           •   C:
                                               Cancellation of the article.
                                               – N = No cancellation of the article.
                                               – Y = Article was canceled.
                                           •   Stack:
                                               Stack number.
                                           •   Description:
                                               Description of the stack.
                                           •   Quantity:
                                               Display of actual quantity of the counted article in the stack.
                                           •   Price:
                                               Total price of the actual stock of the article.
                                           •   Remark:
                                               Inventory remark for statistical evaluations.


                                           Inventory – Rack stock
                                           Inventory > Rack stock




                 Fig. E-24   Inventory - rack stock


                                           On this dialog, you can perform and complete the inventory for the rack stock.
                                           A description of the fields is found here:
                                            “Header area” on page E-55
1.01 / 01-2017




                                            “Footer area” on page E-56




                 A+W Enterprise Stock                                                                               E-61
                 Inventory Management                                                                Software Reference




                                        Rump area
                                        •   Stock:
                                            Stock number.
                                        •   Article:
                                            Product code.
                                        •   Variant:
                                            Dimensional variant of the item.
                                        •   C:
                                            Cancellation of the article.
                                            – N = No cancellation of the article.
                                            – Y = Article was canceled.
                                        •   Def.qty.:
                                            Target quantity of the article.
                                        •   Actual qty.:
                                            Display of actual quantity of the counted article in the stack.
                                        •   Price:
                                            Total price of the actual stock of the article.
                                        •   QU:
                                            Quantity.
                                        •   Remark:
                                            Inventory remark for statistical evaluations.
                                        With <F2>, you can display the following columns:
                                        •   G:
                                            Article variants that are on the rack.
                                             Various article variants are on one rack.
                                             Only the same article variants are on one rack.
                                        •   Rack:
                                            Designation of the rack.
                                        •   Slot:
                                            Designation of the slot.
                                        •   Target:
                                            Target quantity of the article.
                                        •   Actual:
                                            Actual quantity of the article.
                                        •   FIFO date:
                                            Date for the rack booking according to the FIFO principle.
                                        •   Status:
                                            Status of the bookings in the rack storage.
1.01 / 01-2017




                 E-62                                                                             A+W Enterprise Stock
                 Software Reference                                                               Inventory Management




                                        Booking status with        Meaning
                                        colored markings

                                          Gray                     Booking item has been booked by the process
                                                                   (program).

                                          Red                      Booking item has not or not yet been booked by the
                                                                   process (program).

                                          Yellow                   Booking item has been changed.

                                          Half yellow/half gray    Booking item is a subpart of an order. Booking item
                                                                   must be booked to another stock, e.g. slot stock.

                                        Tab. E-12    Booking status of the rack storage
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                E-63
                 Evaluation                                                               Software Reference




                              Evaluation
                              In the evaluation, you can edit the value losses of circulating assets within an
                              inventory. For the inventory, the objects of the circulating assets can be imple-
                              mented with the lowest-value principle (procurement, manufacturing or day
                              value) on the final balance sheet.
                              This section explains the following dialogs:
                              •   “Evaluation – Standard stock” on page E-65
                              •   “Evaluation – Box stock” on page E-67
                              •   “Evaluation – Slot stock” on page E-68
                              •   “Evaluation – Stack stock” on page E-69
                              •   “Rack stock evaluation” on page E-70
1.01 / 01-2017




                 E-64                                                                  A+W Enterprise Stock
                 Software Reference                                                                             Evaluation




                                          Evaluation – Standard stock
                                          Evaluation > Stock




                 Fig. E-25   Evaluation – standard stock


                                          On this dialog, you can make a value correction of the article stock within an
                                          inventory, e.g. if the values of a stock article deviate from the current values.
                                          The dialogs for the inventory evaluation in the various stock types are struc-
                                          tured identically and are therefore described for the standard stock. The de-
                                          scription therefore applies for:
                                          •   Box stock
                                          •   Slot stock
                                          •   Stack stock
                                          •   Rack stock
                                          You can execute the following keyboard commands:
                                          •   With <F2>, you can switch the display between articles in pieces and arti-
                                              cles in quantity unit. The function applies only for the standard stock.
                                          •   With <End>, you can complete the value correction.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                 E-65
                 Evaluation                                                                 Software Reference




                              Header area

                              from Article, to Article Value range of the article numbers in order to filter
                              the list.

                              from Stock, to Stock Input of the stock numbers:
                              •   If in the from Stock, to Stock fields you enter the same stock number, the
                                  stock is enabled for the stock evaluation.
                              •   If in the from Stock, to Stock fields you enter a range of stock numbers, the
                                  data records are loaded into the dialog for viewing.

                              Inventory/assessment of Date of the inventory evaluation.

                              Rump area
                              The following columns are displayed:
                              •   Stock:
                                  Stock number.
                              •   Article:
                                  Product code.
                              •   Variant:
                                  Dimensional variant of the item.
                              •   C:
                                  Cancellation of the article.
                                  – N = No cancellation of the article.
                                  – Y = Article was canceled.
                              •   Def.qty.:
                                  Display of target quantity of the article in the stock.
                              •   Actual qty.:
                                  Display of actual quantity of the counted article in the stock.
                              •   Price:
                                  Input for the total price of the actual stock of the article.
                              •   QU:
                                  Input of the average price per quantity unit for the actual stock, e.g. € 75.00
                                  per square m.
                              •   Remark:
                                  Inventory remark for statistical evaluations.
                              With <F2>, you can display the following columns:
                              •   Target stock:
                                  Display of target value of the quantity unit of the article stock in the stock.
                              •   Actual stock:
                                  Input for actual value of the counted quantity unit of the article stock in the
                                  stock.
1.01 / 01-2017




                 E-66                                                                    A+W Enterprise Stock
                 Software Reference                                                                             Evaluation




                                          Footer area

                                          Article Article designation of the selected article.

                                          A-Price Average price of the selected article for the actual stock.

                                          TotPrice Total price of the selected article for the actual stock.

                                          Stock Stock designation of the selected stock.

                                          LIFO price Article price in the stock if booking and calculation are done ac-
                                          cording to the LIFO booking method.

                                          FIFO price Article price in the stock if booking and calculation are done ac-
                                          cording to the FIFO booking method.


                                          Evaluation – Box stock
                                          Evaluation > Box stock




                 Fig. E-26   Evaluation – box stock


                                          On this dialog, you can make a value correction of the article stock within an
                                          inventory, e.g. if the values of boxes deviate from the current values.
                                          The stock evaluation may only be carried out within a single stock.
1.01 / 01-2017




                                          The fields and columns are described here:
                                           “Evaluation – Standard stock” on page E-65



                 A+W Enterprise Stock                                                                               E-67
                 Evaluation                                                                           Software Reference




                                            Evaluation – Slot stock
                                            Evaluation > Slot stock




                 Fig. E-27    Evaluation – slot stock


                                            On this dialog, you can make a value correction of the article stock within an
                                            inventory, e.g. if the values of a slot deviate from the current values.
                                            The stock evaluation may only be carried out within a single stock.
                                            The fields and columns are described here:
                                             “Evaluation – Standard stock” on page E-65
1.01 / 01-2017




                 E-68                                                                              A+W Enterprise Stock
                 Software Reference                                                                              Evaluation




                                           Evaluation – Stack stock
                                           Evaluation > Stack stock




                 Fig. E-28   Evaluation – stack stock


                                           On this dialog, you can make a value correction of the article stock within an
                                           inventory, e.g. if the values of a stack deviate from the current values.
                                           The stock evaluation may only be carried out within a single stock.
                                           The fields and columns are described here:
                                            “Evaluation – Standard stock” on page E-65
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                E-69
                 Evaluation                                                                            Software Reference




                                           Rack stock evaluation
                                           Evaluation > Rack stock




                 Fig. E-29    Rack stock evaluation


                                           On this dialog, you can make a value correction of the article stock within an
                                           inventory, e.g. if the values of a rack deviate from the current values.
                                           The stock evaluation may only be carried out within a single stock.
                                           The fields and columns are described here:
                                            “Evaluation – Standard stock” on page E-65
                                           You can execute the following keyboard command:
                                           With <F2>, you can switch the display for articles in pieces to articles in quan-
                                           tity unit. The function applies only for the rack stock.
1.01 / 01-2017




                 E-70                                                                               A+W Enterprise Stock
                 Software Reference                                                                Information System




                                        Information System
                                        In the information system, you can monitor the stock data. With the information
                                        system, you can execute the search functions.
                                        This section explains the following dialogs:
                                        •   “Info: Stock products” on page E-72
                                        •   “Info: Stock variants” on page E-75
                                        •   “Info: Stock slots” on page E-80
                                        •   “Info: Stock racks” on page E-83
                                        •   “Info: Stock stacks” on page E-87
                                        •   “Info: Stock sheets” on page E-90
                                        •   “Info: Stock history” on page E-93
                                        •   “Orders/Purchase Orders” on page E-98
                                        •   “Booking Status” on page E-102
                                        •   “Stock Information – Pick list” on page E-108
                                        •   “Stock Information – Hit list” on page E-109
                                        •   “LVR Status” on page E-110
                                        •   “Range – Stock Forecast” on page E-110
                                        •   “Range – Hit list” on page E-111
                                        •   “Available stock” on page E-112
                                        •   “Stock forecast” on page E-113
                                        In addition, you can compile individual information overviews using SQL que-
                                        ries.
                                         Sales, “SQL query – Execute” on page D-220
1.01 / 01-2017




                 A+W Enterprise Stock                                                                            E-71
                 Information System                                                                 Software Reference




                                      Info: Stock products
                                      Info System > Article
                                      On this dialog, you can display the stocks or article stocks.
                                      This dialog displays the following subdialogs:
                                      •   “Info: Stock products – Filter dialog” on page E-72
                                      •   “Info: Stock products – Hit list” on page E-73
                                      •   “Info: Stock products – Hit list details” on page E-74


                                      Info: Stock products – Filter dialog
                                      Info System > Article




                                      Fig. E-30     Info: stock products - filter dialog


                                      On this dialog, you can specify the search criteria for displaying the stocks or
                                      article stocks. You can display the results of the search in the hit list and in the
                                      detail view.
                                       “Info: Stock products – Hit list” on page E-73
                                       “Info: Stock products – Hit list details” on page E-74

                                      Article Product code.

                                      Stock Stock number.

                                      Quantity Articles in quantity unit.

                                      Total Total price of the article stock in the selected stock.

                                      Average price Average price per quantity unit of the article.

                                      Last change Date on which the booking status was last booked.
1.01 / 01-2017




                 E-72                                                                            A+W Enterprise Stock
                 Software Reference                                                                  Information System




                                        Info: Stock products – Hit list
                                        Info System > Article > Filter




                                        Fig. E-31     Info: stock products - hit list


                                        This dialog displays the results of the search for stock articles.
                                        Details about the stock articles are displayed in the detail view.
                                         “Info: Stock products – Hit list details” on page E-74
                                        With <F5>, you change between the hit list and the detail view of the selected
                                        item.

                                        Hit list
                                        The following columns are displayed:
                                        •   Article:
                                            Product code.
                                        •   Stock:
                                            Stock number.
                                        •   Stock:
                                            Stock of the article in quantity unit.
                                        •   TotPric:
                                            Total price of the article.
                                        •   A-Price:
                                            Average price per quantity unit.
                                        •   H-Price:
                                            Highest purchase price per quantity unit.
                                        •   L-Price:
                                            Lowest purchase price per quantity unit.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                            E-73
                 Information System                                                                  Software Reference




                                      Info: Stock products – Hit list details
                                      Info System > Article > Filter > <F5>




                                      Fig. E-32     Info: stock products - hit list details


                                      This dialog displays the details of the hit list of stock articles.
                                      With <F5>, you change between the hit list and the detail view of the selected
                                      item.

                                      Details

                                      Article Article number and name.

                                      Stock Stock number.

                                      Stock Stock of the article in quantity unit.

                                      Minimum stock Minimum stock of the article in stock.

                                      Alarm stock Alarm stock of the article in stock.

                                      Maximum stock Maximum stock of the article in stock.

                                      Max. stock Maximum stock of the article in stock since the last inventory.

                                      Min. stock Minimum stock of the article in stock since the last inventory.

                                      A-Stock Average stock of the article since the last inventory.

                                      A-Consumption Average stock withdrawals of the article since the last in-
1.01 / 01-2017




                                      ventory.

                                      Total Total price of the article.



                 E-74                                                                             A+W Enterprise Stock
                 Software Reference                                                                   Information System




                                        A-Price Average price per quantity unit.

                                        Maximum price Highest purchase price of the article.

                                        Minimum price Lowest purchase price of the article.

                                        LIFO total price Total price of the article variant in the stock if booking and
                                        calculation are done according to the LIFO booking method.

                                        FIFO total price Total price of the article variant in the stock if booking and
                                        calculation are done according to the FIFO booking method.

                                        Last amendment on Date on which the booking record was booked and
                                        name of the user who made the last booking.


                                        Info: Stock variants
                                        Info System > Variant
                                        On this dialog, you can display the information about the article variants ac-
                                        cording to selected criteria.
                                        This dialog displays the following subdialogs:
                                        •   “Info: Stock variants – Filter dialog” on page E-75
                                        •   “Info: Stock variants – Hit list” on page E-76
                                        •   “Info: Stock variants – Hit list details” on page E-78


                                        Info: Stock variants – Filter dialog
                                        Info System > Variant




                                        Fig. E-33     Info: stock variants - filter dialog


                                        On this dialog, you can filter the information about the article variants accord-
                                        ing to selected criteria. The results are displayed in a hit list. You can view the
                                        details in the detail view.
1.01 / 01-2017




                                         “Info: Stock variants – Hit list” on page E-76
                                         “Info: Stock variants – Hit list details” on page E-78



                 A+W Enterprise Stock                                                                                E-75
                 Information System                                                                     Software Reference




                                             Article Product code.

                                             Stock Stock number.

                                             Variant Dimensional variant of the article in the box.

                                             Color Color variant of the article.

                                             Box Box number.

                                             Box description Designation of the box.

                                             Last change Date on which the booking record was booked.

                                             Qty Articles in quantity unit.

                                             Pieces Quantity of the article.

                                             Total price Total price of the article stock.

                                             Average price Average price per quantity unit of the article.


                                             Info: Stock variants – Hit list
                                             Info System > Variant > Filter




                 Fig. E-34   Info: stock variants - hit list
1.01 / 01-2017




                 E-76                                                                                 A+W Enterprise Stock
                 Software Reference                                                                   Information System




                                        On this dialog, you can filter the information about the article variants accord-
                                        ing to selected criteria. The results are displayed in a hit list. You can view the
                                        details in the detail view.
                                         “Info: Stock variants – Hit list details” on page E-78
                                        With <F5>, you change between the hit list and the detail view of the selected
                                        item.

                                        Hit list
                                        •   Article:
                                            Article number.
                                        •   Description:
                                            Article description.
                                        •   Stock:
                                            Stock number.
                                        •   Box:
                                            Box number.
                                        •   Variant:
                                            Dimensional variant of the article in the box.
                                        •   Color:
                                            Color variant of the article.
                                        •   Quantity:
                                            Quantity of the article.
                                        •   Stock:
                                            Article stock in quantity unit.
                                        •   Net QU:
                                            Net quantity per box in quantity unit of the article.
                                        •   Price:
                                            Total price of the article.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                                E-77
                 Information System                                                                         Software Reference




                                             Info: Stock variants – Hit list details
                                             Info System > Variant > Filter > <F5>




                 Fig. E-35   Info: stock variants - hit list details


                                             This dialog displays the details of the hit list of article variants.
                                             With <F5>, you change between the hit list and the detail view of the selected
                                             item.

                                             Details

                                             Article Article number and name.

                                             Stock Stock number.

                                             Box Box number and box designation.

                                             Variant Dimensions of the variant.

                                             Color Color variant of the article.

                                             Pieces Quantity of the article.

                                             Stock Article stock in quantity unit.

                                             net quantity Net quantity per box in quantity unit of the article.

                                             Minimum stock Minimum stock of the article in stock.

                                             Alarm stock Alarm stock of the article in stock.

                                             Maximum stock Maximum stock of the article in stock.

                                             Max. stock Maximum stock of the article in stock since the last inventory.
1.01 / 01-2017




                                             Min. stock Minimum stock of the article in stock since the last inventory.



                 E-78                                                                                    A+W Enterprise Stock
                 Software Reference                                                                Information System




                                        A-Stock Average stock of the article since the last inventory.

                                        A-Consumption Average stock withdrawals of the article since the last in-
                                        ventory.

                                        Total Total price of the article.

                                        A-Price Average price per quantity unit.

                                        Max. price Highest purchase price of the article.

                                        Minimum price Lowest purchase price of the article.

                                        LIFO total price Total price of the article variant in the stock if booking and
                                        calculation are done according to the LIFO booking method.

                                        FIFO total price Total price of the article variant in the stock if booking and
                                        calculation are done according to the FIFO booking method.

                                        Last amendment on Date on which the booking record was booked and
                                        name of the user who made the last booking.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                             E-79
                 Information System                                                                 Software Reference




                                      Info: Stock slots
                                      Info System > Slot
                                      On this dialog, you can display the information about the stock slots.
                                      This dialog displays the following subdialogs:
                                      •   “Info: Stock slots” on page E-80
                                      •   “Info: Stock slots – Hit list” on page E-81
                                      •   “Info: Stock slots – Hit list details” on page E-82


                                      Info: Stock slots
                                      Info System > Slot




                                      Fig. E-36     Info-stock-slots - filter dialog


                                      On this dialog, you can filter the information about the stock slots according to
                                      selected criteria. The results are displayed in a hit list. You can view the details
                                      in the detail view.
                                       “Info: Stock slots – Hit list” on page E-81
                                       “Info: Stock slots – Hit list details” on page E-82

                                      Article Product code.

                                      Stock Stock number.

                                      Slot Designation of the slot.

                                      Variant Dimensions of the variant.

                                      Color Color variant of the article.

                                      Date Date on which the booking record was booked.

                                      Piece Quantity of the article.

                                      Qty Articles in quantity unit.
1.01 / 01-2017




                 E-80                                                                            A+W Enterprise Stock
                 Software Reference                                                                 Information System




                                        Info: Stock slots – Hit list
                                        Info System > Slot > Filter




                                        Fig. E-37     Info-stock-slots - hit list


                                        This dialog displays the results of the search for stock slots. You can view the
                                        details in the detail view.
                                         “Info: Stock products – Hit list details” on page E-74
                                        With <F5>, you change between the hit list and the detail view of the selected
                                        item.

                                        Hit list
                                        •   Article:
                                            Product code.
                                        •   Stock:
                                            Stock number.
                                        •   Slot:
                                            Designation of the slot.
                                        •   Variant:
                                            Dimensions of the variant.
                                        •   Qty:
                                            Articles in quantity unit.
                                        •   Piece:
                                            Number of pieces of the article.
                                        •   Price:
                                            Total price of the article.
                                        •   Date:
                                            Date on which the booking record was booked.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                             E-81
                 Information System                                                                  Software Reference




                                      Info: Stock slots – Hit list details
                                      Info System > Slot > Filter > <F5>




                                      Fig. E-38     Info-stock-slots - hit list details


                                      This dialog displays the details of the hit list of stock slots.
                                      With <F5>, you change between the hit list and the detail view of the selected
                                      item.

                                      Details

                                      Article Product code.

                                      Stock Stock number.

                                      Slot Designation of the slot.

                                      Variant Dimensions of the variant.

                                      Color Color variant of the article.

                                      Qty Articles in quantity unit.

                                      Piece Number of pieces of the article.

                                      Price Total price of the article.
1.01 / 01-2017




                 E-82                                                                             A+W Enterprise Stock
                 Software Reference                                                                       Information System




                                        Info: Stock racks
                                        Info System > Rack
                                        On this dialog, you can display the information about the stock racks.
                                        This dialog displays the following subdialogs:
                                        •   “Info: Stock racks – Filter dialog” on page E-83
                                        •   “Info: Stock racks – Hit list details – General” on page E-84
                                        •   “Info: Stock racks – Hit list details” on page E-85


                                        Info: Stock racks – Filter dialog
                                        Info System > Rack




                                        Fig. E-39     Info-Stock-Rack - filter dialog


                                        On this dialog, you can filter the information about the stock racks according
                                        to selected criteria. The results are displayed in a hit list. You can view the de-
                                        tails in the detail view.
                                         “Info: Stock racks – Hit list details – General” on page E-84
                                         “Info: Stock racks – Hit list details” on page E-85

                                        Stock Stock number.

                                        Rack no. Number of the stock rack.

                                        Rack Designation of the rack.

                                        Slot Designation of the slot.

                                        Article Product code.

                                        Variant Dimensions of the variant.

                                        Color Color variant of the article.
1.01 / 01-2017




                                        Piece Number of pieces of the article.

                                        FIFO date Date for the rack booking according to the FIFO principle.



                 A+W Enterprise Stock                                                                                 E-83
                 Information System                                                                    Software Reference




                                            Info: Stock racks – Hit list details – General
                                            Info System > Rack > Filter > General




                 Fig. E-40   Info-Stock-Racks - hit list details-general


                                            This dialog displays the results of the search for stock racks. You can view the
                                            details in the detail view.
                                             “Info: Stock racks – Hit list details” on page E-85
                                            With <F5>, you change between the hit list and the detail view of the selected
                                            item.

                                            Hit list
                                            •   Stock:
                                                Stock number.
                                            •   Article:
                                                Product code.
                                            •   Variant:
                                                Dimensions of the variant.
                                            •   Rack no..:
                                                Number of the stock rack.
                                            •   Rack:
                                                Designation of the rack.
                                            •   Slot:
                                                Designation of the slot.
                                            •   Description:
1.01 / 01-2017




                                                Designation of the slot.




                 E-84                                                                               A+W Enterprise Stock
                 Software Reference                                                                           Information System




                                            •   Piece:
                                                Number of pieces of the article.
                                            •   Price:
                                                Total price of the article.
                                            •   FIFO date:
                                                Date for the rack booking according to the FIFO principle.


                                            Info: Stock racks – Hit list details
                                            Info System > Rack > Filter > Details




                 Fig. E-41   Info-Stock-Racks - hit list details


                                            This dialog displays the details of the hit list of stock rack.
                                            With <F5>, you change between the hit list and the detail view of the selected
                                            item.

                                            Details

                                            Article Product code.

                                            Variant Dimensions of the variant.

                                            Color Color variant of the article.

                                            Piece Number of pieces of the article.
1.01 / 01-2017




                                            Price Total price of the article.

                                            Stock Stock number.


                 A+W Enterprise Stock                                                                                     E-85
                 Information System                                                           Software Reference




                                      Rack Designation of the rack.

                                      Slot Designation of the slot.

                                      FIFO date Date for the rack booking according to the FIFO principle.

                                      Last change on Date of the last change to the booking record and name of
                                      the user who made the last booking.
1.01 / 01-2017




                 E-86                                                                      A+W Enterprise Stock
                 Software Reference                                                                   Information System




                                        Info: Stock stacks
                                        Info System > Stack
                                        On this dialog, you can display the information about the stock stacks.
                                        This dialog displays the following subdialogs:
                                        •   “Info: Stock stacks – Filter dialog” on page E-87
                                        •   “Info: Stock stacks – Hit list” on page E-88
                                        •   “Info: Stock stacks – Hit list details” on page E-89


                                        Info: Stock stacks – Filter dialog
                                        Info System > Stack




                                        Fig. E-42     Info-stock-stack- filter dialog


                                        On this dialog, you can filter the information about the stock stacks according
                                        to selected criteria. The results are displayed in a hit list. You can view the de-
                                        tails in the detail view.
                                         “Info: Stock stacks – Hit list” on page E-88
                                         “Info: Stock stacks – Hit list details” on page E-89

                                        Article Product code.

                                        Stock Stock number.

                                        Stack Stack number.

                                        Stack des. Description of the stack.

                                        Variant Dimensions of the variant.

                                        Color Color variant of the article.

                                        Date Date on which the booking record was booked.

                                        Piece Number of pieces of the article.
1.01 / 01-2017




                                        Quantity Articles in quantity unit.



                 A+W Enterprise Stock                                                                                E-87
                 Information System                                                                     Software Reference




                                             Info: Stock stacks – Hit list
                                             Info System > Stack > Filter




                 Fig. E-43   Info-stock-stack - hit list


                                             This dialog displays the results of the search for stock stacks. You can view
                                             the details in the detail view.
                                              “Info: Stock stacks – Hit list details” on page E-89
                                             With <F5>, you change between the hit list and the detail view of the selected
                                             item.

                                             Hit list
                                             •   Stack:
                                                 Stack number.
                                             •   Description:
                                                 Description of the stack.
                                             •   Article:
                                                 Product code.
                                             •   Stock:
                                                 Stock number.
                                             •   Variant:
                                                 Dimensions of the variant.
                                             •   Qty:
                                                 Articles in quantity unit.
1.01 / 01-2017




                 E-88                                                                                 A+W Enterprise Stock
                 Software Reference                                                                    Information System




                                        •   Piece:
                                            Number of pieces of the article.
                                        •   Price:
                                            Total price of the article.
                                        •   Date:
                                            Date on which the booking record was booked.


                                        Info: Stock stacks – Hit list details
                                        Info System > Stack > Filter > <F5>




                                        Fig. E-44     Info-stock-stack - hit list details


                                        This dialog displays the details of the hit list of the stock stack.
                                        With <F5>, you change between the hit list and the detail view of the selected
                                        item.

                                        Details

                                        Article Product code.

                                        Stock Stock number.

                                        Stack Stack number.

                                        Variant Dimensions of the variant.
1.01 / 01-2017




                                        Color Color variant of the article.

                                        Qty Articles in quantity unit.

                 A+W Enterprise Stock                                                                              E-89
                 Information System                                                               Software Reference




                                      Piece Number of pieces of the article.

                                      Price Total price of the article.

                                      Last change on Date of the last change to the booking record and name of
                                      the user who made the last booking.


                                      Info: Stock sheets
                                      Info System > Sheet
                                      On this dialog, you can display the information about the glass sheets in the
                                      individual sheet box stock.
                                      This dialog displays the following subdialogs:
                                      •   “Info: Stock sheets – Filter dialog” on page E-90
                                      •   “Info: Stock sheets – Hit list” on page E-92


                                      Info: Stock sheets – Filter dialog
                                      Info System > Sheet




                                      Fig. E-45     Info-stock-sheets- filter dialog


                                      On this dialog, you can filter the information about the glass sheets in the indi-
                                      vidual sheet box stock according to selected criteria. The results are displayed
                                      in a hit list.
                                       “Info: Stock sheets – Hit list” on page E-92
1.01 / 01-2017




                 E-90                                                                          A+W Enterprise Stock
                 Software Reference                                                   Information System




                                        Sheet Number of the glass sheet.

                                        Description Description of the glass sheet.

                                        Article Product code.

                                        Stock Stock number.

                                        Box Box number.

                                        Box description Designation of the box.

                                        Variant Dimensions of the variant.

                                        Color Color variant of the article.

                                        Price Piece price of the glass sheet.

                                        Yield Yield of the glass sheet in percent.
1.01 / 01-2017




                 A+W Enterprise Stock                                                             E-91
                 Information System                                                               Software Reference




                                      Info: Stock sheets – Hit list
                                      Info System > Sheet > Filter




                                      Fig. E-46    Info-stock-sheets- hit list


                                      This dialog displays the results of the search for glass sheets in the individual
                                      sheet box stock.

                                      Hit list
                                      •   Article:
                                          Product code.
                                      •   Stock:
                                          Stock number.
                                      •   Box:
                                          Box number.
                                      •   Variant:
                                          Dimensions of the variant.
                                      •   Sheet:
                                          Number of the glass sheet.
                                      •   Description:
                                          Description of the glass sheet.
                                      •   Price:
                                          Piece price of the glass sheet.
                                      •   Yield.:
                                          Yield of the glass sheet in percent.
                                      •   R.:
                                          Reservation code.
1.01 / 01-2017




                                          – Y = Variant is reserved for a process.
                                          – N = Variant is not reserved for a process.



                 E-92                                                                          A+W Enterprise Stock
                 Software Reference                                                                   Information System




                                        Info: Stock history
                                        Info System > History
                                        On this dialog, you can display the information about the stock bookings.
                                        This dialog displays the following subdialogs:
                                        •   “Info: Stock history – Filter dialog” on page E-93
                                        •   “Info: Stock history – Hit list” on page E-94
                                        •   “Info: Stock history – Hit list details” on page E-96


                                        Info: Stock history – Filter dialog
                                        Info System > History




                                        Fig. E-47     Info-stock-history - filter dialog


                                        On this dialog, you can filter the information about the stock bookings accord-
                                        ing to selected criteria. The results are displayed in a hit list. You can view the
                                        details in the detail view.
                                         “Info: Stock history – Hit list” on page E-94
                                         “Info: Stock history – Hit list details” on page E-96

                                        Article Product code.

                                        Stock Stock number.

                                        Supplier Supplier number.

                                        Order Order number.

                                        Opti. no The job number for the XTV interface is only displayed if the function
                                        was configured appropriately.

                                        Variant Dimensional variant of the article.

                                        Color Color variant of the article.
1.01 / 01-2017




                                        Stack Stack number.

                                        SheetDesign Description of the glass sheet.


                 A+W Enterprise Stock                                                                                E-93
                 Information System                                                                      Software Reference




                                             Box Box number.

                                             Date Date on which the booking record was booked.

                                             Piece Number of pieces of the article.

                                             Quantity Articles in quantity unit.

                                             Price Total price of the article.

                                             Cost center Designation of the cost center.

                                             Status Status of the current record, e.g. warehouse out.


                                             Info: Stock history – Hit list
                                             Info System > History > Filter




                 Fig. E-48   Info-stock-history - hit list


                                             This dialog displays the results of the search for stock bookings. You can view
                                             the details in the detail view.
                                              “Info: Stock history – Hit list details” on page E-96
                                             With <F5>, you change between the hit list and the detail view of the selected
                                             item.
1.01 / 01-2017




                 E-94                                                                                  A+W Enterprise Stock
                 Software Reference                                                                 Information System




                                        Hit list
                                        •   Article:
                                            Product code.
                                        •   Stock:
                                            Stock number.
                                        •   Variant:
                                            Dimensional variant of the article.
                                        •   Slot:
                                            Designation of the slot.
                                        •   Piece:
                                            Number of pieces of the article.
                                        With <F2>, you can display the following columns:
                                        •   Box:
                                            Box number.
                                        •   DT:
                                            Identification of the packing type.
                                        •   Supplier:
                                            Supplier number.
                                        •   Stack:
                                            Stack number.
                                        •   L-Price:
                                            Article price in the stock if booking and calculation are done according to
                                            the LIFO booking method.
                                        •   F-Price:
                                            Article price in the stock if booking and calculation are done according to
                                            the FIFO booking method.
                                        •   Order no.:
                                            Order number.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                             E-95
                 Information System                                                                       Software Reference




                                             Info: Stock history – Hit list details
                                             Info System > History > Filter > <F5>




                 Fig. E-49   Info-stock-history - hit list details


                                             This dialog displays the details of the hit list of the stock bookings.
                                             With <F5>, you change between the hit list and the detail view of the selected
                                             item.

                                             Details

                                             Article Product code.

                                             Stock Stock number.

                                             Box Box number.

                                             Pack type Identification of the packing type.

                                             Supplier Supplier number.

                                             Slot Designation of the slot.

                                             Sheet Number and designation of the sheet.

                                             Order Order number.
1.01 / 01-2017




                                             Opti. no The job number for the XTV interface is only displayed if the function
                                             was configured appropriately.


                 E-96                                                                                  A+W Enterprise Stock
                 Software Reference                                                               Information System




                                        Customer Customer number and name.

                                        Variant Dimensional variant of the article.

                                        Color Color variant of the article.

                                        Booked qty Quantity that was booked for this booking record.

                                        Qty booked Total quantity in quantity unit that was booked.

                                        Booking price Total price of the booked quantities.

                                        LIFO price Article price in the stock if booking and calculation are done ac-
                                        cording to the LIFO booking method.

                                        FIFO price Article price in the stock if booking and calculation are done ac-
                                        cording to the FIFO booking method.

                                        Cost center Designation of the cost center.

                                        Last booking on Date of the last change to the booking record and name of
                                        the user who made the last booking.

                                        Remark Additional information about the warehouse in booking.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                           E-97
                 Information System                                                                 Software Reference




                                      Orders/Purchase Orders
                                      Info System > Orders/Purchase Orders
                                      On this dialog, you can display the information about order or purchase order-
                                      related bookings.
                                      This dialog displays the following subdialogs:
                                      •   “Orders/Purch. Orders – Filter dialog” on page E-98
                                      •   “Orders/Purch. Orders – Hit list” on page E-99
                                      •   “Orders/Purch. Orders – Hit list details” on page E-100


                                      Orders/Purch. Orders – Filter dialog
                                      Info System > Orders/Purchase Orders




                                      Fig. E-50     Orders/Purch. Orders – filter dialog


                                      On this dialog, you can filter the information about order and purchase order-
                                      related bookings in the stock according to selected criteria. The results are dis-
                                      played in a hit list. You can view the details in the detail view.
                                       “Orders/Purch. Orders – Hit list” on page E-99
                                       “Orders/Purch. Orders – Hit list details” on page E-100

                                      Order Order number or purchase order number.

                                      Article Product code.

                                      Stock Stock number.

                                      Variant Number of the article variant.

                                      Color Number of the color variant.
1.01 / 01-2017




                 E-98                                                                             A+W Enterprise Stock
                 Software Reference                                                                    Information System




                                           Booking Booking status of the order or purchase order.
                                           The following options are available:
                                           • 0 = no booking has been made.
                                           • 1 = partial booking of an item has been made.
                                           • 2 = item is completely booked.
                                           • 3 = order or purchase order was completely booked.

                                           Date Date on which the stock booking for the order or purchase order was
                                           made.


                                           Orders/Purch. Orders – Hit list
                                           Info System > Orders/Purchase Orders > Filter




                 Fig. E-51   Orders/Purch. Orders – hit list


                                           This dialog displays the results of the search for order or purchase order-relat-
                                           ed bookings in the stock. You can view the details in the detail view.
                                            “Orders/Purch. Orders – Hit list details” on page E-100
                                           With <F5>, you change between the hit list and the detail view of the selected
                                           item.

                                           Hit list
                                           •   Order:
                                               Order number or purchase order number.
1.01 / 01-2017




                                           •   Item:
                                               Number of the item in the order or purchase order.



                 A+W Enterprise Stock                                                                                 E-99
                 Information System                                                                     Software Reference




                                            •   Article:
                                                Product code.
                                            •   Stock:
                                                Stock number.
                                            •   Variant:
                                                Number of the article variant.
                                            •   Pieces:
                                                Number of pieces to be booked per item.
                                            •   Qty:
                                                Booking quantity in the quantity unit of the item.
                                            •   Booked:
                                                Booking quantity in pieces that was booked.
                                            •   Date:
                                                Date on which the stock booking for the order or purchase order was made.


                                            Orders/Purch. Orders – Hit list details
                                            Info System > Orders/Purchase Orders > Filter > <F5>




                 Fig. E-52   Orders/Purch. Orders – hit list details


                                            This dialog displays the results of the hit list of the order or purchase order-
                                            related bookings in the stock.
                                            With <F5>, you change between the hit list and the detail view of the selected
                                            item.
1.01 / 01-2017




                 E-100                                                                               A+W Enterprise Stock
                 Software Reference                                                               Information System




                                        Details

                                        Article no. Article number and name.

                                        Stock Stock number.

                                        Variant Number of the article variant.

                                        Color Number of the color variant.

                                        Order Order number or purchase order number.

                                        Item Number of the item in the order or purchase order.

                                        Pieces Number of pieces to be booked per item.

                                        Quantity Booking quantity in the quantity unit of the item.

                                        Booking Booking status of the order or purchase order.
                                        The following options are available:
                                        • 0 = no booking has been made.
                                        • 1 = partial booking of an item has been made.
                                        • 2 = item is completely booked.
                                        • 3 = order or purchase order was completely booked.

                                        Date Date on which the stock booking for the order or purchase order was
                                        made.

                                        Booked (pieces) Booked pieces of the article.

                                        Booked (quantity) Booking quantity in the quantity unit of the article.

                                        Staff Recording date and employee who recorded the booking.

                                        Staff Booking date and employee who recorded the booking.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                             E-101
                 Information System                                                            Software Reference




                                      Booking Status
                                      Info System > Booking Status
                                      In the booking status, you can display the booking information about the
                                      stocks that contain unbooked or flawed booking records or stocks that are in
                                      inventory at the moment. On the Booking status – Correction dialog, you can
                                      correct the data for the booking status.
                                      This dialog displays the following subdialogs:
                                      •   “Booking Status – Unbooked” on page E-102
                                      •   “Booking Status – Error” on page E-104
                                      •   “Booking Status – Inventory” on page E-105
                                      •   “Booking Status – Correction” on page E-106


                                      Booking Status – Unbooked
                                      Info System > Booking Status > Unbooked




                                      Fig. E-53    Booking Status – unbooked


                                      On this dialog, you can display booking information about the stocks that con-
                                      tain unbooked booking records.
                                      You can execute the following keyboard commands:
                                      •   With <F5>, you can call up the Booking Status – Correction dialog.
                                      •   With <F2>, you can display additional columns:
1.01 / 01-2017




                 E-102                                                                      A+W Enterprise Stock
                 Software Reference                                                                   Information System




                                        Rump area
                                        •   Article:
                                            Product code.
                                        •   Stock:
                                            Stock number.
                                        •   Box:
                                            Box number.
                                        •   Variant:
                                            Dimensional variant of the article.
                                        •   Color:
                                            Number of the article color.
                                        •   Qty:
                                            Number of unbooked articles.
                                        •   Status:
                                            Number of the status of the current booking, e.g. warehouse out.
                                        •   Error:
                                            Number of the error status. The error status is in plain text in the footer ar-
                                            ea.
                                        With <F2>, you can display additional columns:
                                        •   Quantity:
                                            Quantity unit of the article.
                                        •   Price:
                                            Price per quantity unit, e.g. articles per piece.
                                        •   Date:
                                            Date of the stock booking.
                                        •   Order:
                                            Order number.
                                        •   Item:
                                            Item number in the order.

                                        Footer area
                                        The field descriptions correspond to the column descriptions for the dialog.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                              E-103
                 Information System                                                                Software Reference




                                      Booking Status – Error
                                      Info System > Booking Status > Error




                                      Fig. E-54     Booking Status – Error


                                      On this dialog, you can display booking information about the stocks that con-
                                      tain flawed booking records. On the Booking status – Correction dialog, you
                                      can correct the data for the booking status.
                                      You can execute the following keyboard commands:
                                      •   With <F5>, you can call up the Booking Status – Correction dialog.
                                      •   With <F2>, you can display additional columns:

                                      Rump area
                                      •   Article:
                                          Product code.
                                      •   Stock:
                                          Stock number.
                                      •   Box:
                                          Box number.
                                      •   Variant:
                                          Dimensional variant of the article.
                                      •   Color:
                                          Number of the article color.
                                      •   Quantity:
                                          Number of unbooked articles.
                                      •   Status:
                                          Number of the status of the current booking, e.g. warehouse out.
                                      •   Error:
                                          Number of the error status. The error status is in plain text in the footer ar-
1.01 / 01-2017




                                          ea.




                 E-104                                                                          A+W Enterprise Stock
                 Software Reference                                                               Information System




                                        With <F2>, you can display additional columns:
                                        •   Quantity:
                                            Quantity unit of the article.
                                        •   Price:
                                            Price per quantity unit, e.g. articles per piece.
                                        •   Date:
                                            Date of the stock booking.
                                        •   Order:
                                            Order number.
                                        •   Item:
                                            Item number in the order.

                                        Footer area
                                        The field descriptions correspond to the column descriptions for the dialog.


                                        Booking Status – Inventory
                                        Info System > Booking Status > Inventory




                                        Fig. E-55     Booking Status – Inventory


                                        On this dialog, you can display the booking information about the stocks that
                                        contain unbooked or flawed booking records or stocks that are in inventory at
                                        the moment. On the Booking status – Correction dialog, you can correct the
                                        data for the booking status.
                                        You can execute the following keyboard command:
                                        •   With <F5>, you can call up the Booking Status – Correction dialog.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                            E-105
                 Information System                                                              Software Reference




                                      Rump area
                                      •   Stock:
                                          Stock number of the stock that is enabled for inventory.
                                      •   Description:
                                          Description of the stock in inventory.
                                      •   Date:
                                          Date on which the stock was prepared for inventory.
                                      •   Employee:
                                          Employee number of the employee who prepared the stock for inventory.


                                      Booking Status – Correction
                                      Info System > Booking Status > Unbooked, error, inventory > <F5>




                                      Fig. E-56    Booking Status – Correction


                                      On this dialog, you can correct the data of the booking status of the following
                                      dialogs:
                                      •   Booking Status – unbooked
                                      •   Booking Status – Error
                                      •   Booking Status – Inventory

                                      Rump area

                                      Article Article number and name.

                                      Stock Stock number and name.

                                      Supplier Supplier number and name.

                                      Box Box number and box designation.
1.01 / 01-2017




                                      Slot Designation of the slot in the slot stock.



                 E-106                                                                        A+W Enterprise Stock
                 Software Reference                                                               Information System




                                        Order Order number for order-related stock bookings.

                                        Variant Dimensional variant of the article.

                                        Color Number of the article color.

                                        Booked qty Booked quantity in pieces.

                                        Qty booked Booked quantity in the appropriate quantity unit.

                                        Booking price Total price of the article.

                                        Booked on Date of the last booking of the current booking record.

                                        from Name of the employee who last booked the current booking record.

                                        Footer area

                                        Article Article description.

                                        Stock Stock designation.

                                        Error Error status in plain text.

                                        Status Status of the current record in plain text, e.g. warehouse out.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                            E-107
                 Information System                                                              Software Reference




                                      Stock Information – Pick list
                                      Info System > Order list




                                      Fig. E-57    Stock Information – Pick list


                                      On this dialog, you can display the order-related stock articles. For the output
                                      of the stock information for the pick list, the ad hoc SQL group 1 and the SQL
                                      query 26 are used. If necessary, this query must be adjusted separately. You
                                      can adjust the query with <Ctrl> + <F4> > SQL queries > change.

                                      Order Order number for which the pick list is created.
1.01 / 01-2017




                 E-108                                                                         A+W Enterprise Stock
                 Software Reference                                                                    Information System




                                        Stock Information – Hit list
                                        Info System > Order list > Filter




                                        Fig. E-58     Stock Information – hit list


                                        This dialog displays the hit list for order-related stock articles.

                                        Hit list
                                        •   Product:
                                            Product code.
                                        •   Description:
                                            Article description.
                                        •   Color:
                                            Designation of the color variant of the article.
                                        •   Variant:
                                            Dimensions of the article variant.
                                        •   Quantity:
                                            Number of pieces of the article.
                                        •   Order:
                                            Order number.
                                        •   Columns without names:
                                            Item number in the order.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                             E-109
                 Information System                                                                Software Reference




                                      LVR Status
                                      Info System > LVR Status




                                      Fig. E-59    SQL queries - stock management calculator (LVR)


                                      At present, this dialog is not used.


                                      Range – Stock Forecast
                                      Info System > Range




                                      Fig. E-60    Range - SQL queries.


                                      On this dialog, you can display the stock forecast for stock articles. For the out-
                                      put of the stock forecast for the range, the ad hoc SQL group 1 and the SQL
                                      query 21 are used. If necessary, this query must be adjusted separately. You
                                      can adjust the query with <Ctrl> + <F4> > SQL queries > change.

                                      From product Start value for the value range of product codes for filtering the
                                      hit list.

                                      To product Maximum value for the value range of product codes for filtering
                                      the hit list.

                                      From stock Start value for the value range of stock numbers for filtering the
                                      hit list.

                                      To stock Maximum value for the value range of stock numbers for filtering the
                                      hit list.
1.01 / 01-2017




                 E-110                                                                          A+W Enterprise Stock
                 Software Reference                                                                   Information System




                                        Range – Hit list
                                        Info System > Range > Filter




                                        Fig. E-61     Range – hit list


                                        This dialog displays a forecast using stock bookings for how many months the
                                        current stock of the stock article will suffice for production.

                                        Hit list
                                        •   Product:
                                            Product code.
                                        •   Stock:
                                            Current stock of the article.
                                        •   Consumption:
                                            Consumption of the article in the past.
                                        •   Range (Months):
                                            Estimated time in months that the article will still be available in stock.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                               E-111
                 Information System                                                               Software Reference




                                      Available stock
                                      Info System > Available Stock




                                      Fig. E-62     Available stock


                                      On this dialog, you can display the current stock of the article, as well as the
                                      ordered, planned, and available quantities of the stock article.

                                      Header area

                                      Date Filter criterion by date.

                                      Article Filter criterion for the article number.

                                      Variant Filter criterion for the dimensional variant.

                                      Rump area
                                      •   Variant:
                                          Dimensional variant of the article.
                                      •   Stock:
                                          Stock number of the stock in which the article is stored.
                                      •   Description:
                                          Description of the stock article.
                                      •   Stock:
                                          Current stock of the stock article.
                                      •   Ordered:
                                          Currently-ordered quantity of the stock article.
                                      •   Scheduled:
                                          Currently-scheduled quantity of the stock article, e.g. for production.
                                      •   Available:
1.01 / 01-2017




                                          Currently-ordered quantity of the stock article.




                 E-112                                                                         A+W Enterprise Stock
                 Software Reference                                                                   Information System




                                        Footer area

                                        Totals Totaled value for each column. The following columns are displayed
                                        totaled:
                                        •   Stock
                                        •   Ordered
                                        •   Scheduled
                                        •   Available


                                        Stock forecast
                                        Info System > Forecast




                                        Fig. E-63    Stock forecast


                                        On this dialog, you can display the forecast for the stock of the article for a se-
                                        lected time period. Scheduled stocks arise due to orders recorded. The fore-
                                        cast shows the stock based on orders present in the system and already-
                                        placed orders.
                                        The over or undercoverage of the stocks can be prevented with defined alarm
                                        stocks.
                                         “Article master data stock” on page E-51
                                        With <Shift> + <F5>, you can display the stock forecast in a graphic overview
                                        for the selected articles.
1.01 / 01-2017




                 A+W Enterprise Stock                                                                              E-113
                 Information System                                                               Software Reference




                                      Header area

                                      Article Article number for the filtered listing.

                                      Stock Stock number. If there is no entry in this field, a stock-spanning stock
                                      forecast is created.

                                      Version Dimensional version of the article.

                                      Date Time period of the stock forecast.

                                      Period Time distances in the stock forecast.

                                      Rump area
                                      The columns are described in the header area. In addition, the following col-
                                      umns are displayed:
                                      •   Date:
                                          Date specification for the stock forecast for scheduled, ordered and in-
                                          stock articles.
                                      •   Scheduled:
                                          Scheduled articles from the stock for the date displayed in the first column.
                                      •   Ordered:
                                          Scheduled articles for the stock for the date displayed in the first column.
                                      •   Stock:
                                          Stock of the article in stock for the date displayed in the first column.
1.01 / 01-2017




                 E-114                                                                         A+W Enterprise Stock
                 Software Reference                                                                                  Print




                                        Print
                                        In Print, you can print information about the stock data or labels. You can freely
                                        define the page layout for the list printing or the labels.
                                        This section explains the following dialogs:
                                        •   “Print labels for boxes” on page E-116
                                        •   “List printing” on page E-117
1.01 / 01-2017




                 A+W Enterprise Stock                                                                              E-115
                 Print                                                               Software Reference




                         Print labels for boxes
                         Print > Labels




                         Fig. E-64    Print labels for boxes


                         On this dialog, you can display the open print orders for box labels and print
                         them.
                         With <Shift> + <F3>, you start the label printing.
                         •   Box:
                             Box number.
                         •   Pieces:
                             Quantity of the article in the box.
                         •   Article:
                             Product code.
                         •   Variant:
                             Dimensional version of the article.
                         •   Stock:
                             Stock number.
                         •   C.centr:
                             Designation of the cost center.
                         •   Column without designation:
                             Display for the label printing:
                             – Y = print labels.
                             – N = do not print labels.
                         •   Qty.:
                             Number of labels to be printed
                         •
1.01 / 01-2017




                             Ent’rd:
                             Date on which the box receipt was entered.
                         •   Printed:
                             Date on which the label for the box was last printed.


                 E-116                                                           A+W Enterprise Stock
                 Software Reference                                                                     Print




                                        List printing
                                        Print > List print




                                        Fig. E-65     List printing


                                        This dialog is described in detail in the following section:
                                         Sales, “List printing” on page D-162
1.01 / 01-2017




                 A+W Enterprise Stock                                                                  E-117
                 System Administration                                                            Software Reference




                                         System Administration
                                         In the system administration, you can manage the stock lots and price correc-
                                         tions of the stock articles.
                                         This section explains the following dialogs:
                                         •   “Delete stock log” on page E-119
                                         •   “Stock price correction” on page E-119
1.01 / 01-2017




                 E-118                                                                         A+W Enterprise Stock
                 Software Reference                                                              System Administration




                                        Delete stock log
                                        System > Delete stock log




                                        Fig. E-66    Deleting storage log


                                        On this dialog, you can delete a stock log on the system.

                                        Article Product code.

                                        Stock Stock number.

                                        Variant Dimensional variant of the article.

                                        Color Color variant of the article.


                                        Stock price correction
                                        System > Price correction




                                        Fig. E-67    Stock price correction


                                        On this dialog, you can correct the average price for purchased stock articles.
                                        Flawed price bookings for stock articles falsify the average price in the statis-
                                        tics and can only be corrected using the highest and lowest prices.

                                        Article Product code.

                                        Stock Stock number.

                                        Variant Dimensional variant of the article.

                                        Color Color variant of the article.
1.01 / 01-2017




                                        Max. price Maximum purchase price of the variant in the stock.

                                        Minimum price Minimum purchase price of the variant in the stock.

                 A+W Enterprise Stock                                                                             E-119
                 Service Functions                                                            Software Reference




                                     Service Functions
                                     Service functions are only executed on request by the A+W Software GmbH
                                     service technicians.
                                     The service functions are found here:
                                      Dispatch Control, “Service Functions” on page G-92
1.01 / 01-2017




                 E-120                                                                      A+W Enterprise Stock
Stock                 E

            Section index




        A+W Enterprise
                 Section index                                                                   Index




                 Index
                 A                                        I
                 Article master data                      Info
                 – Stock limits for stock articles E-51   – Display stocks E-72
                 Article stock                            – stock hit list E-73
                 – Correct box stock E-67                 Info System
                 – Correct rack stock E-70                – Available stock E-112
                 – Correct slot stock E-68                – Booking Status, correction E-106
                 – Correct stack stock E-69               – Booking Status, error E-104
                 – Correct standard stock E-65            – Booking Status, inventory E-105
                 Available stock                          – Booking status, unbooked booking
                 – Info System E-112                        records E-102
                                                          – Orders/Purchase Orders E-98, E-99, E-100
                 B                                        – Stock forecast E-113
                 Booking                                  – Stock range E-111
                 – Box stock E-23, E-28                   Info-stock-history
                 – Modify stack warehouse E-36            – Display stocks E-93, E-94, E-96
                 – Order-related, with E-44               Info-Stock-Racks
                 – Rack stock E-38, E-40                  – Display stocks E-83, E-84, E-85
                 – Slot stock E-29, E-34                  Info-stock-sheets
                 – Stack warehouse in E-35                – Display stocks E-90, E-92
                 – Standard Stock E-16, E-22              Info-stock-slots
                 Booking correction                       – Display stocks E-80, E-81, E-82
                 – Edit open bookings E-46, E-47          Info-stock-stack
                 Booking status                           – Display stocks E-87, E-88, E-89
                 – Correction E-106                       Inventory
                 – Error E-104                            – Box stock E-57
                 – Inventory E-105                        – Rack stock E-61
                 – Unbooked booking records E-102         – Slot stock E-59
                 Box labels                               – Stack stock E-60
                 – Print E-116                            – Standard Stock E-54
                 Box stock
                 – Book warehouse ins E-23                L
                 – Book warehouse outs E-28               List printing
                 – Correct article stock E-67             – printing E-117
                 – Inventory E-57                         LVR status
                                                          – SQL queries E-110
                 D
                 Delete                                   M
                 – Stock log E-119                        Menus   E-9
                 Display stocks
                 – Article variants E-75                  O
                 – Rack stock E-83, E-84, E-85            Orders/Purchase Orders
                 – Sheets E-90, E-92                      – Info System E-98, E-99, E-100
                 – Stack stock E-87, E-88, E-89           Outgoing stock
                 – Stock articles E-72                    – book order-related E-44
1.01 / 01-2017




                 – Stock history E-93, E-94, E-96
                 – Stock slots E-80, E-81, E-82




                 A+W Enterprise Stock                                                           E-123
                 Index                                                            Section index




                 P                              Stock information
                 Pick list                      – Pick list E-109
                 – Stock information E-109      – SQL Queries E-108
                 Price correction               Stock limits for stock articles
                 – Stock articles E-119         – Article master data E-51
                 Print                          Stock log
                 – Box labels E-116             – delete E-119
                 – Lists E-117                  Stock products
                                                – Display stocks E-72
                                                Stock room administration
                 R
                                                – Stock rooms, create new E-50
                 Rack stock
                                                Stock variants
                 – Book receipts E-38
                                                – Display stocks E-75
                 – Book warehouse outs E-40
                                                – hit list E-76
                 – Correct article stock E-70
                                                – hit list details E-78
                 – Inventory E-61
                 Range
                 – Info System E-111            W
                 – SQL Queries E-110            Warehouse in
                                                – book E-16
                                                Warehouse out
                 S
                                                – book E-22
                 Slot stock
                 – Book receipts E-29
                 – Book warehouse outs E-34
                 – Correct article stock E-68
                 – Inventory E-59
                 SQL Queries
                 – Stock information E-108
                 – Stock range E-110
                 SQL queries
                 – LVR status E-110
                 Stack stock
                 – Book changes E-36
                 – Book warehouse ins E-35
                 – Book warehouse outs E-36
                 – Correct article stock E-69
                 – Inventory E-60
                 Standard Stock
                 – Book warehouse ins E-16
                 – Book warehouse outs E-22
                 – Correct article stock E-65
                 – Inventory E-54
                 Stock articles
                 – Price correction E-119
                 Stock evaluation
                 – Box stock E-67
                 – Rack stock E-70
                 – Slot stock E-68
                 – Stack stock E-69
                 – Standard Stock E-65
1.01 / 01-2017




                 Stock forecast
                 – Info System E-113



                 E-124                                                  A+W Enterprise Stock

