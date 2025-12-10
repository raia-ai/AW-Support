---
description: "EN AWEnterprise DispatchControl"
---



# EN AWEnterprise DispatchControl

Dispatch Control              G




                              deutsch




                   A+W Enterprise
                                                                                                            Introduction




                                        Introduction
                                        This part of the documentation contains editorial notes.


                                        Revision Overview
                                        Section           Software    Description
                                        Version/Date      version

                                        2.00/ 04-2022     6           Update of software reference.

                                        1.03 / 01-2017    5.2.4       Product and company names adjusted.

                                        1.02 / 02-2014    5.2.4       Product names adjusted

                                        1.01 / 01-2013    5.2.4       Layout adapted to CI 2013

                                        1.00 / 11-2012    5.2.4       Original version



                                        Editorial
                                        The editorial provides information on the following topics:
                                        •   Notes on this Document
                                        •   Copyrights
                                        •   Trademarks
                                        •   Contacts

                                        Notes on this Document
                                        This document is intended for end users of A+W Enterprise.
                                        The documentation and software described are licenses that must be used or
                                        copied only in accordance with the conditions of our license agreement. The
                                        contents of the documentation are only informative and are subject to changes
                                        without prior notice.The documentation and software described are licenses
                                        that must be used or copied only in accordance with the conditions of our li-
                                        cense agreement. The contents of the documentation are only informative and
                                        are subject to changes without prior notice.
                                        The text and illustrations were compiled with the utmost care. Still, errors can-
                                        not be totally excluded. A+W Software GmbH cannot be held liable for errors
                                        or inaccuracies, unless they can be attributed to wilful or grossly negligent ac-
                                        tion.
                                        The descriptions in this document are based on the full program level of A+W
                                        Enterprise.

                                        Copyrights
2.00 / 04-2022




                                        © 2022, A+W Software GmbH, all rights reserved, also those for reprinting, the
                                        making of copies and translation.



                 A+W Enterprise Despatch Control                                                                   G-3
                 Introduction




                                The documentation may be copied, completely or in part, saved in an archiving
                                system, or transferred in any other form only in accordance with our license
                                agreement. Transmission of the documentation is not allowed, neither elec-
                                tronically, nor mechanically, nor by recording or in any other way, without A+W
                                Software GmbH's prior approval in writing.

                                Trademarks
                                All hardware and software names mentioned in this documentation can also
                                be registered trademarks or other property rights of third parties. Third-party
                                copyrights must therefore be observed.

                                Contacts
                                A+W Software GmbH
                                Am Pfahlgraben 4-10
                                35415 Pohlheim
                                +49 6404 2051-0
                                +49 6404 2051 877
                                Zentrale@a-w.com
                                http://www.a-w.com
2.00 / 04-2022




                 G-4                                                        A+W Enterprise Despatch Control
                                                                                                                                                        Contents




                                        Contents
                                        Introduction ............................................................................................................ G-3
                                          Revision Overview .............................................................................................. G-3
                                          Editorial .............................................................................................................. G-3

                                        Software Reference                                                                                                   G-7
                                        Overview ................................................................................................................ G-9
                                        Start functions ...................................................................................................... G-10
                                           Program start .................................................................................................... G-11
                                           Find Order ........................................................................................................ G-13
                                           Find Market Partner .......................................................................................... G-14
                                        Dispatch Explorer ................................................................................................ G-15
                                           Explorer – Tree structure .................................................................................. G-16
                                              Overview of the delivery date level ............................................................... G-17
                                              Overview for the tour level ............................................................................ G-19
                                              Overview of the order level ........................................................................... G-20
                                              Overview of the item level ............................................................................. G-21
                                        Dispatch Control – menus ................................................................................... G-22
                                           Supplementary menu ....................................................................................... G-22
                                           Info Menu ......................................................................................................... G-25
                                           Buttons ............................................................................................................. G-27
                                        Tours .................................................................................................................... G-28
                                           RouteInfo tab .................................................................................................... G-29
                                           RackInfo tab ..................................................................................................... G-32
                                           VehicleInfo tab .................................................................................................. G-34
                                           Optimization tab ............................................................................................... G-36
                                        Order Level .......................................................................................................... G-38
                                           Order Info tab ................................................................................................... G-39
                                           OrderInfo/Rack tab ........................................................................................... G-43
                                           Delivery Address tab ........................................................................................ G-45
                                           Dispatch Info I tab ............................................................................................ G-47
                                           Dispatch Info II tab ........................................................................................... G-49
                                           Add. Info tab ..................................................................................................... G-51
                                        Item Level ............................................................................................................ G-54
                                           Item Info I tab ................................................................................................... G-55
                                           Item Info II tab .................................................................................................. G-58
                                        Functions in Dispatch .......................................................................................... G-60
                                           Search .............................................................................................................. G-61
                                           Go to ................................................................................................................. G-62
                                           Postpone .......................................................................................................... G-64
                                           Postponement of several items - selection ....................................................... G-66
                                           Postponement of several items - action ........................................................... G-67
                                           Order Info ......................................................................................................... G-69
                                              Information on the Order ............................................................................... G-70
                                           Book goods received for ................................................................................... G-73
                                           Cancel receipt of goods .................................................................................... G-74
                                           Missing quantity check for ................................................................................ G-75
                                           Missing quantity check - actions ....................................................................... G-76
                                           Book to transport ............................................................................................. G-78
                                           Cancel transport booking ................................................................................. G-79
                                           Rack View for Order ......................................................................................... G-80
2.00 / 04-2022




                                           Results of the rack scheduling ......................................................................... G-81
                                           Packaging Planning .......................................................................................... G-82
                                           Find delivery address ....................................................................................... G-83
                                           New delivery address ....................................................................................... G-84


                 A+W Enterprise Despatch Control                                                                                                             G-5
                 Contents




                              Rack information .............................................................................................. G-85
                              Set/remove tour lock ........................................................................................ G-86
                              Lock all tours .................................................................................................... G-87
                              Transport data .................................................................................................. G-88
                              Stock Reference ............................................................................................... G-89
                            Cancel .................................................................................................................. G-90
                              Cancel delivery note ......................................................................................... G-90
                              Cancel order ..................................................................................................... G-91
                              Cancel receipt of goods .................................................................................... G-92
                              Cancel shipping status ..................................................................................... G-93
                            Racks ................................................................................................................... G-94
                              Rack allocation -selection ................................................................................. G-95
                              Rack allocation - view ....................................................................................... G-96
                              Resolve rack - selection ................................................................................... G-98
                              Resolve rack - view .......................................................................................... G-98
                              Free racks (overview) ..................................................................................... G-100
                              Booked racks (overview) ................................................................................ G-102
                              All racks (overview) ........................................................................................ G-103
                              Individual racks ............................................................................................... G-105
                              Racks for order ............................................................................................... G-106
                              Lite allocation ................................................................................................. G-108
                              SA/PU information .......................................................................................... G-111
                              SA/PU info (global) ......................................................................................... G-113
                              Dispatch Control – Overview .......................................................................... G-115
                              Delivery Date Change List .............................................................................. G-118
                              Dispatch Information ...................................................................................... G-119
                              Via Details ...................................................................................................... G-120
                              Finished goods stock ...................................................................................... G-121
                                 Finished goods stock .................................................................................. G-122
                                 Finished goods stock - overview ................................................................. G-123
                                 Finished goods stock - inventory ................................................................ G-124
                                 Close inventory ........................................................................................... G-124
                                 Log .............................................................................................................. G-125
                              Graphical Tour Overview ................................................................................ G-127
                            Print ................................................................................................................... G-128
                              Print loading list .............................................................................................. G-129
                              Print all loading lists ........................................................................................ G-130
                              Print supplementary loading lists .................................................................... G-131
                              Print list ........................................................................................................... G-132
                              Preliminary delivery note printing ................................................................... G-133
                              Deliv./receipt release + print ........................................................................... G-135
                              Print format ..................................................................................................... G-136
                              Printer selection .............................................................................................. G-136

                            Partindex                                                                                                      G-137
                            Index .................................................................................................................. G-139
2.00 / 04-2022




                 G-6                                                                             A+W Enterprise Despatch Control
Dispatch Control                 G

                   Software Reference




                   A+W Enterprise
                 Software Reference                                                                            Overview




                                        Overview
                                        All Dispatch Control views, dialogs, and functions are accessible via the Logis-
                                        tics module. You can also start the module directly from FixWin. In the default
                                        configuration, you start directly with the Dispatch Explorer:
                                         "Dispatch Explorer" on page G15
                                        With Dispatch Control, you find, plan, process, and send your delivery orders
                                        on time. Dispatch Control is the control center for dispatch and provides quick
                                        and easy access to all delivery orders. For example, you create a list of all de-
                                        livery dates for a period or jump directly into the delivery order you're looking
                                        for. For the overview of the dispatch documents, each delivery order is divided
                                        into the following four levels:
                                        •   Delivery dates
                                        •   Tours and routes
                                        •   Orders
                                        •   Items
                                        The first level shows the delivery dates. A delivery date includes the corre-
                                        sponding routes or tours.
                                        The second level shows the routes and tours. A tour includes the correspond-
                                        ing orders and can consist of one or more routes. A tour represents at least
                                        one route on a certain delivery date. The route is a defined route to be traveled.
                                        Routes can be assigned to certain weekdays or certain times. The tour level
                                        offers an overview of existing dispatch documents.
                                        The orders are shown on the third level. An order consists of the appropriate
                                        items and shipping address. The order level offers an overview of existing dis-
                                        patch documents.
                                        Items are shown on the fourth level. An item includes the appropriate units.
                                        Open tours, orders or items are locked for processing by other employees.
                                        They are then only opened with read rights.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                   G-9
                 Start functions                                                             Software Reference




                                   Start functions
                                   A+W Enterprise offers various functions for searching for delivery dates and
                                   orders.
                                   The following information is available on this subject:
                                    "Program start" on page G11
                                    "Find Order" on page G13
                                    "Find Market Partner" on page G14
2.00 / 2022-04




                 G - 10                                                         A+W Enterprise Dispatch Control
                 Software Reference                                                                         Start functions




                                          Program start
                                          Logistics > Dispatch Control




                 Fig. G 1   Search Mode


                                          You start Dispatch Control with the entry of the following criteria:
                                          •   Dispatch mode (all, SA outgoing, PU outgoing and incoming goods)
                                          •   Site number or client number
                                          •   Delivery date
                                          •   Delivery period
                                          The fields in the header are used to filter your search; the system will list the
                                          delivery dates for the defined data.

                                          SA Deliv. Dispatch mode. By default, only the orders to be delivered are han-
                                          dled in the Dispatch Control. With appropriate configuration, however, the
                                          POs, complete or only with ordered processings, can be processed in the Dis-
                                          patch module. Contact an A+W employee if you need more information about
                                          this. If the sales and purchase documents are handled via dispatch, all orders
                                          for the selected date or for the selected time period can be displayed, as, e.g.,
                                          in the Dispatch Explorer, or on a data level.
                                          Technical info: Toggle field, DB field: lapool.vmodus
2.00 / 2022-04




                                          Site Site number or client number.
                                          Technical info: numeric field, DB field: lapool.hausnr




                 A+W Enterprise Dispatch Control                                                                    G - 11
                 Start functions                                                                Software Reference




                                   Deliv. Date Input field for the delivery date on a certain day.
                                   Technical info: date field, DB field: lapool.ltplan

                                   to Input field for the delivery date in a certain period.
                                   Technical info: date field, DB field: lapool.ltplan

                                      Delivery date
                                      The entry of the period is only possible if you are working with the Dispatch
                                      Explorer. Alternatively, only a Delivery date field is active. If you enter the
                                      same date in both date fields, the Dispatch Control starts directly with the
                                      route level.
2.00 / 2022-04




                 G - 12                                                          A+W Enterprise Dispatch Control
                 Software Reference                                                                        Start functions




                                         Find Order
                                         Dispatch Control > [Search] > <F9>




                 Fig. G 2   Find Order


                                         In Dispatch Control, it is possible to search in many places for orders using the
                                         extended search. You enter the criteria for the search in the input fields. The
                                         lower area displays the hit list. The search results are summarized on various
                                         tabs.
                                         The search for particular types of documents was designed uniformly across
                                         A+W Enterprise with Version 6.
                                         For details, please consult the Sales section:
                                          Sales, “Find Orders” on page D-25
                                          Sales, “Find Orders – Hit List” on page D-31
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                   G - 13
                 Start functions                                                                     Software Reference




                                           Find Market Partner
                                           Dispatch Control > [Search] > <F9> > Customer Field > <F9>




                 Fig. G 3     Find Market Partner search dialog


                                           For details of the market partner search, please consult the Sales section:
                                            Sales, “Find Market Partner” on page D-41
2.00 / 2022-04




                 G - 14                                                                  A+W Enterprise Dispatch Control
                 Software Reference                                                                        Dispatch Explorer




                                            Dispatch Explorer
                                            Logistics > Dispatch Control > Defining a Period


                 A


                 B


                                                                                                                         E




                 C
                 D




                 A Header data: Entry of search      B Explorer – Tree structure          C Detailed information about the
                   criteria                                                                 selected delivery date
                 D Detailed information about the    E Selected date level
                   selected route
                 Fig. G 4     Dispatch Control – Explorer view


                                            Dispatch control lists the orders found - based on the search criteria - by de-
                                            livery date.

                                            SA Deliv. SA Deliv.: selected dispatch mode.
                                            Technical info: Toggle field, DB field: lapool.vmodus

                                            Site Site number or client number.
                                            Technical info: numeric field, DB field: lapool.hausnr

                                            Deliv. Date Input field for the delivery date on a certain day.
                                            Technical info: date field, DB field: lapool.ltplan

                                            to Input field for the delivery date in a certain period.
                                            Technical info: date field, DB field: lapool.ltplan
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                      G - 15
                 Dispatch Explorer                                                                Software Reference




                                     Explorer – Tree structure
                                     For clarity's sake, orders are listed in the Explorer structure. Work with the Dis-
                                     patch Explorer must be configured appropriately. The dispatch data is dis-
                                     played on several levels in the Explorer:
                                     •   Date level
                                     •   Route level
                                     •   Document level
                                     •   Item level
                                     Each level is marked by a certain icon. A brief overview of the existing deliver-
                                     ies is displayed in the right half of the dialog.
                                     Select a level from the tree structure. When a level has been selected, the lev-
                                     el field is highlighted in blue.
                                     The following four levels provide short bits of information:
                                      "Overview of the delivery date level" on page G17
                                      "Overview for the tour level" on page G19
                                      "Overview of the order level" on page G20
                                      "Overview of the item level" on page G21
2.00 / 2022-04




                 G - 16                                                            A+W Enterprise Dispatch Control
                 Software Reference                                                                      Dispatch Explorer




                                          Overview of the delivery date level
                                          Logistics > Dispatch Control > Enter a period or date in the Explorer




                 Fig. G 5   Date level in the Dispatch Explorer


                                          After the delivery date selection in the Explorer, the following fields are dis-
                                          played in the overview:

                                          Route Route number.
                                          Technical info: numeric field, DB field: lapool.routenr

                                          Site Site number or client number.
                                          Technical info: numeric field, DB field: lapool.hausnr

                                          Type Dispatch mode: Due to the limited space, the name of the field (Dispatch
                                          mode=type) and the display of the dispatch mode are abbreviated:
                                          • SA: SA withdrawal
                                          • E1: PU receipt of goods
                                          • E2: PU issue of goods
                                          Technical info: alphanumeric field, DB field: lapool.vmodus

                                          Name Route description from the A+W Enterprise master data.
                                          Technical info: Display field, DB field: route.routenname
2.00 / 2022-04




                                          Tot. Total number of items entered for this tour.
                                          Technical info: numeric field, DB field: lapool.gesstk


                 A+W Enterprise Dispatch Control                                                                     G - 17
                 Dispatch Explorer                                                             Software Reference




                                     Call Number of items the customer has ordered for that date.
                                     Technical info: numeric field, DB field: lapool.abrufstk

                                     Call Available quantity for this item.
                                     Technical info: numeric field, DB field: lapool.sollstk

                                     Packed Quantity packed for this item.
                                     Technical info: numeric field, DB field: lapool.iststk

                                     Compl. Route reported completed. All orders have been packed.
                                      All items are ready for delivery.
                                      Not all of the items are ready to be delivered.
                                     Technical info: display field
2.00 / 2022-04




                 G - 18                                                            A+W Enterprise Dispatch Control
                 Software Reference                                                                     Dispatch Explorer




                                          Overview for the tour level
                                          Logistics > Dispatch Control > Enter a period or date in the Explorer




                 Fig. G 6   Tour level in the Dispatch Explorer


                                          After the route selection in the Explorer, the following fields are displayed in
                                          the overview:

                                          Order Order or PO number for the scheduled delivery depending on dispatch
                                          mode. There is always a distinction according to the document type: 5=order,
                                          2=PO
                                          Technical info: Numeric field, DB field: lapool.auftrnr, lapool.vorgang

                                          Customer Customer name for orders or supplier name for POs for the sched-
                                          uled delivery.
                                          Technical info: Alphanumeric field, DB field: mp.name
                                          The following fields are adopted from the previous overview:
                                          •   Total
                                          •   Call
                                          •   Avail. (available)
                                          •   Packed
                                          •   Compl. (completed)
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                    G - 19
                 Dispatch Explorer                                                                    Software Reference




                                           Overview of the order level
                                           Logistics > Dispatch Control > Enter a period or date in the Explorer




                 Fig. G 7    Order level in the Dispatch Explorer


                                           After the order/PO selection in the Explorer, the following fields are displayed
                                           in the overview:

                                           Itm Sequential item number from the order or PO.
                                           Technical info: Numeric field, DB field: lapool.posnr

                                           Article Description of the article to be delivered.
                                           Technical info: numeric field, DB field: artikel.artbez1
                                           The following fields are adopted from the previous overview:
                                           •   Total
                                           •   Call
                                           •   Avail. (available)
                                           •   Packed
                                           •   Compl. (completed)
2.00 / 2022-04




                 G - 20                                                                  A+W Enterprise Dispatch Control
                 Software Reference                                                                     Dispatch Explorer




                                          Overview of the item level
                                          Logistics > Dispatch Control > Enter a period or date in the Explorer




                 Fig. G 8   Item level in the Dispatch Explorer


                                          The overview from the item level lists all order items or items from the purchas-
                                          ing document with the respective fields, as on the order level.
                                          The fields are described in the following section:
                                           "Overview of the delivery date level" on page G17
                                           "Overview of the order level" on page G20
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                   G - 21
                 Dispatch Control – menus                                                           Software Reference




                                         Dispatch Control – menus
                                         In the Dispatch Control, there are additional functions available. These are
                                         summarized on all available levels under supplementary and info menus. A
                                         detailed overview of both menus is provided in the following sections.
                                          "Supplementary menu" on page G22
                                          "Info Menu" on page G25



                                         Supplementary menu
                                         Dispatch Control – overview levels > <F4>




                 Fig. G 9   Supplementary menu on the tour level


                                         On all levels of the Dispatch Control, you have additional functions that can be
                                         accessed via the supplementary menu <F4>. Depending on the configuration,
                                         context, and data stock, the functions listed here may not be available or only
                                         available to a limited extent.
                                          "Supplementary menu on tour level" on page G23
                                          "Supplementary menu on order level" on page G24
                                          "Supplementary menu on item level" on page G24
2.00 / 2022-04




                 G - 22                                                               A+W Enterprise Dispatch Control
                 Software Reference                                                                Dispatch Control – menus




                                            Supplementary menu on tour level

                 Shortcut   Entry                                  Description

                     a      Postpone <F3>                           "Postpone" on page G64

                     b      Go to <F5>                              "Go to" on page G62

                     c      Postpone several items <Ctrl> + <E>  "Postponement of several items - selection" on page G66

                     d      Order info <Ctrl> + <K>                 "Order Info" on page G69

                     e      Print a cargo list <Ctrl> + <F8>        "Print loading list" on page G129

                     f      Print all cargo lists <Ctrl> + <F12>    "Print all loading lists" on page G130

                     g      Printing a supplementary cargo list     "Print supplementary loading lists" on page G131
                            <Ctrl> + <F10>

                     h      List printing                           "Print list" on page G132

                     i      Book receipt of goods                   "Book goods received for" on page G73

                     j      Cancel receipt of goods                 "Cancel receipt of goods" on page G74

                     k      Missing quantity check <Shift> + <F9>  "Missing quantity check for" on page G75

                     l      Preliminary delivery note printing      "Print loading list" on page G129
                            <Ctrl> + <F11>

                     m      Book to transport                       "Book to transport" on page G78

                     n      Cancel transport booking                "Cancel transport booking" on page G79

                     o      Delivery/receipt release + print <Ctrl>  "Deliv./receipt release + print" on page G135
                            + <F9>
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                        G - 23
                 Dispatch Control – menus                                                              Software Reference




                                          Supplementary menu on order level
                                          In addition to some functions that are also available on the tour level, the fol-
                                          lowing menu entries are available on the order level:


                 Shortcut   Entry                                Description

                     i      Barcode rack view                     "Rack View for Order" on page G80

                     j      Results of the rack scheduling <Shift>  "Results of the rack scheduling" on page G81
                            + <F12>

                     k      Rack Scheduling                       "Packaging Planning" on page G82

                     oa     Find Delivery Address                 "Find delivery address" on page G83

                    ob      New Delivery Address                  "New delivery address" on page G84

                     t      Rack Information                      "Rack information" on page G85


                                          Supplementary menu on item level
                                          In addition to some functions that are also available on the route and order lev-
                                          el, the following menu entries are available on the item level:


                 Shortcut   Entry                                Description

                     j      Correct Packed Quantity <Shift> +    You can use <F4> > Correct packed quantity to change the
                            <F10>                                entry in this field.

                     p      Overview                              "Dispatch Control – Overview" on page G115

                     n      Change Delivery Date                  "Delivery Date Change List" on page G118
2.00 / 2022-04




                 G - 24                                                                  A+W Enterprise Dispatch Control
                 Software Reference                                                             Dispatch Control – menus




                                            Info Menu
                                            Dispatch Control – Overview Levels > <Shift> + <F4>




                 Fig. G 10   Info menu on order level


                                            The info menu <Shift> + <F4> is the same for all levels. You can use this menu
                                            to open other dialogs and start functions. The following entries are displayed:


                 Shortcut    Entry                                     Description

                      a      Lock/Unlock Tour <Shift> + <F10>           "Set/remove tour lock" on page G86

                      b      Lock all Tours <Shift> + <F12>             "Lock all tours" on page G87

                      c      Transport Data                             "Transport data" on page G88

                      d      Stock Reference                            "Stock Reference" on page G89

                      e      Cancel                                    Open the submenu
                                                                        "Cancel" on page G90

                     ea      Cancel Delivery Note                       "Cancel delivery note" on page G90

                     eb      Cancel Order                               "Cancel order" on page G91

                     ec      Cancel Receipt of Goods                    "Cancel receipt of goods" on page G92
2.00 / 2022-04




                     ed      Cancel Dispatch Status                     "Cancel shipping status" on page G93




                 A+W Enterprise Dispatch Control                                                                   G - 25
                 Dispatch Control – menus                                                        Software Reference




                 Shortcut   Entry                                 Description

                      f     Racks                                 Open the submenu
                                                                   "Racks" on page G94

                     fa     Rack Allocation <Ctrl> + <G>           "Rack allocation -selection" on page G95

                     fb     Resolve Rack <Ctrl> + <F>              "Resolve rack - selection" on page G98

                     fc     Free Racks (Overview) <Ctrl> + <L>     "Free racks (overview)" on page G100

                     fd     Booked Racks (Overview) <Alt> + <E>    "Booked racks (overview)" on page G102

                     fe     All Racks (Overview) <Alt> + <G>       "All racks (overview)" on page G103

                     ff     Individual Racks <Alt> + <B>           "Individual racks" on page G105

                     fg     Racks for Order <Alt> + <A>            "Resolve rack - selection" on page G98

                     fh     Lite Allocation <Alt> + <F>            "Lite allocation" on page G108

                     g      SA/PU Information <Ctrl> + <O>         "SA/PU information" on page G111

                     h      SA/PU Info (Global)                    "SA/PU info (global)" on page G113

                      i     Overview                               "Dispatch Control – Overview" on page G115

                      j     Delivery Date Changes                  "Delivery Date Change List" on page G118

                     k      Dispatch Information <Alt> + <I>       "Dispatch Information" on page G119

                      l     Via Details                            "Via Details" on page G120

                     m      Finished Goods Stock                   "Finished goods stock" on page G121

                    ma      Finished Goods Stock                   "Finished goods stock" on page G122

                    mb      Finished Goods Stock - Inventory       "Finished goods stock - inventory" on page G124

                    mc      Close Inventory                        "Close inventory" on page G124

                     d      Log                                    "Log" on page G125
2.00 / 2022-04




                 G - 26                                                            A+W Enterprise Dispatch Control
                 Software Reference                                                                      Dispatch Control – menus




                                                Buttons
                                                On the data levels of the Dispatch Control, you can use the following buttons:


                 Button                 Entry                                   Description

                      [Search]]         Starts the document search               "Search" on page G61

                     [Overview]         Graphic overview of the deliveries       "Graphical Tour Overview" on page G127

                       [Go to]          Go to a particular document              "Go to" on page G62

                     [Postpone]         Starts the Postpone dialog               "Postpone" on page G64

                      [Trigger]         Triggers the selected action            With this button, or alternatively with the <F3>
                                                                                button, you can start the selected action.

                      [Details]         Starts the route overview                "RouteInfo tab" on page G29

                      [Routes]          Changes from the lower levels to the     "RouteInfo tab" on page G29
                                        tour level

                      [Orders]          Changes from the lower or higher         "Order Info tab" on page G39
                                        levels to the order level

                       [Items]          Changes from the higher levels to the    "Item Info I tab" on page G55
                                        item level

                     [Explorer]         Changes from the data levels in the      "Dispatch Explorer" on page G15
                                        Explorer

                       [End]            Ends the overview display               It is possible to enter another date. The next [End]
                                                                                closes the Dispatch Control.

                 Tab. G-1        Overview of the buttons in the Dispatch Control
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                               G - 27
                 Tours                                                                Software Reference




                          Tours
                          On the tour level, all routes are listed that are driven on the selected delivery
                          date. The orders or POs with additional details and tour status are listed for
                          each route.
                          The search fields in the header are explained in the following section:
                           "Dispatch Explorer" on page G15

                             Technical info in dispatch
                             Some important data is stored in the database table lapool. This data exists
                             per order or PO item, route and delivery date. Various displays on the dia-
                             logs are formed dynamically or calculated at program runtime. Therefore,
                             the details about the technical information are generally not possible 1:1. In
                             such cases, the Technical Info entry is omitted in this document.The field
                             contents that are determined program-internally (via SQL statement) are
                             not listed in this document. If necessary, please consult the database doc-
                             umentation.

                          The tour level consists of the following tabs:
                           "RouteInfo tab" on page G29
                           "RackInfo tab" on page G32
                           "VehicleInfo tab" on page G34
                           "Optimization tab" on page G36
2.00 / 2022-04




                 G - 28                                                A+W Enterprise Dispatch Control
                 Software Reference                                                                                             Tours




                                               RouteInfo tab
                                               Dispatch Control – Delivery date entry
                                               Dispatch control – Delivery date level > [Details] > RouteInfo tab




                 Fig. G 11    Dispatch Control – RouteInfo tab


                                               On the RouteInfo tab, general data about the routes is summarized.

                                               S Current route status. For the meaning of the individual icons, please consult
                                               the following table.
                                               Technical info: Display field


                 S (Status)        Meaning                   Information

                    white          Open                      Not all of the items for this route have been completely packed.

                    green/yellow   Available                 Items with available quantity are present for this route.

                     yellow        Packed                    All of the items for this route have been completely packed.

                     blue/yellow   En route                  All items scheduled for this route are on their way.

                     blue          Delivery note created     All items of this route have been completely delivery to the customer.

                     red           locked                    This route has been locked. The route lock is set only if one order of
2.00 / 2022-04




                                                             the route is booked by another site or client as being en route.
                                                              "Set/remove tour lock" on page G86

                 Tab. G-2     Route status


                 A+W Enterprise Dispatch Control                                                                            G - 29
                 Tours                                                                   Software Reference




                          No. Route number.
                          Technical info: numeric field, DB field: lapooltou.routenr

                          Route Route description from the A+W Enterprise master data.
                          Technical info: Display field, DB field: route.routenname

                          Total Total number of items entered for this route.
                          Technical info: display field, DB field: lapooltou.gesstk

                          Call Number of items the customer has ordered for that date.
                          Technical info: display field, DB field: lapooltou.abrufstk

                          Packed Quantity packed for this item. Use <F4> to check for missing quanti-
                          ties.
                          Technical info: display field, DB field: lapooltou.iststk
                          The packed quantity can be changed on the following dialogs:
                           "Missing quantity check for" on page G75
                           "Rack View for Order" on page G80

                          Back. Backlog. Item quantity that is not available for the desired tour.
                          If a tour is moved because of Backlog, this quantity will be adopted.
                          Technical info: display field, DB field: lapooltou.rueckstk
                           "Functions in Dispatch" on page G60

                          kg/N Net weight in kilogram for this route. The net weight is the total weight
                          of the item, without rack or packaging. The weight is calculated in the program
                          at runtime and displayed rounded on this tab.
                          Technical info: Display field, DB field: lapooltou.gewicht

                          sqft Item surface in square feet.
                          Technical info: display field, DB field: lapooltou.qm

                          LL Number of the loading list if a loading list has been printed for this route.
                          Use <F4> to print the loading lists.
                          Technical info: display field, DB field: lapooltou.llnr
                           "Print loading list" on page G129
                           "Print all loading lists" on page G130

                          cmpl. Complete code:
                           All items are packed for delivery.
                           Not all of the items are packed for delivery.
                          Technical info: Display field, DB field: lapooltou.liefkompl

                          PrDn The preliminary delivery note shows whether all preliminary delivery
                          notes have been printed for this tour.
                           All preliminary delivery notes have been printed.
                           Not all of the preliminary delivery notes have been printed.
                          Press <F4> to print a preliminary delivery note.
2.00 / 2022-04




                          Technical info: display field, DB field: lapooltou.vlsdrukz
                           "Print loading list" on page G129




                 G - 30                                                A+W Enterprise Dispatch Control
                 Software Reference                                                                              Tours




                                        DN The delivery note code indicates whether all delivery notes for the deliv-
                                        eries on this tour are printed.
                                         At least one delivery note has been printed.
                                         No delivery notes have been printed.
                                        Press <F4> to print the delivery note.
                                        Technical info: display field, DB field: lapooltou.lsdrukz
                                         "Rack information" on page G85

                                        I Dispatch information code indicates whether there is dispatch information for
                                        at least one order on this tour.
                                         There is at least one order with dispatch info.
                                         No dispatch info is available.
                                        The dispatch information can be stored in the documents during entry.
                                        Technical info: Display field, DB field: lapooltou.vlsdrukz
                                         Sales, “External Information” on page D-262

                                        TL The tour lock code indicates whether the current tour is locked or booked:
                                        • gray- The current tour is still en route
                                        • yellow- The current tour is booked
                                        • red- The current tour is locked
                                        You can use <F4> to lock or book the tour.
                                        Technical info: Display field
                                         "Rack information" on page G85
                                         "Lock all tours" on page G87


                                        Additional information
                                         "Supplementary menu" on page G22
                                         "Info Menu" on page G25
                                         "Buttons" on page G27
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                G - 31
                 Tours                                                                                  Software Reference




                                           RackInfo tab
                                           Dispatch Control – Delivery date entry
                                           Dispatch control – Delivery date level > [Details] > RackInfo tab




                 Fig. G 12   Dispatch Control – tour level – RackInfo tab


                                           On the RackInfo tab, general data about the routes is summarized and addi-
                                           tional rack information is displayed. The display of this tab is dynamic; that is,
                                           it is only shown if the work with racks is configured in Dispatch Control.
                                           Most fields have already been described in the previous section:
                                            "RouteInfo tab" on page G29
                                           In addition, the following fields are displayed on the RackInfo tab:

                                           On Rack Rack number on which the lites to be delivered are located. For the
                                           configuration of the free racks in the Dispatch Control, you must contact an
                                           A+W employee.
                                           Technical info: Display field, DB field: lapooltou.freigeststk

                                           kg/N Net weight in kilogram for this route. The weight is calculated in the pro-
                                           gram at runtime and displayed to three decimal places on this tab.
                                           Technical info: Display field, DB field: lapooltou.gewicht
2.00 / 2022-04




                                           kg/Tara Empty weight of the rack (tarage weight), in kilograms. The tarage
                                           weight is displayed in this field if it is stored appropriately in the master data



                 G - 32                                                                  A+W Enterprise Dispatch Control
                 Software Reference                                                                                Tours




                                        and the goods delivered are already scheduled on the racks.
                                        Technical info: Display field, DB field: lapooltou.gewichttara

                                        kg/G Gross weight in kilograms for this route. The weight is calculated in the
                                        program at runtime and displayed to three decimal places on this tab. The
                                        gross weight is calculated from the net weight and tarage weight together. The
                                        gross weight is displayed in this field if the goods delivered are already sched-
                                        uled on the racks.
                                        Technical info: Display field, DB field: lapooltou.gewichtbrutto


                                        Additional information
                                         "Supplementary menu" on page G22
                                         "Info Menu" on page G25
                                         "Buttons" on page G27
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                 G - 33
                 Tours                                                                                 Software Reference




                                           VehicleInfo tab
                                           Dispatch Control – Delivery date entry
                                           Dispatch Control – Delivery Date Level > [Details] > VehicleInfo tab




                 Fig. G 13   Dispatch control – VehicleInfo tab


                                           The VehicleInfo tab shows the drivers and vehicle data in addition to the tours.
                                           Most fields have already been described in the previous section:
                                            "RouteInfo tab" on page G29
                                           In addition, the following fields are displayed on the VehicleInfo tab:

                                           Driver Personnel number of the driver from the employee master data. The
                                           driver for this route can be selected on the TransportData dialog.
                                           Technical info: Numeric field, DB field: mitarb.manr
                                            "Transport data" on page G88

                                           Name Driver's name. If the driver for this route is selected on the Transport-
                                           Data dialog, the name is taken over here directly from the employee master
                                           data.
                                           Technical info: Display field, mitarb.maname

                                           Vehicle License plate of the truck. The vehicle for this route is selected on the
2.00 / 2022-04




                                           TransportData dialog. The vehicles must first be stored in the master data.
                                           Technical info: Numeric field, DB field: lkw.lkw.nr
                                            Master Data, “Vehicles” on page B-172


                 G - 34                                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                                   Tours




                                        Trailer I/II License plate of the trailer used. It is possible to select two trailers
                                        on the TransportData dialog. The trailer must first be stored in the master data.
                                        Technical info: Numeric field, DB field: lkw.lkw.nr
                                         Master Data, “Vehicles” on page B-172


                                        Additional information
                                         "Supplementary menu" on page G22
                                         "Info Menu" on page G25
                                         "Buttons" on page G27
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                     G - 35
                 Tours                                                                                  Software Reference




                                           Optimization tab
                                           Dispatch Control – Delivery date entry
                                           Dispatch control – Delivery date level > [Details] > Optimization tab




                 Fig. G 14   Dispatch Control – tour level – Optimization tab


                                           General data about the routes is summarized and additional information about
                                           the route optimization is displayed on the Optimization tab. The display of this
                                           tab is dynamic; that is, it is only shown if work with the A+W Logistics Optimizer
                                           is configured in Dispatch Control.
                                           Most fields have already been described in the previous sections:
                                            "RouteInfo tab" on page G29
                                            "RackInfo tab" on page G32
                                            "VehicleInfo tab" on page G34
                                           In addition, the following fields are displayed on the Optimization tab:

                                           Opti status Current status of the route optimization in plain text.
                                           Technical info: Display field, DB field: lapooltou.optistatus

                                           Opt. Checkbox for route selection for the upcoming optimization.
                                            Current route is selected for the optimization.
2.00 / 2022-04




                                            The current route is not selected for the optimization.
                                           Start the route optimization with the [StartOTR] button.
                                           Technical info: Display field, DB field: lapooltou.optkz



                 G - 36                                                                  A+W Enterprise Dispatch Control
                 Software Reference                                                                            Tours




                                           Route optimization in A+W Enterprise
                                           Route optimization with the A+W Logistics Optimizer is a separately avail-
                                           able and configurable extension for A+W Enterprise. Please contact the re-
                                           sponsible A+W employee for more information.
                                           The documentation for the A+W Logistics Optimizer is not part of this doc-
                                           ument.


                                        Additional information
                                         "Supplementary menu" on page G22
                                         "Info Menu" on page G25
                                         "Buttons" on page G27
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                              G - 37
                 Order Level                                                             Software Reference




                               Order Level
                               On the order level, Dispatch Control provides detailed information on the en-
                               tered orders such as delivery address, dispatch information, and additional in-
                               formation.
                               This level offers the following tabs:
                                "Order Info tab" on page G39
                                "OrderInfo/Rack tab" on page G43
                                "Delivery Address tab" on page G45
                                "Dispatch Info I tab" on page G47
                                "Dispatch Info II tab" on page G49
                                "Add. Info tab" on page G51
2.00 / 2022-04




                 G - 38                                                    A+W Enterprise Dispatch Control
                 Software Reference                                                                          Order Level




                                           Order Info tab
                                           Dispatch control – Delivery date selection > Route selection > Order info tab




                 Fig. G 15   Dispatch control – Order info tab


                                           The Order info tab shows information about the orders and the dispatch status
                                           for every tour.
                                           The search fields in the header are explained in connection with the Dispatch
                                           Control dialog. The route number and name are shown as well.
                                            "Dispatch Explorer" on page G15

                                           S Current order status. The meaning of the traffic light display on the order
                                           level is the same as on the tour level. Here's an explanation:
                                            "Route status" on page G29

                                           Mode Dispatch mode. The field is only displayed if you are using the Dispatch
                                           Control for the purchasing documents and have made the appropriate selec-
                                           tion.
                                           Technical info: Display field, DB field: lapoolauf.vmodus

                                           Order Order or PO number. All documents are listed here that are scheduled
                                           for the route on the selected date. Whether an order or PO number is dis-
                                           played in this field depends on the dispatch mode selected.
2.00 / 2022-04




                                           Technical info: Numeric field, DB field: lapoolauf.auftrnr




                 A+W Enterprise Dispatch Control                                                                  G - 39
                 Order Level                                                                Software Reference




                               No. Delivery note sub-number. If a complete delivery note or several partial
                               delivery notes were already entered, the appropriate number is displayed
                               here.
                               • A complete delivery note always has the sub-number 1 and is also marked
                                   as complete (Cmp checkbox).
                               • Partial delivery notes always have sub-numbers larger than 1 and are not
                                   marked as complete (Cmp checkbox).
                               If an order is transferred from another site, this field shows the original order
                               number assigned by the sender.
                               Technical info: numeric field, DB field: lapoolauf.subnr

                               Customer Customer or supplier name from the order or the PO.
                               Technical info: Alphanumeric field, DB field: mp.name

                               Total Total number of pieces in the order or in the PO.
                               Technical info: Numeric field, DB field: lapoolauf.gesstk

                               Call Number of items the customer or supplier has requested for that date.
                               Technical info: Numeric field, DB field: lapoolauf.abrufstk

                               Avail. Number of items available for packing.
                               Technical info: numeric field, DB field: lapoolauf.sollstk

                               Packed Quantity packed for this item. Use <F4> to check for missing quanti-
                               ties.
                               Technical info: numeric field, DB field: lapoolauf.iststk
                                "Missing quantity check for" on page G75

                               Back. Backlog. Item quantity which is not available for the desired tour.
                               If a tour is moved because of Backlog, this quantity will be adopted.
                               Technical info: numeric field, DB field: lapoolauf.rueckstk
                                "Functions in Dispatch" on page G60

                               Later To be delivered later. Quantity to be shipped later. Those additional
                               shipments may be due to postponements.
                               Technical info: Display field
                                "Functions in Dispatch" on page G60

                               Excess Excess quantity. Number of items exceeding the ordered quantity.
                               Excess quantities may be due to the movement of items.
                               Technical info: display field
                                "Functions in Dispatch" on page G60

                               LL Loading list number if loading lists have already been printed for this tour.
                               Use <F4> to print the loading lists.
                               Technical info: numeric field, DB field: lapoolauf.llnr
                                "Print loading list" on page G129
2.00 / 2022-04




                                "Print all loading lists" on page G130

                               PL The preliminary delivery note shows whether all preliminary delivery notes
                               have been printed for this route.


                 G - 40                                                     A+W Enterprise Dispatch Control
                 Software Reference                                                                                        Order Level




                                              All preliminary delivery notes have been printed.
                                              Not all of the preliminary delivery notes have been printed.
                                             Use <F4> to print a preliminary delivery note.
                                              Software Reference, “Print loading list” on page G-129
                                             A+W Enterprise will mark the field as 'not printed' in the following cases:
                                             • Change of route
                                             • Change of order
                                             • Change of order item(s)
                                             Preliminary delivery notes can be printed even if the shipment has not been
                                             reported complete. If only the preliminary note has been printed for an order,
                                             the order can still be changed in shipping control. If a delivery note has been
                                             printed for an order, the order cannot be changed any more in shipping control.
                                             A preliminary delivery note is no separate document in the database. The or-
                                             der status does not change because of a preliminary delivery note.
                                             When the goods are shipped, the shipped quantity has to be corrected on the
                                             preliminary delivery note. To print the delivery note, the corrected quantities
                                             must be transferred.
                                             Technical info: toggle field, DB field: lapoolauf.vlsdrukz

                                             DN Current status of the delivery note:


                 DN                 Meaning                    Information

                    gray            Open                       No delivery note created yet.

                    yellow          Booked to transport         "Book to transport" on page G78

                    blue            Delivery note created.     Document has been fully delivered.

                    red-gray        Delivery stop              A delivery stop has been specified for the customer (this status
                                                               indicator must be configured explicitly).

                    gray-red        No partial delivery        No partial deliveries are desired for this order (this status indicator
                                                               must be configured explicitly).

                    red-red         Delivery stop/no partial   There is a delivery stop for this customer and no partial delivery is
                                    delivery                   desired for the current order (this status indicator must be configured
                                                               explicitly).

                 Tab. G-3      Status of the delivery note

                                             Use <F4> to create and print the delivery note. Printing the delivery note cre-
                                             ates the corresponding record for financial accounting.
                                             Technical info: display field
                                              "Rack information" on page G85
                                             Use <Shift> + <F4> > Cancel to cancel the delivery notes.
                                              "Cancel delivery note" on page G90

                                             Cmp. Order reported complete. All items have been packed.
                                              All items are ready for shipment.
2.00 / 2022-04




                                              Not all of the items are ready to be shipped.
                                             Technical info: display field, DB field: lapoolauf.kompl



                 A+W Enterprise Dispatch Control                                                                                 G - 41
                 Order Level                                                               Software Reference




                               Call Call order. The order will be shipped on the customer's request.
                                Call order.
                                No call order.
                               Technical info: display field, DB field: lapoolauf.abruf

                               I Invoiced shows whether the order has been completely invoiced.
                                Order completely invoiced.
                                Invoiced not yet completely invoiced.
                               Technical info: display field, DB field: lapoolauf.fakturakz

                               I Shipping information shows whether shipping information is available for this
                               order.
                               Shipping information is entered in Sales or Purchasing in dialog External infor-
                               mation. Use <Shift> + <F4> > SA/PU information to call up this information.
                                There is dispatch information for this order or receipt of goods.
                                There is no dispatch information for this order.
                               Technical info: Display field, DB field: lapoolauf.info

                               Footer
                               The footer of the tab shows for all items the total quantities in the following
                               fields:
                               •   Tot. (total)
                               •   Call (request)
                               •   Avail. (available)
                               •   Pack. (packed)
                               •   Back. (backlog)
                               •   Later (to be delivered later)
                               •   Excess (delivered quantity)


                               Additional information
                                "Supplementary menu" on page G22
                                "Info Menu" on page G25
                                "Buttons" on page G27
2.00 / 2022-04




                 G - 42                                                     A+W Enterprise Dispatch Control
                 Software Reference                                                                            Order Level




                                          OrderInfo/Rack tab
                                          Dispatch control – Delivery date selection > Route selection > Order Info/Rack
                                          tab




                 Fig. G 16   Dispatch control – OrderInfo/Rack tab


                                          The Order info/Rack tab is displayed dynamically if you are working with the
                                          Rack module in Dispatch Control.
                                          The search fields in the header are explained in connection with Dispatch con-
                                          trol. Tour number and name are shown as well.
                                           "Dispatch Explorer" on page G15
                                          Most fields have already been described in the previous section:
                                           "Order Info tab" on page G39
                                          In addition, the following fields are displayed on the OrderInfo/Rack tab:

                                          On Rack Rack number on which the lites to be delivered are located. For the
                                          configuration of the free racks in the Dispatch Control, you must contact an
                                          A+W employee.
                                          Technical info: numeric field, DB field: lapoolauf.freigeststk

                                          Footer
2.00 / 2022-04




                                          The footer of the tab shows for all items the total quantities in the following
                                          fields:



                 A+W Enterprise Dispatch Control                                                                    G - 43
                 Order Level                                                    Software Reference




                               •   Tot. (total)
                               •   Call (request)
                               •   Avail. (available)
                               •   Pack. (packed)
                               •   On rack (on the rack)


                               Additional information
                                "Supplementary menu" on page G22
                                "Info Menu" on page G25
                                "Buttons" on page G27
2.00 / 2022-04




                 G - 44                                             A+W Enterprise Dispatch Control
                 Software Reference                                                                           Order Level




                                           Delivery Address tab
                                           Dispatch control – Delivery date selection > Route selection > Delivery Ad-
                                           dress tab




                 Fig. G 17   Dispatch control – Delivery address tab


                                           The Delivery address tab provides dispatch information on every order such
                                           as: address, travel time, and loading sequence on the truck or trailer.
                                           The search fields in the header are explained in connection with Dispatch con-
                                           trol. Route number and name are shown as well.
                                            "Dispatch Explorer" on page G15
                                           Most fields have already been described in the previous section:
                                            "Order Info tab" on page G39
                                           In addition, the following fields are displayed on the OrderInfo/Rack tab:

                                           LS Loading sequence of orders on the truck. The sequence of customers on
                                           a tour or route determines the loading sequence for the orders. When a new
                                           entry is made or an existing entry is changed, A+W Enterprise will want to
                                           know whether the changed loading sequence shall be applied to other orders.
                                           Technical info: numeric field, DB field: lapoolrouteposnr
2.00 / 2022-04




                                           Deliv. date Scheduled delivery date at the customer's.
                                           Technical info: date field, DB field: lapool.ankunft




                 A+W Enterprise Dispatch Control                                                                   G - 45
                 Order Level                                                                 Software Reference




                               D. time The delivery time is taken over from the order if you are working with
                               the via-Plant delivery.
                               Technical info: Alphanumeric field, DB field: lapool.ankunftszeit
                                "Dispatch Information" on page G119

                               TT Travel time to the customer. The planned travel time is determined from
                               the delivery address for the document (order/PO).
                               Technical info: Numeric field, DB field: lapool.fahrtzeit

                               Shipping address, street, post code, city Customer's or supplier's deliv-
                               ery address. These fields are taken over from the delivery address in the doc-
                               ument. The delivery address can be changed in Dispatch Control.
                               Technical info: Display fields, DB field: lapool.lname, lapool.lstr, lapoolauf.lplz,
                               lapoolauf.lort.
                                "Find delivery address" on page G83
                                "New delivery address" on page G84

                               Spl Split. A number entry in the Split field causes the breakdown of the total
                               quantity into the appropriate number of deliveries.
                               Technical info: Numeric field, DB field: lapool.splitt

                               Footer
                               The footer of the tab shows for all items the total quantities in the following
                               fields:
                               • Weight (of the order) of (the total weight to be transported)
                               • Surface (of the order) of (the total surface to be transported)
                               • Requested date


                               Additional information
                                "Supplementary menu" on page G22
                                "Info Menu" on page G25
                                "Buttons" on page G27
2.00 / 2022-04




                 G - 46                                                       A+W Enterprise Dispatch Control
                 Software Reference                                                                             Order Level




                                           Dispatch Info I tab
                                           Dispatch control – Delivery date selection > Route selection > Dispatch Info I
                                           tab




                 Fig. G 18   Dispatch Control – Dispatch Info I tab


                                           The Dispatch Info I tab provides further shipping information about the order.
                                           The search fields in the header are explained in connection with Dispatch con-
                                           trol. Tour number and name are shown as well.
                                            "Dispatch Explorer" on page G15
                                           Most fields have already been described in the previous section:
                                            "Order Info tab" on page G39
                                           In addition, the following fields are displayed on the Dispatch Info I tab:

                                           Reference Reference document for orders transferred from another site.
                                           Technical info: numeric field, DB field: kauf.parauftrnr

                                           Ex. sender External sender. For transferred orders, the client number of the
                                           sending site is displayed.
                                           Technical info: numeric field, DB field: kauf.parhausnr
2.00 / 2022-04




                                           In. sender Internal sender. For transferred orders, the order number of the re-
                                           ceiving site is displayed.
                                           Technical info: numeric field, DB field: kauf.parhausnr



                 A+W Enterprise Dispatch Control                                                                     G - 47
                 Order Level                                                                Software Reference




                               Shipping information Shipping information is displayed only if it has been
                               defined at order entry.
                               You can edit existing dispatch information or enter new dispatch information in
                               this field. You can use <Ctrl> + <B> to take the dispatch information over into
                               the order.
                               Technical info: Numeric field, DB field: lapool.exbez2

                               PAT ID of the new packing type from the order. The assigned packing type is
                               displayed on the Dispatch Info I tab in plain text. You can assign a new packing
                               type to the order with the <F9> key. This change is only taken over into the or-
                               der with <Ctrl> + <B>.
                               Technical info: Numeric field, DB field: lapool.verpackart

                               ST ID of the dispatch type from the order. The assigned dispatch type is dis-
                               played on the Dispatch Info II tab in plain text.
                               You can assign a new dispatch type to the order with <F9>. This change can
                               only be taken over into the order with <Ctrl> + <B>. Alternatively, the dispatch
                               type can be stored or changed via the info menu <Shift> + <F4>.
                                "Dispatch Information" on page G119
                               Technical info: numeric field, DB field: lapool.versandart

                               ST Delivery type ID. The assigned delivery type is displayed on the Dispatch
                               Info II tab in plain text.
                               You can assign a new delivery type to the order with the <F9> key. This change
                               is only taken over with <Ctrl> + <B>.
                               Technical info: Numeric field, DB field: lapool.lieferart

                               E.Cust Exit customs. Number of the customs office in the country of origin.
                               You can enter a different customs clearance office.
                               Technical info: numeric field, DB field: lapool.azsnr

                               D.Cust Destination customs. Number of the customs office in the country of
                               destination.
                               You can enter another customs office in the country of destination.
                               Technical info: numeric field, DB field: lapool.bzsnr

                               via S Number of the site that makes the delivery. The field is only assigned
                               with use of the via-plan module.
                               Technical info: Numeric field, DB field: lapool.viahaus

                               Route Number of the route by which the shipment is made. The field is only
                               assigned with use of the via-plan module.
                               Technical info: Numeric field, DB field: lapool.endroute


                               Additional information
                                "Supplementary menu" on page G22
                                "Info Menu" on page G25
                                "Buttons" on page G27
2.00 / 2022-04




                 G - 48                                                    A+W Enterprise Dispatch Control
                 Software Reference                                                                             Order Level




                                           Dispatch Info II tab
                                           Dispatch control – Delivery date selection > Route selection > Dispatch Info II
                                           tab




                 Fig. G 19   Dispatch Control – Dispatch Info II tab


                                           Dispatch Info II tab shows the information from the Dispatch Info I tab in detail.
                                           The search fields in the header are explained in connection with Dispatch Con-
                                           trol. Route number and name are shown as well.
                                            "Dispatch Explorer" on page G15
                                           Most fields have already been described in the previous section:
                                            "Dispatch Info I tab" on page G47
                                           In addition, the following fields are displayed on the Dispatch Info II tab:

                                           Dispatch Info Abbreviated dispatch information. This is only displayed if it is
                                           stored in the order or the PO. You can change the dispatch information or enter
                                           new dispatch information in the field.
                                           Technical info: Display field

                                           Packing Type Description of the packing type. The allocated ID appears on
                                           Shipping info I tab.
2.00 / 2022-04




                                           Technical info: display field




                 A+W Enterprise Dispatch Control                                                                     G - 49
                 Order Level                                                               Software Reference




                               Dispatch Type Description of the dispatch type. The allocated ID appears on
                               Dispatch info I tab.
                               Technical info: Dispatch field

                               Incoterm Description of the delivery type. The assigned ID is displayed on
                               the Dispatch Info I tab.
                               Technical info: Display field

                               PL1, PL2 Private Long 1 and Private Long 2 are meant for customized sup-
                               plementary information. At Order entry you can save information in the form of
                               numbers. The field names PL1 and PL2 can be configured customer-specifi-
                               cally. Via the info menu <Shift> + <F4> to the Dispatch Control, you can store
                               or change these fields.
                                "Dispatch Information" on page G119
                               Technical info: numeric field, DB field: lapool.private_long1, lapool.pri-
                               vate_long2

                               PC1, PC2 Private Long 1 and Private Long 2 are meant for customized sup-
                               plementary information. At Order entry you can save informational texts. The
                               field names PC1 and PC2 can be configured customer-specifically. The max-
                               imum input per field is 15 characters. Via the info menu <Shift> + <F4> in the
                               Dispatch Control, you can store or change these fields.
                                "Dispatch Information" on page G119
                               Technical info: alphanumeric field, DB field: lapool.private_char1, lapool.pri-
                               vate_char2

                               Footer
                               No additional information is output in the tab's footer.


                               Additional information
                                "Supplementary menu" on page G22
                                "Info Menu" on page G25
                                "Buttons" on page G27
2.00 / 2022-04




                 G - 50                                                     A+W Enterprise Dispatch Control
                 Software Reference                                                                            Order Level




                                           Add. Info tab
                                           Dispatch Control – Delivery date selection > Route selection > Add. Info tab




                 Fig. G 20   Dispatch control – Add. Info tab


                                           Additional info tab shows the delivered quantity and further information on the
                                           order, item weight, movements, and information on the release for shipment
                                           provided by the customer.
                                           The search fields in the header are explained in connection with Dispatch con-
                                           trol. Tour number and name are shown as well.
                                            "Dispatch Explorer" on page G15
                                           Most fields have already been described in the previous section:
                                            "Dispatch Info I tab" on page G47
                                           In addition, the following fields are displayed on the Add. Info tab:

                                           Customer Customer name or supplier name from the order or PO.
                                           Technical info: Display field, DB field: mp.name

                                           T/Del Total quantity delivered to the customer so far.
                                           Technical info: numeric field, DB field: lapoolauf.geslief
2.00 / 2022-04




                                           kg/N Net weight of the order in kilograms. The net weight is the weight of all
                                           items, excluding racks or packaging.
                                           Technical info: toggle field, DB field: lapoolauf.gewicht



                 A+W Enterprise Dispatch Control                                                                   G - 51
                 Order Level                                                                Software Reference




                               kg/G Gross weight of the order in kilograms. The gross weight is the weight
                               of all items including racks and packaging.
                               Technical info: toggle field, DB field: lapoolauf.gewichtbrutto

                               sf Total square meters of glass from the order.
                               Technical info: Display field, DB field: lapoolauf.qm

                               DN Traffic light display for the delivery note.
                                "Status of the delivery note" on page G41

                               Call Call code for the order. The order is delivered on request from the cus-
                               tomer.
                               Technical info: Display field, DB field: lapoolauf.abrufkz

                               Postp. Code to mark to postpone the order. If you would like to postpone sev-
                               eral orders to another dispatch date, then you must click the checkboxes of the
                               orders in question. The selected orders are then marked with a checkmark.
                               You postpone the orders on the Postpone (Dispatch) dialog.
                                The order will be postponed.
                                The order will not be postponed.
                               Technical info: display field
                                "Functions in Dispatch" on page G60

                               Call Shows whether the customer is informed of the shipment of goods by
                               phone.
                                Customer will be called prior to dispatch.
                                Customer will get no call.
                               If you enable the field, the Call checkbox will automatically be enabled for all
                               other orders for this customer.
                               Technical info: Alphanumeric field, DB field: lapoolauf.anruf

                               Print Defines whether a delivery note has been printed.
                                Delivery note has been printed.
                                Delivery note has not been printed yet.
                               Technical info: display field, DB field: lapoolauf.druckkz

                               Type The selected delivery note type for this order is shown as a code.
                               The following codes are available:
                               • I = individual delivery note
                               • C = collective delivery note
                                  Technical info: display field

                               Footer
                               The footer of the tab shows for all items the total quantities in the following
                               fields:
                               • kg/N (net weight)
2.00 / 2022-04




                               • kg/G (gross weight)
                               • sqm (total surface in square meters)
                                   Technical info: Display field


                 G - 52                                                      A+W Enterprise Dispatch Control
                 Software Reference                                          Order Level




                                        Additional information
                                         "Supplementary menu" on page G22
                                         "Info Menu" on page G25
                                         "Buttons" on page G27
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                 G - 53
                 Item Level                                                             Software Reference




                              Item Level
                              Item level in Dispatch Control provides detailed information on the individual
                              order items or purchase orders.
                              This level offers the following tabs:
                               "Item Info I tab" on page G55
                               "Item Info II tab" on page G58
                              From the item level, you can change back to the order or tour level. If you are
                              working with the Dispatch Explorer, you can also change to the Dispatch Ex-
                              plorer to select another date.
                               "Dispatch Explorer" on page G15
2.00 / 2022-04




                 G - 54                                                   A+W Enterprise Dispatch Control
                 Software Reference                                                                            Item Level




                                           Item Info I tab
                                           Dispatch control – Delivery date selection > Route selection > Item Info I tab




                 Fig. G 21   Dispatch control – Item info I tab


                                           Item info I tab provides detailed information on the orders.
                                           The search fields in the header are explained in connection with Dispatch con-
                                           trol. The route, order number, and customer name are shown as well.
                                            "Dispatch Explorer" on page G15

                                           S The entries in column S (status) are loaded from TourInfo and OrderInfo
                                           tab.
                                           Technical info: display field
                                            "Route status" on page G29

                                           Itm Sequential item number from the order or PO.
                                           Technical info: Display field, DB field: lapool.posnr

                                           Article Name of the article to be delivered.
                                           Technical info: display field, DB field: artikel.artbez1

                                           Tot. Total quantity of the item to be delivered.
                                           Technical info: display field, DB field: lapoolpos.gesstk
2.00 / 2022-04




                                           Call Number of items the customer has ordered for that date.
                                           Technical info: display field, DB field: lapoolpos.abrufstk


                 A+W Enterprise Dispatch Control                                                                  G - 55
                 Item Level                                                                   Software Reference




                              Sched Scheduled. Item quantity scheduled for dispatch.
                              Technical info: display field, DB field: lapoolpos.sollstk

                              Avail Available quantity for this item.
                              Technical info: display field, DB field: lapoolpos.gefstk

                              Pack Quantity packed for this item. Use <F4> to check for missing quantities.
                              You can use <F4> > Correct packed quantity to change the entry in this field.
                              Technical info: numeric field, DB field: lapoolpos.iststk
                               "Missing quantity check for" on page G75
                               "Rack View for Order" on page G80

                              B.Log Item quantity that is not available for the desired tour.
                              Technical info: display field, DB field: lapoolpos.rueckstk

                              Add. Quantity to be shipped later. Those shipments may be due to move-
                              ment.
                              Technical info: display field, DB field: lapoolpos.nachstk
                               "Postpone" on page G64

                              ExcSh Excess quantity. Number of items exceeding the ordered quantity. Ex-
                              cess quantities may be due to the movement of items.
                              Technical info: display field, DB field: lapoolpos.ueberstk

                              T/Del Total quantity delivered to the customer so far.
                              Technical info: display field, DB field: lapoolpos.gesliefstk

                              kg Item weight in kilograms.
                              Technical info: display field, DB field: lapoolpos.gewicht

                              sf Item surface in square feet
                              Technical info: display field, DB field: lapoolpos.qm

                              Cmp Completely packed item.
                               All items are ready for shipment.
                               Not all of the items are ready to be shipped.
                              Technical info: display field, DB field: lapoolpos.kompl
                               "Missing quantity check for" on page G75

                              I (invoiced) Completely invoiced item.
                               Order item has been invoiced.
                               Order item has not been invoiced yet.
                              Technical info: display field, DB field: lapoolpos.fakturakz

                              Footer
                              The footer of the tab shows for all items the total quantities in the following
                              fields:
                              • Tot.
2.00 / 2022-04




                              • Call (request)
                              • Sched (scheduled)



                 G - 56                                                     A+W Enterprise Dispatch Control
                 Software Reference                                          Item Level




                                        •   Avail (available)
                                        •   Pack (packed)
                                        •   B.Log (backlog)
                                        •   Add (Additional delivery)
                                        •   ExcSh (excess shipment)
                                        •   T/Del. (delivered in total)
                                        •   kg
                                        •   sf


                                        Additional information
                                         "Supplementary menu" on page G22
                                         "Info Menu" on page G25
                                         "Buttons" on page G27
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                G - 57
                 Item Level                                                                               Software Reference




                                             Item Info II tab
                                             Dispatch Control – Delivery date selection > Route selection > Item Info II tab




                 Fig. G 22    Dispatch control – Item info II tab


                                             Item info II tab shows the items for the order in question plus additional infor-
                                             mation on the individual items.
                                             The search fields in the header are explained in connection with Dispatch con-
                                             trol. The route, order number, and customer name are shown as well.
                                              "Dispatch Explorer" on page G15
                                             Most fields have already been described in the previous section:
                                              "Item Info I tab" on page G55
                                             In addition, the following fields are displayed on the Add. Info tab:

                                             Pack/Pack. type Number and description of the packing type.
                                             Technical info: display field, DB field: lapoolpos.verpackart

                                             Width, height Item size.
                                             Technical info: display field, DB field: lapoolpos.breite

                                             mm Thickness of the item lite in millimeters.
2.00 / 2022-04




                                             Technical info: Display field, DB field: lapoolpos.staerke




                 G - 58                                                                    A+W Enterprise Dispatch Control
                 Software Reference                                                                           Item Level




                                        Footer
                                        The footer of the tab shows for all items the total quantities in the following
                                        fields:
                                        • Tot. (total)
                                        • Sched (scheduled)
                                        • Pack (packed)
                                        • kg
                                        • sf


                                        Additional information
                                         "Supplementary menu" on page G22
                                         "Info Menu" on page G25
                                         "Buttons" on page G27
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                  G - 59
                 Functions in Dispatch                                                               Software Reference




                                         Functions in Dispatch
                                         In the Dispatch Control, you have the opportunity to pack the item quantity
                                         manually or to postpone it, to manage racks and print the dispatch documents.
                                         Depending on the status of the selected data on the item, order or tour level
                                         and the available system configuration, the following functions are available:
                                          "Go to" on page G62
                                          "Postponement of several items - selection" on page G66
                                          "Missing quantity check - actions" on page G76
                                          "Print loading list" on page G129
                                          "Book to transport" on page G78
                                          "Rack View for Order" on page G80
                                          "Rack information" on page G85
                                         Furthermore, you have many overview opportunities and information dialogs
                                         using the pre-determined criteria:
                                          "Cancel transport booking" on page G79
                                          "SA/PU info (global)" on page G113
                                          "Booked racks (overview)" on page G102
                                          "Information on the Order" on page G70
                                          "Finished goods stock - overview" on page G123
                                          "Dispatch Information" on page G119
                                          "Set/remove tour lock" on page G86
                                          "Information on the Order" on page G70
2.00 / 2022-04




                 G - 60                                                              A+W Enterprise Dispatch Control
                 Software Reference                                                             Functions in Dispatch




                                        Search
                                        Dispatch Control – [Search]




                                        Fig. G 23    Go to…


                                        You can reach the Search dialog on all data levels. This way, you can search
                                        for a particular document and jump directly to this document.
                                        With the key combination <Ctrl> + <K>, you are also taken to the Order info.

                                        Order Order number. Enter the number in this field or select the number with
                                        <F9>. With this search, you get detailed information about the selected docu-
                                        ment.
                                        Technical info: Numeric field, selection field, <F9>
                                         "Information on the Order" on page G70

                                        Mode Dispatch mode. If you want to change directly to the PO documents,
                                        toggle in the Mode field to the value in question. With a purchasing mode, you
                                        can then search for a PO instead of an order.
                                        Technical info: Toggle field


                                        Button           Description

                                        [Trigger]        Use Trigger to start the search.
                                        [Cancel]         Use Cancel to discard the search.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                               G - 61
                 Functions in Dispatch                                                              Software Reference




                                         Go to
                                         Dispatch control – [Go to]




                                         Fig. G 24    Go to…


                                         You can reach the Go to dialog on all data levels. This way, you can search for
                                         a particular document and jump directly to this document. The Delivery date,
                                         Site, and Mode fields are pre-populated with their current values. If needed,
                                         you can change the search criteria.

                                         Deliv. Date Delivery date of the orders. This field is pre-populated with the
                                         current date. You can change the value.
                                         Technical info: Input field, date format.

                                         Site Number of the site or client whose orders you are searching. The field is
                                         pre-populated with the value that is assigned by default to the current employ-
                                         ee in the master data.
                                         Technical info: Selection field, <F9>

                                         Route Route number. If you leave the Route field empty and there are
                                         planned routes for the Delivery date, you jump directly to the Tour Info.
                                         Technical info: selection field, <F9>
                                          "RouteInfo tab" on page G29

                                         Order Order number. If you leave the Order field empty and there are orders
                                         for the Delivery date and the selected route, you jump directly to the Order In-
                                         fo.
                                         Technical info: Selection field, <F9>
                                          "Order Info tab" on page G39

                                         Item Sequential item number from the document. If you select the fields De-
                                         livery date, Route, and Order, the Item Info starts directly.
                                         Technical info: Selection field, <F9>
                                          "Item Info I tab" on page G55
2.00 / 2022-04




                                         Mode Dispatch mode. If you want to change directly to the PO documents,
                                         toggle in the Mode field to the value in question. With a purchasing mode, you



                 G - 62                                                              A+W Enterprise Dispatch Control
                 Software Reference                                                           Functions in Dispatch




                                        can then search for a PO instead of an order.
                                        Technical info: Toggle field


                                        Button           Description

                                        [Trigger]        Use Trigger to start the search.
                                        Cont. Delete     You can empty the dialog fields with Delete Content.
                                        [Cancel]         Use Cancel to discard the search.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                G - 63
                 Functions in Dispatch                                                               Software Reference




                                         Postpone
                                         Dispatch control – Data level > <F4> Postpone




                                         Fig. G 25    Postponement (dispatch)


                                         This dialog is used to postpone tours, orders, or units to another date or an-
                                         other route. You can enter text describing the reason of postponement in field
                                         Reason.
                                         If you start Postponement on the tour level, the whole route can be postponed.
                                         In this case, the Order and Item fields in the upper part of the dialog are empty.
                                         If you start Postponement on the order or item level, these two fields are pre-
                                         populated accordingly.
                                         The fields in the upper part of the dialog indicate what will be postponed:

                                         Frm Tour D. Originally scheduled delivery date.

                                         Route Number of the originally scheduled route.

                                         Units Number of units to be postponed.

                                         Order Number of the order to be postponed. The display is empty if the entire
                                         route is postponed.

                                         Item Sequential order item number that will be postponed. The display is
                                         empty if the entire route or the entire order is postponed.
                                         The fields in the middle of the dialog indicate to when and why the postpone-
                                         ment:

                                         Reasons Choose a reason for the postponement. It can be configured in the
                                         system which of these reasons appears as default value on the dialog. The fol-
                                         lowing reasons are possible:
                                         • Cust. Request:
                                            The customer has asked for the postponement.
                                         • Backlog:
                                            The item is still incomplete or not ready for shipment.
                                         • Client-Cancel:
2.00 / 2022-04




                                            The customer has canceled the order, the item, or part of the quantity. With
                                            the postponement as customer cancellation, both the call quantity as well
                                            as the planned quantity are reduced by the amount canceled.


                 G - 64                                                                A+W Enterprise Dispatch Control
                 Software Reference                                                              Functions in Dispatch




                                        •   Prod.-Cancel:
                                            Delivery is canceled for internal reasons, e.g. if the product is no longer
                                            available. With Prod. Cancel, only the planned quantity is reduced. The
                                            postponement can be configured separately with the reason Prod. Cancel.
                                        •   Tour Planning:
                                            The postponement is due to route planning or scheduling. The postpone-
                                            ment is done analogous to the Cust Request only on the tour level. This
                                            possibility can be configured separately. Similarly, the Tour Planning rea-
                                            son can be configured as the default reason.
                                        With additional configuration, customer-specific reasons can be stored as a
                                        selection selo. With this configuration, the Reason field can be left empty or a
                                        free text entered. Here, the system sends an e-mail with the postponement
                                        reason to the responsible employee.

                                        Postponement Text field for entering the reason of postponement. This text
                                        will appear in the shipping log.

                                        Rack Rack number. If you are working with racks in the Dispatch Control, un-
                                        der some circumstances, entire racks can be postponed. However, this possi-
                                        bility depends on other criteria, such as packed and available quantity, rack
                                        scheduling, item status.

                                        Postpone Several Records Toggle field.

                                        To Tour Day New delivery date. When you start postponement, the system
                                        checks whether the defined date is a valid delivery date. If the new date is not
                                        a valid tour date, then the tour or delivery cannot be postponed. If you are
                                        working with planned routes, you can search for a particular tour in this field
                                        with <F9>.
                                         Master Data: Software Reference, “Route Plan” on page B-170

                                        Route Number of the new route if the route needs to be amended due to the
                                        postponement.

                                        Units Number of units to be postponed. A+W Enterprise shows the total
                                        quantity by default.
                                        The fields in the lower part of the dialog specify who and when is postponing:

                                        Executed by Employee number of the person who has made the postpone-
                                        ment. This information is written to the log.
                                         "Dispatch Information" on page G119

                                        on Date on which the postponement was made. This information is written to
                                        the log.
                                         "Dispatch Information" on page G119
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                 G - 65
                 Functions in Dispatch                                                             Software Reference




                                         Postponement of several items - selec-
                                         tion
                                         Dispatch control – Data level > <F4> Postpone several items




                                         Fig. G 26    Postpone several items - selection dialog


                                         This dialog is used to filter your shipments in order to postpone several items
                                         of an order or several orders at the same time. On the following dialog, you
                                         specify the quantity to be postponed per item.
                                          "Postponement of several items - action" on page G67

                                         Site Site number. The field is pre-populated with the current site number. You
                                         can only change the value if you are working on a multi-client system.
                                         Technical info: Selection field, <F9>, DB field: lapool.hausnr

                                         Date Delivery date. The field is pre-populated with the date that you displayed
                                         on the original data level.
                                         Technical info: Input field, date format, DB field: lapool.ltplan

                                         Route Route number. The field is pre-populated with the route number that
                                         you displayed on the original tour level.
                                         Technical info: Selection field, <F9>, DB field: lapool.ltplan

                                         Order Order number. The field is pre-populated with the order number that
                                         you displayed on the original order level.
                                         Technical info: Selection field, <F9>, DB field: lapool.auftrnr

                                         L/L Loading/cargo list number. You can search for a particular loading list
                                         here if it has already been assigned.
                                         Technical info: Selection field, <F9>, DB field: lapool.llnr
2.00 / 2022-04




                 G - 66                                                                A+W Enterprise Dispatch Control
                 Software Reference                                                                   Functions in Dispatch




                                          Postponement of several items - action
                                          Dispatch control – Data level > <F4> Postpone several items, make selection




                 Fig. G 27   Postponement of several items


                                          On this dialog, you select the items for postponement. You also adjust the
                                          quantity per item that must be postponed. You have already made the pre-se-
                                          lection through details:
                                           "Postponement of several items - selection" on page G66
                                          Most fields have already been described in the following section:
                                           "Item Info I tab" on page G55
                                          You can change the following fields to make the postponement:

                                          Postpone The Postpone field is pre-populated with the item quantity. You can
                                          change this quantity if only part of the item should be postponed. At most the
                                          item quantity may be postponed. The program checks the plausibility of the
                                          value entered.
                                          Technical info: Input field, numeric field.

                                          Booking date Checkbox for action marking the booking.
                                          Item is marked for postponement.
                                           Item will not be postponed.
2.00 / 2022-04




                                          Technical info: Selection field, checkbox.




                 A+W Enterprise Dispatch Control                                                                    G - 67
                 Functions in Dispatch                                                              Software Reference




                                         Start the postponement with the [Trigger] button. In the following dialog, enter
                                         to when the marked items should postponed.
                                          "Postpone" on page G64
2.00 / 2022-04




                 G - 68                                                               A+W Enterprise Dispatch Control
                 Software Reference                                                             Functions in Dispatch




                                        Order Info
                                        Dispatch control – Data level> <F4> > Order info.




                                        Fig. G 28    Postpone several items


                                        On this dialog, you search for an order (in dispatch mode for sales documents)
                                        or for a PO (in dispatch mode with purchasing documents). With the [Trigger]
                                        button, you can access the information you're looking for.

                                        Order/PO Document number. With <F9> you can search for the desired doc-
                                        ument number.
                                        Technical info: <F9>, numeric field, DB field: lapool.auftrnr

                                        Mode Dispatch mode. In this field, you select the dispatch mode. This de-
                                        cides whether the selection will be made by order or PO. With <F9> you can
                                        search for the desired document number.
                                        Technical info: Selection field, <F9>, DB field: lapool.vmodus
                                        The search results are described in the next section:
                                         "Information on the Order" on page G70
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                               G - 69
                 Functions in Dispatch                                                                         Software Reference




                                                  Information on the Order
                                                  Dispatch control – Data level > <F4> > Order info > [Trigger]




                 Fig. G 29       Information on the order or the PO


                                                  On this dialog, you see additional information about the selected document.
                                                  The dialog title is dynamic; the display is adjusted depending on the dispatch
                                                  mode. In addition, the appropriate document number appears in the title.
                                                  All fields on this dialog are informative and cannot be changed.

                                                  S Status of current delivery item.


                 S (Status)           Meaning                   Information

                    white             Open                      There is no dispatch planning for this item.

                    green/yellow      Available                 Part of this item is reported as Available.

                     yellow/white     Part on rack              Part of this item is already on the rack.

                     yellow           Packed                    This item is completely packed.

                     half blue        En route                  Part of this item is already en route.

                     blue             Delivered                 This item has been fully delivered.

                     red              Locked                    This item is on a locked tour.
2.00 / 2022-04




                 Tab. G-4        Status of delivery items




                 G - 70                                                                           A+W Enterprise Dispatch Control
                 Software Reference                                                                Functions in Dispatch




                                        Site Site number or client number.
                                        Technical info: display field, DB field: lapool.hausnr

                                        HT Handling time from the order or PO in order to load and unload the goods.
                                        The handling time can be specified in the market partner master data.
                                        Technical info: Display field, DB field: lapool.hausnr

                                        Del. Date Date on which the order will be delivered to the customer.
                                        Technical info: display field, DB field: lapool.ltplan, kauf.ltplan

                                        Arrival Date on which the shipment reaches the customer. The arrival date is
                                        calculated starting from the delivery date - taking into account various other
                                        criteria - such as travel time, handling time, tour plan, route days, and the cal-
                                        endar.
                                        Technical info: Display field, <F9>, DB field: lapool.auftrnr

                                        Route Route number.
                                        Technical info: display field, DB field: lapool.routenr

                                        Order Order/purchase order number.
                                        Technical info: display field, DB field: lapool.auftrnr, lapool.vorgang

                                        Itm Item number.
                                        Technical info: display field, DB field: lapool.posnr

                                        Tot. Total item quantity.
                                        Technical info: display field, DB field: lapool.gesstk, kpos.menge

                                        Call Number of items the customer has ordered for that date.
                                        Technical info: display field, DB field: lapool.abrufstk

                                        Sched. Quantity of the item already scheduled.
                                        Technical info: display field, DB field: lapool.sollstk

                                        Pack Quantity packed for this item.
                                        Technical info: display field, DB field: lapool.iststk

                                        Width Width of the lite from the item.
                                        Technical info: Display field, DB field: lapool.laenge

                                        Height Height of the lite from the item.
                                        Technical info: Display field, DB field: lapool.breite

                                        kg Item weight in kilogram.
                                        Technical info: display field, DB field: lapool.gewicht

                                        VP Display checkbox if the goods are delivered via-plant.
                                        Technical info: Display field
2.00 / 2022-04




                                        [FP Stock] This button opens the Finished Goods dialog.
                                         "Finished goods stock - overview" on page G123




                 A+W Enterprise Dispatch Control                                                                  G - 71
                 Functions in Dispatch                                                        Software Reference




                                         [Go to] This button opens the Go to dialog.
                                          "Go to" on page G62
2.00 / 2022-04




                 G - 72                                                           A+W Enterprise Dispatch Control
                 Software Reference                                                              Functions in Dispatch




                                        Book goods received for
                                        Dispatch control - Data level > <F4> > Book goods received for




                                        Fig. G 30    Book goods receipt for


                                        On this dialog, you select an order for which you would like to book the receipt
                                        of goods. This function is only available for the via-plant configuration.


                                        via-plant configuration
                                        The function scope via-plant is not part of this documentation. If necessary,
                                        please request a detailed description from the responsible A+W employee.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                 G - 73
                 Functions in Dispatch                                                              Software Reference




                                         Cancel receipt of goods
                                         Dispatch control - Data level > <F4> > Cancel receipt of goods




                                         Fig. G 31    Information on the order


                                         On this dialog, you select an order for which you would like to book the receipt
                                         of goods. This function is only available for the via-plant configuration.

                                            via-plant configuration
                                            The function scope via-plant is not part of this documentation. If necessary,
                                            please request a detailed description from the responsible A+W employee.
2.00 / 2022-04




                 G - 74                                                               A+W Enterprise Dispatch Control
                 Software Reference                                                               Functions in Dispatch




                                        Missing quantity check for
                                        Dispatch Control – data level > <F4> > Missing quantity check for




                                        Fig. G 32    Missing quantity check for ...


                                        On this dialog, you select for which order you would like to check the item
                                        quantity. You can check all orders for the particular delivery date or the route
                                        or you can select only a particular order. A missing quantity check for is con-
                                        ducted if an item cannot be delivered completely on the specified delivery
                                        date.

                                           Missing quantity check in dispatch
                                           A missing quantity check in dispatch is conducted only at the user's own
                                           responsibility. When working with A+W Production, the production software
                                           takes over all quantity bookings. If, however, you run the check in Dispatch
                                           Control, some of the conditions for the missing quantity check and subse-
                                           quent booking in the system can be configured individually. Contact an
                                           A+W employee for this.

                                        Del. Date Delivery date for which missing quantities shall be checked. The
                                        field is pre-populated with the date that you selected on the previous dialog.
                                        Technical info: Input field, DB info: lapool.ltplan

                                        Route Number of the route to be checked for missing quantities. If you leave
                                        the field empty, all orders for the selected delivery date are loaded into the ac-
                                        tion dialog.
                                        Technical info: Selection field <F9>, numeric field, DB info: lapool.routenr

                                        Order Number of the order to be checked for missing quantities. If you leave
                                        the field empty, all orders for the selected delivery date and the selected route
                                        are loaded into the action dialog.
                                        Technical info: Selection field, date format, DB info: lapool.auftrnr

                                        L/L Number of the loading/cargo list to be checked for missing quantities. By
                                        entering the loading list number, you restrict the selection.
                                        Technical info: Selection field <F9>, numeric field, DB info: lapool.llnr

                                        [Trigger] Use this button to open the Check missing quantities dialog.
2.00 / 2022-04




                                        Additional information
                                         "Missing quantity check - actions" on page G76




                 A+W Enterprise Dispatch Control                                                                  G - 75
                 Functions in Dispatch                                                                Software Reference




                                           Missing quantity check - actions
                                           Dispatch Control – data level > <F4> > Missing quantity check for > Make se-
                                           lection > [Trigger]




                 Fig. G 33   Dispatch control – Missing quantity check view


                                           You conduct the missing quantity check on this dialog. When entering the di-
                                           alog, the Pack column is pre-populated with the order or item quantity. If the
                                           total quantity is not available, you can correct this for the affected order. The
                                           missing quantity is written automatically to the BLog (backlog) field. You can
                                           postpone the missing quantity to a different date or another route subsequent-
                                           ly.
                                           The pre-population is done with the Missing quantity check for... search dialog.
                                            "Missing quantity check for" on page G75
2.00 / 2022-04




                                           The fields in the header serve for orientation. These fields provide information
                                           about where you are.



                 G - 76                                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                              Functions in Dispatch




                                        All fields have already been described in the previous sections:
                                         "Order Info tab" on page G39
                                         "Item Info I tab" on page G55

                                        Pack Packed quantity. Changing the packed quantity will also change the en-
                                        try in field Backlog. field. You can postpone the entire item.
                                        Technical info: Input field, date format, DB info: lapool.iststk
                                         "Postponement of several items - action" on page G67

                                        B.Log The backlog is the result of deducting the packed quantity from the
                                        scheduled quantity.
                                        Technical info: Display field, date format, DB info: lapool.rueckstk
                                        If the planned units are not available on the planned date, then you must post-
                                        pone the remaining units (backlog) to another date. When you trigger the
                                        booking, you can postpone the missing quantity as backlog:
                                         Postponement of several items - action

                                        Date Scheduled shipping date. If you change the date, A+W Enterprise will
                                        want to know whether the date shall be passed on downwards. This means
                                        that all items shown in this dialogue will be shipped at the amended date.
                                        Technical info: Selection field, date format, DB info: lapool.ltplan

                                        Book. Date Selection field for booking this record.
                                        Technical info: Checkbox

                                        Buttons
                                        If there is a backlog, the corresponding order item must be postponed to an-
                                        other date.
                                        Use [Postpone] to open the dialog Postponement.
                                         "Postponement of several items - action" on page G67
                                        Use [Book] to save the changes. The selected item is reported packed. If the
                                        item quantity is packed completely, the status of the item is set to cmp. (com-
                                        plete).
                                         "Item Info I tab" on page G55
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                               G - 77
                 Functions in Dispatch                                                              Software Reference




                                         Book to transport
                                         Dispatch control - Data level > <F4> > Book to transport
                                         Completely packed items can be booked to transport using this menu element.
                                         The booking is done in the background. Depending on the system configura-
                                         tion, a delivery note can be generated. Furthermore, it can also be configured
                                         whether the bookings to transport for the past and/or future are permitted.
                                         A transport booking causes the appropriate status change:
                                          "Status of delivery items" on page G70
                                         For booking results, see, for example:
                                          "Log" on page G125

                                            Book to transport
                                            This function can be configured separately. Talk to an A+W employee.
2.00 / 2022-04




                 G - 78                                                             A+W Enterprise Dispatch Control
                 Software Reference                                                               Functions in Dispatch




                                        Cancel transport booking
                                        Dispatch control – Data level > <F4> > Cancel transport booking




                                        Fig. G 34    Cancel transport booking for…


                                        On this dialog, you select an order for the transport rebooking. This action as-
                                        sumes that there was already a transport booking. After you have rebooked
                                        the transport booking, you can create a new preliminary delivery note or a de-
                                        livery note for the corrected delivery quantity.

                                        Del. Date Delivery date for which the transport booking is reversed.
                                        Technical info: entry field, DB field: lapool.ltplan

                                        Site Client number of site number for which the transport booking is reversed.
                                        Technical info: selection field, DB field: lapool.hausnr

                                        Order Order number for which the transport booking is cancelled.
                                        Technical info: numeric field, DB field: lapool.hausnr

                                        Via Site Number of the site used to cancel the transport booking.
                                        Technical info: numeric field, DB field: lapool.hausnr, lapool.viaflag

                                        [Trigger] Use this button to trigger the rebooking.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                 G - 79
                 Functions in Dispatch                                                              Software Reference




                                         Rack View for Order
                                         Dispatch control - Data level > <F4> > Rack view for Order




                                         Fig. G 35    Barcode rack view


                                         On this dialog, you receive information about the rack barcodes if these al-
                                         ready exist. The information is in the database table bcbock.

                                         Order External order number.
                                         Technical info: numeric field, DB field: bcbock.auftrnr

                                         Item Item number in the order.
                                         Technical info: numeric field, DB field: bcbock.posnr

                                         Rack Rack number on which the order item is located. If an order item is split
                                         and distributed across several racks, you will see all assignments on this dia-
                                         log, e.g. order 4002466, item 3.
                                         Technical info: Numeric field, DB info: bcbock.gnr

                                         Slot Slot number if the current item is in a slot.
                                         Technical info: Numeric field, DB info: bcbock.subnr

                                         Piece Number of lites on the rack. Since one record per piece is written to the
                                         table bcbock, this quantity is totaled up for the rack in question and displayed
                                         here.
                                         Technical info: Numeric field, DB info: bcbock.anzahl

                                            Table bcbock in dispatch
                                            The booking of the database table bcbock is only done if the Free rack
                                            function is configured appropriately. Contact an A+W about this.
2.00 / 2022-04




                 G - 80                                                               A+W Enterprise Dispatch Control
                 Software Reference                                                               Functions in Dispatch




                                        Results of the rack scheduling
                                        Dispatch control – Order Level > <F4> > Results of the rack scheduling




                                        Fig. G 36    Results of the rack scheduling


                                        On this dialog, you can view information about the rack scheduling.

                                           Database tables for rack scheduling
                                           The results of the rack scheduling distinguish themselves depending on the
                                           system configuration. If you are using the Free racks function, rack-related
                                           data is booked to the database tables gest and gestzu after reporting from
                                           A+W Production. If you are using other configurations, the tables kposgest
                                           and bcbock are used. For this reason, the technical info is not always listed
                                           in the following fields. For detailed information about rack scheduling,
                                           please contact an A+W employee.

                                        The following fields appear on this dialog:

                                        Order Order number. Display of the rack scheduling is only possible on the
                                        order level. You start the display for a particular order.
                                        Technical info: Display field, DB info: lapool.auftrnr

                                        Item Item number from the selected order.
                                        Technical info: Display field, DB info: lapool.posnr

                                        Qty Item quantity that is present on the current rack.

                                        Total Total item quantity.
                                        Technical info: Display field, DB info: lapool.sollstk

                                        Rack Rack number.

                                        Type Rack type. This designation is determined from the master data.
                                        Technical info: Alphanumeric field, DB info: gtyp.kurzbez

                                        Del. Date Delivery date for the current order item.
                                        Technical info: Display field, DB info: lapool.ltplan
2.00 / 2022-04




                                        Route Number of the delivery route.
                                        Technical info: Display field, DB info: lapool.routennr




                 A+W Enterprise Dispatch Control                                                                 G - 81
                 Functions in Dispatch                                                              Software Reference




                                         Packaging Planning
                                         Dispatch control - Order level > <F4> > Packaging planning




                                         Fig. G 37   Preliminary delivery note for...


                                         On this dialog, you can view information about the packaging planning.

                                            Packaging planning in A+W Enterprise
                                            The results of packaging planning depend on the system configuration.
                                            The packaging planning from the order entry is described below:

                                             Sales, “Packaging Planning” on page D-239



                                            Customized settings
                                            Customized settings are not part of this documentation.
2.00 / 2022-04




                 G - 82                                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                              Functions in Dispatch




                                        Find delivery address
                                        Dispatch control - Order level > <F4> Delivery address > Find delivery address




                                        Fig. G 38    Find addresses


                                        On this dialog, you can select a delivery address insofar as it must be
                                        changed. By default, the delivery address from the order is taken over into Dis-
                                        patch Control. The Find address function is also available in the order entry
                                        and was also described there. All addresses are displayed that are stored from
                                        the customer for the current order. Displayed fields can differ depending on the
                                        system configuration. Use the search fields to filter for a saved address.
                                         Sales, “Find Addresses” on page D-49
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                G - 83
                 Functions in Dispatch                                                              Software Reference




                                         New delivery address
                                         Dispatch control - Order level > <F4> > Delivery address > New delivery ad-
                                         dress




                                         Fig. G 39    Delivery address


                                         Use this dialog to enter a new delivery address if no address could be found.
                                         Clicking [OK] saves the address only for this delivery. With <F3> you can write
                                         the new address to the master data.
                                         The fields for the dialog are described in the following section:
                                          Sales, “New Delivery Address” on page D-141
2.00 / 2022-04




                 G - 84                                                               A+W Enterprise Dispatch Control
                 Software Reference                                                              Functions in Dispatch




                                        Rack information
                                        Dispatch control - Order Level > <F4> Rack information




                                        Fig. G 40    Rack information


                                        On this dialog, you can set up customer-specifically whether and which rack
                                        information can be output.
                                        Access to the dialog is enabled with the environment variable SQL_GEST_IN-
                                        FO. The GruppeID and SQL number are stored in this variable that control the
                                        language, fields, and operations output. The figure above serves only to clarify
                                        this and will not be described in any more detail in this document.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                G - 85
                 Functions in Dispatch                                                                 Software Reference




                                         Set/remove tour lock
                                         Dispatch control - Tour level > <Shift> + <F4> > Set/remove tour lock




                                         Fig. G 41     One of the messages for the tour lock


                                         Use this function to lock the selected tour, or unlock the selected tour. A tour
                                         is a route scheduled for a certain delivery date.
                                         A tour is locked when it has been scheduled and no further orders shall be
                                         added.
                                         An alternative route must be defined in master data for the tour to be locked.
                                         When a new order is booked for this tour at order entry after the tour has been
                                         locked, the new order will be automatically assigned to the alternative route.
                                         The route lock is set only if one order of the route is booked by another site or
                                         client as being en route.
                                         If a tour lock has been set, field TS (tour status) has the status Tour locked (tool
                                         tip: red).
                                          "Lock all tours" on page G87
                                          "Route status" on page G29
2.00 / 2022-04




                 G - 86                                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                 Functions in Dispatch




                                        Lock all tours
                                        Dispatch control - Tour level > <Shift> + <F4> > Lock all tours




                                        Fig. G 42     Result of the tour lock


                                        This function is used to lock all tours shown on the tab.
                                        A tour is locked when it has been scheduled and no further orders shall be
                                        added.
                                        Alternative routes must be defined in master data for the tours to be locked.
                                        When a new order is booked for this tour at order entry after the tour has been
                                        locked, the new order will be automatically assigned to the alternative routed.
                                        If all tours are locked, all TS (tour status) have the status Tour locked (tool tip:
                                        red).
                                         "Route status" on page G29
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                    G - 87
                 Functions in Dispatch                                                                Software Reference




                                         Transport data
                                         Dispatch control - Tour level > <Shift> + <F4> > Transport data




                                         Fig. G 43    Transport data


                                         On this dialog, you store the transport data for the current tour. You can enter
                                         transport data for orders and purchased orders if you have configured the pur-
                                         chasing documents in Dispatch Control.
                                          "Dispatch Control – menus" on page G22

                                         Route Number of the route for which the transport data is defined.
                                         Technical info: display field, DB field: lapool.routennr

                                         Driver Name of the driver for this tour. Employees are defined in master data.
                                         Technical info: selection field, numeric field, DB field: mitarb.manr

                                         Vehicle Vehicle for the tour. The vehicles are defined in master data.
                                         Technical info: selection field, numeric field, DB field: lkw.lkw.nr

                                         Trailer Two fields for the input of trailers for transport. The trailers are stored
                                         in the master data.
                                         Technical info: Selection field, numeric field, DB field: lkw.lkw.nr
                                         Use <End> to save the settings.
                                         The transport data entered is displayed on the VehicleInfo tab:
                                          "VehicleInfo tab" on page G34
2.00 / 2022-04




                 G - 88                                                                A+W Enterprise Dispatch Control
                 Software Reference                                                                Functions in Dispatch




                                        Stock Reference
                                        Dispatch control - Tour level > <Shift> + <F4> > Stock reference




                                        Fig. G 44    Message on printing stock reference


                                        This dialog shows the number of the list of picked orders to be printed. For
                                        stored goods, this function is used to start the picking or stock withdrawal. This
                                        function is configured customer-specifically.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                   G - 89
                 Cancel                                                               Software Reference




                          Cancel
                          Dispatch control – Order Level > <Shift> + <F4> > Cancel
                          You can access the following dialogs via the Cancel menu:
                           "Cancel delivery note" on page G90
                           "Cancel order" on page G91
                           "Cancel receipt of goods" on page G92
                           "Cancel shipping status" on page G93
                          A delivery receipt within the via-plant configuration can be canceled on the fol-
                          lowing dialog:
                           "Cancel receipt of goods" on page G74



                          Cancel delivery note
                          Dispatch control – Order Level > <Shift> + <F4> > Cancel > Cancel delivery
                          note




                          Fig. G 45    Cancel delivery note


                          This dialog is used to cancel existing delivery notes. The marking on Order info
                          tab in field DN (delivery note) changes its status to booked to transport (tool
                          tip: yellow). Status S of the order changes to en route (tool tip: half blue).
                          Before you trigger the cancellation, the order data that you are canceling is dis-
                          played on the dialog.

                          Deliv. Date Date on which the order shall be delivered to the customer.
                          Technical info: display field, DB field: lapool.ltplan

                          Route Route number.
                          Technical info: display field, DB field: lapool.routennr

                          Order Order number for the delivery note to be cancelled.
                          Technical info: display field, DB field: lapool.auftrnr
2.00 / 2022-04




                 G - 90                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                               Cancel




                                        Cancel order
                                        Dispatch control – Order Level > <Shift> + <F4> > Cancel > Cancel order




                                        Fig. G 46     Cancel order


                                        This dialog is used for canceling an order. In the rules, orders in the Sales area
                                        are canceled since the logistics employees do not have the necessary sales
                                        information under some circumstances. For order cancellation in dispatch,
                                        there can be data inconsistencies if the order is already in production and has
                                        the status Local-correction.

                                        Order Number of the order to be cancelled.
                                        Technical info: display field, DB field: lapool.auftrnr

                                        Canc. Inform. Information on the cancelled order. The maximum length of
                                        this text is 60 characters.
                                        Technical info: Alphanumeric field, DB info: kauf.exbez2
                                        You trigger this action with <Trigger>. Depending on the order status, the pro-
                                        gram can output a security query with a status indication or decline the action.
                                        If you want to cancel the order nevertheless, you must enter the reason for
                                        cancellation on the following dialog. This reason is displayed in the foreground
                                        for the user when the order is called up.


                                        Additional information
                                         Sales, “Cancel” on page D-148
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                   G - 91
                 Cancel                                                              Software Reference




                          Cancel receipt of goods
                          Dispatch control – Order Level > <Shift> + <F4> > Cancel > Cancel receipt of
                          goods > [Trigger]




                          Fig. G 47    Cancellation info


                          This dialog is used for canceling a goods receipt. This menu element can only
                          be called up for purchasing documents in dispatch mode.
                          Before you trigger the cancellation, the data for the goods receipt that you are
                          canceling is displayed on the dialog.

                          Deliv. Date Delivery date on which the receipt of goods should occur.
                          Technical info: Display field, DB info: lapool.ltplan

                          Route Route number.
                          Technical info: display field, DB field: lapool.routennr

                          Order Number of the PO for which the goods receipt should be canceled.
                          Technical info: Display field, DB info: lapool.auftrnr, lapool.,vorgang=2

                          Cancellation Info Information text for the cancelled goods receipt. Maximum
                          length of this text is 60 characters.
                          Technical info: Alphanumeric field, DB info: kauf.exbez2
2.00 / 2022-04




                 G - 92                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                             Cancel




                                        Cancel shipping status
                                        Dispatch control – Data level > <Shift> + <F4> > Cancel > Cancel dispatch
                                        status




                                        Fig. G 48    Message on the cancelled dispatch status


                                        This function is used to cancel the dispatch status. Dispatch Control automat-
                                        ically sets an order's dispatch status to Scheduled if an order is postponed to
                                        another delivery date in Dispatch Control. When the dispatch status has been
                                        cancelled, the order can be amended at order entry without restrictions.
                                        The Dispatch Control staff has to check with order entry if an order has not
                                        been passed on to production yet. The reasons for this are:
                                        •   When an order is entered or changed at order entry, the data will be trans-
                                            ferred to production. Production produces the order for the defined delivery
                                            date.
                                        •   If Dispatch Control postpones a released order, production will not be au-
                                            tomatically informed of the postponement.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                G - 93
                 Racks                                                              Software Reference




                          Racks
                          Lites are generally placed on racks in production and transported this way.
                          These racks can also be managed in Dispatch Control.
                          The use of rack scheduling and rack management is customer-specific, so that
                          not all functions and dialogs are available to the same extent. For additional
                          information about the racks in Dispatch Control, please contact an A+W em-
                          ployee.
                          Dialogs that can be called up with <Shift> + <F4> Racks are described below:
                           "Rack allocation -selection" on page G95
                           "Rack allocation - view" on page G96
                           "Resolve rack - selection" on page G98
                           "Resolve rack - view" on page G98
                           "Free racks (overview)" on page G100
                           "Booked racks (overview)" on page G102
                           "All racks (overview)" on page G103
                           "Individual racks" on page G105
                           "Racks for order" on page G106
                           "Lite allocation" on page G108
2.00 / 2022-04




                 G - 94                                                A+W Enterprise Dispatch Control
                 Software Reference                                                                               Racks




                                        Rack allocation -selection
                                        Dispatch control - Data level >Shift> + >F4> > Racks > Rack allocation




                                        Fig. G 49    Selection dialog rack allocation


                                        On this dialog, you search for an order for which you want to see the rack
                                        scheduling. The order selected here must already be scheduled on one or sev-
                                        eral racks.

                                        Site Site number on which you work in dispatch.
                                        Technical info: Display field, DB info: lapool.hausnr

                                        Del. Date Delivery date whose data you want to edit in dispatch.
                                        Technical info: Selection field, date format, DB info: lapool.ltplan

                                        Route Route number whose data you want to edit in dispatch.
                                        Technical info: Selection field <F9>, DB info: lapool.routennr

                                        Order Order number of the order to be edited. The order selection is possible
                                        with <F9>. In the field next to this, the appropriate Dispatch mode is dis-
                                        played.Technical info: Numeric field, DB info: lapool.auftrnr

                                        L/L Loading list number if a loading list has already been printed for the order.
                                        Technical info: Display field, DB info: lapool.llnr
                                        With [Trigger] you load the rack data for the selected order. The results of the
                                        displays are described on the following dialog:
                                         "Rack allocation - view" on page G96
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                 G - 95
                 Racks                                                                 Software Reference




                          Rack allocation - view
                          Dispatch control - Data level >Shift> + >F4> > Racks > Rack allocation, selec-
                          tion made




                          Fig. G 50    Rack allocation


                          On this dialog, you see the rack allocation for the selected order. The rack al-
                          location is done in A+W Production in that the order items are packed on racks
                          and reported off-site. In addition, there can be tour allocation. You see the re-
                          sults of the report on this dialog.
                          The dialog title is constructed dynamically, so that in the title, you can see the
                          delivery date and route on which your order is scheduled.

                          Cmp Complete code for the current order item on the rack. The code is set if
                          the total item quantity is already allocated to the rack.
                          Technical info: Display field

                          Rack Rack number on which the current order item is located.
                          Technical info: display field, DB field: gest.exgnr

                          RType Rack type of the current rack number from the rack master data.
                          Technical info: Display field, DB field: gest.exgnr

                          Order Current order number.
                          Technical info: display field, DB field: lapool.auftrnr, gestzu.auftrnr

                          Itm Item number of the selected order.
                          Technical info: display field, DB field: lapool.posnr

                          Article Article description from the master data.
                          Technical info: display field, DB field: artikel.artbez1

                          Tot. Total quantity of the item.
2.00 / 2022-04




                          Call Already called quantity of the item.




                 G - 96                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                               Racks




                                        Width Width of the lite from the item.
                                        Technical info: Numeric field, DB field: lapool.laenge

                                        Length Height of the lite from the item.
                                        Technical info: Numeric field, DB field: lapool.breite

                                        On rack Quantity that is on the rack.

                                        Book Checkbox for the booking.
                                         Item is marked for booking.
                                         Item will not be booked.
                                        With [All] you can mark all rack records on the dialog to start other actions.
                                        With [Trigger] you save the rack allocation if you have to make manual chang-
                                        es on the dialog.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                 G - 97
                 Racks                                                                Software Reference




                          Resolve rack - selection
                          Dispatch control - Data level <Shift> + <F4> > Racks > Resolve rack




                          Fig. G 51    Selection dialog for rack resolution


                          On this dialog, you select for which delivery date and route you want to resolve
                          the rack.
                          The selection fields are identical to those in the rack allocation:
                           "Rack allocation -selection" on page G95



                          Resolve rack - view
                          Dispatch control - Data level <Shift> + <F4> > Racks > Resolve rack




                          Fig. G 52    Rack Resolved dialog


                          On this dialog, you trigger the rack resolution. If you mark the rack for editing
                          (Free column) and execute the action, the allocation to the route and delivery
                          date is triggered and the packed quantities are unpacked again. Subsequently,
                          there can be a new rack-PDC booking, insofar as all criteria for the new book-
                          ing are fulfilled.
2.00 / 2022-04




                 G - 98                                                   A+W Enterprise Dispatch Control
                 Software Reference                                                                               Racks




                                           Rack bookings via PDC in Dispatch Control
                                           The Rack bookings via PDC function must be configured appropriately in
                                           your system. Please contact the responsible A+W employee for more infor-
                                           mation.

                                        Rack Rack number on which the current order item is located.
                                        Technical info: Display field, DB info: gest.exgnr

                                        RType Rack type (name) of the current rack number from the rack master da-
                                        ta.
                                        Technical info: Display field, DB info: gest.typnr, gtyp.kurzbez

                                        Order Current order number.
                                        Technical info: Display field, DB info: lapoolauftrnr, gestzu.auftrnr

                                        Itm Item number of the selected order.
                                        Technical info: display field, DB info: lapool.posnr, gestzu.posnr

                                        Article Article description from the master data.
                                        Technical info: display field, DB field: artikel.artbez1

                                        Tot. Total quantity.
                                        Technical info: Display field, DB info: lapool.geststk

                                        Width Width of the lite from the item.
                                        Technical info: Display field, DB field: lapool.laenge

                                        Length Height of the lite from the item.
                                        Technical info: Display field, DB field: lapool.breite

                                        on Rack Quantity that is on the rack.
                                        Technical info: Display field, DB info: gestzu.menge

                                        Free Checkbox for marking.
                                         Item is marked for booking.
                                         Item will not be booked.
                                        If you [Trigger] the booking, you are first asked whether the existing rack allo-
                                        cation should actually be deleted and the packed quantity unpacked
                                        again.With [All] you mark all rack records on the dialog to start additional ac-
                                        tions.
                                        With [Trigger] you resolve the rack allocation.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                 G - 99
                 Racks                                                                  Software Reference




                           Free racks (overview)
                           Dispatch control - Data level <Shift> + <F4> > Racks > Free racks (overview)




                           Fig. G 53    Free racks dialog (tour overview)


                           On this dialog, you get information about free racks on the current tour. When
                           entering the dialog, it is checked whether there are complete racks for the de-
                           sired delivery date and tour. If not, you can display all racks for this tour.

                           Cmp Complete code for the current order item on the rack. The question mark
                           indicates that the item is not yet completely available.
                           Technical info: Display field

                           Rack Rack number on which the current order item is located.
                           Technical info: Display field, DB info: gest.exgnr

                           Order Order number on this tour.
                           Technical info: Display field, DB info: lapool.auftrnr, gestzu.auftrnr

                           Itm Item number of the selected order.
                           Technical info: display field, DB info: lapool.posnr, gestzu.posnr

                           Article Article description from the master data.
                           Technical info: display field, DB field: artikel.artbez1

                           Tot. Total quantity.
                           Technical info: display field, DB field: lapool.gesstk

                           Plan. Scheduled quantity.
                           Technical info: Display field, DB info: lapool.sollstk

                           Call Quantity called.
                           Technical info: Display field, DB info: lapool.abrufstk
2.00 / 2022-04




                           on Rack Quantity that is on the rack.
                           Technical info: Display field, DB info: gestzu.menge


                 G - 100                                                    A+W Enterprise Dispatch Control
                 Software Reference                                                                                Racks




                                        Width Width of the lite from the item.
                                        Technical info: Display field, DB field: lapool.laenge

                                        Length Height of the lite from the item.

                                        Technical info: Display field, DB field: lapool.breite
                                        With [Rack] you start the Lite allocation dialog for the selected rack:
                                         "Lite allocation" on page G108
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                  G - 101
                 Racks                                                                Software Reference




                           Booked racks (overview)
                           Dispatch control - Data level <Shift> + <F4> > Racks > Booked racks (over-
                           view)




                           Fig. G 54     Booked racks dialog (tour overview)


                           This dialog displays all booked racks for the current tour. You can postpone
                           the desired (marked) racks on this dialog to another tour.

                           Book. Date Checkbox for the booking. Mark the desired item in order to post-
                           pone it with the [Postpone] button. On the Postpone dialog, the data is pre-
                           populated with the current tour and it can then be changed. If a different tour
                           is entered, all rack quantities are postponed and rebooked to racks. Here, the
                           packed quantity is always postponed, even if the postponement is to an earlier
                           date.
                           The dialog displays the same field as on the dialog for free racks:
                            "Free racks (overview)" on page G100
                           You can use the following buttons on the dialog:
                           •   [Postpone]/<F3>
                                "Postpone" on page G64
                           •   [Rack]/<F5>
                                "Lite allocation" on page G108
                           •   [Total]/<Shift> + <F9>
                               The total of all lites per rack is formed and displayed on the dialog.
                           •   [All/Complete]/<Shift> + <F8>
                               If on the dialog free and complete racks are displayed, you can restrict the
                               display to all or complete.
2.00 / 2022-04




                 G - 102                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                               Racks




                                        All racks (overview)
                                        Dispatch control - Data level <Shift> + <F4> > Racks > All racks (overview)




                                        Fig. G 55    All racks dialog (tour overview)


                                        On this dialog, you can see the total rack overview for the current order. With
                                        the [Rack] button, you can rebook rack quantities:
                                         "Lite allocation" on page G108
                                        The following fields appear on this dialog:

                                        Cmp Complete code for the current order item on the rack.
                                          • The question mark ? indicates that the item is not yet completely avail-
                                            able.
                                          • An asterisk * indicates that the item is complete.
                                          • An empty field indicates that this item is not yet packed.

                                        Rack Rack number on which the current order item is located.
                                        Technical info: Display field, DB info: gest.exgnr

                                        Order Order number on this tour.
                                        Technical info: Display field, DB info: lapool.auftrnr, gestzu.auftrnr

                                        Itm Item number of the selected order.
                                        Technical info: display field, DB info: lapool.posnr, gestzu.posnr

                                        Article Article description from the master data.
                                        Technical info: display field, DB field: artikel.artbez1

                                        Tot. Total quantity.
                                        Technical info: display field, DB field: lapool.gesstk

                                        Sched Scheduled quantity.
                                        Technical info: Display field, DB info: lapool.sollstk
2.00 / 2022-04




                                        Pack Quantity called.
                                        Technical info: Display field, DB info: lapool.iststk


                 A+W Enterprise Dispatch Control                                                                 G - 103
                 Racks                                                                  Software Reference




                           on Rack Quantity that is on the rack.
                           Technical info: Display field, DB info: gestzu.menge

                           Width Width of the lite from the item.
                           Technical info: Display field, DB field: lapool.laenge.

                           Length Height of the lite from the item.
                           Technical info: Display field, DB field: lapool.breite.

                           Del. Date Delivery date on which the rack is already allocated.
                           Technical info: Display field, DB info: gest.mdat

                           Route Route number to which the rack is already allocated.
                           Technical info: Display field, DB info: gest.routnr

                              Lite-rack allocation via PDC report
                              For the allocation of lites to racks via PDC report, no fixed allocation is pos-
                              sible if the quantities reported do not match the data in dispatch. Then
                              these racks remain in the system as free racks. If a fixed allocation to a tour
                              is not possible because the quantities in dispatch are on different tours,
                              then you can total up the dispatch quantity from the individual racks on this
                              view in order to make the allocation subsequently.Prerequisite: The tours
                              from which the quantities are postponed to the desired tour are not locked
                              by another user.
2.00 / 2022-04




                 G - 104                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                                   Racks




                                        Individual racks
                                        Dispatch control - Data level <Shift> + <F4> > Racks > Individual racks




                                        Fig. G 56     Individual racks


                                        Use this menu element to call up complete information about a rack. On the
                                        selection dialog, you select the desired rack number with <F9> or you enter it
                                        manually. With [Trigger] you start the lite-rack allocation. The fields for the Lite-
                                        Rack allocation dialog are described in the following section:
                                         "Lite allocation" on page G108

                                        Racks Name of the rack for which the information should be determined.
                                        Technical info: Selection field, <F9> alphanumeric, DB field: gest.exgnr
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                   G - 105
                 Racks                                                                  Software Reference




                           Racks for order
                           Dispatch control - Data level <Shift> + <F4> > Racks > Racks for order




                           Fig. G 57    Rack view for order


                           Use this menu element to call up complete rack information for an order. In the
                           selection dialog, you select the desired order number with <F9> or you enter
                           it manually.
                           With the [Trigger] button, you will see the rack overview for the selected order.
                           With the [Rack] button, you start the lite-rack assignment.
                           The fields for the Lite-Rack allocation dialog are described in the following sec-
                           tion:
                            "Lite allocation" on page G108

                           Racks Number of the rack for which the information should be determined.
                           This number is then taken over on the Rack view for the order dialog and dis-
                           played in the Rack field.
                           Technical info: selection field, <F9> alphanumeric, DB field: gest.exgnr

                           Order Number of the order for which documents are listed.
                           Technical info: display field, DB field: lapool.auftrnr, gestzu.auftrnr

                           Itm Item number of the selected order.
                           Technical info: display field, DB field: lapool.posnr, gestzu.posnr
2.00 / 2022-04




                           Article Article description from the master data.
                           Technical info: display field, DB field: artikel.artbez1




                 G - 106                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                        Racks




                                        Total Total quantity.
                                        Technical info: display field, DB field: lapool.gesstk

                                        Del. Date Delivery date on which the rack is already allocated.
                                        Technical info: Display field, DB info: gest.mdat

                                        Route Route number to which the rack is already allocated.
                                        Technical info: Display field, DB info: gest.routnrZ

                                        Piece Quantity that is on the rack.
                                        Technical info: Display field, DB info: gestzu.menge

                                        Width Width of the lite from the item.
                                        Technical info: Display field, DB field: lapool.laenge.

                                        Length Height of the lite from the item.
                                        Technical info: Display field, DB field: lapool.breite.

                                        DN Delivery note code.
                                         "Status of the delivery note" on page G41
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                          G - 107
                 Racks                                                                Software Reference




                           Lite allocation
                           Dispatch control - Data level <Shift> + <F4> > Racks > Lite rack allocation




                           Fig. G 58    Lite rack allocation dialog


                           On this dialog, you allocate lites to a rack, route, and delivery date or you get
                           information about existing allocations. You can delete the allocation and there-
                           fore empty the rack.

                              Lite rack allocation
                              The functional principle of rack allocation is described separately and can
                              be requested from a responsible A+W employee.

                           Rack Rack number for which the rack allocation is executed, displayed or
                           should be changed.
                           Technical info: Alphanumeric field, DB field: gest.exgnr

                           Type Rack type number. The rack types are stored under Logistics - Rack
                           Management - Rack Master Data - Rack Types.
                           Technical info: Numeric field, DB field: gtyp.gtypnr

                           Remark Information field with 60 characters for the rack-lite allocation.
                           Technical info: Alphanumeric field, DB field: gest.bemerk

                           Weight Empty weight of the selected rack. The rack weight is stored per Rack
                           type under Logistics - Rack Management - Rack Master Data - Rack Types.
                           With <Shift>+<F8> you can change the Weight field. This change applies only
                           for the current rack and is not taken over into the master data for all racks of
                           the rack type.
                           Technical info: Numeric field, DB field: gtyp.eiggew
2.00 / 2022-04




                           Modified Name of the employee who made the last change to the rack allo-
                           cation data. The name is determined from the employee master data using the



                 G - 108                                                A+W Enterprise Dispatch Control
                 Software Reference                                                                                Racks




                                        employee number.
                                        Technical info: Display field, DB field: gtyp.aendermanr

                                        Fixed Tour Allocat. If the lite-rack allocation has already been made, the
                                        route-delivery date allocation will be displayed as information on this line.

                                        Booked Name of the employee who made the last change to the rack alloca-
                                        tion data. The name is determined from the employee master data using the
                                        employee number.
                                        Technical info: Display field, DB field: gtyp.aendermanr

                                        Lite Allocation Under the lite allocation, the name of the employee and date
                                        of the last change or booking are output. The name is determined from the em-
                                        ployee master data using the employee number.
                                        Technical info: Display field, DB field: gtyp.aendermanr

                                        Order Number of the order that is allocated to the current rack.
                                        Technical info: Numeric field, DB field: gestzu.auftrnr

                                        Itm Internal item number from the order.
                                        Technical info: Numeric field, DB field: gestzu.posnr

                                        Tnr Tupel number. The field is only relevant for purchasing documents with
                                        extended workbench.
                                        Technical info: Numeric field, DB field: aufstrukt.tnr

                                        Qty Item quantity that is on the rack.
                                        Technical info: Numeric field, DB field: gestzu.menge

                                        Total Total item quantity from the order.
                                        Technical info: Display field, DB field: lapool.gesstk, kpos.menge

                                        Available Available item quantity.
                                        Technical info: Display field

                                        D.Route Dispatch route. As soon as a fixed lite-rack allocation is made, the
                                        appropriate route number is displayed in this field and in the next field, the De-
                                        livery date.
                                        Technical info: Display field

                                        Deliv. Date Specified delivery date. As soon as a fixed lite-rack allocation is
                                        made, the appropriate delivery date is displayed in this field, and in the field
                                        before this one, the Dispatch route.
                                        Technical info: Display field

                                        Width Width of the lite from the item.
                                        Technical info: Display field, DB field: lapool.laenge

                                        Height Height of the lite from the item.
2.00 / 2022-04




                                        Technical info: Display field, DB field: lapool.breite

                                        Article Product name of the item article from the master data.



                 A+W Enterprise Dispatch Control                                                                 G - 109
                 Racks                                                            Software Reference




                           You have additional possibilities on this dialog:
                           • With <Shift>+<F8> you can change the Weight field.
                           • With <F5> you can show the Dispatch info dialog. The dialog is only dis-
                              played if there is dispatch information.
                           • With [Empty] or <Ctrl>+<F8> you can empty the rack. That is, the content
                              of the rack is removed.
2.00 / 2022-04




                 G - 110                                            A+W Enterprise Dispatch Control
                 Software Reference                                                                             Racks




                                        SA/PU information
                                        Dispatch control - Order level > <Shift> + <F4> > SA/PU information




                                        Fig. G 59    SA/PU information dialog


                                        This dialog provides information about the selectged order. Insofar as you are
                                        working with POs in Dispatch Control, the order information is combined with
                                        the associated PO information.

                                        Order Current order number.
                                        Technical info: display field

                                        Itm Internal item number from the order.
                                        Technical info: Display field

                                        Tot. Total item quantity from the order.
                                        Technical info: Display field

                                        Call Quantity already called.
                                        Technical info: Display field

                                        Pack Quantity already packed.
                                        Technical info: Display field

                                        Width Width of the lite from the item.
                                        Technical info: Display field

                                        Height Height of the lite from the item.
                                        Technical info: Display field

                                        Purchase order Current PO number if a PO was created for the order item.
                                        Technical info: Display field
2.00 / 2022-04




                                        Itm Internal item number from the PO.
                                        Technical info: Display field



                 A+W Enterprise Dispatch Control                                                              G - 111
                 Racks                                                 Software Reference




                           Date PO date.
                           Technical info: Display field

                           Mode Dispatch mode.
                           Technical info: Display field
2.00 / 2022-04




                 G - 112                                   A+W Enterprise Dispatch Control
                 Software Reference                                                                             Racks




                                        SA/PU info (global)
                                        Dispatch control – Order level > <Shift> + <F4> > SA/PU info (global)




                                        Fig. G 60     SA/PU info (global) dialog


                                        With the SA/PU Info (global) menu item, you can call up the combined sales
                                        and purchasing information for a selected order. On the selection dialog (small
                                        figure) you enter the number or select the desired document with <F9>. De-
                                        pending on the dispatch mode selected, you can search for an order or a PO.
                                        The search fields in the header and dispatch mode are described in the follow-
                                        ing section:
                                         "Dispatch Explorer" on page G15

                                        Order Order number.
                                        Technical info: display field, DB field: lapool.auftrnr
                                        If you have selected a PO on the selection dialog, then a PO number is in the
                                        Order field and the order number in the Reference field.

                                        Itm Item number.
                                        Technical info: display field, DB field: lapool.lfdpos

                                        Article Article name of the order.
                                        Technical info: display field, DB field: artikel.artbez1

                                        Tot. Total item quantity.
                                        Technical info: display field, DB field: lapool.gesstk
2.00 / 2022-04




                                        Call Number of items the customer has ordered for that date.
                                        Technical info: display field, DB field: lapool.abrufstk


                 A+W Enterprise Dispatch Control                                                              G - 113
                 Racks                                                                Software Reference




                           Date Delivery date from the order or PO (1st column on the dialog).
                           Technical info: Display field, DB info: lapool.ltplan

                           Route Route number.
                           Technical info: display field, DB field: lapool.routenr

                           Site Site number or client number.
                           Technical info: display field, DB field: lapool.hnr

                           Reference Number of the reference document. If you have selected a PO on
                           the selection dialog, then a PO number is in the Order field and the order num-
                           ber in the Reference field.
                           Technical info: Display field, DB info: lapool.auftrnr (lapool.vorgang=2 (PO) or
                           5 (order))

                           Itm Item number from the reference document.
                           Technical info: Display field, DB info: lapool.posnr

                           Date Delivery date from the reference document.
                           Technical info: Display field, DB info: lapool.ltplan

                           Route Number of the route from the reference document.
                           Technical info: Display field, DB info: lapool.routenr

                           Sched Scheduled quantity.
                           Technical info: Display field, DB info: lapool.sollstk

                           Tpe Dispatch mode for reference document. The following values are dis-
                           played:
                           • SA Deliv. (SA outgoing)
                           • P1. (PU outgoing goods)
                           • P2. (PU incoming goods)
                           Technical info: display field, DB field: lapool.vmodus
2.00 / 2022-04




                 G - 114                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                           Racks




                                          Dispatch Control – Overview
                                          Dispatch control - Data level > <Shift> + <F4> > Overview




                 Fig. G 61   Shipping control – overview


                                          With the Overview menu, you start the search dialog with which you can com-
                                          bine various criteria to create an overview.
                                          The following selection criteria are available:
                                              •   Site
                                              •   Del. Dat (planned delivery date)
                                              •   Route (delivery route)
                                              •   Order (order number)
                                              •   External (customer order no.)
                                              •   L/L (number of the loading list)
                                              •   Proj. (project number)
                                              •   Customer (customer number)
                                              •   Weight (item weight in kg)
                                              •   Surface (area per item in sq m)
2.00 / 2022-04




                                              •   Width (lite height in mm)
                                              •   Height (lite length in mm)



                 A+W Enterprise Dispatch Control                                                             G - 115
                 Racks                                                                       Software Reference




                           You can change the filter conditions in all fields as needed:

                           Condition      Meaning

                           =              Search exactly for this value (e.g. market partner field = 600004 lists
                                          only documents relating to this market partner).

                           >              Search for larger values (e.g. market partner field > 600004 lists only
                                          documents with market partner numbers larger than 600004).

                           p              Search for patterns in text fields (e.g. Reference field Shape 12 lists
                                          all documents with the reference text model 12.)

                           0              Search for values = 0 (e.g. market partner field 0 lists only market
                                          partners with the number 0).

                           z              Search all values in the range.

                           !              Search all values except for this value (e.g. Department field! 10 lists
                                          all departments except for the department with the number 10).

                           <              Search for smaller values (e.g. market partner field < 600004 lists
                                          only documents with market partner numbers smaller than 600004).

                           Tab. G-5      Meaning of the filter conditions

                           After entry, use <F3> to trigger the search action. Insofar as the search was
                           successful, a hit quantity is output on the same dialog. Use <F2> to see addi-
                           tional fields for selection.
                           The following fields are displayed on the hit dialogs:

                           Del. Date Delivery date stated in the order.
                           Technical info: date field, DB field: lapool.ltplan

                           Route Route number.
                           Technical info: display field, DB field: lapool.routennr

                           Order External order number. For dispatch mode with purchasing docu-
                           ments, the number of the PO is always output here.
                           Technical info: Display field, DB info: lapool.auftrnr

                           Itm Item number from the order.
                           Technical info: display field, DB field: lapool.posnr

                           Cust. Customer number of the order.
                           Technical info: Display field, DB info: lapool.kunr

                           Proj. Project number from the order if there is one.
                           Technical info: Display field, DB info: lapool.objnr

                           Tot. Total quantity of items that was entered for this order.
                           Technical info: Display field, DB info: lapool.gesstk
2.00 / 2022-04




                           Call Number of items the customer has ordered for that date.
                           Technical info: display field, DB field: lapool.abrufstk



                 G - 116                                                    A+W Enterprise Dispatch Control
                 Software Reference                                                                                  Racks




                                        Pack Quantity packed for this item.
                                        Technical info: display field, DB field: lapool.iststk

                                        Width Height of the lite.
                                        Technical info: display field, DB field: lapool.breite

                                        Height Width of the lite.
                                        Technical info: display field, DB field: lapool.laenge

                                        sf Item surface in square feet.
                                        Technical info: display field, DB field: lapool.iststk

                                        LL Loading list number if there is already a loading list for this order.
                                        Technical info: Display field, DB info: lapool.llnr

                                        DN Indication of whether there is already a delivery note for this order.
                                        Technical info: Display field, DB info: lapool.lsdrukz

                                        Prod.description Product description for the order item.
                                        Technical info: Display field, DB info: lapool.artbez1

                                        Shape Shape number from the order item if there is one.
                                        Technical info: Display field, DB info: lapool.modnr

                                        kg Weight per order item.
                                        Technical info: Display field, DB info: lapool.gewicht

                                        Footer
                                        The footer of the dialog displays additional information for the following fields:
                                        •   External customer OrderNr
                                        •   Width (largest value for lite length from the hit quantity)
                                        •   Height (largest value for lite height from the hit quantity)
                                        •   kg (total weight for all items displayed in the overview)
                                        •   qm (total surface for all items displayed in the overview)
                                        •   Tot. (total quantity of the units entered for all items displayed in the over-
                                            view)
                                        •   Call (total number of units requested for all items displayed in the overview)
                                        •   Pack. (total quantity of packed units for all items displayed in the overview)
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                    G - 117
                 Racks                                                               Software Reference




                           Delivery Date Change List
                           Dispatch control – Order level > <Shift> + <F4> Delivery date changes




                           Fig. G 62    Delivery date changes


                           This dialog displays all changes to delivery dates.
                           There is a detailed description in section:
                            Sales, “Delivery Date Change Log” on page D-178
2.00 / 2022-04




                 G - 118                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                                 Racks




                                        Dispatch Information
                                        Dispatch control – Order level > <Shift> + <F4> Dispatch information




                                        Fig. G 63    Dispatch Information


                                        On this dialog, you can assign an order a Dispatch type or change an already
                                        stored Dispatch type and store additional Dispatch information.
                                         "Dispatch Info I tab" on page G47

                                        Dispatch Type Dispatch type of the order. The possible dispatch types are
                                        stored in the master data (Keys > System > Dispatch > Dispatch Type). After
                                        saving and existing the dialog [[OK] button], the new dispatch type is taken
                                        over onto the Dispatch info tab.
                                        Technical info: Numeric field, <F9>, DB info: lapool.versandart

                                        Arrival Time The arrival time is taken over from the order if you are working
                                        with the via-Plant delivery. You can store the preliminary alternative Arrival
                                        time in this field. The value is taken over in the A.time field on the Delivery ad-
                                        dress tab.
                                         "Delivery Address tab" on page G45
                                        Technical info: alphanumeric field, DB field: lapool.ankunftszeit

                                        Private Long 1/2 Two private fields for the input of an alphanumeric value.
                                        The field names for these fields can be configured customer-specifically via
                                        environment variables.
                                        Technical info: Alphanumeric fields, DB info: lapool.private_long1, lapool.pri-
                                        vate_long2

                                        Private Char 1/2 Two private fields for the input of a numeric value. The field
                                        names for these fields can be configured customer-specifically via environ-
                                        ment variables.
                                        The information from the private fields is taken over onto the DispatchInfo II
                                        fields PL1/2, PC1/2 accordingly.
                                        Technical info: Alphanumeric fields, DB info: lapool.private_char1. lapool.pri-
                                        vate_char2
                                         "Dispatch Info II tab" on page G49
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                  G - 119
                 Racks                                                                 Software Reference




                           Via Details
                           Dispatch control – Order level > <Shift> + <F4> > Via details




                           Fig. G 64    Delivery details


                           This dialog is only available with a via-plant configuration and will not be de-
                           scribed further in this document.

                              via-plant configuration
                              The function scope via-plant is not part of this documentation. If necessary,
                              please request a detailed description from the responsible A+W employee.
2.00 / 2022-04




                 G - 120                                                A+W Enterprise Dispatch Control
                 Software Reference                                                                                  Racks




                                        Finished goods stock
                                        A picking stock for goods is called Finished stock if it is directly for delivery to
                                        the customer. The Finished stock provides an overview of the orders to be de-
                                        livered at any time. The use of the Finished stock function requires special
                                        configuration.
                                        The Finished stock function is not just linked to the Dispatch Control, but also
                                        in the purchasing goods receipts.
                                        The following dialogs for the Finished stock function are part of the document:
                                         "Finished goods stock" on page G122
                                         "Finished goods stock - overview" on page G123
                                         "Finished goods stock - inventory" on page G124
                                         "Close inventory" on page G124
                                         "Log" on page G125
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                   G - 121
                 Racks                                                                 Software Reference




                           Finished goods stock
                           Dispatch control - Tour/Order level > <Shift> + <F4> > Finished goods stock >
                           Finished goods stock




                           Fig. G 65    Finished goods on hand for ...


                           This dialog is used to enter the data for your search. The result of your search
                           appears in dialog Finished goods stock - overview. The overview shows the
                           orders yet to be shipped.

                           Site Site number or client number. Use <F9> to select the site number if you
                           are working with a multi-client system.
                           Technical info: Numeric field, <F9>, DB field: lapfertwb.orghnr

                           Order Order number. Use <F9> to search for an order. If you leave the Order
                           field empty, you get the Finished stock - overview for all orders. With the order
                           selection, you restrict this overview.
                           Technical info: Numeric field, <F9>, DB field: lapfertwb.auftrnr

                           Targ. Site Number of the target site or client.
                           Technical info: numeric field, <F9>, DB field: lapfertwb.zielhnr
2.00 / 2022-04




                 G - 122                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                               Racks




                                        Finished goods stock - overview
                                        Dispatch control - Tour/Order level > <Shift> + <F4> > Finished goods stock >
                                        Finished goods stock > Enter selection criteria




                                        Fig. G 66    Finished goods stock - overview


                                        This dialog provides the overview of the orders that are in the finished goods
                                        stock for delivery.

                                        Order Order number. If you have entered the Order field as a search criterion,
                                        only items for this order are displayed in this column.Technical info: Numeric
                                        field, <F9>, DB field: lapfertwb.auftrnr

                                        Itm Item number from the order.
                                        Technical info: Numeric field, <F9>, DB field: lapfertwb.posnr

                                        Qty Booked quantity.
                                        Technical info: numeric field, <F9>, DB field: lapfertwb.istmenge

                                        Site Site number or client number. Use <F9> to select the site number if you
                                        are working with a multi-client system.
                                        Technical info: Numeric field, <F9>, DB field: lafertwb.orghnr.

                                        TargSite Number of the target site or client. If the Target site field is already
                                        pre-populated, then this item is en route from the site (original site number) to
                                        the target site.Technical info: Numeric field, <F9>, DB field: lapfertwb.zielhnr


                                        Additional information
2.00 / 2022-04




                                         "Log" on page G125




                 A+W Enterprise Dispatch Control                                                                G - 123
                 Racks                                                                  Software Reference




                           Finished goods stock - inventory
                           Dispatch control - Tour/Order level > <Shift> + <F4> > Finished goods stock >
                           Finished goods stock inventory
                           Use this menu element to start the inventory of the finished stock, that is, the
                           current site is locked for the time of the inventory. During the inventory, no fin-
                           ished reports from production can be booked; they are kept in the queue by
                           the return server. After completion of the inventory, these bookings are made.


                           Close inventory
                           Dispatch control - Tour/Order level > <Shift> + <F4> > Finished goods stock >
                           Finished goods stock > Enter selection criteria > Close inventory
                           Use this menu element to close the inventory of the finished stock. All finished
                           reports from production are booked afterwards.
2.00 / 2022-04




                 G - 124                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                                 Racks




                                           Log
                                           Dispatch control - Tour/Order level > <Shift> + <F4> > Finished goods stock >
                                           Finished goods stock > Log




                 Fig. G 67   Finished goods stock - log


                                           This dialog shows the information from the booking log of the finished goods
                                           stock.

                                           Booking data

                                           Date Date of the booking made.
                                           Technical info: Display field, DB field: lapfertwbprot.datum

                                           Time Time of the booking.
                                           Technical info: Display field, DB field: lapfertwbprot.zeit

                                           Del. Date Date on which the order will be delivered to the customer. If this is
                                           a booking record that is not order-related, the date 31.12.1899 is displayed
                                           here.
2.00 / 2022-04




                                           Technical info: Display field, DB field: lapfertwbprot.ltplan




                 A+W Enterprise Dispatch Control                                                                  G - 125
                 Racks                                                                  Software Reference




                           Order Order number. If this is a booking record that is not order-related, the
                           order number -1 is displayed here.
                           Technical info: Display field, DB field: lapfertwbprot.auftrnr

                           Itm Item number. If this is a booking record that is not order-related, this field
                           remains empty.
                           Technical info: Display field, DB field: lapfertwbprot.posnr

                           Booked Booked quantity.
                           Technical info: display field, DB field: lapfertwbprot.menge

                           Site Site number or client number to which the booking is made.
                           Technical info: Display field, DB field: lapfertwbprot.orghnr

                           Targ Number of the target site or client. If the field is populated, then the book-
                           ing was made from the original site to the target site.
                           Technical info: Display field, DB field: lapfertwbprot.zielhnr

                           Booking type Booking type, e. g. check for missing quantities.
                           Technical info: display field, DB field: lapfertwbprot.buchtext

                           Employee Name of the employee who made the booking.
                           Technical info: Display field, DB field: lapfertwbprot.manr, mitarb.maname
2.00 / 2022-04




                 G - 126                                                 A+W Enterprise Dispatch Control
                 Software Reference                                                                               Racks




                                          Graphical Tour Overview
                                          Dispatch control - Data level > Overview (<Shift> + <F1>)




                 Fig. G 68   Graphical Tour Overview


                                          With the Overview (Shift + <F11>) function, which can be selected from the
                                          prompt line, you can get a graphical overview of the deliveries.
                                          Specify the X- and Y-axis for this graphical display with the following parame-
                                          ters:

                                          1st Parameter: Selection value for the Y-axis.
                                             • Piece
                                             • SF
                                             • Weight
                                          Use <Enter> to confirm the first selected parameter.

                                          2nd Parameter: Selection value for the X-axis.
                                            • Display all routes for the current tour day
                                            • Display next tour days for the current route
                                          Use <Enter> to confirm the second selected parameter and trigger the graphic
                                          display.
2.00 / 2022-04




                                          The title for the graphical tour overview is generated dynamically, depending
                                          on the parameters selected program-internally.




                 A+W Enterprise Dispatch Control                                                                G - 127
                 Print                                                                Software Reference




                           Print
                           The print functions can be started in various dialogs and views.
                           This section provides information on the following subjects:
                           •   "Print loading list" on page G129
                           •   "Print all loading lists" on page G130
                           •   "Print supplementary loading lists" on page G131
                           •   "Print list" on page G132
                           •   "Preliminary delivery note printing" on page G133
                           •   "Deliv./receipt release + print" on page G135
                           •   "Print format" on page G136
                           •   "Print format" on page G136

                               Configuration of the print area
                               Use of the print functions in Dispatch Control assumes that your system
                               has a complete configuration of the print area. For additional information,
                               please contact an A+Wemployee.
2.00 / 2022-04




                 G - 128                                                A+W Enterprise Dispatch Control
                 Software Reference                                                                                   Print




                                        Print loading list
                                        Dispatch control - Data level > <F4> > Print loading list




                                        Fig. G 69    Print dialog on


                                        It is only possible to print a loading list if it has already been created. You can
                                        make the following selection on this dialog:

                                        Printer selection Use <F9> to select the printer on which the loading list is
                                        printed. Printers must be configured on the system in advance (System >
                                        Printer Management > Setup Printer).
                                        Technical info: Numeric field, <F9>, DB field: drucker.drunr

                                        Number of Copies Number of copies to be printed.
                                        Technical info: Numeric field, without DB reference

                                        File Name If you want to write the loading list to a file (Printer Selection = File
                                        Print), then you have to enter a file name. This file created by printing is then
                                        in the pre-defined directory.

                                        Footer
                                        Shows the name of the selected or assigned list.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                  G - 129
                 Print                                                                  Software Reference




                           Print all loading lists
                           Dispatch control - Data level > <F4> > Print all loading lists




                           Fig. G 70    Selection dialog for loading list printing


                           Use this dialog to print all loading lists for the selected period at once.
                            "Print loading list" on page G129
                           The loading list printing is only possible if the loading lists have already been
                           created. Before you print the lists, make the following selection:

                           Site Number of the site for which the loading lists are printed.
                           Technical info: numeric field, DB field: lapool.hnr

                           frm, to Space of time for which the loading lists are printed.
                           Technical info: numeric field, DB field: lapoolll.ltplan
                           After this selection, the Printer selection dialog opens automatically:
                            "Printer selection" on page G136
2.00 / 2022-04




                 G - 130                                                    A+W Enterprise Dispatch Control
                 Software Reference                                                                                  Print




                                        Print supplementary loading lists
                                        Dispatch control - Data level > <F4> > Print supplementary loading lists




                                        Fig. G 71    Selection dialog for supplementary loading list printing


                                        This dialog is used to print supplementary loading lists. Supplementary loading
                                        lists must always be printed if changes were made in the order or in dispatch
                                        scheduling and there is already a loading list.

                                        Site Number of the site for which the loading lists are printed.
                                        Technical info: numeric field, DB field: lapool.hnr

                                        frm, to Space of time for which the loading lists are printed.
                                        Technical info: numeric field, DB field: lapoolll.ltplan
                                        After this selection, the Printer selection dialog opens automatically:
                                         "Printer selection" on page G136
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                  G - 131
                 Print                                                                  Software Reference




                           Print list
                           Dispatch control - Data level > <F4> > Print list




                           Fig. G 72      Print list


                           This dialog shows the user-defined lists available for printing. User-defined
                           lists (reports) are created individually on customer request. The figure in this
                           document is just an example.
                           After the selection of the desired lists, a dialog for entry of the required param-
                           eters may open. Depending on the list selected, the appropriate fields are
                           shown.

                              Example:

                              List name                          NDU label

                              Parameters                         •   Delivery date
                                                                 •   Route
                                                                 •   Order
                                                                 •   POSITION
                                                                 •   NVE number


                           After the value specification, the Printer Selection dialog opens automatically:
                            "Printer selection" on page G136
2.00 / 2022-04




                 G - 132                                                  A+W Enterprise Dispatch Control
                 Software Reference                                                                                   Print




                                        Preliminary delivery note printing
                                        Dispatch control - Order level > <F4> > Preliminary delivery note printing




                                        Fig. G 73    Preliminary delivery note for...


                                        On this dialog, you select for which document or documents you want to print
                                        preliminary delivery notes.
                                        With dialog start from an order level, this selection dialog is pre-populated with
                                        current values depending on dispatch mode between order the PO or goods
                                        receipt.
                                        On dialog start from the tour level, the Order field remains empty. If you leave
                                        the field empty, then after [Trigger], all preliminary delivery notes for this tour
                                        will be printed.
                                        Use <F3> or [Start] to start the printout.
                                         "Printer selection" on page G136
                                        Then the D checkbox for the affected documents is enabled.
                                         "Order Info tab" on page G39
                                        If only the preliminary note has been printed for an order, the order can still be
                                        changed in shipping control. If a delivery note has been printed for an order,
                                        the order cannot be changed any more in shipping control.
                                        A preliminary delivery note is no separate document in the database. The or-
                                        der status does not change because of a preliminary delivery note.

                                        Del. Date Delivery date for which the preliminary delivery note is issued.
                                        Technical info: numeric field, DB field: lapool.ltplan

                                        Route Number of the route for which the preliminary delivery note is issued.
                                        Technical info: numeric field, DB field: lapool.routenr
2.00 / 2022-04




                                        Order Number of the order for which the preliminary delivery note is issued.
                                        Technical info: numeric field, DB field: lapool.auftrnr




                 A+W Enterprise Dispatch Control                                                                  G - 133
                 Print                                                              Software Reference




                           L/L Loading/cargo list number of the order for which the preliminary delivery
                           note is issued.
                           Technical info: numeric field, DB field: lapool.llnr
2.00 / 2022-04




                 G - 134                                              A+W Enterprise Dispatch Control
                 Software Reference                                                                                 Print




                                        Deliv./receipt release + print
                                        Dispatch control - Order level > <F4> Delivery/receipt release + print




                                        Fig. G 74    Release delivery note for …


                                        Choose the order for which the delivery note shall be printed.
                                        When the final delivery note is printed, the shipping dates of the order cannot
                                        be changed any more. The new status is adopted for the order. This function
                                        can be configured so that the invoice is printed at the same time.

                                        Del. Date Delivery date for which the delivery note is printed.
                                        Technical info: numeric field, DB field: lapool.ltplan

                                        Route Number of the route for which the delivery note is printed.
                                        Technical info: numeric field, DB field: lapool.routenr

                                        Order Number of the order for which the delivery note is printed.
                                        Technical info: numeric field, DB field: lapool.auftrnr

                                        L/L Select the loading list for which the delivery note is printed.
                                        Technical info: numeric field, DB field: lapool.llnr

                                           Delivery notes in Dispatch Control
                                           Generally delivery notes are only created if the goods for delivery are re-
                                           ported finished in production and they have already been booked to trans-
                                           port. In case of a possible change of the workflow, contact the responsible
                                           A+W employee.
2.00 / 2022-04




                 A+W Enterprise Dispatch Control                                                                 G - 135
                 Print                                                                 Software Reference




                           Print format
                           Additional menu <F4> > Print preliminary delivery note > Enter data > [Start]




                           Fig. G 75    Printer format dialog


                           You enter the printer-related data on this dialog.

                           No. of copies Number of copies to be printed.
                           Technical info: Numeric field, without DB reference

                           Sorted by Sort sequence during printing. Possible values are:
                           • Orders
                           • Delivery note copies
                           Technical info: Numeric field, without DB reference


                           Printer selection
                           Menu <F4> > Delivery/receipt release + print [Start]




                           Fig. G 76    Print on dialog


                           Use this dialog to select the printer on which you would like to print.

                           Printer selection Printer number on which the previously selected document
                           is printed. Use <F9> to open the list with the available printers. Printers must
                           be configured on the system in advance (System > Printer Management < Set-
                           up Printer).
                           Technical info: Numeric field, <F9>, DB field: drucker.drunr

                           Number of Copies Number of copies to be printed.
                           Technical info: Numeric field, without DB reference

                           Footer
                           The footer displays the name of the form that will be printed, e.g. Loading list
2.00 / 2022-04




                           (Dispatch).




                 G - 136                                                A+W Enterprise Dispatch Control
Dispatch Control               G

                          Partindex




                   A+W Enterprise
                 Partindex                                                                                 Index




                 Index
                 A                                               E
                 Additional information                          Explorer
                 – Order G-51                                    – Function G-16
                 Address                                         – Overview G-16
                 – Search G-83                                   – Overview of delivery dates   G-15
                 – Select G-83
                                                                 F
                 B                                               Finished goods stock
                 Book                                            – Booking log G-125
                 – Missing quantity check G-76                   – Inventory, close G-124
                 – to transport G-78                             – Inventory, start G-124
                 Booking log                                     – Overview G-119
                 – Draw up, for packed quantity G-81             – Search G-121
                 – Finished goods stock G-125
                                                                 G
                 C                                               Go
                 Cancel                                          – Order, to   G-62
                 – Delivery note G-90
                 – Order G-91                                    I
                 – Shipping status G-93                          Info menu
                 – Transport booking G-79                        – Overview G-25
                                                                 Inventory
                 D                                               – close, for finished goods stock G-124
                 Delete                                          – Finished goods stock, start for G-124
                 – Tour lock G-86                                – Start, for finished goods stock G-124
                 Delivery date                                   Item
                 – Postpone G-64                                 – Item info I G-55
                 – Search G-11                                   – Item info II G-58
                 Delivery date level                             – move via filter function G-66, G-67, G-69
                 – Quick information G-17                        Item level
                 – Structure G-9                                 – Quick information G-21
                 Delivery dates                                  – Structure G-9
                 – Dispatch control, overview in G-15
                 Delivery note                                   L
                 – Cancel G-90                                   Levels
                 – Print G-136                                   – Structure G-9
                 – Release and print G-85, G-115, G-118, G-135   Loading list
                 Delivery receipt of goods                       – Print, one G-129
                 – Release and print G-85, G-115, G-118, G-135   – Print,all G-130
                 Dispatch control                                – Supplementary loading list G-129
                 – Delivery dates, overview for G-15             Lock
                 – Overview G-9                                  – Tour, all G-87
                 Dispatch info I                                 – Tour, one G-86
                 – Order, details on G-47                        Log
                 Dispatch info II
2.00 / 04-2022




                                                                 – Finished goods stock, book G-125
                 – Order, details on G-49




                 A+W Enterprise Versandsteuerung                                                          G-139
                 Index                                                                                      Partindex




                 M                                                   Q
                 Market partner                                      Quick information
                 – Search G-14                                       – Delivery date level G-17
                 Missing quantity check                              – Item level G-21
                 – Book G-76                                         – Order level G-20
                 – Execute G-75                                      – Route level G-19
                 Move
                 – Item, filter before moving   G-66, G-67, G-69     R
                                                                     Racks
                 O                                                   – Lite allocation G-108
                 Order                                               Release and print
                 – Additional information G-51                       – Delivery note G-85, G-115, G-118, G-135
                 – Cancel G-91                                       – Delivery receipt of goods G-85, G-115, G-118,
                 – Dispatch info I G-47                                G-135
                 – Dispatch info II G-49                             Route
                 – Go to… G-62                                       – Information, global G-111, G-113, G-120
                 – Information G-70, G-73, G-74                      Route level
                 – Information, global G-111, G-113, G-120           – Quick information G-19
                 – Order information G-39                            – Structure G-9
                 – Postpone G-64
                 – Search finished goods stock G-121                 S
                 – Search, extended G-13                             SA (sales)
                 – Shipping address G-45                             – Info (global), start search for G-98, G-100,
                 Order level                                           G-102, G-103, G-105, G-106
                 – Quick information G-20                            – Information, global G-111, G-113, G-120
                                                                     SA/PU
                 P                                                   – Info (global), start search for G-98, G-100,
                 Packed quantity                                       G-102, G-103, G-105, G-106
                 – correct G-81                                      – Information, global G-111, G-113, G-120
                 – Draw up booking log G-81                          Search
                 Postpone (dispatch)                                 – Address G-83
                 – Delivery date G-64                                – Delivery Date G-11
                 – Order G-64                                        – Extended order search G-13
                 – Tour G-64                                         – Finished goods stock, orders G-121
                 Preliminary delivery note                           – Market partner G-14
                 – Print G-136                                       – Order, go to G-62
                 – Printing, enter data for G-80, G-82, G-133        – SA/PU, information on G-98, G-100, G-102,
                 Print                                                 G-103, G-105, G-106
                 – Delivery note G-136                               – Shipping address G-83
                 – Loading list, one G-129                           Shift+F4
                 – Loading lists, all G-130                          – Lite rack allocation G-108
                 – Preliminary delivery note, enter data for G-80,   Shipping address
                   G-82, G-133                                       – Enter new G-84
                 – Print preliminary delivery note G-136             – Order G-45
                 – Supplementary loading list G-131                  – Search G-83
                 – User-defined lists G-132                          – Select G-83
                 PU (purchasing)                                     Shipping status
                 – Info (global), start search for G-98, G-100,      – Cancel G-93
                   G-102, G-103, G-105, G-106                        Start
2.00 / 04-2022




                 – Information, global G-111, G-113, G-120           – Inventory, finished goods stock G-124
                                                                     – Missing quantity check G-75
                                                                     Start functions


                 G-140                                                            A+W Enterprise Versandsteuerung
                 Partindex                                    Index




                 – Program start G-10
                 Stock picking
                 – Print picking list, information on G-89
                 – Stock withdrawal, information on G-89
                 Supplementary loading list
                 – Print G-131

                 T
                 Tour
                 – Delete lock G-86
                 – Lock, all G-87
                 – Postpone G-64
                 – Set lock G-86
                 – Tour info G-29, G-32
                 – View vehicle information G-34
                 Tour info
                 – Delivery Tour G-29, G-32
                 Tour level
                 – Structure G-9
                 Transport
                 – Book to G-78
                 – Cancel G-79
                 Transport data
                 – Enter G-88

                 U
                 User-defined lists
                 – Print G-132

                 V
                 Vehicle information
                 – Tour, for G-34
2.00 / 04-2022




                 A+W Enterprise Versandsteuerung             G-141
                 Index                          Partindex
2.00 / 04-2022




                 G-142   A+W Enterprise Versandsteuerung

