---
description: "EN AWEnterprise Purchasing"
---



# EN AWEnterprise Purchasing

Purchasing              E




                        English




             A+W Enterprise
                                                                                                                 Introduction




                                        Introduction
                                        This part of the documentation contains editorial notes.


                                        Revision Overview
                                        Part                       Descriptions
                                        Version / Date

                                        5.00 / 12-2022             Various additions to the software reference

                                        4.00 / 08-2020             Complete revision

                                        3.00 / 06-2019             Complete reworking

                                        2.01 / 01-2017             Product and company names adjusted.

                                        2.00 / 03-2014             Complete reworking

                                        1.00 / 02-2007             Original version



                                        Editorial
                                        The editorial provides information on the following topics:
                                        •    Notes on this document
                                        •    Copyrights
                                        •    Trademarks
                                        •    Contact

                                        Notes on this document
                                        This document is intended for end users of A+W Enterprise.
                                        The documentation and software described are licenses that must be used or
                                        copied only in accordance with the conditions of our license agreement. The
                                        contents of the documentation are only informative and are subject to changes
                                        without prior notice.
                                        The text and illustrations were compiled with the utmost care. Still, errors can-
                                        not be totally excluded. A+W Software GmbH cannot be held liable for errors
                                        or inaccuracies, unless they can be attributed to willful or grossly negligent ac-
                                        tion.
                                        The descriptions in this document are based on the full program level of
                                        A+W Enterprise.

                                        Copyrights
                                        © 2022, A+W Software GmbH, all rights reserved, also those for reprinting,
5.00 / 12-2022




                                        the making of copies and translation.
                                        The documentation may be copied, completely or in part, saved in an archiving
                                        system, or transferred in any other form only in accordance with our license

                 A+W Enterprise Purchasing                                                                              E-3
                 Introduction




                                agreement. Transmission of the documentation is not allowed, neither elec-
                                tronically, nor mechanically, nor by recording or in any other way, without
                                A+W Software GmbH's prior approval in writing.

                                Trademarks
                                All hardware and software names mentioned in this documentation can also
                                be registered trademarks or other property rights of third parties. Third party
                                copyrights must be observed.

                                Contact
                                A+W Software GmbH
                                Am Pfahlgraben 4-10
                                35415 Pohlheim
                                +49 6404 2051-0
                                +49 6404 2051 877
                                Zentrale@a-w.com
                                http://www.a-w.com
5.00 / 12-2022




                 E-4                                                              A+W Enterprise Purchasing
                                                                                                                                                        Contents




                                        Contents
                                        Introduction ............................................................................................................. E-3
                                          Revision Overview ............................................................................................... E-3
                                          Editorial ............................................................................................................... E-3
                                        Contents ................................................................................................................. E-5

                                        Software Reference                                                                                                   E-9
                                        Overview ............................................................................................................... E-11
                                          The Purchasing Menu ....................................................................................... E-11
                                            PO Pool Configuration ................................................................................... E-12
                                            Individual Purchasing Documents Configuration ........................................... E-12
                                            Receipt of Goods Submenu ........................................................................... E-13
                                            Invoices Submenu ......................................................................................... E-13
                                            Overview Submenu ........................................................................................ E-14
                                         Supplementary Menu ........................................................................................ E-15
                                            Prices Submenu ............................................................................................. E-16
                                            Order Prices Submenu .................................................................................. E-17
                                            Special Texts Submenu ................................................................................. E-17
                                            Product Details Submenu .............................................................................. E-17
                                            Technical Values Submenu ........................................................................... E-18
                                         Info Menu .......................................................................................................... E-19
                                            Notes Submenu ............................................................................................. E-20
                                         Goods Receipt Supplementary Menu ............................................................... E-21
                                            Receipt of Goods Supplementary Menu ........................................................ E-21
                                        Search Functions .................................................................................................. E-22
                                         Find Purchase Orders ....................................................................................... E-23
                                            Find Purchase Orders – Document Key ........................................................ E-23
                                            Find Purchase Orders – Item Code ............................................................... E-25
                                            Find Purchase Orders – Direct Search .......................................................... E-26
                                         Find Purchase Orders – Hit List ........................................................................ E-27
                                            Hit List – General ........................................................................................... E-28
                                            Hit List - Quantities ......................................................................................... E-30
                                            Hit List - GR Info ............................................................................................ E-31
                                            Hit List – Article .............................................................................................. E-32
                                            Hit List - Miscellaneous Tab ........................................................................... E-33
                                        Purchase Order Pool ............................................................................................ E-35
                                         Special Menus for the PO Pool ......................................................................... E-36
                                            Purchase Order Pool – Additional Menu ........................................................ E-36
                                            Purchase Order Pool – Menu Info ................................................................. E-37
                                         Creating Purchase Orders ................................................................................. E-38
                                            Create Purchase Orders – Supplier ............................................................... E-38
                                            Create Purchase Orders – Item ..................................................................... E-42
                                            Create Purchase Orders – Details ................................................................. E-43
                                        Document Management ....................................................................................... E-47
                                          Explanation of Symbols ..................................................................................... E-47
                                          Supplier Inquiries ............................................................................................... E-50
                                          Purchase Order Entry ........................................................................................ E-51
                                            Purchase Order Entry – Header, Footer ........................................................ E-52
                                            Purchase Order Entry – Addresses ............................................................... E-58
                                            Purchase Order Entry – Properties ................................................................ E-60
                                            Purchase Order Entry – Miscellaneous ......................................................... E-65
5.00 / 12-2022




                                            Purchase Order Entry - Totals ....................................................................... E-69
                                            Purchase Order Entry - Discounts Detailed View .......................................... E-70
                                          Purchase Order Items ....................................................................................... E-71
                                            Purchase Order Items - General .................................................................... E-72


                 A+W Enterprise Purchasing                                                                                                                      E-5
                 Contents




                                 Purchase Order Items - Properties ................................................................ E-81
                                 Purchase Order Items - Prices ....................................................................... E-84
                                 Purchase Order Items - Order Info ................................................................ E-87
                                 Purchase Order Items - Status ...................................................................... E-88
                                 Purchase Order Items - Evaluation ................................................................ E-91
                              Pick-up Address ................................................................................................ E-92
                              PO Type ............................................................................................................ E-95
                              Allocation of Document Types ........................................................................... E-96
                            Texts ..................................................................................................................... E-97
                              Order Texts ....................................................................................................... E-97
                            Form Printing ........................................................................................................ E-98
                            Purchase Order Release ...................................................................................... E-99
                              Purchase Order Release - Selection ................................................................. E-99
                                 Purchase Order Release – Details .............................................................. E-100
                                 Purchase Order Release - Additional Fields ................................................ E-102
                            Receipt of Goods ................................................................................................ E-104
                              Dispatch Notifications ...................................................................................... E-104
                                 Notifications – Overview .............................................................................. E-105
                                 Notifications – Details .................................................................................. E-107
                                 Purchase Order – Overview (Notification) ................................................... E-109
                                 Purchase Order – Details (Notification) ....................................................... E-110
                              Delivery Plan ................................................................................................... E-112
                                 Delivery Plan – Details ................................................................................. E-114
                              Receipt of Goods (Automatic) ......................................................................... E-115
                              Item Info .......................................................................................................... E-117
                              Booking Racks ................................................................................................ E-118
                              Receipt of Goods (Manual) ............................................................................. E-119
                              Rack-Related Receipt of Goods ...................................................................... E-121
                                 Rack-Related Receipt of Goods .................................................................. E-121
                                 Rack Load .................................................................................................... E-122
                              Check Receipt of Goods ................................................................................. E-124
                              Missing Quantities Check Pool ........................................................................ E-126
                                 Missing Quantities Check Pool - Overview .................................................. E-126
                                 Missing Quantities Check Pool – Details ..................................................... E-127
                              Receipt of Goods Log ...................................................................................... E-127
                            Invoices and Credit Notes ................................................................................... E-128
                              Invoice Check .................................................................................................. E-128
                                 Supplier’s Invoice – Purchase Overview ...................................................... E-129
                                 Supplier’s Invoice – Detailed View ............................................................... E-132
                                 Supplier’s Invoice – Item Overview .............................................................. E-133
                                 Supplier’s Invoice – Discounts ..................................................................... E-134
                              Supplier’s Invoice (Automatic) ......................................................................... E-135
                              Transferred Invoices ........................................................................................ E-137
                              Supplier's Invoice (Manual) ............................................................................. E-138
                              Supplier's Invoice (Collective Invoice) ............................................................. E-139
                              Booking of Invoices ......................................................................................... E-139
                              Close Purchase Orders ................................................................................... E-141
                              Invoice Log ...................................................................................................... E-142
                              Supplier's Credit Note ..................................................................................... E-142
                            Overviews ........................................................................................................... E-144
                              Document Information ..................................................................................... E-144
                              Overview of Documents .................................................................................. E-145
                              Purchase Search ............................................................................................. E-145
                                 Purchase Search – Search Mode ................................................................ E-146
5.00 / 12-2022




                                 Purchase Search – Overview ...................................................................... E-147
                                 Purchase Search – Details .......................................................................... E-149




                 E-6                                                                                        A+W Enterprise Purchasing
                                                                                                                                                        Contents




                                        Partindex                                                                                                      E-151
                                        Index ................................................................................................................... E-153
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                                                                      E-7
                 Contents
5.00 / 12-2022




                 E-8        A+W Enterprise Purchasing
Purchasing                  E

             Software Reference




             A+W Enterprise
                 Software Reference                                                                            Overview




                                        Overview
                                        In the Purchasing module, you manage the documents that are required for
                                        the successful processing of the purchasing business, such as purchase or-
                                        ders, inquiries, receipt of goods, and invoices.
                                        In the Purchasing part, you will find the following topics:
                                         “Search Functions” on page E-22
                                         “Document Management” on page E-47
                                         “Purchase Order Pool” on page E-35
                                         “Texts” on page E-97
                                         “Receipt of Goods” on page E-104
                                         “Invoices and Credit Notes” on page E-128
                                         “Overviews” on page E-144



                                        The Purchasing Menu
                                        Some of the available menu entries branch out to submenus. If these include
                                        more than three entries, they are listed separately according to the following
                                        overview.
                                        The displayed entries depend on the respective configuration.
                                        •    PO Pool Configuration
                                        •    Configuration Order-Oriented PO Printing - this configuration is not used.
                                             That's why it will not be described here.
                                        •    Individual Purchasing Documents Configuration
                                        For customer-specific adjustments, contact your contact person at A+W Soft-
                                        ware GmbH.

                                             Context menus
                                             On the context menus (right mouse button), only the menu elements are
                                             offered that make sense in the context for the individual fields of the dia-
                                             logs. You can also call up the functions on the context menus via the menus
                                             described. Generally, the menu elements on the context menu correspond
                                             to the functions offered on the prompt display.

                                        You can reach all dialogs and functions relating to sales via the Purchasing
                                        menu:
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                          E-11
                 Overview                                                                                  Software Reference




                                             PO Pool Configuration
                                             The purchasing configuration PO Pool includes the most-used settings. The
                                             explanations, examples, and other notes in this document are based, insofar
                                             as nothing else explicit is mentioned, on this configuration.


                  Shortcut   Entry                                Description

                        a    Create P.O.s                          “Creating Purchase Orders” on page E-38

                        b    Inquiries                             “Supplier Inquiries” on page E-50

                        c    PO management                         “Purchase Order Entry” on page E-51

                        d    Form

                    da       • Print                               Sales, “Form Printing” on page D-361

                    db       • E-Mail/Fax                          Sales, “E-mail” on page D-365

                        e    List printing                         Sales, “List Printing” on page D-368

                        f    P.O. release                          “Purchase Order Release” on page E-99

                        g    Dispatch notifications                “Dispatch Notifications” on page E-104

                        h    Receipt of goods                      “Receipt of Goods Submenu” on page E-13

                        i    Invoices                              “Invoices Submenu” on page E-13

                        j    Credit notes

                    ja       • Enter credit notes                  “Supplier's Credit Note” on page E-142

                    jb       • Book credit notes                   Sales, “Book Credit Notes” on page D-358

                        k    Overview                              “Overview Submenu” on page E-14

                        l    Search                                “Purchase Search” on page E-145



                                             Individual Purchasing Documents Configuration

                  Shortcut   Entry                                Description

                        a    Generate stock order                  “Creating Purchase Orders” on page E-38

                        b    Enter and edit inquiries              “Supplier Inquiries” on page E-50

                        c    Enter and edit purchase orders        “Purchase Order Entry” on page E-51

                        e    Manage form printing                  Sales, “Form Printing” on page D-361

                        e    Manage list printing                  Sales, “List Printing” on page D-368

                        f    Release and manage several POs        “Purchase Order Release” on page E-99

                        g    Release and manage individual POs     “Purchase Order Release” on page E-99
5.00 / 12-2022




                        h    Enter and manage delivery             “Dispatch Notifications” on page E-104
                             confirmations



                 E-12                                                                          A+W Enterprise Purchasing
                 Software Reference                                                                                   Overview




                  Shortcut   Entry                                 Description

                     i       Manage receipt of goods                “Receipt of Goods Submenu” on page E-13

                     j       Enter and edit invoices                “Invoices Submenu” on page E-13

                    ka       Enter supplier credit notes            “Supplier's Credit Note” on page E-142

                    kb       Book credit notes                      Sales, “Book Credit Notes” on page D-358

                     l       Display document overviews             “Overview Submenu” on page E-14

                     p       Search documents in purchasing         “Purchase Search” on page E-145



                                             Receipt of Goods Submenu
                                             Purchase > Goods Receipt
                                             Use this menu to access the dialogs on which you manage the receipt of
                                             goods.


                  Shortcut   Entry                                 Description

                    ha       Delivery plan                          “Delivery Plan” on page E-112

                    hb       Automatic receipt of goods             “Receipt of Goods (Automatic)” on page E-115

                    hc       Manual receipt of goods                “Receipt of Goods (Manual)” on page E-119

                    hd       Rack-related receipt of goods          “Rack-Related Receipt of Goods” on page E-121

                    he       Close purchase orders                  “Receipt of Goods” on page E-104

                    hf       Check receipt of goods                 “Check Receipt of Goods” on page E-124

                    hg       Missing quantities check pool          “Missing Quantities Check Pool” on page E-126

                    hh       Log                                    “Invoice Log” on page E-142



                                             Invoices Submenu
                                             Purchase > Invoices
                                             Use this menu to access the dialogs on which you manage purchase invoices.


                  Shortcut   Entry                                 Description

                    ia       Invoice check                          “Invoice Check” on page E-128

                    ib       Automatic invoices                     “Supplier’s Invoice (Automatic)” on page E-135

                     ic      Invoices transferred                   “Transferred Invoices” on page E-137

                    id       Manual invoices                        “Supplier's Invoice (Manual)” on page E-138
5.00 / 12-2022




                    ie       Collective invoices                    “Supplier's Invoice (Collective Invoice)” on page E-139

                     if      Booking of invoices                    “Booking of Invoices” on page E-139




                 A+W Enterprise Purchasing                                                                               E-13
                 Overview                                                                                 Software Reference




                  Shortcut   Entry                                  Description

                    ig       Close purchase orders                   “Receipt of Goods” on page E-104

                    ih       Log                                     “Invoice Log” on page E-142



                                            Overview Submenu
                                            Purchase > Overview
                                            Use this menu to access the dialogs on which you can display overviews of
                                            the various documents.


                  Shortcut   Entry                                  Description

                    ka       Receipt of goods today                  “These overview depend on the configuration and must be
                                                                      released separately. These dialogs can be designed cus-
                                                                      tomer-specifically if necessary. Please contact a service
                                                                      employee of A+W Software GmbH” on page E-145

                    kb       Delayed receipt of goods                “Overview of Documents” on page E-145

                    kc       Scheduled receipt of goods from – to    “Overview of Documents” on page E-145

                    kd       Delivered – but not invoiced            “Overview of Documents” on page E-145

                    ke       Invoiced – but not booked               “Overview of Documents” on page E-145

                    kf       Purchase orders not transferred yet:    “Overview of Documents” on page E-145

                    kg       Search document                         Sales, “Search Document” on page D-384

                    kh       Purchase information                    “Document Information” on page E-144
5.00 / 12-2022




                 E-14                                                                            A+W Enterprise Purchasing
                 Software Reference                                                                                   Overview




                                               Supplementary Menu
                                               The supplementary menu can be called up with <F4> for entering various doc-
                                               uments, e.g. for a purchase order.
                                               The entries on the supplementary menu are displayed in context-dependent
                                               versions.
                                               •   Supplementary menu for the header and footer area
                                               •   Supplementary menu for the item area

                                               Supplementary menu for the header and footer area

                  Shortcut   Entry                                  Description

                     a       Text

                    aa       • Header text                           Sales, “Header and Footer Texts” on page D-256

                    ab       • Footer text                           Sales, “Header and Footer Texts” on page D-256

                    ac       • External information                  Sales, “External Information” on page D-262

                     b       Addresses

                    ba       • Find delivery addresses               Sales, “Find Addresses” on page D-49

                    bb       • New shipping address                  Sales, “New Delivery Address” on page D-141

                    bc       • Delete delivery address              Deletes the delivery address from the document.

                    bd       • Pick-up address                       “Pick-up Address” on page E-92

                     c       Cancel                                  “PO Type” on page E-95

                     d       Prices                                  “Prices Submenu” on page E-16

                     e       Product details

                    ea       • Product exchange                      “PO Type” on page E-95

                    eb       • E/A rules                             Stammdaten, “Austausch-/Zusatzregel” auf Seite J-102

                     f       Resubmission                            Sales, “Resubmission” on page D-402

                     g       Configurable fields                     Sales, “Configurable Fields” on page D-149


                                               Supplementary menu for the item area

                  Shortcut   Entry                                  Description

                     a       Texts

                    aa       • Header text                           Sales, “Header and Footer Texts” on page D-256

                    ab       • Footer text                           Sales, “Header and Footer Texts” on page D-256
5.00 / 12-2022




                    ac       • External information                  Sales, “External Information” on page D-262

                    ad       • Article text                          Sales, “Article and Item Texts” on page D-258



                 A+W Enterprise Purchasing                                                                               E-15
                 Overview                                                                                    Software Reference




                  Shortcut    Entry                                   Description

                     ae       • Item text                              Sales, “Article and Item Texts” on page D-258

                     af       • Special texts                          “Prices Submenu” on page E-16

                        b     Addresses

                     ba       • Find delivery addresses                Sales, “Find Addresses” on page D-49

                     bb       • New shipping address                   Sales, “New Delivery Address” on page D-141

                     bc       • Delete delivery address               Deletes the delivery address from the document.

                     bd       • End customer address                   Sales, “End customer address” on page D-143

                        c     Cancel                                   “PO Type” on page E-95

                        d     Private fields                           Sales, “Private Fields” on page D-168

                        e     Prices                                   “Prices Submenu” on page E-16

                        f     Product details                          “Product Details Submenu” on page E-17

                        g     Resubmission                             Sales, “Resubmission” on page D-402

                        h     Reference

                     ha       • New reference                          “Purchase Order Items - General” on page E-72

                     hb       • Change reference                       “Purchase Order Items - General” on page E-72

                        i     Delivery Plan                            Sales, “Deliv. Plan” on page D-329

                        j     Warehouse

                     ja       • Stack                                  “Purchase Order Items - General” on page E-72

                     jb       • Stock forecast                         Sales, “Stock Forecast” on page D-154

                        h     Configurable fields                      Sales, “Configurable Fields” on page D-149



                                                Prices Submenu
                                                <F4> > Price info
                                                Use this menu to manage the prices and conditions for the article of the
                                                marked item.


                  Shortcut    Entry                                   Description

                        a     Order conditions                         Sales, “Conditions for PCD Processing” on page D-283

                        b     Order prices                             “Order Prices Submenu” on page E-17

                        c     Partial calculation                      Sales, “Production Cost Calculation” on page D-315

                 The following entries are only displayed in the item area:
5.00 / 12-2022




                        d     Item conditions                          Sales, “Conditions for PCD Processing” on page D-283




                 E-16                                                                              A+W Enterprise Purchasing
                 Software Reference                                                                                      Overview




                  Shortcut    Entry                                   Description

                      e       Load conditions                         Determine the sales price with the item conditions and
                                                                      recalculate the price.

                      f       Price calculation                       Recalculate the item price.


                      g       Price check                              “Purchase Order Items - General” on page E-72



                                               Order Prices Submenu
                                               <F4> > Price Info> Order Prices
                                               Use this menu to manage the order prices.


                  Shortcut    Entry                                   Description

                      a       Article prices                           Sales, “Order Prices” on page D-271

                      b       Muntin prices                            Sales, “Order Muntin Prices” on page D-273

                      c       Exchange prices                          Sales, “Order Exchange Prices” on page D-276

                      d       Sub-element prices                       Sales, “Order Sub-part Prices” on page D-278



                                               Special Texts Submenu
                                               <F4> > Texts > Special Texts
                                               Use this menu to manage all special texts that you can assign to the docu-
                                               ment. These texts can generally be configured customer-specifically and are
                                               therefore not part of this documentation.
                                               For customer-specific adjustments, contact your contact person at A+W Soft-
                                               ware GmbH.


                                               Product Details Submenu
                                               <F4> > Product Details
                                               Use this menu to manage the details for the products, e.g. exchange and ad-
                                               ditional rules.


                  Shortcut    Entry                                   Description

                      a       Product exchange                         “PO Type” on page E-95

                      b       E/A rules                                Master Data, “Exchange/Additional Rules” on page B-209

                 The following entries are only displayed in the item area:

                      c       Product group                            “Purchase Order Items - General” on page E-72
5.00 / 12-2022




                      d       Technical values                         “Technical Values Submenu” on page E-18




                 A+W Enterprise Purchasing                                                                                     E-17
                 Overview                                                                              Software Reference




                                           Technical Values Submenu
                                           <F4> > Product Details > Technical Values
                                           Use this menu to manage the technical values.


                 Shortcut   Entry                              Description

                        a   Show technical details             Show the technical values.

                        b   Change technical values            Switches to the technical values so that they can be edited.
                                                               The cursor changes to the db value field of the technical
                                                               values on the Items tab.

                        c   Declaration of performance          Sales, “Texts” on page E-97

                        d   Show hidden dimensions             Shows the hidden dimensions on the Items tab.

                        e   Change hidden dimensions            Sales, “Article Dimensions” on page D-153
5.00 / 12-2022




                 E-18                                                                        A+W Enterprise Purchasing
                 Software Reference                                                                                    Overview




                                             Info Menu
                                             <Shift> + <F4>
                                             The info menu is displayed in context-dependent forms:
                                             •   Info menu for the header and footer area
                                             •   Info menu for the item area

                                             Info menu for the header and footer area

                  Shortcut   Entry                                  Description

                     a       Document notes                          Sales, “Notes” on page D-247
                     b       Market partner notes
                     c       Project notes

                     d       Search document                         Sales, “Search Document” on page D-384

                     e       Document overview                       Sales, “Overview” on page D-150

                     f       Market partner information              Sales, “Market Partner Info” on page D-145

                     g       Change log                              Sales, “Amendment Log” on page D-176

                     h       Delivery plan                           “Delivery Plan” on page E-112

                     i       Delivery date changes                   Sales, “Delivery Date Change Log” on page D-178

                     j       Receipt of goods today                  “These overview depend on the configuration and must be
                                                                      released separately. These dialogs can be designed cus-
                                                                      tomer-specifically if necessary. Please contact a service
                                                                      employee of A+W Software GmbH” on page E-145

                     k       Delayed receipt of goods                “Overview of Documents” on page E-145

                     l       Scheduled receipt of goods from – to    “Overview of Documents” on page E-145

                     p       Delivered – but not invoiced            “Overview of Documents” on page E-145

                     n       Invoiced – but not booked               “Overview of Documents” on page E-145

                     o       Rack management                         “Booking Racks” on page E-118

                     p       Delivery date                          Displays the following information from the customer order
                                                                    for order-related POs:
                                                                    - Order number
                                                                    - Delivery date
                                                                    - Route

                     r       Purchase information                    “Document Information” on page E-144


                                             Info menu for the item area

                  Shortcut   Entry                                  Description
5.00 / 12-2022




                     a       Notes                                   Notes Submenu

                     b       Search document                         Sales, “Search Document” on page D-384


                 A+W Enterprise Purchasing                                                                                 E-19
                 Overview                                                                                 Software Reference




                  Shortcut   Entry                                 Description

                        c    Document overview                      Sales, “Overview” on page D-150

                        d    Market partner information             Sales, “Market Partner Info” on page D-145

                        e    Change log                             Sales, “Amendment Log” on page D-176

                        f    Delivery plan                          “Delivery Plan” on page E-112

                        g    Rack management                        “Booking Racks” on page E-118

                        h    Note                                   “Purchase Order Items - General” on page E-72

                        i    Delivery date                         Displays the following information from the customer order
                                                                   for order-related POs:
                                                                   - Order number
                                                                   - Delivery date
                                                                   - Route

                        j    Purchase information                   “Document Information” on page E-144



                                              Notes Submenu
                                              <Shift> + <F4> > Notes
                                              The Notes info menu is only displayed on the PO Management – Items tab.
                                              In the PO header, you open the existing Notes directly via the info menu
                                              <Shift> + <F4>.


                  Shortcut   Entry                                 Description

                        a    Document notes                         Sales, “Notes” on page D-247
                        b    Supplier notes
                        c    Supplier article notes
                        d    Project notes
                        e    Project article notes
                        f    Customer notes
                        g    Customer article notes
5.00 / 12-2022




                 E-20                                                                           A+W Enterprise Purchasing
                 Software Reference                                                                                  Overview




                                           Goods Receipt Supplementary Menu
                                           On the dialogs with automatic data processing, such as Receipt of goods,
                                           Supplier invoice, Close POs, you can use <F4> to call up the dialog-specific
                                           additional menu. The entries displayed are optional depending on the dialog
                                           from which the menu was called. The following overview of the menus always
                                           lists all entries.

                                                Context menus
                                                On the context menus for the individual fields of the dialog, only the menu
                                                elements are offered that make sense in the context. The functions corre-
                                                spond to the functions that you call up via the menus described below.


                                           Receipt of Goods Supplementary Menu
                                           Purchase > Receipt of Good > Automatic Receipt of Goods> <F4>


                 Shortcut Entry                                   Description

                     a    Tag (downwards) (Shift+F9)              Enables the Cr. (Create) checkboxes for the selected and all
                                                                  following POs.

                     b    Tag (all) (Ctrl+F9)                     Enables the Cr. (Create) checkbox for all POs.

                     c    Import values (Ctrl+F8)                 Opens a dialog for specifying a time period and imports all
                                                                  non-booked POs with a delivery date within the specified time
                                                                  period. The hit list also displays future deliveries.

                     d    Supplier evaluation (Ctrl+N)            At present, this menu entry is not supported.

                     e    Check receipt of goods (Shift+F10)      After the successful check of the receipt of goods, it is
                                                                  possible to enable the Chk. checkbox by calling this menu
                                                                  element or using the key combination.

                     f    Status check from current record        Enables the Chk. (Check) checkboxes for the selected and all
                          (Shift+F11)                             subsequent POs.

                     g    Status check all records (Ctrl+F11)     Enables the Chk. (Check) checkbox for all POs.

                     h    Rack management (Ctrl+G)                Opens the dialog Book racks.
                                                                   “Rack-Related Receipt of Goods” on page E-121

                     i    Note (Ctrl+B)                           Displays the Note column in which you can specify additional
                                                                  information about the PO.
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                                E-21
                 Search Functions                                                             Software Reference




                                    Search Functions
                                    In the Purchase module, you can search via various categories for documents,
                                    market partners, addresses, articles, and projects.
                                    The search dialogs are structured the same way for all document types in Pur-
                                    chasing. Operation of the search dialogs has been developed analog to pur-
                                    chasing. In these instructions, the search functions are described using the
                                    example of POs. Deviations from other dialogs and from Sales are mentioned
                                    explicitly.
                                    The following dialogs are described in this section:
                                     “Find Purchase Orders” on page E-23
                                     “Find Purchase Orders – Hit List” on page E-27
                                    Additional search dialogs are the same in Purchasing and Sales. They are de-
                                    scribed in detail in the Sales section:
                                     Sales, “Find Reference Document” on page D-47
                                     Sales, “Find Market Partner” on page D-41
                                     Sales, “Find Addresses” on page D-49
                                     Sales, “Find Article” on page D-51
                                     Sales, “Find Article by Types” on page D-61
                                     Sales, “Find Product by Element” on page D-62
                                     Sales, “Find Project” on page D-69
5.00 / 12-2022




                 E-22                                                                  A+W Enterprise Purchasing
                 Software Reference                                                                    Search Functions




                                         Find Purchase Orders
                                         Purchase > Inquiries > <F9> > Enter Search Criteria > <F3>
                                         Use this dialog to find purchase orders.
                                         Specify the search criteria in the header area. The hits for the search are dis-
                                         played on the tabs.
                                         •   Use <F2> to change to the header area of the tab.
                                         •   Use <F3> to start the search.
                                         •   Use <F2> to change tabs on the hit list.
                                         This dialog contains the following tabs in the header area:
                                          “Find Purchase Orders – Document Key” on page E-23
                                          “Find Purchase Orders – Item Code” on page E-25
                                          “Find Purchase Orders – Direct Search” on page E-26
                                         The search results are shown in the hit list:
                                          “Find Purchase Orders – Hit List” on page E-27


                                         Find Purchase Orders – Document Key
                                         Purchase > Inquiries, P.O. Management> <F9>




                 Fig. E-1   Find orders – document key


                                         You can search for purchase orders on this tab using delivery data.
                                         •   Use <F2> to change to the header area of the tab.
                                         •   Use <F3> to start the search.
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                         E-23
                 Search Functions                                                               Software Reference




                                    Document key

                                    P.O. From Number starting from which purchase orders are searched for.
                                    The field name varies depending on the dialog from which you open the
                                    search, e.g. Inquiries from.
                                    Technical info: numeric field, DB field: kauf.auftrnr

                                    Supplier Supplier number. If you specify a number, the supplier name is dis-
                                    played in plain text.
                                    Technical info: numeric field, display field, DB fields: kauf.kunr

                                    Ext. No. Order number from Purchasing that is specified by the customer.
                                    The number is specified if the PO is entered with reference. Depending on the
                                    configuration, alternative data can be displayed. The alternative data is de-
                                    scribed for the Purchase Order Entry dialog:
                                     “Cust. Order” on page E-54
                                    Technical info: alphanumeric field, DB field: kauf.exaufnr
                                    If the field includes alphanumeric characters, then capitalization must be heed-
                                    ed for the search. However, using an environment variable, you can enable the
                                    search for alphanumeric characters regardless of capitalization.

                                    Input Date Date when the purchase order was released.
                                    Technical info: date field, DB field: kauf.bdat

                                    Site Number Number of site. By default, the own site number is selected. The
                                    field can only be edited if you ware working with internal site separation.
                                    Technical info: numeric field, DB field: xhaus.haus

                                    Customer Customer number. If you specify a number, the customer name is
                                    displayed in plain text.
                                    Technical info: numeric field, display field, DB field: kauf.orgkunr, kauf.or-
                                    gname

                                    Input Date Date of document entry.
                                    Technical info: date field, DB field: kauf.edat

                                    Entered by Employee number of the person who entered the document. If
                                    you specify a number, the name of the employee is displayed in plain text.
                                    Technical info: numeric field, DB field: kauf.eusr

                                    Invoice No. Number of the supplier invoice.
                                    Technical info: numeric field, DB field: kauf.rechnr

                                    VAT ID No. Supplier's VAT ID number.
                                    Technical info: alphanumeric field, DB field: kaufp.steuernr

                                    Hit list
5.00 / 12-2022




                                    The hit list displays the result of the search. It is structured the same way for
                                    all tabs in the header area:
                                     “Find Purchase Orders – Hit List” on page E-27


                 E-24                                                                  A+W Enterprise Purchasing
                 Software Reference                                                                     Search Functions




                                         Find Purchase Orders – Item Code
                                         Purchase > P.O. Management> <F9> > Tab Item Code




                 Fig. E-2   Find purchase orders – item code


                                         You can search for purchase orders on this tab using item codes.
                                         •   Use <F2> to change to the header area of the tab.
                                         •   Use <F3> to start the search.

                                         Item key
                                         You can search for the POs using the data from the items. For this search, en-
                                         ter the values you know. The following fields are available for entry:

                                         Suppl. OC Number of order confirmation from supplier.
                                         Technical info: numerical field, DB field: bpos.abnr

                                         DN No. Delivery note number of supplier.
                                         Technical info: numerical field, DB field: bpos.lieferschein

                                         Remark Text field for an item-related remark that you can enter in the dialog
                                         Supplier inquiries > P.O. info tab > Remark field related to the item.
                                         Technical info: alpha-numerical field, DB field: bpos.bemerkung

                                         Order No. Order number for order-related purchase orders.
                                         Technical info: numerical field, DB field: bpos.vksuftrnr

                                         Delivery date Planned delivery date starting on which POs will be searched
5.00 / 12-2022




                                         for.
                                         Technical info: Date field, DB field: bpos.ltplan




                 A+W Enterprise Purchasing                                                                         E-25
                 Search Functions                                                                    Software Reference




                                         Project Project number. If you specify a number, the project name is dis-
                                         played in plain text.
                                         Technical info: numeric field, display field, DB field: bpos.vkobjnr

                                         Article Article number. If you specify a number, the article name is displayed
                                         in plain text.
                                         Technical info: numeric field, DB field: kpos.artnr

                                         QU Quantity unit for the item, e.g. square meter.
                                         Technical info: numeric field, DB field: kpos.me

                                         Stock Stock number for the purchase order. If you specify a number, the
                                         warehouse name is displayed in plain text.
                                         Technical info: numeric field, DB field: bpos.lnr

                                         Dim. Variant Dimensional variant of the article.
                                         Technical info: numeric field, DB field: kpos.var

                                         Hit list
                                         The hit list displays the result of the search. It is structured the same way for
                                         all tabs in the header area:
                                          “Find Purchase Orders – Hit List” on page E-27


                                         Find Purchase Orders – Direct Search
                                         Purchase > P.O. Management> <F9> > Tab Direct Search




                 Fig. E-3   Find purchase orders – direct search
5.00 / 12-2022




                 E-26                                                                        A+W Enterprise Purchasing
                 Software Reference                                                                    Search Functions




                                        On this tab, you search for POs starting from a particular PO number. Thanks
                                        to a system configuration, it is possible to configure this tab as start dialog to
                                        use a simple search.
                                        •    Use <F2> to change to the header area of the tab.
                                        •    Use <F3> to start the search.

                                        P.O. From Number starting from which purchase orders are searched for.
                                        The field description varies depending on the dialog from which you open the
                                        search, e.g. Inquiries from.
                                        Technical info: numeric field, DB field: kauf.auftrnr

                                        Hit list
                                        The hit list displays the result of the search. It is structured the same way for
                                        all tabs in the header area:
                                         “Find Purchase Orders – Hit List” on page E-27



                                        Find Purchase Orders – Hit List
                                        Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3>
                                        The hit list contains the following tabs:
                                         “Hit List – General” on page E-28
                                         “Hit List - Quantities” on page E-30
                                         “Hit List - GR Info” on page E-31
                                         “Hit List – Article” on page E-32
                                         “Hit List - Miscellaneous Tab” on page E-33
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                          E-27
                 Search Functions                                                                        Software Reference




                                           Hit List – General
                                           Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3> > Gen-
                                           eral Tab




                 Fig. E-4   Hit list (find purchase orders) – general


                                           This tab displays general information about the purchase orders that fits the
                                           search criteria.
                                           Use <F2> to change tabs on the hit list.

                                               Show record
                                               At the right top of the dialog frame, the record display is offered: e. g.: Doc-
                                               ument overview: 137:227.
                                               137 = the record number of the selected line in the hit list
                                               227 = the number of records in the hit list.

                                           Header
                                           The fields in the header area are described for the Find Purchase Orders dia-
                                           log:
                                            “Find Purchase Orders” on page E-23

                                           General tab
                                           •   Site:
                                               Site number of the respective purchase order.
                                               Technical info: display field, DB field: kauf.hausnr
                                           •   P-Order No.:
                                               Purchase order number. The column name varies depending on the dialog
5.00 / 12-2022




                                               from which you open the search.
                                               Technical info: display field, DB field: kauf.auftrnr



                 E-28                                                                           A+W Enterprise Purchasing
                 Software Reference                                                                    Search Functions




                                        •    SubNo:
                                             Number of the partial delivery note or partial invoice.
                                             Technical info: display field, DB field: kauf.subnr
                                        •    Supplier:
                                             Name of the supplier.
                                             Technical info: display field, DB field: mp.name
                                        •    VAT ID No..:
                                             Supplier's VAT ID number.
                                             Technical info: display field, DB field: kaufp.steuernr
                                        •    Invoice:
                                             Number of the supplier invoice.
                                             Technical info: display field, DB field: kauf.rechnr
                                        •    Ordered:
                                             Date when the purchase order was released.
                                             Technical info: display field, DB field: kauf.bdat
                                        •    Entered:
                                             Date of the purchase order entry.
                                             Technical info: display field, DB field: kauf.edat
                                        •    Operator:
                                             Name of the person who entered this order.
                                             Technical info: display field, DB field: kauf.eusr
                                        •    Cancelled:
                                             Specification of the processing state, e.g. cancellation status.
                                             – 0: Order not cancelled.
                                             – 1: Order cancelled by the operator.
                                             – 2: Order cancelled by the system.
                                             – -3, -10, …, -x: Order in background processing.
                                             Technical info: display field, DB field: kauf.still
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                        E-29
                 Search Functions                                                                      Software Reference




                                           Hit List - Quantities
                                           Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3> > Quan-
                                           tities Tab




                 Fig. E-5   Hit list (find purchase orders) - quantities


                                           This tab displays item information about the ordered articles and the quantities
                                           that fit the search criteria. One line is displayed per article order item.
                                           Use <F2> to change tabs on the hit list.

                                           Header
                                           The fields in the header area are described for the Find Purchase Orders dia-
                                           log:
                                            “Find Purchase Orders” on page E-23

                                           Quantities tab
                                           The columns are described for the General tab:
                                            “General tab” on page E-28
                                           In addition, the following columns are displayed:
                                           •   Itm:
                                               Item number in the purchase order.
                                               Technical info: display field, DB field: kpos.posnr
                                           •   ArtNo, Article:
                                               Article number and article name.
                                               Technical info: display fields, DB fields: kpos.artnr, kpos.artbez1
5.00 / 12-2022




                                           •   Qty:
                                               Ordered quantity of the item.
                                               Technical info: display field, DB field: kpos.menge



                 E-30                                                                          A+W Enterprise Purchasing
                 Software Reference                                                                      Search Functions




                                           •   Receipt:
                                               Quantity received in receipt of goods.
                                               Technical info: display field, DB field: kpos.geslief
                                           •   Compl.:
                                               An asterisk * indicates if the item has been delivered completely.
                                               Technical info: display field
                                           •   Invcd:
                                               Invoiced quantity of the item.
                                               Technical info: display field, DB field: kpos.gesberech
                                           •   C:
                                               An C indicates if the item has been invoiced completely.
                                               Technical info: display field
                                           •   Width, Height:
                                               Sizes of the item in millimeters.
                                               Technical info: display fields: DB fields: kpos.laenge, kpos.breite


                                           Hit List - GR Info
                                           Purchase > P.O. Management> <F9> > Enter Search Criteria > <F3> > Tab
                                           GR Info




                 Fig. E-6   Hit list - Goods receipt info


                                           This tab displays receipt of goods information about the purchase orders. One
                                           line is displayed per purchase order item.
                                           Use <F2> to change tabs on the hit list.

                                           Header
5.00 / 12-2022




                                           The fields in the header area are described for the Find Purchase Orders dia-
                                           log:
                                            “Find Purchase Orders” on page E-23


                 A+W Enterprise Purchasing                                                                           E-31
                 Search Functions                                                                     Software Reference




                                           GR info tab
                                           The columns are described for the General and Quantities tab:
                                            “Hit List – General” on page E-28
                                            “Hit List - Quantities” on page E-30
                                           In addition, the following columns are displayed:
                                           •   Deliv.Date:
                                               Planned date of delivery starting on which POs will be searched for.
                                               Technical info: display field, DB field: bpos.ltplan
                                           •   OC No.Suppl.:
                                               Number of order confirmation from supplier.
                                               Technical info: display field, DB field: bpos.abnr
                                           •   Deliv.Note:
                                               Delivery note number of supplier.
                                               Technical info: display field, DB field: bpos.lieferschein
                                           •   Order:
                                               Order number for order-related purchase orders.
                                               Technical info: display field, DB field: bpos.vksuftrnr
                                           •   Delivery:
                                               Planned delivery date of the customer order.
                                               Technical info: display field, DB field: bpos.ltplan


                                           Hit List – Article
                                           Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3> > Article
                                           Tab




                 Fig. E-7   Hit list (find purchase orders) - article
5.00 / 12-2022




                                           This tab displays information about the article properties of the PO items. One
                                           line per PO item is displayed.


                 E-32                                                                          A+W Enterprise Purchasing
                 Software Reference                                                                   Search Functions




                                          Use <F2> to change tabs on the hit list.

                                          Header
                                          The fields in the header area are described for the Find Purchase Orders dia-
                                          log:
                                           “Find Purchase Orders” on page E-23

                                          Article tab
                                          The columns are described for the General and Quantities tab:
                                           “Hit List – General” on page E-28
                                           “Hit List - Quantities” on page E-30
                                          In addition, the following columns are displayed:
                                          •   QU:
                                              Quantity unit for the item, e.g. square meter.
                                              Technical info: display field, DB field: kpos.me
                                          •   Dimens. Variant
                                              Dimensional variant of article.
                                              Technical info: display field, DB field: kpos.var


                                          Hit List - Miscellaneous Tab
                                          Purchase > P.O. Management > <F9> > Enter Search Criteria > <F3> > Mis-
                                          cellaneous Tab




                 Fig. E-8   Hit list (find purchase orders) - miscellaneous
5.00 / 12-2022




                                          This tab displays various information about the purchase orders that fits the
                                          search criteria. One line is displayed per purchase order item.
                                          Use <F2> to change tabs on the hit list.


                 A+W Enterprise Purchasing                                                                         E-33
                 Search Functions                                                              Software Reference




                                    Header
                                    The fields in the header area are described for the Find Purchase Orders dia-
                                    log:
                                     “Find Purchase Orders” on page E-23

                                    Miscellaneous tab
                                    The columns are described for the Quantities and Articles tab:
                                     “Hit List - Quantities” on page E-30
                                     “Hit List – Article” on page E-32
                                    In addition, the following columns are displayed:
                                    •   Stock:
                                        Stock number for the purchase order.
                                        Technical info: display field, DB field: bpos.lnr
                                    •   Customer:
                                        Customer name for order-related P.O.s.
                                        Technical info: display field, DB field: mp.name
5.00 / 12-2022




                 E-34                                                                   A+W Enterprise Purchasing
                 Software Reference                                                               Purchase Order Pool




                                        Purchase Order Pool
                                        In the PO pool, the following PO proposals are collected, which are combined
                                        into one or several PO/s:
                                        •    Order-related PO proposals from Sales.
                                        •    PO proposals from stock, e.g. before stock inventory runs too low. This
                                             function must be configured.
                                             If no automatic PO proposals can be generated by the stock, you can cre-
                                             ate the stock POs via the Purchase Order Entry dialog.
                                        Depending on system configuration and specified supplier master data, POs
                                        can be grouped 1:1 from the order data by the background process or first
                                        grouped manually in the PO pool, then generated.
                                        The PO release is done either automatically or when the PO is printed. The
                                        following are the possibilities:
                                        •    The purchase order is created and automatically released.
                                        •    The purchase order is printed and automatically released.
                                        •    The purchase order is manually released using the Purchase order release
                                             dialog.
                                        Depending on the system configuration, the PO release is possible via the
                                        Purchase Order Release menu element:
                                         “Purchase Order Release” on page E-99
                                        Another possibility is when storing an advice note. Insofar as the PO advice
                                        note is saved, the order is set to the status Ordered. This possibility must be
                                        configured separately.
                                         “Dispatch Notifications” on page E-104
                                        Use the Printing of forms or Email dialog to print purchase orders and send
                                        them to the supplier. The dialogs are described in detail in the Sales section:
                                         Sales, “Form Printing” on page D-361
                                         Sales, “E-mail” on page D-365
                                        In the change log, you can check the status of a PO. The dialog is described
                                        in detail for the Sales section:
                                         Sales, “Amendment Log” on page D-176
                                        The following information is available on this chapter:
                                         “Special Menus for the PO Pool” on page E-36
                                         “Purchase Order Release” on page E-99
                                         “Creating Purchase Orders” on page E-38
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                        E-35
                 Purchase Order Pool                                                                         Software Reference




                                             Special Menus for the PO Pool
                                             In the PO pool, dialog-specific menus can be called up.
                                             •      Use <F4> to open the supplementary menu for the PO pool.
                                             •      Use <Shift> + <F4> to open the info menu for the PO pool.
                                             The displayed entries depend on the respective configuration. The following
                                             overviews of the menus always list all entries.
                                             The following supplementary menus are available:
                                              “Purchase Order Pool – Additional Menu” on page E-36
                                              “Purchase Order Pool – Menu Info” on page E-37

                                                    Context menus
                                                    On the context menus, only the menu elements are offered that make
                                                    sense in the context for the individual fields of the dialogs. The functions
                                                    are described in the following chapters:


                                             Purchase Order Pool – Additional Menu
                                             Purchase > Create Purchase Orders > Enter Department > <F3> > <F4>

                                             Most-used configuration

                  Shortcut   Entry                                    Description

                        a    Reset tagged items (Shift+F12)           Disables the Cr. (Create PO) checkbox for the marked items.
                                                                      The items can be edited once again.

                        b    Group by tag (Ctrl+F8)                   Groups the items under one PO number.
                                                                      The Cr. (Create PO) checkbox must be enabled.

                        c    Group by order (Ctrl+O)                  The Cr. (Create PO) checkbox must be enabled.
                                                                      • Items with the same order number and the same supplier
                                                                        are grouped under a common PO.
                                                                      • For items with the same order number but different
                                                                        suppliers, individual POs are created for the items per
                                                                        supplier.Grouping by orders depends, among other things,
                                                                        on configuration. Please contact an A+W Software GmbH
                                                                        service employee.

                        d    Sort by purchase order (Ctrl+F12)        Sorts the purchase order numbers in descending order.

                        e    Purchase order header (Ctrl+K)            Sales, “Header and Footer Texts” on page D-256

                        f    Purchase order footer (Ctrl+F)            Sales, “Header and Footer Texts” on page D-256

                        g    Tag (downwards) (Shift+F11)              Enables the Cr. (Create PO) checkboxes for the selected and
                                                                      all subsequent items.

                        h    Tag (all) (Ctrl+F11)                     Enables the Cr. (Create PO) checkbox for all items.
5.00 / 12-2022




                        i    Cancel                                   No action at this point




                 E-36                                                                               A+W Enterprise Purchasing
                 Software Reference                                                                         Purchase Order Pool




                  Shortcut   Entry                                  Description

                     j       Inquiry (Ctrl+E)                       Selects the In (Inquiry) column of the selected item with an E.
                                                                    If the Cr. (Create PO) checkbox of the item is enabled, you
                                                                    can create an inquiry for the supplier with <Ctrl>+<F8>.

                     k       All inquiries (Ctrl+L)                 Selects the In (Inquiry) column of all items with an E.
                                                                    If the Cr. (Create PO) checkbox of the item is enabled, you
                                                                    can create an inquiry for the supplier with <Ctrl>+<F8>.

                     l       Enquiries starting from cursor position Selects the In (inquiry) column with an E for the selected and
                             (Ctrl+G)                                all subsequent items.
                                                                    If the Cr. (Create PO) checkbox for the item is enabled, you
                                                                    can create an inquiry for the supplier with <Ctrl>+<F8>.

                     p       Tag inquiries (Ctrl+N)                 Enables the Cr. (Create PO) checkbox for all items with an E
                                                                    in the In (inquiry) column.

                     n       Purchase orders not transferred yet     “Overview of Documents” on page E-145



                                                Purchase Order Pool – Menu Info
                                                Purchase > Create Purchase Orders > Enter Department > <F3> > <Shift> +
                                                <F4>


                  Shortcut   Entry                                  Description

                     a       Show order texts (Ctrl+F10)             “Order Texts” on page E-97

                     b       Purchase info                          In the selected order item to be ordered, an extra field
                                                                    Purchase info is displayed. Insofar as such information was
                                                                    entered in the associated order, this text is displayed in the
                                                                    field. New entry of the purchasing information in the PO pool
                                                                    is not possible.

                     c       Suppliers notes                         Sales, “Market Partner, Project, Article Notes” on
                                                                      page D-250

                     d       Supplier article notes                  Sales, “Customer Article, Supplier Article, Project Article
                                                                      Notes” on page D-253

                     e       Article notes                           Sales, “Market Partner, Project, Article Notes” on
                                                                      page D-250

                     f       Information on complaints              Displays the complaint information for the selected item from
                                                                    the order.
                                                                     “Creating Purchase Orders” on page E-38
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                                    E-37
                 Purchase Order Pool                                                                 Software Reference




                                         Creating Purchase Orders
                                         Purchase > Create Purchase Orders > Enter Department > <F3>
                                         Purchase > Create Stock Orders
                                         Use this dialog to convert PO proposals into POs. Depending on the configu-
                                         ration of the program and the desired result, you can also create the PO from
                                         a PO proposal or group several POs under one PO number.
                                         PO proposals can also be created automatically if:
                                         •   the supplier for the goods ordered from the order is selected in the master
                                             data as direct supplier.
                                         •   if there is insufficient stock. The function for automatic POs from the stock
                                             must be configured.If PO proposals cannot be created automatically by the
                                             stock, you must create the stock POs via the Purchase Order Entry dialog.
                                              “Purchase Order Entry” on page E-51
                                         This dialog offers the following tabs:
                                          “Create Purchase Orders – Supplier” on page E-38
                                          “Create Purchase Orders – Item” on page E-42
                                          “Create Purchase Orders – Details” on page E-43


                                         Create Purchase Orders – Supplier
                                         Purchase > Create Purchase Orders > Enter Department > <F3> > Supplier
                                         Tab
5.00 / 12-2022




                 Fig. E-9   Create purchase order – supplier




                 E-38                                                                       A+W Enterprise Purchasing
                 Software Reference                                                                Purchase Order Pool




                                        All PO proposals are collected in the PO pool. When working with several pur-
                                        chasing departments and/or companies, you can configure the selection dia-
                                        log to minimize the data and distribute it appropriately. After selection of the
                                        company and/or department, the PO proposals are listed on the Create PO di-
                                        alog.
                                        On this tab, the supplier information for the PO proposals is displayed.
                                        You can release the purchase orders in the Purchase Order Release dialog.
                                         “Purchase Order Release” on page E-99

                                        Selection dialog

                                        Site Selection of the number of the client. This field is only available with in-
                                        ternal client separation.
                                        Technical info: display field, DB field: kauf.hausnr

                                        Department Number of department. You can use <F9> to search for a num-
                                        ber.
                                        Technical info: mandatory field, numeric field, DB field: kauf.abtnr

                                        Additional purchase orders Purchase order number. You can use <F9> to
                                        search for a number. Use <Enter> to specify another PO number that is added
                                        in a new cell. You can sort the PO numbers in ascending or descending order
                                        with the Additional POs button.
                                        Technical info: numeric field, DB field: kauf.auftrnr (kauf.vorgang=2)
                                        Use <F3> to confirm the selection.

                                        Create purchase order
                                        To create the POs, the following steps must be taken:
                                        •    In the Cr. field, select the PO proposals for which you want to create a PO.
                                             Depending on the system configuration, with selection of a PO item from
                                             the order, all other PO items from the same order are marked. The Keep
                                             order items together option can also be used for selection deletion.
                                        •    With <Ctrl>+<F8> you group the PO proposals and create POs. If you se-
                                             lect several items, one or several POs can be created for the items. The
                                             grouping is done either according to selection, supplier change or orders.
                                             The type of grouping can be specified via the system configuration.
                                        •    Use <End> to trigger the PO creation and save the settings made. The POs
                                             can be corrected on the PO Management dialog and released on the PO
                                             Release dialog.

                                        Delete grouping
                                        You can reset the grouped item with already-assigned PO numbers in order to
                                        leave the item in the PO pool. For this, select the item in question and remove
                                        it from an order-related PO proposal by selecting the order item and deleting
                                        the PO number for this PO item via <F4> > Reset selected items.
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                          E-39
                 Purchase Order Pool                                                              Software Reference




                                       Supplier tag

                                       Site Number of site.
                                       Technical info: display field, DB field: kauf.hausnr

                                       PO No. Purchase order number under which the purchase orders can be
                                       grouped. Purchase order numbers are preliminarily created using the selec-
                                       tion in the Cr. column or canceled using the selection of column C. You can
                                       confirm your selection using <End> or [OK].
                                       Technical info: numeric field, DB field: bestpool.baufnr

                                       Cr. Specification of whether a PO should be created for the item. You can se-
                                       lect several entries and group them in a PO.
                                        The item in the PO pool is selected for PO creation.
                                        There will be no PO creation for this item.
                                       Use <Ctrl>+<F8> to group the selected item for the PO creation. If you select
                                       several items at the same time, one or several POs will be created depending
                                       on the system configuration.
                                       Technical info: checkbox

                                       Order Order number for PO proposals that are determined with reference to
                                       an order.
                                       Technical info: numeric field, DB field: bestpool.orgauftrnr

                                       Article Article number to be ordered.
                                       Technical info: mandatory field, numeric field, DB field: bestpool.artnr

                                       Description Article description of the purchase item.
                                       Technical info: alphanumeric field, DB field: bestpool.artbez1

                                       C Indication whether the article to be ordered was already canceled, e.g. be-
                                       cause an order correction has been made in the meantime. The flag is set by
                                       the system and cannot be changed here.
                                        The PO item was canceled and can no longer be created.
                                        The PO item is not canceled and can still be edited.
                                       Technical info: checkbox, DB field: bestpool.still

                                       Supplier Supplier number for the article. By default, the number of the default
                                       supplier for the article from the master data is displayed. If another supplier
                                       was assigned to the article in the customer order, the number of this supplier
                                       is displayed.
                                       • Use <F10> to open the market partner search for selection of another sup-
                                           plier.
                                        Sales, “Find Market Partner” on page D-41
                                       •   Use <F5> to open the dialog Addresses for selecting a different address.
                                        Sales, “Find Market Partner” on page D-41
                                       •  Use <Ctrl> + <O> to store the new supplier as default supplier for the se-
5.00 / 12-2022




                                          lected article in the master data.
                                       Technical info: mandatory field, numeric field, DB field: bestpool.linr



                 E-40                                                                     A+W Enterprise Purchasing
                 Software Reference                                                                  Purchase Order Pool




                                        Quantity Article quantity of the ordered item. Depending on the assigned
                                        quantity unit of the article, the quantity is displayed in this quantity unit. For
                                        stock POs, the PO quantity from the stock master data is used. You can
                                        change the PO quantity.
                                        Technical info: numerical field, DB field: bestpool.menge

                                        Ordered for Probable delivery date of the PO. The delivery date is calculated
                                        from the master data. You can change the date.
                                        Technical info: date field, DB field: bestpool.solldat

                                        Txt. Texts. Specification whether texts are entered for the PO item.
                                        • A: Article texts are stored for the item.
                                        • B: Article and item texts are stored for the item.
                                        • P: Item texts are stored for the item.
                                        Use <Shift> + <F4> > Show order texts to view the stored information.
                                              “Order Texts” on page E-97
                                        Technical info: numeric field, DB field: bestpool.arttxtnr and bestpool.poskotx-
                                        tnr

                                        PI Purchase information. Indication whether third-party information in the cus-
                                        tomer order is stored for the PO item. If purchase information is stored, an I is
                                        displayed in the field.
                                        Use <Shift> + <F4> > Purchase info to view the stored information.
                                        Technical info: display field

                                        Cm Complaint. Indication whether the PO was created due to a customer
                                        complaint.
                                         The item is being re-ordered due to a customer complaint.
                                         The item is not part of a complaint order.
                                        Technical info: checkbox

                                        In Inquiry. Indication whether an inquiry to the supplier is created. If a supplier
                                        inquiry is created, an I is displayed in the field.
                                        Via the supplementary menu, you can specify for which PO items a supplier
                                        inquiry should be created.
                                        Technical info: display field

                                        In Info indication. The field is not currently used.
                                        Technical info: display field

                                        SB Substitute order. Indication whether a broken item must be reordered.
                                        Technical info: display field

                                        Footer

                                        Supplier Supplier name of the selected item.
                                        Technical info: display field
5.00 / 12-2022




                                        Groups one or several PO/s from the selected PO proposals.




                 A+W Enterprise Purchasing                                                                            E-41
                 Purchase Order Pool                                                                    Software Reference




                                          Triggers the function in question, that is, the grouped PO proposals are trans-
                                          formed into POs and saved in the system under the specified number. The but-
                                          ton is only displayed if the grouping has already been made.


                                          Create Purchase Orders – Item
                                          Purchase > Create Purchase Order > Enter Department > <F3> > Item Tab




                 Fig. E-10   Create purchase orders – item tab


                                          This tab displays item information for ordered articles.

                                          Item tab
                                          The fields are described in connection with the Create Purchase Order dialog:
                                           “Create Purchase Orders – Supplier” on page E-38
                                          In addition, the following fields are displayed:

                                          Itm Item number for PO items from customer orders.
                                          Technical info: numeric field, DB field: bestpool.orglfdpos

                                          Stock Stock number for the PO for stock articles. You can change the stock
                                          number.
                                          Technical info: numeric field, DB field: bestpool.lnr

                                          Width, Height Dimensions of the item in millimeters. You can change the di-
5.00 / 12-2022




                                          mensions if required. If a variant item is entered in the PO item, you can use
                                          <F9> to select another dimensional variant or remove the variant reference
                                          and specify freely selected dimensions.


                 E-42                                                                        A+W Enterprise Purchasing
                 Software Reference                                                                  Purchase Order Pool




                                          Technical info: numeric fields, DB fields: bestpool.laenge, bestpool.breite

                                          Qt Indication whether article in the PO item is not an item article, but a subpart
                                          from a BOM. If the article is a BOM subpart, an asterisk * is displayed in the
                                          field.
                                          Technical info: numeric field, DB field: bestpool.orglfdpos

                                          Footer
                                          The fields and buttons in the footer area are described for the Create Purchase
                                          Order – Supplier tab:
                                           “Create Purchase Orders – Supplier” on page E-38


                                          Create Purchase Orders – Details
                                          Purchase > Create Purchase Orders > Enter Department > <F3> > Details Tab




                 Fig. E-11   Create purchase orders – details


                                          The detailed information about the articles to be ordered is displayed on this
                                          tab. You can add item data if necessary.

                                          Details tab

                                          Site Site number for which the POs are triggered.
                                          Technical info: display field, DB field: bestpool.hausnr
5.00 / 12-2022




                                          P.O. PO number and item number in the PO.
                                          Technical info: display fields, DB fields: bestpool.baufnr, bestpool.orglfdpos


                 A+W Enterprise Purchasing                                                                            E-43
                 Purchase Order Pool                                                               Software Reference




                                       Order Order number, item number and tuple number for the ordered order
                                       subparts for which the PO proposal is made.
                                       Technical info: display fields, DB fields: bestpool.orgauftrnr,
                                       bestpool.orglfdpos, bestpool.orgtnr

                                       Customer Number and name of the customer for PO items from customer or-
                                       ders.
                                       Technical info: display fields, DB fields: bestpool.kunr, mp.name

                                       Operator Name of the person entering the order for PO items from customer
                                       orders.
                                       Technical info: display field, DB field: kauf.eusr

                                       Proj. Number and description of the project.
                                       Technical info: display fields, DB fields: bestpool.objnr, mp.name

                                       Purch. Info Third-party information for purchasing for PO items from custom-
                                       er orders. The field is only shown if purchase info was stored in the order.
                                       Technical info: display fields, DB fields: kauf.exbez1

                                       (without name) Number for different address if it was entered as delivery ad-
                                       dress.
                                       Technical info: numeric field, display field, DB fields: bestpool.divadrnr

                                       Stock Number and designation of the stock for stock articles. You can change
                                       the stock.
                                       Technical info: numeric field, display field, DB field: bestpool.lnr

                                       Article Number and description of the article.
                                       Technical info: mandatory field, numeric field, display field, DB fields: best-
                                       pool.artnr, bestpool.artbez1

                                       Shape Shape number for PO items with lite shape.
                                       Technical info: display field, DB field: bestpool.modnr

                                       Supplier Number and name of the supplier. You can change the supplier.
                                       • With <F9> you can select the supplier from the suppliers that are stored for
                                          the article in the master data.
                                       • Use <F10> to open the market partner search dialog for selection of anoth-
                                          er supplier.
                                       • Use <Ctrl> + <O> to store the selected market partner as default supplier
                                          for the current article in the master data.
                                       • Use <F5> to change the delivery address. By default, the supplier's main
                                          delivery address is selected.
                                       Technical info: numeric field, display field, DB fields: bestpool.linr, mp.name

                                       Fax Fax number of the supplier from the master data.
5.00 / 12-2022




                                       Technical info: display field, DB field: bestpool.faxnr




                 E-44                                                                     A+W Enterprise Purchasing
                 Software Reference                                                                 Purchase Order Pool




                                        P.O. No. Supplier-side number and designation of the article if a supplier-spe-
                                        cific article number is stored for the article in the master data.
                                        Technical info: alphanumeric field, DB fields: bestpool.exartnr,
                                        bestpool.exartbez

                                        Quantity PO quantity of the ordered item in the quantity unit of the article
                                        stored in the master data. You can change the PO quantity.
                                        Technical info: mandatory field, numeric field, DB field: bestpool.menge

                                        QU Quantity unit. For length, time, and piece articles, the respective quantity
                                        unit is displayed in this field, e.g. meter, liter.
                                        Technical info: display field, DB field: bestpool.me

                                        Width, Height Dimension of the item in the quantity unit of the article stored
                                        in the master data. You can change the dimensions. If a variant article is en-
                                        tered in the PO item, you can use <F9> to select a different dimension variant
                                        or remove the variant reference and specify freely selectable dimensions. For
                                        PO proposals from the stock, the dimensions of the PO variant are used. For
                                        missing entries, this information is urgently needed when opening the item in
                                        question.
                                        Technical info: numeric fields, DB fields: bestpool.laenge, bestpool.breite

                                        AIR Width of the airspace in the appropriate dimensional units. You can
                                        change the airspace. The airspace is only displayed if an IG article is entered
                                        in the PO item.
                                        Technical info: numeric field, DB field: bestpool.szr

                                        Variant Variant number and variant designation of the article. You can change
                                        the variant. If you select another dimensional variant, the Width and Height
                                        fields are adjusted automatically.
                                        Technical info: alphanumeric field, DB fields: bestpool.bitnr, bestpool.varart

                                        Cust. Route Delivery date to the customer.
                                        Technical info: display field, DB field: bestpool.liefdat

                                        Ordered for Probable delivery date of the PO. The delivery date is calculated
                                        from the master data. You can change the date.
                                        Technical info: mandatory field, date field, DB field: bestpool.solldat

                                        Ordered on Date of the purchase order entry.
                                        Technical info: mandatory field, date field, DB field: bestpool.bestdat

                                        Own Curr. Unit price and item price in the national currency, e.g. euros. Tech-
                                        nical info: display field, DB fields: bestpool.nstpreis, bestpool.npospreis

                                        For. Curr. Unit price and item price in a foreign currency, e.g. dollars.
                                        Technical info: display fields, DB fields: bestpool.fnstpreis, bestpool.fnstpreis
5.00 / 12-2022




                                        Currency, Rate Number and name of the currency and currency rate, e.g.
                                        rate for conversion of Euros to dollars.



                 A+W Enterprise Purchasing                                                                          E-45
                 Purchase Order Pool                                                              Software Reference




                                       Technical info: display fields, DB fields: bestpool.waehrung,
                                       waehrung.kurzbez, bestpool.kurs

                                       Cost Center Cost center name for statistical evaluations for PO items from
                                       customer orders.
                                       Technical info: display field, DB field: bestpool.kostenst

                                       Incoterms Requested type of delivery:
                                       • Pickup:
                                          Customer collects the goods.
                                       • Third-party business transaction:
                                          The producing plant will ship the goods directly to the customer.
                                       • No selection:
                                          Goods will be delivered via the route that has been entered in the customer
                                          order.
                                       Technical info: toggle field, DB field: bestpool.geschart

                                       Reject Place Number and name of the reject place where the glass break
                                       happened. The number only needs to be specified if an item needs to be reor-
                                       dered due to glass breakage. Generally the reject place is transferred from
                                       production and taken over in this field. If needed, you can change the reject
                                       place in A+W Enterprise. The reject place name is displayed in plain text in the
                                       next field.
                                       The reject places are stored in the database table xbruchort. The values from
                                       production are taken over automatically. There is no maintenance dialog for
                                       this table in A+W Enterprise.
                                       Technical info: numeric field, display field, DB field: bestpool.bruchort

                                       Reject Reas. Number and designation of the reject reason. The number must
                                       only be specified if an item has to be reordered due to a glass break. You can
                                       change the reject reason. If you specify a number, the reject reason is dis-
                                       played in plain text.
                                       Technical info: numeric field, display field, DB field: bestpool.bruch

                                       Totals Total of the item for weight in kilograms, area in square meters, and
                                       length in linear meters.
                                       Technical info: display fields

                                       Item The Item indication specifies that displayed totals per item apply.
                                       Technical info: display field

                                       Footer
                                       The buttons in the footer are described for the Create Purchase Order - Sup-
                                       plier tab:
                                        “Create Purchase Orders – Supplier” on page E-38
5.00 / 12-2022




                 E-46                                                                    A+W Enterprise Purchasing
                 Software Reference                                                            Document Management




                                        Document Management
                                        The documents that you edit in the Purchasing area include supplier inquiries,
                                        POs, receipts of goods, supplier invoices, and credit notes. The dialogs look
                                        and work largely the same way as those for the Sales area.
                                        The following sections are part of the document management:
                                         “Explanation of Symbols” on page E-47
                                         “Supplier Inquiries” on page E-50
                                         “Purchase Order Entry” on page E-51
                                         “Creating Purchase Orders” on page E-38
                                         “Receipt of Goods (Manual)” on page E-119
                                         “Supplier's Invoice (Manual)” on page E-138
                                         “Supplier's Credit Note” on page E-142



                                        Explanation of Symbols
                                        This section describes the identifiers for the dialog mode, the item status, and
                                        the item identifier.

                                        Dialog mode
                                        The dialog mode is shown in the title line of the dialog.

                                        Symbol     Symbol description     Meaning

                                                   Dialog with cross      In this mode, you can create new records.


                                                   Dialog with pen        In this mode, you can edit a document.


                                                   Yellow triangle with   In this mode, you can not edit the document.
                                                   exclamation point

                                                   Find                   In this mode, you can search for documents.


                                        Tab. E-1      Dialog mode

                                        Item status and symbols
                                        The item status is displayed on the Items tab next to the Item column.

                                        Symbol     Symbol description     Meaning

                                                   green                  The item can be changed as desired since the
                                                                          purchase order has not yet been released.

                                                   yellow                 The item or sub-parts of the item have been
5.00 / 12-2022




                                                                          ordered or the purchase order has been
                                                                          printed.

                                        Tab. E-2      Item status


                 A+W Enterprise Purchasing                                                                            E-47
                 Document Management                                                                 Software Reference




                                       Symbol     Symbol description      Meaning

                                                  red                     The item is released in the PO. It can no longer
                                                                          be changed.

                                                  red/red-blue            Item has been partially delivered.


                                                  red/blue                Item has been fully delivered.


                                                  red-blue/blue           Item has been partially invoiced.


                                                  blue                    Item has been invoiced completely.


                                       Tab. E-2      Item status

                                       The item identifier is displayed in front of the Item column.

                                       Symbol     Symbol description     Meaning

                                                  Yellow star            The product dimension and additional
                                                                         processing of the article are stored for the
                                                                         selected supplier.
                                                                         After saving the supplier-specific article, a
                                                                         green star is displayed.
                                                                          Sales, Help Cards, “Fix item” on page D-29

                                                  Green star             The article has been defined supplier-
                                                                         specifically and can only be entered for this
                                                                         specific supplier.
                                                                         When you create a supplier-specific article,
                                                                         you can create the BOM structure with
                                                                         additional processings, articles, dimension
                                                                         changes and additional supplier-specific
                                                                         requests.
                                                                          Sales, “Article Details for Dimensioned Vari-
                                                                           ants” on page D-164

                                                  Lite shape             Item is entered with shape.
                                                                          Sales, “Shape - Dimensions” on
                                                                           page D-180

                                                  Window with Georgian   Item has been entered with muntins.
                                                  bars
                                                                          Sales, “Muntin Entry” on page D-229

                                       Tab. E-3      Item identifier

                                       The status in text format is shown in the dialog line or in the General tab above
                                       the Proc.type column when the item status changes. The following status dis-
5.00 / 12-2022




                                       plays are possible:




                 E-48                                                                      A+W Enterprise Purchasing
                 Software Reference                                                                  Document Management




                                        Status in text format       Meaning

                                        Stock withdrawal            A stock withdrawal has been booked for this item.

                                        Partially ordered           A partial order exists for the item, e.g. for an article
                                                                    from the bill of material.

                                        Cancel                      The purchase order has been canceled.

                                        Invoiced                    The purchase order has been invoiced and can no
                                                                    longer be changed. On the right hand side next to
                                                                    Invoiced, the number of the supplier invoice is
                                                                    displayed.

                                        Dispatch planning           The PO is planned in dispatch. Commercial changes,
                                        available                   such as price changes, are still possible under some
                                                                    circumstances.

                                        Global correction           Changes in the PO are no longer transferred to the
                                                                    database. Commercial changes such as price
                                                                    changes, are still possible under some circumstances.

                                        Local correction            Changes in the item are no longer transferred to the
                                                                    system during PO entry if they affect the PO, e.g.
                                                                    dimension changes. Commercial changes, such as
                                                                    price changes, are still possible under some
                                                                    circumstances.

                                        Tab. E-4      Status display in text format
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                                     E-49
                 Document Management                                                                    Software Reference




                                           Supplier Inquiries
                                           Purchase > Inquiries




                 Fig. E-12   Supplier inquiries


                                           Use this dialog to create and edit inquiries to suppliers.
                                           If you enter a delivery date in the inquiry, you can create a resubmission date
                                           to ensure the post-processing of an inquiry. When the resubmission date has
                                           arrived, a message will be displayed at the program start or a reminder e-mail
                                           sent.
                                           The resubmission is described in detail in the Sales section:
                                            Sales, “Resubmission” on page D-402
                                           Each inquiry can be converted into a purchase order.
                                           The dialog is structured the same as the Purchase Order Entry dialog. Devia-
                                           tions will be described explicitly for the Purchase Entry dialog.
                                            “Purchase Order Entry” on page E-51
5.00 / 12-2022




                 E-50                                                                         A+W Enterprise Purchasing
                 Software Reference                                                              Document Management




                                        Purchase Order Entry
                                        Purchase > P.O. Management
                                        On this dialog, you enter and/or edit purchase orders.
                                        For regular creation of POs, you usually use the Create Purchase Order dia-
                                        log. Then you can view or edit the POs created on the Order Management di-
                                        alog.
                                         “Creating Purchase Orders” on page E-38
                                        This dialog contains the following tabs in the header area:
                                         “Purchase Order Entry – Header, Footer” on page E-52
                                         “Purchase Order Entry – Addresses” on page E-58
                                         “Purchase Order Entry – Properties” on page E-60
                                         “Purchase Order Entry – Miscellaneous” on page E-65
                                        The Items tab offers the following tabs:
                                         “Purchase Order Items - General” on page E-72
                                         “Purchase Order Items - Properties” on page E-81
                                         “Purchase Order Items - Prices” on page E-84
                                         “Purchase Order Items - Order Info” on page E-87
                                         “Purchase Order Items - Status” on page E-88
                                         “Purchase Order Items - Evaluation” on page E-91
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                     E-51
                 Document Management                                                                  Software Reference




                                          Purchase Order Entry – Header, Footer
                                          Purchase > P.O. Management > Open Purchase Order > Items Tab




                 Fig. E-13   Purchase order entry – items tab


                                          On this dialog, you specify the supplier data and enter the PO items. If you en-
                                          ter items, it is generally sufficient to enter the data in the General tab.
                                          •   Use <Enter> to change to the next field, <Page Up> to jump to the first item,
                                              <Page Down> to jump to the last item.
                                          •   Use <End> to switch to the footer and conclude the purchase order man-
                                              agement.
                                          •   Use <F2> to switch from the Contract field to the Addresses, Properties or
                                              Miscellaneous tabs.

                                          Header
                                          •   Use <Ctrl>+<F12> to change from the Receipt, Invoice Type or Project
                                              fields to the PO Type dialog.
                                               “PO Type” on page E-95
                                          •   Use <F2> to change from the Receipt, Invoice Type or Project fields to the
                                              Item area.

                                              List purchase orders
                                              If you open the Purchase Order Entry dialog, you can use <F5> to change
                                              to the S-order field and search for the associated POs by entering the order
5.00 / 12-2022




                                              number. Alternatively, you can list and then select all existing POs with
                                              <F9>.




                 E-52                                                                        A+W Enterprise Purchasing
                 Software Reference                                                              Document Management




                                        Purchase Purchase order number.
                                        Technical info: mandatory field, numeric field, DB field: kauf.auftrnr (kauf.vor-
                                        gang=2)

                                        Supplier Supplier number. If you specify a number, the supplier's name and
                                        location are displayed in plain text.
                                        Technical info: mandatory field, numeric field, display fields, DB field:
                                        kauf.kunr, kauf.orgname

                                        Reason Reason for a date change. The Reason field is only displayed if you
                                        change the delivery date in an purchase order previously entered.
                                        Technical info: alphanumeric field, DB field: kaufltedit.text

                                        Ref. Document number that is being referenced.

                                        Pre-selecting document type for the reference
                                        Depending on the system configuration, it is possible to specify one of the doc-
                                        ument types as pre-selection for the reference entry:
                                        •    Use <F8> display the document type configured as default in the Refer-
                                             ence field.
                                        •    Use <F9> to open a selection dialog with all document types that can be
                                             referred to. use the arrow keys to select a document type.
                                        •    Use <Enter> to confirm the selection.
                                        •    The Reference field displays the number of the current market partner.
                                        •    If you would like to specify the current market partner as pre-selection, then
                                             confirm with <Enter>.
                                        •    If you would like to specify another market partner as pre-selection, use
                                             <F9> to open the Find Market Partner dialog in order to select a market
                                             partner. Alternatively, you can enter the market partner number directly in
                                             the field. Use <Enter> to confirm the selection.
                                        •    The Reference field is empty. If you open the Find Reference dialog now,
                                             the document type and market partner that you have specified are pre-se-
                                             lected as search criteria.

                                        Enter document with reference
                                        •   Use <F9> to open the Find Reference dialog in order to select a reference
                                            document for the specified criteria. Alternatively, you can enter the docu-
                                            ment number directly in the field.
                                        • Use <Enter> to confirm the selection. You can take over all data from the
                                            reference document or only the header data from the reference document.
                                        You can take over all data from the reference document or only the header
                                        data from the reference document. This decision is made via confirmation of
                                        the corresponding Yes/no message.
                                        Use <F9> to open the Find Reference dialog. The dialog is described in detail
                                        in the Sales section.
                                         Sales, “Find Reference Document” on page D-47
5.00 / 12-2022




                                        Technical info: numeric field, DB field: kauf.referenz




                 A+W Enterprise Purchasing                                                                           E-53
                 Document Management                                                                Software Reference




                                          Reference to order
                                          If you reference an order in the PO, then all order items will be loaded into
                                          the PO entry. If necessary, items on the General tab must be deleted or ad-
                                          justed.

                                       Site Site number at which the PO is entered. If you are working with internal
                                       client separation, the Client field is released. If you are also working with site-
                                       company assignment, the first field displays the company number to which the
                                       site is assigned from the system master data.
                                       Technical info: numeric fields, DB fields: kauf.company, kauf.hausnr

                                       Entry Date Entry date. By default, the field is pre-populated with the current
                                       date. This entry can be changed.
                                       Technical info: mandatory field, date field, DB field: kauf.edat

                                       Cust. Order Customer order number from sales for order-related purchase
                                       orders. Depending on the configuration, alternative data can be shown:
                                       • Cus.Ord.-No.:
                                          External customer purchase order number. For orders from another site,
                                          the order number of the sending site is in this field.
                                       • In the event of internal remote data transmissions between two plants, the
                                          following data can also be shown in combination:
                                          – Purchase order number from the sending site.
                                          – Order number.
                                          – Customer purchase order number.
                                       • Stock P.O.:
                                          Display that a stock purchase order is being executed.
                                       • Collective purchase order:
                                          Display that order-related order items have been combined into a collective
                                          purchase order. Collective purchase orders can be executed by the suppli-
                                          er in the form of partial deliveries.
                                       • External number system, e.g. quotation number from the supplier.
                                       Technical info: alphanumeric field, DB field: kauf.exaufnr

                                       Date Requested delivery data of purchase order. In the first field you can en-
                                       ter the calendar week. In the second field you can enter the date in the format
                                       DD.MM.YYYY.
                                       Technical info: mandatory field, numeric field, date field, DB fields: kauf.kwide-
                                       al, kauf.ltideal

                                       Route Route number. Route selection shows the routes and corresponding
                                       route dates. You can store one main route and three alternative routes for a
                                       customer in the master data. If the via-plant function is configured, use <F5>
                                       to select the site via which the delivery should be organized.
                                       Technical info: mandatory field, numeric field, DB field: kauf.routenr

                                       Deliv. Date Display of the planned delivery date.
5.00 / 12-2022




                                       Technical info: display field, DB field: kauf.ltplan

                                       Suppl. Item Specification of supplier items in the PO.


                 E-54                                                                      A+W Enterprise Purchasing
                 Software Reference                                                             Document Management




                                        •  yes:
                                           The items can be entered with the supplier's article numbers. If you have
                                           assigned the supplier's article numbers to the articles in your master dat,
                                           you can select articles via your master data. In the PO, the supplier's article
                                           numbers are transferred to the suppliers
                                           For the item entry via supplier-related article data, the field S.Item is en-
                                           abled on the General tab.
                                        • no:
                                           The individual article numbers are entered.
                                        Technical info: toggle field, DB field: kauf.kndposkz

                                        DateType Information about the date type that will be printed on the order.
                                        • Call: date on call.
                                        • urgent: as soon as possible.
                                        • poss.: if possible, by the date.
                                        • bind.: date is binding.
                                        • without: without date type.
                                        • Auto: currently not used.
                                        • follows: date to follow.
                                        Technical info: toggle field, DB field: kauf.abrufkz

                                        Receipt Will not be used.
                                        Technical info: toggle field, Database field: kauf.eingang

                                        Invoice type Specification of the services for which the invoice is issued.
                                        Usually, the glass and the installation work are invoiced together. Upon re-
                                        quest, you can create individual invoices.
                                        • Total:
                                           The invoice is created for the total purchase order, that is, for material and
                                           installation services.
                                        • Glass:
                                           The invoice is only created for the material of the purchase order.
                                        • Service
                                           The invoice is only created for the installation services of the purchase or-
                                           der.
                                        Technical info: toggle field, DB field: kauf.rechart

                                        Project Project number. A project is assigned to the market partner and can,
                                        e.g. be a construction site that is supplied directly by the supplier and have a
                                        different delivery address. You can link particular conditions with the project
                                        that only apply to this project, e.g. discounts or payment options. You have the
                                        opportunity to bill project-related.
                                        Use <F9> to open the project search. The project search is described in detail
                                        in the Sales section.
                                         Sales, “Find Project” on page D-69
                                        Technical info: numerical field, DB field: kauf.objnr
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                          E-55
                 Document Management                                                                Software Reference




                                       Item area
                                       In this area, you are shown information concerning a selected item or column.
                                       The tabs and subtabs are described separately:
                                        “Purchase Order Items” on page E-71

                                       Footer
                                       In the footer area, the total order values for the individual dimensional units
                                       and the total amounts of the items are displayed. You can grant a general dis-
                                       count and overwrite the amount in the Net Total field, e.g. if you have made a
                                       special agreement with the supplier.
                                       Use <F2> to open the Purchase Order Entry dialog for calculating discounts
                                       and the net amount.
                                        “Purchase Order Entry - Totals” on page E-69

                                       Sender Display of the site number and the reference number. The reference
                                       number can be the quotation number or for EDI orders the order or purchase
                                       order number.
                                       Technical info: display fields, DB fields: kauf.hausnr

                                       Qt, lb, sf Display of the total purchase order value for the quantity in pieces,
                                       weight in kilograms, and area in square meters.
                                       Technical info: display fields, DB fields: kauf.gesst, kauf.gesm2, kauf.ges-
                                       gewicht

                                       Total Display of the total price of all items less the item discount from the field
                                       Minus on the Prices tab. The total price of an item is calculated as item price
                                       x item quantity.
                                        “Purchase Order Items - Prices” on page E-84
                                       Technical info: display field, DB field: kauf.gesnetto

                                       Discount Discount granted for the total amount in percent. With discount
                                       granted, the amount in the NetTotal field is adjusted.
                                       Technical info: numeric field, DB field: kauf.gesfaktor

                                       Net Total Total of all item prices, incl. the discounts and plus the surcharges.
                                       It is not possible to edit the amount. The system calculates the difference and
                                       displays it in the Gen. discount or Gen. surcharge field on the calculation dia-
                                       log.
                                        “Purchase Order Entry - Totals” on page E-69
                                       Technical info: numerical field, DB field: kauf.nettototal

                                       +VAT () Display of the VAT. The VAT amount is in the field that is assessed on
                                       the net amount. In the brackets, the applicable VAT is displayed in percentage.
                                       Technical info: display field, DB field: kauf.mwstbetrag

                                       Gross Display of the gross total amount. The amount is calculated from the
5.00 / 12-2022




                                       net amount plus the VAT.
                                       Technical info: display field, DB field: kauf.gesbrutto



                 E-56                                                                      A+W Enterprise Purchasing
                 Software Reference                                                             Document Management




                                        C. Margin Display of the contribution margin (gross margin) that a product
                                        contributes to covering the fixed costs and to achieving the net profit. All dis-
                                        counts and surcharges are taken into account.
                                        Technical info: display field, DB field: kauf.dbdm
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                          E-57
                 Document Management                                                                   Software Reference




                                          Purchase Order Entry – Addresses
                                          Purchase > P.O. Management > Open Purchase Order > Field Entry Date, In-
                                          voice Type > <F2> > Addresses Tab




                 Fig. E-14   Purchase order entry – addresses


                                          On this tab, you can edit the supplier and delivery address. By default, the de-
                                          livery address from the supplier master data is used in the delivery address ar-
                                          ea. You can configure the determination of the delivery address customer-
                                          specifically. For customer-specific adjustments, contact your contact person at
                                          A+W Software GmbH.

                                          Header
                                          The fields in the header area are described for the Purchase Order Entry –
                                          Header, Footer tab:
                                           “Purchase Order Entry – Header, Footer” on page E-52

                                          Supplier's address

                                          Name, 1stName Supplier's first and last names.
                                          Technical info: alphanumeric fields, DB fields: kauf.orgname, kauf.orgvorname

                                          Title Number of the title. If you select a number, the title is displayed in plain
                                          text.
5.00 / 12-2022




                                          Technical info: numeric field, DB field: kauf.organrede

                                          Attn. For the attention of. Name of the person who should receive the pur-
                                          chase order.


                 E-58                                                                         A+W Enterprise Purchasing
                 Software Reference                                                            Document Management




                                        Technical info: alphanumeric field, DB field: kauf.orgzhd

                                        Addition Additional text for address.
                                        Technical info: alphanumeric field, DB field: kauf.orgbranche

                                        Street Street address of the supplier.
                                        Technical info: alphanumeric field, DB field: kauf.orgstr

                                        PCd. POB Postal code and P.O. box number.
                                        Technical info: alphanumeric fields, DB fields: kauf.orgpfplz, kauf.orgpostfach

                                        PBoxCity City name for the PO box of the supplier outside Europe.
                                        Technical info: alphanumeric field, DB field: kauf.vertr

                                        PCd.City Postal code and city of the supplier's address.
                                        Technical info: alphanumeric field, DB fields: kauf.orgplz, kauf.orgort

                                        Country License plate ID for the target country. If you select a code, the coun-
                                        try name is displayed in plain text.
                                        Technical info: alphanumeric fields, DB fields: kauf.orgkfzcode, kauf.orgland

                                        Pho Supplier's phone number.
                                        Technical info: alphanumeric field, DB field: kauf.orgtel

                                        Fax Supplier's fax number.
                                        Technical info: alphanumeric field, DB field: kauf.faxnr

                                        Language Number of the national language of the supplier in which the doc-
                                        uments will be printed. If you select a number, the language is displayed in
                                        plain text.
                                        Technical info: numeric field, DB field: kauf.sprkz

                                        Code Number of tax code. The tax code is the tax key that is used to calculate
                                        the VAT. If you select a number, the description of the tax code is displayed in
                                        plain text.
                                        Technical info: numeric field, DB field: kauf.kukz

                                        Delivery address
                                        You can enter a different shipping address, e.g. for direct delivery the address
                                        of a construction site.
                                        •    Use <Ctrl>+<N> to create a new delivery address for the supplier.
                                        •    Use <Ctrl> + <L> to select the stored delivery address of a supplier.
                                        The fields are described for the Supplier Address area:
                                         “Supplier's address” on page E-58
                                        In addition, the following field is described:
5.00 / 12-2022




                                        Reg. No Dispatch region. The dispatch region is stored in the master data
                                        and is determined via the postal code. It is relevant only for orders.


                 A+W Enterprise Purchasing                                                                           E-59
                 Document Management                                                                  Software Reference




                                          Technical info: display field

                                          Footer
                                          The fields in the footer area can only be entered on the Items tab. They are
                                          described for the Purchase Order Entry - Header, Footer tab:
                                           “Purchase Order Entry – Header, Footer” on page E-52


                                          Purchase Order Entry – Properties
                                          Purchase > P.O. Management > Open Purchase Order > from Field Entry Date
                                          on <F2> > Properties Tab




                 Fig. E-15   Purchase order entry – properties


                                          On this tab you can edit information relating to staff allocation, shipping infor-
                                          mation, and invoice and printing options.

                                          Header
                                          The fields in the header area are described for the Purchase Order Entry –
                                          Header, Footer tab:
                                           “Purchase Order Entry – Header, Footer” on page E-52

                                          Staff allocation
5.00 / 12-2022




                                          Ordered by Employee number of the supplier. If you select a number, the em-
                                          ployee's name is displayed in plain text. Use <F5> to open the Contact Person




                 E-60                                                                        A+W Enterprise Purchasing
                 Software Reference                                                            Document Management




                                        dialog where you can select or create a new contact person. The Contact Per-
                                        son dialog is described in detail in the Sales section.
                                         Sales, “Contacts” on page D-147
                                        Technical info: numeric field, DB field: kauf.busnr

                                        PO Date Date of the purchase order entry.
                                        Technical info: date field, DB field: kauf.bdat

                                        Operator Displays the number and name of the operator.
                                        Technical info: display fields, DB field: kauf.esuer

                                        Handled by Name of the administrator. If you select a number, the adminis-
                                        trator's name is displayed in plain text.
                                        Technical info: numeric field, DB field: kauf.abvertr

                                        Field Staff Name of the field employee.
                                        Technical info: alphanumeric field, DB field: kauf.vertr

                                        Sales Repres. Sales representative. Number of the representative to whom
                                        the commission will be paid. If you select a number, the representative's name
                                        is displayed in plain text.
                                        Technical info: numeric field, DB field: kauf.vertrerloe

                                        Shipment Information

                                        Maximum Load Maximum weight that the supplier can unload with its tech-
                                        nical equipment.
                                        Technical info: numerical field, DB field: kauf.gmaxgew

                                        Delivery Comment about the requested delivery method. Usually, the type of
                                        delivery is not used in the Purchase area.
                                        • Pick-up:
                                           Goods will be picked up with PO.
                                        • Third-party business transaction:
                                           The producing plant will ship the goods directly to the supplier.
                                        • No selection:
                                           Goods will be delivered via the route that has been entered in the header.
                                        Technical info: toggle field, DB field: kauf.geschart

                                        Dir. Dispatch Indicator as to whether the supplier will receive the delivery di-
                                        rectly from the production facilities or whether the goods will be delivered to
                                        the dealer. The code is not used in the Purchase area.
                                        Technical info: toggle field, DB field: kauf.drkliefkz

                                        Incoterm Number of the method of delivery, e.g. carriage paid. If you select
                                        a number, the name of the delivery type is displayed in plain text.
                                        Technical info: numeric field, DB field: kauf.lieferart
5.00 / 12-2022




                                        Disp. Type Number of the dispatch type, e.g. truck. If you select a number,
                                        the description of the dispatch type is displayed in plain text.


                 A+W Enterprise Purchasing                                                                        E-61
                 Document Management                                                                 Software Reference




                                       Technical info: numeric field, DB field: kauf.versandart

                                       Packing Type Number of the packing type, e.g. box. If you select a number,
                                       the name of the packing type is displayed in plain text.
                                       Technical info: numeric field, DB field: kauf.verpackart

                                       Rack Load Rack load. Select by which criteria the goods shall be sorted on
                                       the racks:
                                       • Item: by item.
                                       • Size: by size.
                                       • Air+Size: by airspace and size.
                                       • Item (free): items kept together, but freely organized.
                                       • HD Glass Col Thick: by hard dimension, glass dimension, and color.
                                       • HD Gl.dim Color - : by hard dimension, glass dimension, and color.
                                       • HD Gl.dim - Thick: by hard dimension, glass dimension, and thickness.
                                       • HD - Color thick: by hard dimension, color, and thickness.
                                       • HD Glass dim - - : by hard dimension and glass dimension.
                                       • HD - Color - : by hard dimension and color.
                                       • HD - - Thick: by hard dimension and thickness.
                                       • HD - - - : by hard dimension.
                                       • Reference: by reference text.
                                       Technical info: toggle field, DB field: kauf.gbelad

                                       Customs Exit Number of the customs exit office for the delivery papers. If
                                       you select a number, the name of the customs office is displayed in plain text.
                                       Technical info: numeric field, DB field: kauf.azsnr

                                       Destin. Customs Number of the customs office in the country of destination.
                                       If you select a number, the name of the customs office is displayed in plain text.
                                       Technical info: numeric field, DB field: kauf.bzsnr

                                       Travel time, Distance Estimated travel time and display of the route. De-
                                       pending on the configuration, the travel time is given in hours or days.. It can
                                       affect the delivery date. The route is drawn from the Distance field of the de-
                                       livery address.
                                       Technical info: numeric fields, DB fields: kauf.anfahrt

                                       Invoice and Print Options

                                       VAT ID No. Supplier's VAT ID no.
                                       Technical info: alphanumeric field, DB field: kauf.steuernr

                                       Taxpayer's No. Supplier's registered tax number at tax office.
                                       Technical info: alphanumeric field, DB field: kauf.finstnr

                                       Cost Center Cost center name for statistical evaluations.
5.00 / 12-2022




                                       Technical info: alphanumeric field, DB field: kauf.kostenst




                 E-62                                                                     A+W Enterprise Purchasing
                 Software Reference                                                              Document Management




                                             Defining the cost center for the entire purchase order
                                             If you enter a cost center, the item-exact cost centers from the master data
                                             are overwritten related to the purchase order.

                                        Invoice Type Type of invoice.
                                        • Separate invoice:
                                           The addressee will receive a separate invoice for every purchase order.
                                        • Collective invoice:
                                           The addressee will receive one invoice that combines several purchase or-
                                           ders.
                                           You can select at what intervals a collective invoice will be issued.
                                           – weekly
                                           – every 14 days
                                           – monthly
                                        Technical info: toggle field, DB field: kauf.rechnungsart

                                             Note regarding the creation of collective invoices
                                             Both the limit for collective invoices and the invoice recipient's consent to
                                             collective invoicing must be saved in the market partner master data.

                                        Partial Inv. Specification whether partial invoices are created after a partial
                                        delivery:
                                        • Y: permit partial invoices.
                                        • N: do not permit partial invoices.
                                        If you select Collective invoice in the Invoice Type field, and you permit partial
                                        invoices, goods shipped by partial shipment will be included in the next collec-
                                        tive invoice.
                                        Technical info: toggle field, DB field: kauf.teilfakkz

                                        Emergen.Purch Current purchase order receives preferential treatment and
                                        is dispatched to production with higher priority.
                                        • Y: define as high-priority purchase order.
                                        • N: do not assign higher priority for the purchase order.
                                        Technical info: toggle field, DB field: kauf.gbelad

                                        Print Gross Prices Gross prices are printed on market partner documents.
                                        • Y: print gross prices.
                                        • N: do not print gross prices.
                                        Technical info: toggle field, DB field: kauf.preisdrkz

                                        Print Customer Factor The customer-specific factor can be printed on mar-
                                        ket partner documents.
                                        • Y: print customer factor.
                                        • N: do not print customer factor.
                                        Technical info: toggle field, DB field: kauf.rabdrkz
5.00 / 12-2022




                                        Print Article Text The article texts can be printed on the market partner doc-
                                        uments.
                                        • Y: print product text.


                 A+W Enterprise Purchasing                                                                           E-63
                 Document Management                                                             Software Reference




                                       • N: do not print product text.
                                       Technical info: toggle field, DB field: kauf.atxtdrukz

                                       Print Shapes Print shape sketches for items in the attachment of the market
                                       partner documents.
                                       • Y: print shape sketch.
                                       • N: do not print shape sketch.
                                       Technical info: toggle field, DB field: kauf.moddrkz

                                       Suppress Item Prices By default, the item prices are printed on the market
                                       partner documents. You can suppress the listing of the item prices, e.g. if you
                                       have agreed on a fixed price with the supplier for the whole purchase order.
                                       • Y: do not print item prices.
                                       • N: print item prices.
                                       Technical info: toggle field, DB field: kauf.posdrkz

                                       Footer
                                       The fields in the footer area can only be entered on the Items tab. They are
                                       described for the Purchase Order Entry - Header, Footer tab:
                                        “Purchase Order Entry – Header, Footer” on page E-52
5.00 / 12-2022




                 E-64                                                                     A+W Enterprise Purchasing
                 Software Reference                                                                Document Management




                                          Purchase Order Entry – Miscellaneous
                                          Purchase > P.O. Management > Open Purchase Order > from Field Entry Data
                                          on > <F2> > Miscellaneous Tab




                 Fig. E-16   Purchase order entry – Miscellaneous tab


                                          Use this tab to view complaint information, private fields, additional options,
                                          and payment options.

                                          Header
                                          The fields in the header area are described for the Purchase Order Entry –
                                          Header, Footer tab:
                                           “Purchase Order Entry – Header, Footer” on page E-52

                                          Complaint Information
                                          You can maintain complaint statistics with the data. The Reason, Place, and
                                          Type of complaint must be created in the master data.

                                          Cause Number of the complaint type. If you select a number, the description
                                          of the complaint type is displayed in plain text, e.g. glass breakage.
                                          Technical info: numeric field, DB field: kauf.reklamart

                                          Place Number of the complaint place. If you select a number, the name of the
                                          complaint plas is displayed in plain text, e.g. unloading.
5.00 / 12-2022




                                          Technical info: numeric field, DB field: kauf.reklamort




                 A+W Enterprise Purchasing                                                                           E-65
                 Document Management                                                              Software Reference




                                       Type Number of the complaint type. If you select a number, the name of the
                                       complaint type is displayed in plain text, e.g. incorrect color.
                                       Technical info: numeric field, DB field: kauf.reklamspec

                                       Date Complaint date in the format DD.MM.YYYY.
                                       Technical info: date field, DB field: kauf.reklamdat

                                       Payment Options
                                       You can view the payment options that are transmitted by the supplier for the
                                       purchase order and edit them, if necessary. The payment options are deter-
                                       mined from the master data.

                                       Curr. Rate Number and name of the currency and currency rate. The price is
                                       calculated customer-specifically in the currency specified. If you select a num-
                                       ber, the currency name and currency rate are displayed in plain text. The Rate
                                       field is locked if Own Currency is selected.
                                       Technical info: mandatory field, numeric fields, DB fields: kauf.waehrung,
                                       kauf.kurs

                                       Calculate in This field is only enabled if Own Currency is not selected in the
                                       Currency field. You can specify whether the prices are calculated in own cur-
                                       rency or in the market partner's foreign currency:
                                       • Own Currency:
                                          The prices are calculated byA+W Enterprise in own currency.
                                       • Foreign Currency:
                                          The prices are calculated in the currency that is assigned to the market
                                          partner in the Currency field.
                                       Technical info: toggle field, DB field: kauf.waerprs

                                       Print in Number for printing the market partner-specific documents in the cal-
                                       culated currency or foreign currency. If you select a number, the name of the
                                       print option is displayed in plain text. If you select a number, the name of the
                                       print option is displayed in plain text.
                                       Technical info: numeric field, DB field: kauf.waehrdru

                                          The fields Calculate in and Print in
                                          The fields Calculate in and Print in are only accessible if the currency mod-
                                          ule is licensed.

                                       Pay. Term Payment term in days, which has been agreed upon with the mar-
                                       ket partner.
                                       Technical info: numeric field, DB field: kauf.zahlziel

                                       Val.Date Period until the value date in days.
                                       Technical info: numeric field, DB field: kauf.valuta

                                       Cash D.1, 2, 3 Keys for the cash discount rates for the payment term. You
5.00 / 12-2022




                                       can specify up to 3 different keys. This way, you can define scaled payment
                                       terms.




                 E-66                                                                     A+W Enterprise Purchasing
                 Software Reference                                                             Document Management




                                        Technical info: numeric fields, DB fields: kauf._skonto1, kauf._skonto2,
                                        kauf._skonto3

                                        Charact. Number of the form of payment, e.g. bank debit, bank booking. You
                                        store characteristics in the system master data as payment methods. If you
                                        specify a number, the name of the characteristic is displayed in plain text.
                                        Technical info: numeric field, DB field: kauf.zahlngmerk

                                        Payments Type and method of payment, e.g. upon delivery or by direct debit.
                                        The specifications for payment method are specified by the system.
                                        Technical info: toggle field, DB field: kauf.skontoart

                                        FIN. Key Key for transfer to financial accounting. The keys for financial ac-
                                        counting are entered by the system and sent to financial accounting.
                                        Technical info: alphanumeric field, DB field: kauf.fibukey

                                        FinAc Debtor Market partner's supplier number, which is intended as invoice
                                        recipient. The field is pre-populated by default.
                                        Technical info: numeric field, DB field: kauf.stddebnr

                                        Private fields
                                        The private fields are used customer-specifically for additional information.
                                        They can be configured at will. The field names are set via the environment
                                        variables. The two upper lines are numeric field; the two lower lines are free
                                        text fields.
                                        Technical info: numeric fields, alphanumeric fields, DB fields: kauf.pri-
                                        vate_long1, kauf.private_long2, kauf.private_char1, kauf.private_char2

                                        Further options

                                        Check Number of the employee who checks the document. If the field is filled,
                                        the documents will only be released after checking by the appropriate employ-
                                        ee.
                                        Technical info: numeric field: DB field: kauf.kontrollmanr

                                        Wind Load Wind load in the installation location. Wind load (N/m²) is the
                                        pressure applied by direct winds onto the external surface of a building. The
                                        system uses this value to perform a plausibility check to determine whether the
                                        thickness group of the selected glass types suffice for the wind load defined.
                                        The wind load can only be specified for glass with multiple lites.
                                        Technical info: numeric field, DB field: kauf.wlast

                                             Restriction check after input of wind load
                                             If an appropriate entry is created for the wind load in the master data, the
                                             specified wind load is subjected to a restriction check. A note will be dis-
                                             played should the restriction check reveal problems.
5.00 / 12-2022




                                        Facade Zone Specification of the facade zone in which the lites will be in-
                                        stalled. E.g. tall buildings or buildings on the outskirts are loaded with in-
                                        creased wind load.


                 A+W Enterprise Purchasing                                                                          E-67
                 Document Management                                                              Software Reference




                                       • 1 Edge: For buildings with increased wind load.
                                       • 2 Central: For buildings without increased wind load.
                                       Technical info: numerical field, DB field: kauf.bereich

                                       Min IG Tot.Thickn., Max. IG Tot.Thickn. Minimum and maximum glass
                                       thickness for the entire IG article in millimeters. The glass thickness depends
                                       on the selected facade zone and the wind load.
                                       Technical info: numeric fields, DB fields: kauf.minszr, kauf.maxszr

                                       Tight Size Correction size in millimeters. The tight size added to the width
                                       and height of the items. For example, for a glass with the dimensions 1050 mm
                                       x 1250 mm and a tight size of 2 mm, the dimensions 1052 mm x 1252 mm are
                                       stored in the database. The value is transferred to production. If you are work-
                                       ing with A+W Production, this value is generally ignored and the tight size is
                                       drawn from A+W Production.
                                       Technical info: numeric field, DB field: kauf.falzmass

                                       Quot. Status Status of the quotation. This field is only shown for quotations.
                                       If referenced, this field content is transferred.
                                       • open: quotation has not yet been confirmed.
                                       • won: quotation has been confirmed.
                                       • lost: inquiry has been rejected.
                                       • expired: quotation is no longer valid.
                                       Technical info: toggle field, DB field: kauf.angbstatus

                                       Text Formulas Number and description of the product labeling, e.g. spacer
                                       text. The text formulas must be created in the master data.
                                       Technical info: numeric field, DB field: kauf.artikennfrm

                                       Footer
                                       The fields in the footer area can only be entered on the Items tab. They are
                                       described for the Purchase Order Entry - Header, Footer tab:
                                        “Purchase Order Entry – Header, Footer” on page E-52
5.00 / 12-2022




                 E-68                                                                    A+W Enterprise Purchasing
                 Software Reference                                                                  Document Management




                                           Purchase Order Entry - Totals
                                           Purchase > P.O. Management > Find Purchase Order > Items Tab > General
                                           Tab > Price Field > <End> > Net Total Field > <F2>




                 Fig. E-17   Purchase order entry (totals)


                                           On this dialog, you define discounts, rebates, and surcharges for the entire
                                           purchase order and you can edit various payment options.
                                           Discounts are arranged with suppliers. You can define a generally applicable
                                           discount in the master data and allocate a supplier-specific discount to each
                                           supplier. For a purchase order with selected suppliers, the supplier-specific
                                           discount is always allocated first. If no discount has been defined for this sup-
                                           plier, the general discount is applied.
                                           The dialog is described in detail in the Sales section.
                                            Sales, “Order Entry - Totals” on page D-106
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                            E-69
                 Document Management                                                                  Software Reference




                                          Purchase Order Entry - Discounts Detailed View
                                          Purchasing > P.O. Management > Find Purchase Order > Items Tab > General
                                          Tab > Price Field > <End> > Net Total Field > <F2> >




                 Fig. E-18   Discounts detailed view


                                          Enter the details relating to the selected discount on this dialog.
                                          The dialog is described in detail in the Sales section.
                                           Sales, “Order Entry – Detailed View Discounts” on page D-111
5.00 / 12-2022




                 E-70                                                                        A+W Enterprise Purchasing
                 Software Reference                                                           Document Management




                                        Purchase Order Items
                                        Purchasing > P.O. Management > Open Purchase Order > Items Tab – Gen-
                                        eral Tab
                                        The Items tab offers the following tabs:
                                         “Purchase Order Items - General” on page E-72
                                         “Purchase Order Items - Properties” on page E-81
                                         “Purchase Order Items - Prices” on page E-84
                                         “Purchase Order Items - Order Info” on page E-87
                                         “Purchase Order Items - Status” on page E-88
                                         “Purchase Order Items - Evaluation” on page E-91
                                        On the item level, you can enter shapes, processings, steps, and muntin anew
                                        or view and change this information in the POs created. You can also view and
                                        adjust the sales prices for the items.
                                        The dialogs are described in detail in the Sales section.
                                         Sales, “Muntin Entry” on page D-229
                                         Sales, “Stepped Entry (Relevant Parts)” on page D-226
                                         Sales, “BOM View” on page D-198
                                         Sales, “Shape - Dimensions” on page D-180
                                         Sales, “Prices and Conditions” on page D-265
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                      E-71
                 Document Management                                                                   Software Reference




                                          Purchase Order Items - General
                                          Purchasing > P.O. Management > Open Purchase Order > Items Tab – Gen-
                                          eral Tab




                 Fig. E-19   Purchase order items - general


                                          In this area, you enter and edit the items of a purchase order. You can select
                                          the articles, the dimensions, quantity, and supply type and assign processings
                                          to the articles.
                                          In the event of a status change, a corresponding note regarding the purchase
                                          order status is shown at the level of the tab. In front of the Item field, the item
                                          status and if necessary the item code are displayed as traffic light.
                                           “Explanation of Symbols” on page E-47
                                          Order-related purchase orders and stock purchase orders are usually execut-
                                          ed using the Create Purchase Orders dialog and can be edited in the P.O.
                                          Management if required.
                                           “Creating Purchase Orders” on page E-38

                                          Header
                                          The fields in the header area are described for the Purchase Order Entry –
                                          Header, Footer tab:
                                           “Purchase Order Entry – Header, Footer” on page E-52
5.00 / 12-2022




                 E-72                                                                         A+W Enterprise Purchasing
                 Software Reference                                                              Document Management




                                        Items tab (left area)
                                        In the Info area, various information about the marked item is displayed. The
                                        technical values can be edited.
                                         “Items tab (Info area – graphic, technical values)” on page E-75




                                        Fig. E-20      Items tab (info area left)


                                        This area displays information about the marked item. The information about
                                        the header article is always displayed. All other information is only displayed if
                                        it exists. If no information exists, the corresponding position remains empty.

                                        Ref. Commission text for printing. The field can only be entered if the appro-
                                        priate flag is set for the article in the master data. For the first item, you can
                                        enter the commission text directly. If you enter a new item, the commission text
                                        of the previous item is taken over automatically. Alternatively, there are the fol-
                                        lowing possibilities:
                                        • Use <F4> > References > New Reference or Change Reference to create
                                            a new reference text via the supplementary menu or to change the existing
                                            reference text for the entire purchase order.
                                        • Use <Shift>+<F11> to change from the item level to the text entry for the
                                            reference in order to create a reference text for the selected item.
                                        Use <Enter> to change from the Commis field to the General tab, which is in
                                        the item area in order to continue item entry.
                                        Technical info: alphanumeric field, DB field: komm.kommtxt

                                             Inheriting reference text
                                             If you assign a reference text to an item with <Shift>+<F11>, the reference
                                             text can be taken over for all following items. For this, you have to confirm
                                             the query whether the reference should be inherited downward with [Yes].
                                             If you click [No], the reference text is only taken over for the current item.
                                             The query is only displayed if additional items are entered after the current
                                             item. However, it is not usual to enter the reference texts in the Purchase
                                             area. In the rules, the reference texts are transferred from Sales for order-
                                             related purchase orders.

                                        DoP: Declaration of performance. Description of the declaration of perfor-
                                        mance that is assigned to the article. The field is only displayed if a declaration
                                        of performance is assigned to the current article.
                                        Technical info: display field, DB field: kposp.lbrefnr
5.00 / 12-2022




                                        (CAD identifier) Identifier that indicates whether a CAD file is assigned to the
                                        item. If a CAD file is attached, the CAD identifier is displayed. For S/N items,
                                        the S/N code is displayed in brackets next to the CAD identifier.



                 A+W Enterprise Purchasing                                                                           E-73
                 Document Management                                                                 Software Reference




                                       Technical info: display field

                                       (Cost center) Designation of the cost center that is assigned to the item. If no
                                       cost center is assigned to the item, the market partner-specific cost center is
                                       used. If no cost center is assigned to the market partner, the main cost center
                                       will be used.
                                       Technical info: display field, DB field: kpos.kostenst

                                       (Muntin flag) Identifier that indicates whether muntins are entered in the
                                       item.
                                       • S:
                                          Muntins are entered in the item. The muntin structure was not edited.
                                       • E:
                                          Muntins are entered in the item. The muntin structure was edited in the ed-
                                          itor.
                                       • (no identifier):
                                          No muntins are entered in the item.
                                       Technical info: display field

                                       (Header, article) Description of the header article. With multiple glasses, in
                                       addition to the header article, the descriptions of the individual glasses are dis-
                                       played.
                                       Technical info: display field, DB field: aufstrukt.artbez1

                                       (Exchange, additional article, quantity1/quantity2) Description of the ex-
                                       change and additional articles and number of articles in the BOM. Exchange
                                       articles are displayed with an A, additional articles with a Z in front of the de-
                                       scription. Next to the article description, is is indicated how frequently the value
                                       width and how often the value height must be calculated for the article.
                                       Technical info: display fields, DB fields: aufstrukt.artbez1, aufstrukt.anzahl1,
                                       aufstrukt.anzahl2

                                       (Muntin exchange, muntin additional article, quantity1/quantity2) De-
                                       scription of the muntin exchange and/or muntin additional article and number
                                       of muntins in the BOM. Muntin exchange articles are marked with an A,
                                       muntin additional articles with a Z in front of the description. The quantity of
                                       horizontal and vertical muntins is displayed after the muntin description.
                                       Technical info: display fields, DB fields: aufstrukt.artbez1, aufstrukt.anzahl1,
                                       aufstrukt.anzahl2
5.00 / 12-2022




                 E-74                                                                       A+W Enterprise Purchasing
                 Software Reference                                                              Document Management




                                        Items tab (Info area – graphic, technical values)
                                        On the right side of the Items tab, depending on the system configuration and
                                        the settings, some of the following information is displayed:
                                             – Supply, product group and shape
                                             – Technical details
                                             – Hidden dimensions
                                        The information is displayed for the marked item.




                                        A Customer, product group, shape            B Shape, product structure
                                        Fig. E-21     Items tab (info area right)


                                        On the right, there is a schematic depiction of the product. If you have entered
                                        a shape and/or muntins in the item, a schematic product depiction is also dis-
                                        played on the left.

                                        Customer Customer name. The field is only displayed for order-related pur-
                                        chase order items.
                                        Technical info: display field, DB field: mp.name, kauf.kunr

                                        ProductGrp Product group number of the item. Articles are divided into prod-
                                        uct groups for product grouping and analysis of statistics. When you change
                                        the BOM of an item, the product group may also change.
                                        • Use <Ctrl>+<F9> to change from the item level to the input field of the prod-
                                           uct group.
                                        • Use <F9> to open the selection list for the product group. Alternatively, you
                                           can specify a product group number. A correction of the product group is
                                           only possible under certain circumstances.
                                        Technical info: display field, DB field: kpos.wgrp

                                        Shape Shape number.
                                        • Use <Ctrl>+<F12> to change from the item level to the input field for the
                                            shape number.
                                        • Open the Shape Catalog with <F2>.
                                        • Open a selection of shape names with <F9>.
                                        Alternatively, you can enter the shape number directly in the field. After spec-
                                        ifying a shape number, the shape entry begins. By default, the system is con-
                                        figured with the A+W shape catalog.
                                              Sales, “Shape - Dimensions” on page D-180
                                        Technical info: display field, DB field: kpos.modnr
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                        E-75
                 Document Management                                                                 Software Reference




                                       Technical details
                                       Use <F4> > Product Details > Technical Details to select one of the following
                                       entries on the additional menu:
                                       •   Show Technical Details:
                                           Displays the technical details of the selected item. If the selected item is al-
                                           ready assigned a declaration of performance, the Calculated Technical Val-
                                           ues tab opens.
                                            Sales, “Order Entry – Calculated Technical Values” on page D-190
                                       •   Change technical details:
                                           Changes to the input fields for the technical details of the selected item.
                                           You can edit the fields.
                                       Use <End> to save the changes and change back to the General tab.

                                       Item Item number of the selected item. The field is only displayed if you
                                       change the technical details.
                                       Technical info: display field, DB field: kpos.posnr

                                       Article Code Article code of the selected item. The field is only displayed if
                                       you change the technical details.
                                       Technical info: display field, DB field: ktechw.artnrgen

                                       Total Thickn. Glass thickness for the total article of the item. The glass thick-
                                       ness depends on the selected facade zone and the wind load. The entry is
                                       made in millimeters. The field is only displayed if you change the technical de-
                                       tails.
                                       Technical info: numeric field, DB field: ktechw.dicke

                                       Wind Load Wind load in the installation location. Wind load (N/m²) is the
                                       pressure applied by direct winds onto the external surface of a building. The
                                       system uses this value to perform a plausibility check to determine whether the
                                       thickness group of the selected glass types suffice for the wind load defined.
                                       The field is only displayed if you change the technical details.
                                       Technical info: numeric field, DB field: ktechw.wlast

                                       Section Specification of the facade zone in which the lites will be installed.
                                       E.g. tall buildings or buildings on the outskirts are loaded with increased wind
                                       load. The field is only displayed if you change the technical details.
                                       • Edge:
                                          For buildings with increased wind load.
                                       • Central:
                                          For buildings without increased wind load.
                                       Technical info: toggle field, DB field: ktechw.bereich
                                       If you edit the technical details, additional fields are displayed with <F2>.

                                       U Val. DIN Heat transmission coefficient according to DIN standard. Central
                                       dimensional unit for determining the heat loss of a component. The measure-
5.00 / 12-2022




                                       ment unit is W/m²K. The lower the Ug value, the greater the heat insulation.
                                       Technical info: numeric field, DB field: ktechw.kwert



                 E-76                                                                       A+W Enterprise Purchasing
                 Software Reference                                                              Document Management




                                        Ug Value Heat transmission coefficient.
                                        Technical info: numeric field, DB field: ktechw.kbazwert

                                        Transmiss. Light transmission for the percentage of rays that are allowed to
                                        pass through. The reference value of 100 % is an unglazed hole in the wall.
                                        Technical info: numeric field, DB field: ktechw.trwert

                                        g Value Energy transmission coefficient (total transmittance). The variable is
                                        composed of direct solar energy transmission and secondary heat emission to
                                        the inside, as a result of slow radiation and convection.
                                        Technical info: numeric field, DB field: ktechw.gwert

                                        dB Value Sound insulation value of the item in decibels.
                                        Technical info: numeric field, DB field: ktew.dbwert

                                        Hidden dimensions
                                        Use <F4> > Product Details > Technical Details to select one of the following
                                        entries on the additional menu:
                                        •    Show hidden dimensions:Displays the hidden dimensions of the selected
                                             item next to the graphic display of the item, e.g. the spacer deduction di-
                                             mension.
                                        •    Change hidden dimensions:
                                             Opens the Item dimensions dialog where you can edit the various dimen-
                                             sions of the item.
                                        Depending on the item selected, various parameters are listed. Use [OK] or
                                        <End> to save the changes and close the dialog.
                                        The fields are described in detail in connection with the Article-Dimensions di-
                                        alog.
                                         Sales, “Article Dimensions” on page D-153

                                        Graphic display of the item
                                        Various previews are displayed for the item:
                                        •    Schematic view:
                                             Shows the lite structure as a cross-section. The sun marks the outside of
                                             the lite. The schematic structure of the item is always displayed.
                                        •    Top view:
                                             Displays the lite shape and/or the muntin construction of the lite in the top
                                             view. The top view is only displayed if you have entered a shape and/or
                                             muntins in the item.

                                        General tab
                                        The layout of the item level, especially on the General tab depends on the ar-
                                        ticle type that you select. This way, some fields are shown or hidden, e.g.: AIR.
                                        The following fields are available:
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                          E-77
                 Document Management                                                                 Software Reference




                                       Itm Item number. Displayed in front of the Itm column, are the item status and
                                       if necessary the item code of the item in question. The item status is only dis-
                                       played after saving the document.
                                       Technical info: numeric field, DB field: kpos.lfdpos

                                       Supp. Item Supplier item. Specification of the item description from the sup-
                                       plier's item list. The field is only enabled if the entry yes is selected in the Sup-
                                       pl.Item field of the header area.
                                       The item description can be printed on all customer and supplier-side docu-
                                       ments.
                                           “Purchase Order Entry – Header, Footer” on page E-52
                                          Alternatively, you can enter the article name of an existing, fixed-size arti-
                                          cle. The system then pre-populates the fields with the article data.
                                           Sales, Software Reference, “Article Details for Dimensioned Variants” on
                                            page D-164
                                       Technical info: numeric field, DB field: kpos.kuposnr

                                       Article •Article number. In the Article field you can enter a customer- or sup-
                                          plier-specific article number.
                                          – Use <F9> to open the article search.
                                          – Search for customer-specific articles with <F10>.
                                           Sales, Software Reference, “Article Details for Dimensioned Variants” on
                                            page D-164
                                       Technical info: mandatory field, numeric field, DB field: kpos.artnr

                                          Assign original or new BOM
                                          You can assign the article the original BOM or a new BOM. The BOM num-
                                          ber is assigned accordingly. With <F5> in the Article field, you take over the
                                          article's original BOM. With <Shift>+<F5> in the Article field, you assign the
                                          article a new BOM. The article is assigned the next free BOM number by
                                          the system. In the rules, the product BOM in the Sales area is not adjusted.

                                       BMno BOM number of the article. By default, the number is assigned auto-
                                       matically. The BOM includes all parts and processings required for manufac-
                                       turing of the article. Every item in the BOM automatically gets a unique BOM
                                       number which is shown in field BOMNo. After the quantity and the dimensions
                                       of the item were specified, you can use <F3> to display and edit the item's
                                       BOM. The entry in this field has an influence on the price calculation. The field
                                       is locked.
                                           Sales, “Item Processing” on page D-221
                                       Technical info: numeric field, DB field: kpos.poskonr

                                       Quantity Units of the item. For articles with stored dimension, color or thick-
                                       ness variants, after entry of the quantity, a dialog opens for selection of the re-
                                       spective variant.
                                           Sales, “Variant and Color/Thickness Selection” on page D-167
                                       Technical info: mandatory field, numeric field, DB field: kpos.menge
5.00 / 12-2022




                                       Width, Height, AIR Width, height, and airspace in the dimensional units
                                       stored for the article. For variant articles, the system takes the dimensions
                                       from the article master data using the selected variant number. If you change


                 E-78                                                                       A+W Enterprise Purchasing
                 Software Reference                                                              Document Management




                                        these dimensions, the query appears: Can the variant reference really be re-
                                        moved?
                                           – Click on [No] to reset the entered sizes to the stock sizes.
                                           – Click [Yes] to change the stock sizes. This can cause problems in the
                                              warehouse and with pricing.
                                        Technical info: mandatory fields, numeric fields, DB fields: kpos.laenge,
                                        kpos.breite, kpos.szr

                                        (Columns without name) For length, time, and piece articles, instead of
                                        width, height, and AIR, the dimension and corresponding dimension unit that
                                        are assigned to the selected article are displayed. The dimension unit of the
                                        article is drawn from the master data and cannot be edited. For installation
                                        work, for example, the dimension unit hr (hours) is displayed, for gas fillings l
                                        (liters) and for adhesive tape m (meters). You can select the dimension at will.
                                        Technical info: mandatory field, numeric field, DB field: kpos.laenge

                                             Calling up BOM of the item
                                             Use <F3> or <F5> to open the BOM for the selected item. You can only
                                             open the BOM after you have specified the dimension. If you try to open the
                                             BOM before that, the system will notice this action and open the BOM au-
                                             tomatically after specification of the dimension. In addition to the item, you
                                             will see a gray checkbox. A message with this information will also be dis-
                                             played.

                                        SN The checkbox indicates whether an SN file is assigned to the item.

                                        Comm Commission with active representative commission. You can specify
                                        the commission key granted for each item individually. With inactive or margin-
                                        oriented commission calculation, the field is locked and will not be considered.
                                        Technical info: numeric field, DB field: kpos.provnr

                                        PType The supply type determines how an article is supplied. In purchasing,
                                        the field is pre-populated with the supply type PO and cannot be changed.
                                        Technical info: Toggle field, database field: kpos.beschaffart

                                        lbs/Pc, Qty/Pc Quantity unit in kilograms per piece, quantity unit in square
                                        meters per piece.
                                        Use <Ctrl>+<M> in Price filed to change the display of the field.
                                        Technical info: display field, DB field: kpos.gewme

                                        Price(field) Net price per item. The column name varies depending on the
                                        own currency and configuration, e.g. Price/piece, Price/m2. The system calcu-
                                        lates the total price of the item including the conditions in the selected curren-
                                        cy. You determine the currency in the Currency/Rate field on the
                                        Miscellaneous tab.
                                            – Use <Shift>+<F11> to change the display of the field.
                                            – Use <Shift>+<F8> to save the order in the master data as fixed dimen-
                                               sion product.
5.00 / 12-2022




                                                 Sales, “Article Details for Dimensioned Variants” on page D-164
                                             – Use <Ctrl>+<F9> to determine the PU price with the item conditions and
                                               recalculate the price.


                 A+W Enterprise Purchasing                                                                           E-79
                 Document Management                                                                 Software Reference




                                          – Use <F3> to display an overview of the dimensions of the individual
                                            items.
                                              Sales, “Dimensions of Individual BOM Elements” on page D-222
                                       Technical info: numerical field, DB field: kpos.nstpreis
                                       The following columns display on the tab if you use <F4> > Price info > Price
                                       check:

                                       SA Pre-sales price code from the transferring site.
                                       Technical info: display field, DB field: kpos.vorvkpkz

                                       PCD Pre-sales price code from the transferring site.
                                       Technical info: display field, DB field: kpos.vorpkz

                                       nSA Newly determined sales price code.
                                       Technical info: display field, DB field: kpos.neuvkpkz

                                       pSF Pre-sales price factor from the transferring site.
                                       Technical info: display field, DB field: kpos.vorvkfaktor

                                       Factor Percentage pre-sales factor from the transferring site.
                                       Technical info: display field, DB field: kpos.vorfaktor

                                       nSF Newly determined sales factor.
                                       Technical info: display field: DB field: kpos.neuvkfaktor

                                       pSA-Pr. Pre-sales price from the transferring site.
                                       Technical info: display field, DB field: kpos.vorpreis

                                       nSA-Pr. Newly determined sales price.
                                       Technical info: display field, DB field: kpos.neuvknstpreis
                                       With <F4> > Stock> Stack you can show the following field with the right sys-
                                       tem configuration.

                                       Stack Stack ID of the article that is obtained from the stack warehouse.
                                       Use <Shift> + <F4> > Note to display an additional field:

                                       Note You can enter information about the item. The information will be dis-
                                       played in OrderInfo tab.
                                       If you select the box warehouse in the Warehouse field on the Properties tab
                                       and the system is configured appropriately, the following fields are shown:

                                       NB Number of boxes.

                                       Lite Number of lites per box.

                                       PT ID of the packing type Box.
5.00 / 12-2022




                 E-80                                                                     A+W Enterprise Purchasing
                 Software Reference                                                                 Document Management




                                           Footer
                                           The fields in the footer area are described for the Purchase Order Entry –
                                           Header, Footer tab:
                                            “Purchase Order Entry – Header, Footer” on page E-52


                                           Purchase Order Items - Properties
                                           Purchasing > P.O. Management > Find Purchase Order > Items Tab
                                           > Properties Tab




                 Fig. E-22   Purchase order item - properties


                                           On this tab, you can view and edit the properties of the current item, e.g. ware-
                                           house assignment, packing type. You enter the properties individually for each
                                           item. Generally you do not have to edit the details on the Properties tab.
                                           Use <Page Up> and <Page Down> to change to the previous and next item.
                                           In the event of a status change, a corresponding note regarding the purchase
                                           order status is shown at the level of the tab, e.g. Ordered Local – Correction.
                                           In front of the Item column, the item status and if necessary the item code are
                                           displayed.
                                            “Explanation of Symbols” on page E-47

                                           Header
5.00 / 12-2022




                                           The fields in the header area are described for the Purchase Order Entry –
                                           Header, Footer tab:
                                            “Purchase Order Entry – Header, Footer” on page E-52



                 A+W Enterprise Purchasing                                                                            E-81
                 Document Management                                                                Software Reference




                                       Properties tab
                                       The columns are described for the General tab:
                                        “Purchase Order Items - General” on page E-72
                                       In addition, the following fields are displayed:

                                       Description Description of the header article. You can edit the name. The
                                       change is only taken over purchase order-related.
                                       Technical info: alphanumeric field, DB field: kpos.artbez1

                                          Changes to the description
                                          Once changed in this item, the article description will appear on all pur-
                                          chase order-related documents and on all purchase order-related dialogs
                                          for this document.

                                       Cost Center Cost center name for statistical evaluations.
                                       Technical info: alphanumeric field, DB field: kauf.kostenst

                                       DOP Number Number for declaration of performance. You can select or reg-
                                       ister a new number. Use <Ctrl>+<T> to open the Calculated technical details
                                       tab where you can enter a new declaration of performance. You can only reg-
                                       ister a new number if the item has not yet been assigned a declaration of per-
                                       formance. A declaration of performance can only be entered if the system is
                                       configured appropriately.
                                        Sales, “Order Entry – Calculated Technical Values” on page D-190
                                       Technical info: alphanumeric field, DB field: kpos.lbrefnr

                                       Warehouse Number of the warehouse where the article is located. If you se-
                                       lect a number, the description of the warehouse is displayed in plain text.
                                       Technical info: numeric field, DB field: kpos.lnr

                                       Stack Number of the stack warehouse where the article is located. If you se-
                                       lect a number, the description of the stack warehouse is displayed in plain text.
                                       The stack warehouse is only enabled customer-specifically.
                                       Technical info: numeric field, DB field: kpos.sfill1

                                       Box Number of the box warehouse where the article is located. Only com-
                                       plete boxes of an article are entered in the box warehouse. If articles from a
                                       box are required, the remaining lites are booked to the normal stock. If you
                                       select a number, the description of the box warehouse is displayed in plain
                                       text. The box warehouse is only enabled customer-specifically.
                                       Technical info: numerical field, DB field: bpos.kistennr

                                       Slot Name of the slot warehouse where the article is located. Usually, slot
                                       warehouses are used for articles that are billed by pieces or quantities, e.g.,
                                       handles, spacers. The slot warehouse is only enabled customer-specifically.
                                       Technical info: numerical field, DB field: bpos.fach
5.00 / 12-2022




                                       CE Code CE code. You can enter or change a descriptive text. The text is
                                       added to the CE code.
                                       Technical info: alpha-numerical field, database field: kpos.steuerzu


                 E-82                                                                     A+W Enterprise Purchasing
                 Software Reference                                                            Document Management




                                        Account Description of the cost center booking account.
                                        Technical info: alphanumeric field, DB field: kposp.mankonto

                                        Reject Reason Number of reject reason. The number only needs to be spec-
                                        ified if an item needs to be ordered due to glass breakage. If you specify a
                                        number, the reject name is displayed in plain text.
                                        Technical info: numeric field, display field, DB field: bpos.bruch

                                        Reject Place Number and name of the reject place where the glass break
                                        happened. The number only needs to be specified if an item needs to be reor-
                                        dered due to glass breakage. Generally the reject place is transferred from
                                        production and taken over in this field. If needed, you can change the reject
                                        place in A+W Enterprise. The reject place name is displayed in plain text in the
                                        next field.
                                        The reject places are stored in the database table xbruchort. The values from
                                        production are taken over automatically. There is no maintenance dialog for
                                        this table in A+W Enterprise.
                                        Technical info: numeric field, display field, DB field: bestpool.bruchort

                                        Print Sketch Type of the sketch, e.g. SNLive. You can select none, one or
                                        several sketch types. The sketch types can be configured in the system. The
                                        sketch printing can be activated for SN Live sketches, BOMs (AWBom),
                                        sketches for muntins (AWDesign) or schematic sketches (outline). An individ-
                                        ual sketch is printed for each sketch type.
                                        • Open the list of sketch types with <F9>.
                                        • Use the arrow keys to navigate between the sketch types.
                                        • Use <Space> to mark a sketch type.
                                        Use <End> to close the dialog and take over the selection.
                                        Technical info: selection field, DB field: ipos.imagedrkz.
                                        In this field, there is a 4-digit number, in which each place indicates an appro-
                                        priate sketch activation with a 1:
                                        • 1st digit: SNLive sketch.
                                        • 2nd digit: AWBom.
                                        • 3rd digit: AWDesign.
                                        • 4th digit: Outline sketch.

                                        lbs/QU, lbs/Piece, lbs/Item, lbs/Gl Weight of the item. The details can be
                                        displayed in the following fields:
                                        • kg/QU: kilogram per quantity unit
                                        • kg/Piece: kilogram per piece
                                        • kg/Item: kilogram per item
                                        • kg/Gl: kilogram per glass
                                        Only the field is enabled whose weight specification is assigned in the master
                                        data of the current article.
                                        Technical info: numeric fields, DB fields: kpos.gewme, kpos.gewst, kpos.gew-
                                        pos, kpos.gewglas
5.00 / 12-2022




                                        Actual QU/Pc Physical quantity in quantity unit per piece.
                                        Technical info: numeric field, DB field: kpos.phymestk


                 A+W Enterprise Purchasing                                                                         E-83
                 Document Management                                                                 Software Reference




                                           Chargd. QU/Pc Calculated quantity in quantity unit per piece.
                                           Technical info: numeric field, DB field: kpos.qm

                                           Pack. Type Number of the packing type, e.g. box. If you select a number, the
                                           description is displayed in plain text.
                                           Technical info: numeric field, DB field: kpos.verpackart

                                           Footer
                                           The fields in the footer area are described for the Purchase Order Entry –
                                           Header, Footer tab:
                                            “Purchase Order Entry – Header, Footer” on page E-52


                                           Purchase Order Items - Prices
                                           Purchase > P.O. Management > Open Purchase Order > Items Tab > Prices
                                           Tab




                 Fig. E-23   Purchase order item - prices


                                           This tab shows the purchase prices of the current item. The prices are dis-
                                           played individually for each item.
                                           Use <Page Up> and <Page Down> to change to the previous and next item.
                                           Usually, you do not need to open the Prices tab. If you want to edit the prices
                                           of the items, you have to edit the order and/or item conditions.
                                            Sales, “Conditions for PCD Processing” on page D-283
5.00 / 12-2022




                                            Sales, “Conditions for PCD Processing” on page D-283




                 E-84                                                                        A+W Enterprise Purchasing
                 Software Reference                                                                   Document Management




                                        In the event of a status change, a corresponding note regarding the purchase
                                        order status is shown at the level of the tab, e.g. Ordered Local – Correction.
                                        In front of the Item column, the item status and if necessary the item code are
                                        displayed.
                                         “Explanation of Symbols” on page E-47

                                        Header
                                        The fields in the header area are described for the Purchase Order Entry –
                                        Header, Footer tab:
                                         “Purchase Order Entry – Header, Footer” on page E-52

                                        Prices tab
                                        The columns are described for the General tab:
                                         “Purchase Order Items - General” on page E-72
                                        In addition, the following fields are displayed:

                                        Price/QU Price per quantity unit. The price is calculated from the glass price
                                        plus the surcharge.
                                        Technical info: display field, DB field: kpos.ekbmepreis

                                        Gross Pieces Gross price per piece.
                                        Technical info: display field, DB field: kpos.bmstpreis

                                        Factor Factor for the price surcharge in percent. Using the factor, you can
                                        change the price calculation for the article without having to adjust all prices,
                                        e.g. for price increases or discounts. Generally a discount is granted with a
                                        factor. Therefore, the factor is <100 %.
                                         Sales, “Conditions for PCD Processing” on page D-283
                                        Technical info: display field, DB field: kpos.ekfaktor

                                             Example

                                             If a supplier gives a discount of 10%, the corresponding value for the factor is
                                             90%.


                                        Net Pieces Net price per piece.
                                        Technical info: display field, DB field: kpos.eknstpreis

                                        Glazing/Pc. Price per piece for glazing or installation work.
                                        Technical info: display field, DB field: kpos.ekverglas

                                        Total Price Net total price of item. The total price is calculated from piece
                                        price x quantity of the article.
                                        Technical info: display field, DB field: kpos.vorrabatt
5.00 / 12-2022




                                        Minus Minus. Individually agreed upon discount for the item. You can specify
                                        the discount in the first field as percentage or in the second field as amount.
                                        The system calculates the value for the other fields.


                 A+W Enterprise Purchasing                                                                                  E-85
                 Document Management                                                                Software Reference




                                       Technical info: numerical fields, DB fields: kpos.rabatt, kpos.nachlass

                                       Item Price Item price. The item price is calculated from the total price less the
                                       discount from the Discount field. You can overwrite this value, e.g. if a flat fee
                                       has been agreed upon. If you change the item price, the discount in the Dis-
                                       count field is adjusted automatically.
                                       Technical info: numeric field, DB field: kpos.npospreis

                                       Tax Rates ID of the VAT rate per item. You can assign one VAT rate for each
                                       item.
                                       • Open the list of VAT rates with <F9>.
                                       • You can select a VAT rate with <space> (spacebar).
                                       • Save the VAT rate with <End>.
                                       Technical info: selection field, DB field: kpos.steuerzu

                                       Footer
                                       The fields in the footer area are described for the Purchase Order Entry –
                                       Header, Footer tab:
                                        “Purchase Order Entry – Header, Footer” on page E-52
5.00 / 12-2022




                 E-86                                                                     A+W Enterprise Purchasing
                 Software Reference                                                                 Document Management




                                           Purchase Order Items - Order Info
                                           Purchase > P.O. Management > Open Purchase Order > Items Tab > Order
                                           Info Tab




                 Fig. E-24   Purchase order item - order info


                                           This tab shows the referenced order information for the current item. The order
                                           information is displayed individually for each item.
                                           In the event of a status change, a corresponding note regarding the purchase
                                           order status is shown at the level of the tab.
                                            “Explanation of Symbols” on page E-47

                                           Header
                                           The fields in the header area are described for the Purchase Order Entry –
                                           Header, Footer tab:
                                            “Purchase Order Entry – Header, Footer” on page E-52

                                           Order info tab
                                           The fields are described for the General tab.
                                            “Purchase Order Items - General” on page E-72
                                           In addition, the following fields are displayed:
5.00 / 12-2022




                                           Cust.Order, Item Order number and item number of order-related purchase
                                           orders.
                                           Technical info: numeric fields, DB fields: bpos.vkauftrnr, bpos.vklfdpos



                 A+W Enterprise Purchasing                                                                          E-87
                 Document Management                                                              Software Reference




                                       Cst.Project Project number of the customer order for order-related purchase
                                       orders. If you specify a number, the description of the project is displayed in
                                       plain text.
                                       Technical info: numeric field, display field, DB field: bpos.vkobjnr

                                       Orig. Tupel Parts number of the BOM item of the customer order.
                                       Technical info: numerical field, DB field: bpos.orgtnr

                                       Note Additional information on the item.
                                       Technical info: alpha-numerical field, DB field: bpos.bemerkung

                                       Delivery Date Desired delivery date of the item.
                                       Technical info: Date field, DB field: bpos.ltideal

                                       Sched. Planned delivery date of the item.
                                       Technical info: Date field, DB field: bpos.ltplan

                                       Confirmed Delivery date of the item confirmed by the supplier.
                                       Technical info: Date field, DB field: bpos.ltavis

                                       Confirmed Qty. Quantity of the delivery item as confirmed by the supplier.
                                       This confirmed quantity may differ from the ordered quantity.
                                       Technical info: Date field, DB field: bpos.avismenge

                                       OC No.Suppl. Number of order confirmation from supplier.
                                       Technical info: numerical field, DB field: bpos.abnr

                                       Sup.Art.No. Supplier's article number. If a supplier-related article number
                                       has been entered for this article in master data, this is shown here.
                                       Technical info: alpha-numerical field, DB field: bpos.exartnr

                                       DN No. Supplier's delivery note number.
                                       Technical info: alpha-numerical field, DB field: bpos.lieferschein

                                       PurchDescr Supplier-specific article description. If the article name used by
                                       the supplier has been entered for this article in the master data, it is shown
                                       here.
                                       Technical info: alpha-numerical field, DB field: bpos.bestellbez

                                       Footer
                                       The fields in the footer area are described for the Purchase Order Entry –
                                       Header, Footer tab:
                                        “Purchase Order Entry – Header, Footer” on page E-52


                                       Purchase Order Items - Status
5.00 / 12-2022




                                       Purchase > P.O. Management > Open Purchase Order > Items Tab > Status
                                       Tab




                 E-88                                                                      A+W Enterprise Purchasing
                 Software Reference                                                                 Document Management




                 Fig. E-25   Purchase order item - status


                                           This tab shows the status of the items, e.g. number of articles delivered and
                                           invoiced. As first item in the item overview, the item is displayed that is marked
                                           on the General tab. Generally you do not have to edit the details on the Status
                                           tab.
                                            Use the arrow keys and <Page Up>, <Page Down> to navigate in the item
                                           overview.
                                           In the event of a status change, a corresponding note regarding the purchase
                                           order status is shown at the level of the tab, e.g. Ordered Local – Correction.
                                           In front of the Item column, the item status and if necessary the item code are
                                           displayed.
                                            “Explanation of Symbols” on page E-47

                                           Header
                                           The fields in the header area are described for the Purchase Order Entry –
                                           Header, Footer tab:
                                            “Purchase Order Entry – Header, Footer” on page E-52

                                           Status tab
                                           Some fields are described for the General tab.
                                            “Purchase Order Items - General” on page E-72
                                           In addition, the following fields are displayed:
5.00 / 12-2022




                                           Complt Display of the units produced per item.
                                           Technical info: display field, DB field: kpos.gesfert


                 A+W Enterprise Purchasing                                                                             E-89
                 Document Management                                                              Software Reference




                                       Packed Display of the units packed and prepared for transport per item.
                                       Technical info: display field, DB field: kpos.gespack

                                       Deliv. Display of the units delivered per item.
                                       Technical info: display field, DB field: kpos.geslief

                                       Calc Display of the invoiced units per item.
                                       Technical info: display field, DB field: kpos.gesberech

                                       Cancel Display of the canceled units per item.
                                       Technical info: display field, DB field: kpos.gesstorno

                                       Footer
                                       The fields in the footer area are described for the Purchase Order Entry –
                                       Header, Footer tab:
                                        “Purchase Order Entry – Header, Footer” on page E-52
5.00 / 12-2022




                 E-90                                                                      A+W Enterprise Purchasing
                 Software Reference                                                                Document Management




                                          Purchase Order Items - Evaluation
                                          Purchase > P.O. Management > Open Purchase Order > Items Tab > Evalua-
                                          tion Tab




                 Fig. E-26   Purchase order item - evaluation


                                          On this tab, you display details about the delivery, e.g. how reliably the supplier
                                          delivers. You store the assessment criteria in the supplier master data. You
                                          can enter the corresponding fields for supplier assessment with <Ctrl> + <N>
                                          and change them if necessary.

                                          Header
                                          The fields in the header area are described for the Purchase Order Entry –
                                          Header, Footer tab:
                                           “Purchase Order Entry – Header, Footer” on page E-52

                                          Evaluation Tab
                                          Some fields are described for the General tab.
                                           “Purchase Order Items - General” on page E-72
                                          In addition, the following fields are displayed:

                                          Date Evaluation of the supplier's adherence to delivery dates for the item.
                                          Technical info: alpha-numerical field, DB field: bpos.abnr
5.00 / 12-2022




                                          Prices Evaluation of the supplier's pricing for the item.
                                          Technical info: alpha-numerical field, DB field: bpos.wpreis


                 A+W Enterprise Purchasing                                                                             E-91
                 Document Management                                                              Software Reference




                                       Quality Evaluation of the quality of the delivered item.
                                       Technical info: alpha-numerical field, DB field: bpos.wqual

                                       Qty. Evaluation of the delivered quantity of the item.
                                       Technical info: alpha-numerical field, DB field: bpos.wmenge

                                       Special Evaluation of the supplier and the handling process.
                                       Technical info: alpha-numerical field, DB field: bpos.wspec

                                       Footer
                                       The fields in the footer area are described for the Purchase Order Entry –
                                       Header, Footer tab:
                                        “Purchase Order Entry – Header, Footer” on page E-52



                                       Pick-up Address
                                       Purchase > P.O. Management > Open Purchase Order > Field Entry Date >
                                       <F4> > Addresses > Pick-up Address




                                       Fig. E-27    Pick-up address


                                       On this dialog, you enter a pick-up address. If you would like to pick up the
                                       goods yourself, you can store the pick-up address here.

                                       Name, 1stName Customer's last name and first name.
                                       Technical info: mandatory field, alphanumeric fields, DB fields: adr.adrname,
5.00 / 12-2022




                                       adr.adrvname




                 E-92                                                                    A+W Enterprise Purchasing
                 Software Reference                                                                Document Management




                                        Title Number of the customer's title. If you specify a number, the title is dis-
                                        played in plain text.
                                        Technical info: numeric field, DB field: adr.anrede

                                        Attn. Contact's name.
                                        Technical info: alphanumeric field, DB field: adr.zhd

                                        Additional Additional information on the address.
                                        Technical info: alphanumeric field, DB field: adr.branche

                                        Street Street address of the pick-up address.
                                        Technical info: alphanumeric field, DB field: adr.str

                                        P.O. Box Postal code and P.O. box number.
                                        Technical info: alphanumeric fields, DB fields: adr.pfplz, adr.postfach

                                        PBoxCity P.O. box code for the pick-up address (for customers outside Eu-
                                        rope).
                                        Technical info: alphanumeric field, DB field: adr.pfort

                                        Post Code Postal code of the pick-up address.
                                        Technical info: alpha-numerical field, DB field: adr.plz

                                        City City of the pick-up address.
                                        Technical info: alpha-numerical field, DB field: adr.ort

                                        CCd Country International vehicle registration number of the country of des-
                                        tination. If you specify a code, the country name is displayed in plain text.
                                        Technical info: alphanumeric field, DB field: adr.lfzcode

                                        Distance Distance to the supplier in kilometers.
                                        Technical info: numeric field, DB field: adr.kilometer

                                        Travel Time Travel time to the supplier in days.
                                        Technical info: numeric field, DB field: adr.fahrtzeit

                                        Handling Time Time for loading and unloading the shipment.
                                        Technical info: numeric field, DB field: adr.handlingszeit

                                        Arrival Time Requested arrival time to supplier in format hh.mm.
                                        Technical info: alphanumeric field, DB field: adr.ankunftszeit

                                        Unloading Point Details of the shipping address, e.g. gate A.
                                        Technical info: alpha-numerical field, DB field: adr.anlieferstelle

                                        Fax No. Fax number of the supplier
                                        Technical info: alphanumeric field, DB field: adr.fax
5.00 / 12-2022




                                        Route Number of the route.
                                        Technical info: numeric field, DB field: adr.routenr


                 A+W Enterprise Purchasing                                                                         E-93
                 Document Management                                                               Software Reference




                                       Load.Seq. Number of the desired loading sequence. By default, the loading
                                       sequence is specified in shipping control. If you specify a number, it is trans-
                                       ferred to shipping control and considered in route planning.
                                       Technical info: numeric field, DB field: adr.routeposnr

                                       Remark Text fields for additional information.
                                       Technical info: alphanumeric fields, DB fields: adr.text1, adr.text2, adr.text3
5.00 / 12-2022




                 E-94                                                                     A+W Enterprise Purchasing
                 Software Reference                                                               Document Management




                                        PO Type
                                        Purchase > PO Management > Open Purchase Order > Project Field > <Ctrl>
                                        + <F12>




                                        Fig. E-28      Purchase order. types


                                        On this dialog, you specify the type of PO. By default, each PO has the PO
                                        type normal. If you select another PO type, it is displayed as dialog name in
                                        the header line of the dialog. Depending on the system configuration, the sys-
                                        tem may be able to change the PO type. The changed PO type will also appear
                                        as dialog name here.
                                        •    Normal purchase order:
                                             Preset default for purchase order entry that also applies to stock P.O.s.
                                        •    Internal purchase order:
                                             Internal purchase order between the own sites.
                                        •    Purchase order free-of-charge:
                                             Purchase order with the invoice amount 0, e.g. in the event of a complaint
                                             of a purchase order. At the end of the entry, a dialog for specification of the
                                             complaint reason opens.
                                              Sales, “Complaint” on page D-161
                                        •    Forwarding purchase order:
                                             This type is no longer supported!
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                            E-95
                 Document Management                                                                  Software Reference




                                          Allocation of Document Types
                                          Purchase > P.O. Management > Open Purchase Order > Suppl. Item Field >
                                          <Ctrl> + <K>
                                          Purchase > P.O. Management > Open Purchase Order > Items Tab > General
                                          Tab > Prices Field > <Ctrl> + <K>




                 Fig. E-29   Allocation of document types


                                          On this dialog you assign files to a document or individual items. If you want
                                          to assign the file to the complete document, you have to open the dialog in the
                                          header area. If you want to assign the file to a particular item in the document,
                                          you have to open the dialog on the General tab in the document entry and
                                          open the appropriate item.
                                          The assigned files are only displayed if you open the document type assign-
                                          ment for the document or the corresponding item. That is, documents that are
                                          assigned to the complete document are only displayed if the dialog is opened
                                          in the header area. Documents that are assigned to an item are only displayed
                                          if the dialog is opened in the corresponding item.
                                          The dialog is described in detail in the Sales section.
                                           Sales, “Allocation of Document Types” on page D-172

                                              Document allocation from the order
                                              In the order entry, the allocated documents can be marked both on the
                                              header level and on the item level for takeover for the PO generated. For
                                              this, the checkbox PO activated must be enabled. This copies the allocated
                                              document to the new PO.
5.00 / 12-2022




                 E-96                                                                        A+W Enterprise Purchasing
                 Software Reference                                                                                Texts




                                        Texts
                                        Use texts to define additional information about document. The texts can be
                                        printed out on different forms. The menu items where you can view and man-
                                        age the texts are the same in purchase and sales. They are described in detail
                                        in the Sales section.
                                         Sales, “Notes” on page D-247
                                         Sales, “Header and Footer Texts” on page D-256
                                         Sales, “Article and Item Texts” on page D-258
                                         Sales, “Special Texts” on page D-259
                                         Sales, “Phrases” on page D-260
                                         Sales, “External Information” on page D-262



                                        Order Texts
                                        Purchase > Create Purchase Orders > Select Department > <F3> > <Shift> +
                                        <F4> > Show Order Texts




                                        Fig. E-30    Order texts


                                        On this dialog, the order texts for the PO articles are displayed. For a PO item,
                                        item and/or article texts from the associated order can be taken over. Article
                                        texts are marked with the letter A, item texts with the letter P.
                                        On the Create POs dialog, there is an indication in the Txt column whether
                                        texts were entered for the PO item and what kind of texts are stored.
                                         “Create Purchase Orders – Supplier” on page E-38
                                        As an alternative to the Info menu, you can call up the order texts with
                                        <Ctrl>+<F10> from the Create POs dialog.
                                        You can only close the dialog via the Info menu or with <Ctrl>+<F10>.
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                         E-97
                 Form Printing                                                              Software Reference




                                 Form Printing
                                 Use the Printing of forms or Email dialog to print purchase orders and send
                                 them to the supplier. The dialogs are described in detail in the Sales section:
                                  Sales, “Form Printing” on page D-361
                                  Sales, “E-mail” on page D-365
5.00 / 12-2022




                 E-98                                                              A+W Enterprise Purchasing
                 Software Reference                                                              Purchase Order Release




                                        Purchase Order Release
                                        Purchase > P.O. Release
                                        On this dialog, you can release, lock or cancel POs. Depending on the system
                                        configuration, the POs can also be approved directly after PO creation or PO
                                        entry.
                                        In the change log, you can check the status of a PO. The dialog is described
                                        in detail for the Sales section:
                                         Sales, “Amendment Log” on page D-176
                                        This dialog contains the following views:
                                         “Purchase Order Release - Selection” on page E-99
                                         “Purchase Order Release – Details” on page E-100
                                         “Purchase Order Release - Additional Fields” on page E-102



                                        Purchase Order Release - Selection
                                        Purchase > P.O. Release




                                        Fig. E-31     Purchase order release - selection


                                        In this view, you select the PO that you want to edit.
                                        •    Use <F5> to change to the Purchase order release – Details view.
                                              “Purchase Order Release – Details” on page E-100
                                        •    Use <F3> to trigger the selected function.

                                        Header

                                        PO Number Purchase order number.
                                        Technical info: numeric field, DB field: kauf.auftrnr

                                        Current Current status of the purchase order.
                                        • released: the purchase order is released.
                                        • created: the purchase order is created but not released yet.
                                        • canceled: the purchase order has been canceled.
                                        Technical info: display field, DB field: kaufstat.datum

                                        Action Selection of the function that you want to trigger.
5.00 / 12-2022




                                        • released:
                                          The PO is released.



                 A+W Enterprise Purchasing                                                                        E-99
                 Purchase Order Release                                                             Software Reference




                                          •  cancel:
                                             The PO will be canceled and the items to be ordered placed back in the PO
                                             pool; they can be grouped into a different PO.
                                          • reset:
                                             The PO will be canceled. You can only reset POs that have the status re-
                                             leased. Already-canceled POs cannot be reset. The reset PO remains in
                                             the system and can be released at a later point in time.
                                          Technical info: display field

                                          Delivery Date Planned delivery date of the purchase order.
                                          Technical info: display field, DB field: kauf.ltplan

                                          Supplier Number and name of the supplier.
                                          Technical info: display fields, DB fields: kauf.kunr, mp.name

                                          Canc. Inform. Note about cancellation. This field is only displayed if you can-
                                          cel a PO and trigger the function with <F3>.
                                          Technical info: alphanumeric field, DB field: kauf.exbez2

                                          Footer
                                          Triggers the selected function for the current PO.
                                          Changes to the Purchase order release – Details view. Alternatively, you can
                                          use <F5> to change to the detail view.
                                           “Purchase Order Release – Details” on page E-100
                                          Closes the PO release dialog. Changes will not be saved.


                                          Purchase Order Release – Details
                                          Purchase > P.O. Release > Select P.O. > <F5>
5.00 / 12-2022




                                          Fig. E-32    Purchase order release – details


                                          In this view, the item details about the selected PO are displayed.


                 E-100                                                                     A+W Enterprise Purchasing
                 Software Reference                                                             Purchase Order Release




                                        Use <F2> to change to the Purchase order release – Additional Fields view.
                                         “Purchase Order Release - Additional Fields” on page E-102

                                        Header
                                        The header is described for Purchase order release - Selection view:
                                         “Purchase Order Release - Selection” on page E-99

                                        Item overview

                                        Itm Item number.
                                        Technical info: numeric field, DB field: kpos.lfdpos

                                        Article Article d.escription
                                        Technical info: display field, DB field: kpos.artbez1

                                        Ordered Quantity of the ordered item.
                                        Technical info: numerical field, DB field: kpos.menge

                                        Width, Height Dimensions of the item in millimeters.
                                        Technical info: numeric fields, DB fields: kpos.laenge, kpos.breite

                                        Order Order number for PO items from customer orders.
                                        Technical info: numeric field, DB field: bpos.vkauftrnr

                                        Delivery Planned delivery date of the customer order.
                                        Technical info: date field, DB field: kauf.ltplan

                                        Footer
                                        Closes the current view and changes to the Purchase order release – Selec-
                                        tion view.
                                         “Purchase Order Release - Selection” on page E-99
                                        Closes the current view and changes to the Purchase order release – Selec-
                                        tion view.
                                         “Purchase Order Release - Selection” on page E-99
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                      E-101
                 Purchase Order Release                                                               Software Reference




                                          Purchase Order Release - Additional Fields
                                          Purchase > P.O. Release > Select P.O. > <F5> > <F2>




                                          Fig. E-33    Purchase order release - additional fields


                                          This dialog displays information about the selected purchase order item.
                                          •   Use <F2> to change to the Purchase order release – Details view:
                                               “Purchase Order Release – Details” on page E-100
                                          •   Use <Page Up> and <Page Down> to change to the previous and next
                                              item.

                                          Header
                                          The header is described for Purchase order release - Selection view:
                                           “Purchase Order Release - Selection” on page E-99

                                          Purchase order details
                                          In addition to the Purchase Order Release - Details fields, the following fields
                                          are displayed:

                                          Article Number and description of the article.
                                          Technical info: display field, DB field: kpos.artnr, kpos.artbez1

                                          Quantity Quantity of the ordered item.
                                          Technical info: display field, DB field: kpos.menge

                                          Confirmed Quantity for delivery data as confirmed by the supplier.
                                          Technical info: display field, DB field: bpos.avismenge

                                          SizeVar Size variant of the ordered item for articles with variants.
5.00 / 12-2022




                                          Technical info: display field, DB field: kpos.var




                 E-102                                                                         A+W Enterprise Purchasing
                 Software Reference                                                            Purchase Order Release




                                        Lin.M. Linear meters of the PO item. If the article is assigned the quantity unit
                                        linear meters in the master data, the actual quantity of linear meters ordered
                                        is displayed here. If the article is assigned the quantity unit area in the master
                                        data, the size of the lite ordered is noted here.
                                        Technical info: display field, DB field: kpos.umlfdm

                                        Sqm Glass area of the purchase order item in square meters.
                                        Technical info: display field, DB field: kpos.qm

                                        AIR Airspace in millimeters. The field is only preset for IG articles.
                                        Technical info: display field, DB field: kpos.szr

                                        OC No.Suppl. Number of order confirmation from supplier.
                                        Technical info: numerical field, DB field: bpos.abnr

                                        Item Item number from the order in the case of order-related purchase or-
                                        ders.
                                        Technical info: numerical field, DB field: bpos.vklfdpos

                                        Customer Customer name of the PO items from customer orders.
                                        Technical info: display field, DB field: kauf.kunr, mp.name

                                        Warehouse Number and description of warehouse for stock articles.
                                        Technical info: numeric field, display field, DB fields: kauf.hausnr

                                        Project Number and description of the project for purchase order items from
                                        customer orders.
                                        Technical info: numeric field, display field, DB fields: bpos.vkobjnr, mp.name

                                        Price/Pc. Item price of the purchase order item.
                                        Technical info: numerical field, DB field: kpos.nstpreis

                                        Item Price Total price of the purchase order item. The total price is calculated
                                        from piece price x quantity of the article.
                                        Technical info: numeric field, DB field: kpos.npospreis

                                        Footer
                                        Closes the PO release dialog. Change will not be saved. Closes the current
                                        view and changes to the Purchase order release – Selection view.
                                         “Purchase Order Release - Selection” on page E-99
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                         E-103
                 Receipt of Goods                                                                Software Reference




                                    Receipt of Goods
                                    For deliveries, you can view the delivery plan for the purchase order and the
                                    supplier's delivery confirmation. You can advise of partial goods receipts and
                                    goods receipts and therefore check on-time goods receipt.
                                    You can also complete the POs that should no longer be traced in the system.
                                    The following information is available on this chapter:
                                     “Dispatch Notifications” on page E-104
                                     “Delivery Plan” on page E-112
                                     “Receipt of Goods (Automatic)” on page E-115
                                     “Item Info” on page E-117
                                     “Booking Racks” on page E-118
                                     “Receipt of Goods (Manual)” on page E-119
                                     “Rack-Related Receipt of Goods” on page E-121
                                     “Booking Racks” on page E-118
                                     “Close Purchase Orders” on page E-141
                                     “Check Receipt of Goods” on page E-124
                                     “Missing Quantities Check Pool” on page E-126
                                     “Receipt of Goods Log” on page E-127



                                    Dispatch Notifications
                                    Purchase > Notifications
                                    The delivery confirmations from suppliers are managed in this dialog.
                                    This dialog contains the following tabs and views:
                                     “Notifications – Overview” on page E-105
                                     “Notifications – Details” on page E-107
                                     “Purchase Order – Overview (Notification)” on page E-109
                                     “Purchase Order – Details (Notification)” on page E-110
5.00 / 12-2022




                 E-104                                                                A+W Enterprise Purchasing
                 Software Reference                                                                         Receipt of Goods




                                           Notifications – Overview
                                           Purchase > Notifications – Overview Tab




                 Fig. E-34   Notifications – overview tab


                                           Use this tab to enter notifications concerning receipt of goods.
                                           •   Use <F2> to change to the Notification - Details tab.
                                                “Notifications – Details” on page E-107
                                           •   Use <F5> in the OC-No. Supplier field in the body to open the PO dialog in
                                               order to get detailed information about the items ordered.
                                                “Purchase Order – Overview (Notification)” on page E-109

                                           Header

                                           OC No. Supplier OC Supplier:
                                           Number of order confirmation from supplier. If you enter an order confirmation
                                           number that also includes letters, you must enter them in a case-sensitive
                                           manner.
                                           Technical info: alpha-numerical field, DB field: bpos.abnr

                                           Delivery Date Planned delivery date. You can take over the delivery date for
                                           all POs. If you take over the date for all POs, the delivery date of each PO in
                                           the body is overwritten by the delivery date in the header area.
                                           Technical info: mandatory field, date field, DB field: bpos.ltplan
5.00 / 12-2022




                                           Site Site number from the purchase order.
                                           Technical info: display field, DB field: kauf.hausnr



                 A+W Enterprise Purchasing                                                                           E-105
                 Receipt of Goods                                                                Software Reference




                                    Supplier Supplier number. If you specify a number, the name of the supplier
                                    is displayed in plain text. You can take over the supplier for all POs. If you take
                                    over the supplier for all POs, you can only select POs for this supplier for the
                                    order confirmation.
                                    Technical info: numeric field, display field, DB field: kauf.kunr

                                    Body
                                    •   P.O.:
                                        Purchase order number. If you have specified a supplier, you can only
                                        specify POs for this supplier.
                                        Technical info: numeric field, DB field: kauf.auftrnr
                                    •   OC No.Suppl.:
                                        Number of order confirmation from supplier.
                                        Technical info: alpha-numerical field, DB field: bpos.abnr
                                    Use <F5> to edit the Overview and Details of the notifications in the Supplier
                                    OC no. column.
                                     “Purchase Order – Overview (Notification)” on page E-109
                                     “Purchase Order – Details (Notification)” on page E-110
                                    • Ordered for:
                                       Date when the purchase order should be received. Usually the delivery
                                       date of receipt of goods or in the case of direct delivery, e.g. a construction
                                       site.
                                       Technical info: date field, DB field: kauf.ltplan
                                    • Number:
                                       Supplier number from purchase order.
                                       Technical info: display field, DB field: kauf.kunr
                                    • Supplier:
                                       Name of the supplier.
                                       Technical info: display field, DB field: mp.name
                                    • Qty:
                                       Quantity of the item that is delivered.
                                    Technical info: display field, DB field: bpos.avismenge
5.00 / 12-2022




                 E-106                                                                  A+W Enterprise Purchasing
                 Software Reference                                                                          Receipt of Goods




                                            Notifications – Details
                                            Purchase > Notifications – Details Tab




                 Fig. E-35   Notifications – details tab


                                            On this tab you can view the purchase order details. You can enter changes
                                            based on the supplier confirmation.
                                            •   Use <F2> to change to the Notification - Overview tab.
                                                 “Notifications – Overview” on page E-105
                                            •   Use <F5> in field OC No.Suppl. to open the Purchase Order dialog.
                                                 “Purchase Order – Overview (Notification)” on page E-109
                                            •   With <Ctrl> + <L> you can, if this possibility is configured, check the deliv-
                                                ery address. However, the delivery address cannot be changed here.

                                            Header
                                            The header fields are described for the Notification - Overview tab:
                                             “Notifications – Overview” on page E-105

                                            Purchase Information

                                            P.O. No. Purchase order number.
                                            Technical info: numeric field, DB field: kauf.auftrnr

                                            OC No. Suppl. Number of order confirmation from supplier.
5.00 / 12-2022




                                            Technical info: alpha-numerical field, DB field: bpos.abnr

                                            Supplier Number and name of the supplier.


                 A+W Enterprise Purchasing                                                                            E-107
                 Receipt of Goods                                                              Software Reference




                                    Technical info: display fields, DB fields: kauf.kunr

                                    Street, PCd, City Supplier's address. The fields are pre-populated with the
                                    values from the purchase order.
                                    Technical info: numerical field, alpha-numerical field, DB fields: kauf.orgstr,
                                    kauf.orgplz, kauf.orgort

                                    VAT Code ID, description and percentage of the VAT code. The percentage
                                    and the ID are determined using the number from the master data.
                                    Technical info: display fields, DB fields: kauf.kukz

                                    Deliv. Date Actual delivery date of the purchase order.
                                    Technical info: date field, DB field: kauf.ltplan

                                    Old Old, planned delivery date of the purchase order.
                                    Technical info: display field, DB field: bpos.ltplan

                                    Route Number and description of the route. If you specify a number, the de-
                                    scription of the route is displayed in plain text.
                                    Technical info: numeric field, display field, DB field: kauf.routenr

                                    Net Amount Total of all item prices, including all discounts and surcharges.
                                    Technical info: display field, DB field: kauf.nettototal

                                    VAT amount Value-added tax amount of the purchase order.
                                    Technical info: display field, DB field: kauf.mwstbetrag

                                    Gross Amount Gross amount of the purchase order including VAT.
                                    Technical info: display field, DB field: kauf.gesbrutto

                                    Order Information
                                    The fields are only pre-populated, if the purchase order was created from a
                                    customer order.

                                    Order No. Order number for order-related purchase orders.
                                    Technical info: display field, DB field: kauf.auftrnr

                                    Customer Name Customer name from the customer order.
                                    Technical info: display field, DB field: kauf.kunr

                                    Delivery Date Planned delivery date of the customer order.
                                    Technical info: display field, DB field: kauf.ltplan

                                    Route Number and name of the delivery route to the customer.
                                    Technical info: display fields, DB fields: kauf.routenr
5.00 / 12-2022




                 E-108                                                                 A+W Enterprise Purchasing
                 Software Reference                                                                    Receipt of Goods




                                        Purchase Order – Overview (Notification)
                                        Purchase > Notification > Overview Tab > Column OC No. Suppl. > <F5>
                                        Purchase > Notification > Details Tab > OC No. Suppl. Field > <F5>




                                        Fig. E-36     Purchase order – Overview (notification)


                                        Use this tab to edit the item-accurate notifications, e.g. to change the an-
                                        nounced delivery quantity. Changes to the deliveries and partial deliveries are
                                        recorded via the notifications.
                                        Use <F2> to change to Purchase Order - Details (Notification) tab.
                                         “Purchase Order – Details (Notification)” on page E-110

                                        Overview
                                        •    Itm:
                                             Item number.
                                             Technical info: display field, DB field: kpos.lfdpos
                                        •    Article:
                                             Article number of the item.
                                             Technical info: numeric field, DB field: kpos.artnr
                                        •    Ordered:
                                             Quantity of the ordered item.
                                             Technical info: numerical field, DB field: kpos.menge
                                        •    OC No. Suppl.:
                                             Number of order confirmation from supplier.
                                             Technical info: numerical field, DB field: bpos.abnr
                                        •    Confirmed:
                                             Quantity of the delivery as confirmed by the supplier. In the case of boxes,
                                             this equals the total number of lites.
5.00 / 12-2022




                                             Technical info: numeric fields, DB fields: bpos.avismenge




                 A+W Enterprise Purchasing                                                                        E-109
                 Receipt of Goods                                                                Software Reference




                                    •   Price/Pc.:
                                        Net price per piece of item.
                                        Technical info: numeric field, DB field: kpos.nstpreis
                                    •   Item Price:
                                        Net total price of item.
                                        Technical info: numeric field, DB field: kpos.npospreis
                                    •   Invoic.:
                                        Invoice ID of the item. The column indicates whether the selected item has
                                        already been invoiced.
                                        Technical info: display field, DB field: kpos.fakturakz


                                    Purchase Order – Details (Notification)
                                    Purchase > Notifications > Overview Tab > Suppl. OC No. Column > <F5> De-
                                    tails Tab
                                    Purchase > Notifications > Details Tab > Suppl. OC no. Column > <F5> De-
                                    tails Tab




                                    Fig. E-37    Purchase order (notification) – details tab


                                    Use this tab to enter details for the delivery that has been announced by the
                                    supplier, e.g. quantity, price and delivery date. Changes to the deliveries and
                                    partial deliveries are recorded via the notifications.
                                    Use <F2> to change to the Purchase Order - Overview (Notification) tab.
                                     “Purchase Order – Overview (Notification)” on page E-109

                                    Article Number and description of the article. If an article number is specified,
                                    the corresponding description is displayed in plain text.
                                    Technical info: numerical field, display field, DB field: kpos.artnr, kpos.artbez1
5.00 / 12-2022




                                    Note Additional information on the item.
                                    Technical info: alpha-numerical field, DB field: bpos.bemerkung



                 E-110                                                                    A+W Enterprise Purchasing
                 Software Reference                                                                       Receipt of Goods




                                        Cost Center Cost center name for statistical evaluations.
                                        Technical info: numerical field, DB field: kpos.kostenst

                                        Account Description of the cost center booking account.
                                        Technical info: alpha-numerical field, DB field: kpos.konto

                                        Shape Shape number for PO items with lite shape.
                                        Technical info: display field, DB field: kpos.modnr

                                        Ordered Quantity of the ordered item.
                                        Technical info: numerical field, DB field: kpos.menge

                                        Delivered Number of delivered items.
                                        Technical info: display field, DB field: kpos.geliefert

                                        Width, Height Dimensions of the item in millimeters.
                                        Technical info: display fields: DB fields: kpos.laenge, kpos.breite

                                             One-dimensional quantity input
                                             For a system configuration, in incoming goods for articles with quantity
                                             units (1,6,7,8,10), a partial quantity with regard to this quantity unit can also
                                             be reported. The field for input of the quantity kpos.laenge (e.g. a linear me-
                                             ter or liter entry) can be changed accordingly.

                                        AIR Airspace in millimeters. The field is only preset for IG articles.
                                        Technical info: display field, DB field: kpos.szr

                                        sqm Piece Surface in square meters per piece.
                                        Technical info: numeric field, DB field: kpos.qm

                                        OC No.Supplier Number of order confirmation from supplier.
                                        Technical info: alpha-numerical field, DB field: bpos.abnr

                                        Delivery Date Actual delivery date of the purchase item.
                                        Technical info: Date field, DB field: bpos.ltavis

                                        Confirmed Quantity of delivery as confirmed by the supplier. In the case of
                                        boxes, this equals the total number of sheets.
                                        Technical info: numeric fields, DB fields: bpos.avismenge

                                        Old Old, planned delivery date of the purchase order.
                                        Technical info: display field, DB field: bpos.ltplan

                                        Order Order number for order-related purchase orders.
                                        Technical info: display field, DB field: kauf.auftrnr

                                        Item Number of the item, in the case of order-related purchase orders.
5.00 / 12-2022




                                        Technical info: display field, DB field: kpos.lfdpos

                                        Reject Reason The number and the reject description are displayed.


                 A+W Enterprise Purchasing                                                                             E-111
                 Receipt of Goods                                                                Software Reference




                                    Technical info: display field, DB field: bpos.bruch

                                    Deliv. Date Date of delivery at the customer.
                                    Technical info: display field

                                    Cst. Project Project number and name of the customer order for order-relat-
                                    ed purchase orders.
                                    Technical info: display fields, DB fields: bpos.vkobjnr.

                                    Stock Number Number and name of warehouse for stock articles.
                                    Technical info: display fields, DB fields: bpos.lnr

                                    Sup.Art.No. Supplier's article number and ID of the supplier article. Number
                                    and ID are displayed if a supplier-specific article number is stored for the arti-
                                    cle in the master data.
                                    Technical info: numerical field, alpha-numerical field, DB fields: bpos.exartnr,
                                    bpos.bestellbez

                                    Price/QU Price per quantity unit. The price is calculated from the glass price
                                    plus the surcharge.
                                    Technical info: numeric field, DB field: kpos.bmepreis

                                    Net Pieces Net price per piece.
                                    Technical info: numerical field, DB field: kpos.nstpreis

                                    Item Price Net purchase price per piece.
                                    Technical info: numeric field, DB field: kpos.npospreis


                                    Delivery Plan
                                    Purchasing > Receipt of Goods > Delivery Plan
5.00 / 12-2022




                                    Fig. E-38    Delivery plan – overview tab




                 E-112                                                                    A+W Enterprise Purchasing
                 Software Reference                                                                     Receipt of Goods




                                        You can plan the planned deliveries on this dialog. You can determine the de-
                                        livery date and delivery quantity for individual or several POs. The partial de-
                                        liveries will then be used to book goods receipt.
                                        In order to be able to work with the delivery plan in purchasing, the system
                                        must be configured appropriately.
                                        Use <F2> to change to the Delivery Plan - Details tab.
                                         “Delivery Plan – Details” on page E-114
                                        Use <Ctrl> + <G> to change to the Booking Racks dialog.
                                         “Booking Racks” on page E-118
                                        Use <OK> to save the delivery plan and to exit the dialog.

                                        Site Site number. The field is only enabled for multi-site systems.
                                        Technical info: display field, DB field: kauf.hausnr

                                        P.O. Specification of the PO number for which the delivery plan should be cre-
                                        ated or changed.
                                        Technical info: display field, DB field: kauf.vorgang=2

                                        Supplier Displays the name of the supplier from the purchase order. The field
                                        is disabled.
                                        Technical info: display field, DB field: kauf.kunr, mp.name

                                        Overview
                                        The Overview tab displays the following fields:
                                        •    Itm:
                                             Item number.
                                             Technical info: display field, DB field: liefplan.lfdpos
                                        •    Deliv.:
                                             Number of the delivery. The value is incremented for partial deliveries.
                                             Technical info: display field, DB field: liefplan.subnr
                                        •    Delivery Date:
                                             Delivery date for the scheduled product.
                                             Technical info: display field, DB field: liefplan.ltplan
                                        •    Article:
                                             Article name from the purchase order.
                                             Technical info: display field
                                        •    OC No.Suppl.:
                                             Order confirmation of supplier.
                                             Technical item: numeric field, DB field: liefplan.abnr
                                        •    Total:
                                             Total quantity of the item ordered from the PO in article quantity unit, e.g.
                                             pieces.
                                             Technical info: display field, DB field: liefplan.geslief
                                        •    Shipped:
5.00 / 12-2022




                                             Already shipped quantity for the ordered item in article quantity units, e.g.
                                             pieces.
                                             Technical info: display field, DB field: liefplan.geliefert


                 A+W Enterprise Purchasing                                                                         E-113
                 Receipt of Goods                                                                Software Reference




                                    •   Packed:
                                        Already packed quantity for the ordered item in article quantity units, e.g.
                                        pieces.
                                        TEchnical info: display field, DB field: liefplan.gespack
                                    •   Planned:
                                        Planned quantity for the item ordered in article quantity units that should ar-
                                        rive in this (partial) delivery, e.g. pieces.
                                        Technical info: display field, DB field: liefplan.zuliefern


                                    Delivery Plan – Details
                                    Purchase > Receipt of Goods > Delivery Plan > Select Purchase Order > <F2>




                                    Fig. E-39     Delivery plan – details tab


                                    This tab shows detailed information for the selected purchase order item.
                                    Use <F2> to change to the Delivery Plan - Overview tab.
                                     “Delivery Plan” on page E-112
                                    Use <Ctrl> + <G> to change to the Booking Racks dialog.
                                     “Booking Racks” on page E-118
                                    Use <OK> to save the delivery plan and to exit the dialog.

                                    Details
                                    The fields are described on the Deliver Plan - Overview tab. In addition, the
                                    following fields are displayed on the Details tab:

                                    Stock Stock number of the standard stock for stock POs. The designation of
                                    the standard stock is determined from the master data and displayed in the
                                    second field.
5.00 / 12-2022




                                    Technical info: display field, DB field: liefplan.lnr




                 E-114                                                                  A+W Enterprise Purchasing
                 Software Reference                                                                     Receipt of Goods




                                          Stack Stock number of the stack stock for stock POs insofar as the article is
                                          kept in the stack stock. The designation of the stack is determined from the
                                          master data and displayed in the second field.
                                          Technical info: display field, DB field: liefplan.stapel, liefplan.stapelbez

                                          Box Box number of the box stock for stock POs, insofar as the article is kept
                                          in the box stock.
                                          Technical info: display field, DB field: liefplan.kistenr

                                          Slot Slot designation of the slot stock for stock POs, insofar as the article is
                                          keps in the slot stock.
                                          Technical info: display field, DB field: liefplan.fach


                                          Receipt of Goods (Automatic)
                                          Purchasing > Receipt of Goods > Automatic Receipt of Goods




                 Fig. E-40   Receipt of goods (automatic)


                                          Use this dialog to book received deliveries as receipt of goods. You can book
                                          individual or all loaded purchase orders of the dialog.
                                          •   With <Value import> the POs in the system are uploaded to the dialog. The
                                              value import can be configured customer-specifically.
                                          •   Use <F9> to select individual purchase orders that have not been booked.
5.00 / 12-2022




                                          •   Use <F8> to select purchase orders for which a delivery plan exist, that
                                              have not been booked.
                                          •   Use <Ctrl>+<L> to change to the Delivery note column, where you can
                                              specify the external supplier delivery note designation.

                 A+W Enterprise Purchasing                                                                          E-115
                 Receipt of Goods                                                               Software Reference




                                    •   Use <F5> to open the Item Info dialog.
                                         Purchasing, “Item Info” on page E-117
                                    •   Use <F3> to book the previously marked PO as goods receipt.

                                    Purchase orders
                                    The Purchase Orders tab shows the following columns:
                                    •   P.O.:
                                        Purchase order number.
                                        Technical info: numeric field, DB field: kauf.auftrnr
                                    •   1. Column without a name (subnumber):
                                        POs without a delivery plan are booked as complete goods receipt, so this
                                        field remains empty. For POs with a delivery plan, the subnumber from the
                                        delivery plan that is announced for the current date is displayed here. If
                                        there is a delivery plan for the PO, you can use <F9> to select the desired
                                        partial delivery.
                                        Technical info: display fields, DB fields: kauf.subnr
                                    •   2. Column without a name (delivery plan):
                                        Display in plan text whether there is a delivery plan for the PO.
                                        Technical info: display field
                                    •   Site:
                                        Site number of the PO.
                                        Technical info: display field, DB field: kauf.hausnr
                                    •   Receipt:
                                        Indication whether a goods receipt for the PO has already been received.
                                        If the goods receipt was already booked, this is indicated in the Exists col-
                                        umn.
                                        Technical info: display field
                                    •   Invoice:
                                        Number of the supplier's invoice if the PO has already been (partially) in-
                                        voiced.
                                        Technical info: display field, DB field: kauf.auftrnr
                                    •   External No.:
                                        Order number from purchasing if the PO was entered with reference. Dis-
                                        play Collective PO or Stock PO
                                        Technical info: display field, DB field: kauf.exaufnr
                                    •   Date:
                                        Date of entry for the purchase order.
                                        Technical info: date field, DB field: kauf.bdat
                                    •   Deliv. Note:
                                        Text field for the delivery note designation. Use <Ctro> + <L> to switch from
                                        any column to the delivery note column and enter a designation for the sup-
                                        plier delivery note.
                                        Technical info: alphanumeric field, DB field: bpos.lieferschein
                                    •   Chk:
                                        Check. Checkbox whether the purchase order must be checked for com-
                                        pleteness at receipt of goods. The function to check the receipt of goods is
                                        customer-specific.
5.00 / 12-2022




                                         The purchase order is checked at receipt of goods.
                                         The purchase order is not checked.



                 E-116                                                                 A+W Enterprise Purchasing
                 Software Reference                                                                      Receipt of Goods




                                             Use <F4> to set the control status for individual items starting with a partic-
                                             ular one or all items:
                                              “Receipt of Goods Supplementary Menu” on page E-21
                                             Technical info: checkbox, DB field: kauf.kontrolle
                                        •    Cr.:
                                             Create.
                                             Specification whether the purchase order should be booked in receipt of
                                             goods.
                                              The purchase order is booked in receipt of goods.
                                              The purchase order is not booked.
                                             Use <F3> to book all selected purchase orders.
                                             Technical info: Checkbox

                                        Footer
                                        On the Purchase Orders tab, the name of the supplier and net amount for the
                                        marked PO are displayed.
                                        Opens the Item Info dialog for the marked purchase order.
                                        After specifying a time period, imports all non-booked POs with a delivery date
                                        within the specified time period.
                                        Books all marked POs in receipt of goods and closes the dialog.
                                        Closes the dialog without saving the purchase orders.


                                        Item Info
                                        Purchasing > Receipt of Goods > Automatic Receipt of Goods > Search for
                                        Purchase Order > <F5>
                                        Purchasing > Receipt of Goods > Complete Purchase Orders > Find Purchase
                                        Order > <F5>




                                        Fig. E-41      Item overviews
5.00 / 12-2022




                                        This dialog allows you to view the item overview for a purchase order. Use
                                        <F2> to go to the tab.


                 A+W Enterprise Purchasing                                                                           E-117
                 Receipt of Goods                                                                Software Reference




                                    The Item Info tab is described in detail in the Sales section:
                                     Sales, “Item Info” on page D-344



                                    Booking Racks
                                    Purchase > Automatic Receipt of Goods > Select Purchase Order > <F4> >
                                    Rack Management




                                    Fig. E-42     Booking racks


                                    On this dialog, you can assign the lites of a PO to the rack per item.

                                    Header

                                    Docum. Purchase order number for which the rack is booked.
                                    Technical info: display field, DB field: kauf.auftrnr, bcbock.auftrnr

                                    Body
                                    •   Itm:
                                        Number of the item on the delivered rack.
                                        Technical info: display field, DB field: bcbock.bposnr
                                    •   Quantity:
                                        Number of lites in the item.
                                        Technical info: display field, DB field: bcbock.anzahl
                                    •   Rack, designation:
                                        Number and designation of the rack type of the rack delivered. If you spec-
                                        ify a number, the designation of the rack is displayed in plain text.
                                        Technical info: numeric field, display field, DB fields: bcbock.gnr, gest.exgnr
                                    Use <F2> to display the following columns:
                                    •   move:
                                        Rack number of the delivered rack, the glass pieces of which are booked
                                        to a different rack.
                                        Technical info: display field, DB field: bcbock.gnr, gest.exgnr
5.00 / 12-2022




                                    •   Quantity:
                                        Quantity of glass pieces that are booked to the target rack.
                                        Technical info: numerical field, DB field: bcbock.anzahl


                 E-118                                                                  A+W Enterprise Purchasing
                 Software Reference                                                                      Receipt of Goods




                                          •   Target rack:
                                              Rack number of the target rack to which the glass is booked.
                                              Technical info: numeric field, DB field: bcbock.gnr, gest.exgnr


                                          Receipt of Goods (Manual)
                                          Purchase > Manual Receipt of Goods > Find Purchase Order




                 Fig. E-43   Manual receipt of goods


                                          Use this dialog to edit and book received deliveries and partial deliveries that
                                          arrived in receipt of goods.
                                          Use [End] to save your entries and to book the (partial) receipt of goods.

                                              Close purchase orders in the event of partial deliveries
                                              If you book a partial good receipt, you will be asked whether there will be
                                              additional goods receipt to follow. With [Yes,] only the partial goods receipt
                                              will be created and booked; the PO will not be completed. With [No], the
                                              partial goods receipt will be created and booked and the PO will be com-
                                              pleted. Additional partial goods receipts can no longer be booked for the
                                              selected PO.

                                          The dialog is structured the same as the Purchase Order Entry dialog.
                                           “Purchase Order Entry” on page E-51
5.00 / 12-2022




                                          Differences will be described explicitly below.




                 A+W Enterprise Purchasing                                                                           E-119
                 Receipt of Goods                                                               Software Reference




                                    Header

                                    Purchase Purchase order number and partial delivery number. For each new
                                    purchase order, the partial delivery number 1 is automatically specified. In the
                                    case of partial deliveries, you must manually enter consecutive numbers
                                    larger than 1, e.g. the partial delivery number 2 for the second partial delivery.

                                    Technical info: mandatory field, numeric fields, DB fields: kauf.auftrnr,
                                    kauf.subnr

                                    Delivery Note Supplier's delivery note number.
                                    Technical info: alpha-numerical field, DB field: kauf.lieferschein

                                    Check Indication as to whether the purchase order should be checked for
                                    completeness at receipt of goods.
                                    • Control:
                                       The PO is checked in goods receipt, e.g. for completeness. The employee
                                       number and date for the check are logged.
                                    • (No specification):
                                       The PO will not be checked.
                                    Technical info: toggle field, DB field: kauf.kontrolle

                                    General tab
                                    •   Ordered:
                                        Ordered item quantity in the article quantity unit.
                                        Technical info: numeric field, DB field: kpos.menge
                                    •   Alr. recei.:Item quantity already received in the article quantity unit.
                                        Technical info: numeric field
                                    •   Received:
                                        Already delivered item quantity in the article quantity unit. The system cal-
                                        culates the quantity from ordered quantity less the quantity already re-
                                        ceived.
                                        Technical info: numeric field, DB field: kpos.geliefert
                                    •   Confirm:
                                        Supplier-side confirmed item quantity in the article quantity unit of the de-
                                        livery.
                                        Technical info: numeric field, DB field: bpos.avismenge
5.00 / 12-2022




                 E-120                                                                 A+W Enterprise Purchasing
                 Software Reference                                                                      Receipt of Goods




                                           Rack-Related Receipt of Goods
                                           Purchase > Receipt of Goods > Rack-Related Receipt of Goods
                                           On this dialog, you enter and edit goods receipts using the rack.
                                           There are the following views for this dialog:
                                            “Rack-Related Receipt of Goods” on page E-121
                                            “Rack Load” on page E-122


                                           Rack-Related Receipt of Goods
                                           Purchase > Receipt of Goods > Rack-Related Receipt of Goods




                 Fig. E-44   Rack-related receipt of goods


                                           Rack-related receipt of goods are booked on this dialog.
                                           •   Use <F6> to open the Rack Load dialog and create a new rack load and
                                               place the PO items on another (new) rack.
                                           •   Use <F5> to open the Rack Load dialog, where you can edit the marked
                                               goods receipt.
                                                “Rack Load” on page E-122

                                           Overview
                                           •   Rack:
5.00 / 12-2022




                                               Rack number .
                                               Technical info: display field, DB field: waeingestkopf.exgnr




                 A+W Enterprise Purchasing                                                                        E-121
                 Receipt of Goods                                                                  Software Reference




                                    •   Suppl. ID:
                                        Manually-entered ID for a delivery.
                                        Technical info: display field, DB field: waeingestkopf.lieferid
                                    •   Storage location:
                                        Number and name of the storage location where the rack is located.
                                        Technical info: display field, DB field: waeingestkopf.lagerplatz
                                    •   Truck:
                                        License plate number of the truck with which the PO was delivered.
                                        Technical info: display field, DB field: waeingestkopf.lkwkennzeichen
                                    •   Supplier:
                                        Number and name of the supplier.
                                        Technical info: display field, DB field: kauf.kunr, mp.name
                                    •   Qty:
                                        The total quantity of all lites on the rack. This quantity is calculated from all
                                        items on the rack.
                                        Technical info: display field, DB field: waeingestpos.menge
                                    •   Deliv.Date, Time:
                                        Date and time of the delivery.
                                        Technical info: display field, DB field: waeingestkopf.datum. waeingst-
                                        kopf.zeit
                                    •   Bo.:
                                        Specification whether the rack should be booked in goods receipt.
                                         The rack is booked in goods receipt.
                                         The rack is not booked..
                                        Use <F3> to start the booking of the rack.
                                        Technical info: checkbox, DB field: waeingestkopf.gebucht

                                    Footer
                                    Opens the Rack Load dialog where you can enter a new rack in goods receipt.
                                     “Rack Load” on page E-122
                                    Opens the Rack Load dialog where you can edit the selected rack in goods
                                    receipt.
                                     “Rack Load” on page E-122
                                    Deletes the selected rack.
                                    Books the marked rack in goods receipt.
                                    Books the marked rack in goods receipt and closes the dialog.
                                    Closes the dialog without booking the rack.


                                    Rack Load
                                    Purchase > Receipt of Goods > Rack-Related Receipt of Goods > [New], [Cor-
                                    rection]
5.00 / 12-2022




                 E-122                                                                    A+W Enterprise Purchasing
                 Software Reference                                                                        Receipt of Goods




                 Fig. E-45   Rack load


                                         In this view, you enter and edit the rack load for the goods receipt.

                                         Header
                                         You can only edit the fields in the header area if you are entering a new rack
                                         load. If you are editing an existing rack load, the header area is locked.

                                         Rack (No./Name) Rack number and name.
                                         Technical info: mandatory field, numeric and alphanumeric field, DB field:
                                         waeingestkopf.gestellnr, waeingestkopf.exgnr

                                         Suppl.ID Manually entered flag for a delivery.
                                         Technical info: display field, DB field: waeingestkopf.lieferid

                                         Storage Location Number and designation of the storage location for the
                                         rack. If you select a number, the designation is displayed in plain text.
                                         Technical info: mandatory field, numeric field, alphanumeric field, DB field:
                                         adr.str

                                         Truck Plate No. License plate number of the truck with which the rack was
                                         delivered.
                                         Technical info: alphanumeric field, DB field: waeingestkopf.lkwkennzeichen

                                         Total Qty. Total quantity on all racks of the delivery. The total quantity corre-
                                         sponds to the total of all quantities in the Quantity column in the overview.
5.00 / 12-2022




                                         Technical info: display field, DB field: waeingestpos.menge

                                         Date Date of delivery in the format DD.MM.YYYY.


                 A+W Enterprise Purchasing                                                                          E-123
                 Receipt of Goods                                                               Software Reference




                                    Technical info: date field, DB field: waeingestkopf.datum

                                    Time Time of delivery in the format hh:mm.
                                    Technical info: alphanumeric field, DB field: waeingstkopf.mc

                                    Body
                                    All PO items for which goods receipt should be booked to the rack are entered
                                    and edited in the dialog body.
                                    •   P.O.:
                                        Purchase order number.
                                        Technical info: mandatory field, numeric field, DB field: waeingestpos.auf-
                                        trnr
                                    •   ItmNo
                                        Item number in the purchase order.
                                        Technical info: mandatory field, numeric field, DB field: waeingestpos.pos-
                                        nr
                                    •   Supplier:
                                        Name and number of the supplier. If you enter a purchase order number,
                                        the fields are pre-populated by the system.
                                        Technical info: display fields, DB fields: waeingestpos.mpnr
                                    •   Deliv.Note:
                                        Delivery note description of the supplier.
                                        Technical info: alpha-numerical field, DB field: waeingestpos.lieferschein
                                    •   Total:
                                        Total quantity of the selected item.
                                        Technical info: display field, DB field: waeingestpos.menge
                                    •   Included:
                                        Already delivered quantity of the ordered item from a partial delivery.
                                        Technical info: display field
                                    •   Qty:
                                        Currently delivered quantity of the ordered item.
                                        Technical info: numeric field, DB field: waeingestpos.menge
                                    •   Miss. Qty.:
                                        Difference between ordered and delivered quantity.
                                        Technical info: numeric field, DB field: waeingestpos.fehlmenge
                                    •   Side:
                                        Rack side on which the item is located:
                                        0 = not specified
                                        1 = left
                                        2 = right
                                        Technical info: alphanumeric field, DB field: waeingestpos.gestellseite
                                    •   Sequence:
                                        The sequence in which the item is on the rack, from outside to inside.
                                        Technical info: numeric field, DB field: waeingestpos.reihenfolge
5.00 / 12-2022




                                    Check Receipt of Goods
                                    Purchase > Receipt of Goods > Check Receipt of Goods


                 E-124                                                                A+W Enterprise Purchasing
                 Software Reference                                                                    Receipt of Goods




                 Fig. E-46   Check receipt of goods


                                          On this dialog, goods receipts and purchase invoices are created automatical-
                                          ly based on the underlying PO and an invoice received. The data is sent and
                                          received via the data transfer and it can be checked and adjusted on the
                                          Check goods received dialog.
                                          This for-fee function must be configured explicitly. If you have questions,
                                          please contact an A+W Software GmbH service employee.
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                         E-125
                 Receipt of Goods                                                                       Software Reference




                                           Missing Quantities Check Pool
                                           Menu: Purchase > Receipt of Goods > Missing Qty. Check Pool
                                           This dialog shows a list of items the quantity of which has been corrected.
                                           This for-fee function must be configured explicitly. If you have questions,
                                           please contact an A+W Software GmbH service employee.
                                           This dialog offers the following tabs:
                                            “Missing Quantities Check Pool - Overview” on page E-126
                                            “Missing Quantities Check Pool – Details” on page E-127


                                           Missing Quantities Check Pool - Overview
                                           Purchase > Receipt of Goods > Missing Quantity Check Pool > Overview Tab




                 Fig. E-47   Missing quantities check pool - overview


                                           This tab shows a list of items the quantity of which has been corrected. The
                                           data is transferred via openTrans interface.
                                           This function description is not part of the manual and must be requested if
                                           needed.
5.00 / 12-2022




                 E-126                                                                       A+W Enterprise Purchasing
                 Software Reference                                                                    Receipt of Goods




                                           Missing Quantities Check Pool – Details
                                           Purchase > Receipt of Goods > Missing Quantities Check Pool > Details Tab




                 Fig. E-48   Missing quantities check pool - details


                                           This tab provides you with detailed information about the selected item.
                                           This function description is not part of the manual and must be requested if
                                           needed.


                                           Receipt of Goods Log
                                           Purchase > Receipt of Goods > Log




                                           Fig. E-49      Receipt of goods log


                                           On this dialog, you can display a log about the creation and booking of goods
5.00 / 12-2022




                                           receipts for the current day. All documents for goods receipt are logged with
                                           the specification of the date and time.




                 A+W Enterprise Purchasing                                                                        E-127
                 Invoices and Credit Notes                                                          Software Reference




                                         Invoices and Credit Notes
                                         Invoices for purchase orders are entered and booked in the program. Depend-
                                         ing on the configuration, the internal invoice is automatically sent by the pro-
                                         gram to Financial Accounting (FinAc).
                                         The following information is available on this chapter:
                                         •   “Invoice Check” on page E-128
                                         •   “Supplier’s Invoice (Automatic)” on page E-135
                                         •   “Supplier's Invoice (Manual)” on page E-138
                                         •   “Supplier's Invoice (Collective Invoice)” on page E-139
                                         •   “Transferred Invoices” on page E-137
                                         •   “Booking of Invoices” on page E-139
                                         •   “Close Purchase Orders” on page E-141
                                         •   “Invoice Log” on page E-142
                                         •   “Supplier's Credit Note” on page E-142
                                         The dialog Book Credit Notes is described in detail in the Sales section.
                                          Sales, “Book Credit Notes” on page D-358



                                         Invoice Check
                                         Purchase > Invoices > Invoice Check
                                         Use this dialog to enter and check supplier invoices, and to create and book
                                         internal invoices. The use of the invoice check in purchasing requires config-
                                         uration by A+W Software GmbH.
                                         There are the following views for this dialog:
                                         •   “Supplier’s Invoice – Purchase Overview” on page E-129
                                         •   “Supplier’s Invoice – Detailed View” on page E-132
                                         •   “Supplier’s Invoice – Item Overview” on page E-133
                                         •   “Supplier’s Invoice – Discounts” on page E-134
5.00 / 12-2022




                 E-128                                                                     A+W Enterprise Purchasing
                 Software Reference                                                              Invoices and Credit Notes




                                          Supplier’s Invoice – Purchase Overview
                                          Purchase > Invoices > Invoice Check




                 Fig. E-50   Supplier's Invoice - Purchase Overview


                                          On this dialog, you enter the PO data for checking. Then you can create and
                                          book the supplier invoice for the PO checked.
                                          •   Use <F2> to change to the body in the detail view.
                                               “Supplier’s Invoice – Detailed View” on page E-132
                                          •   Use <F5> in the Net amount field to change to the item detail overview.
                                               “Supplier’s Invoice – Item Overview” on page E-133
                                          •   Use <Ctrl>+<A> to change to the discount overview.
                                               “Supplier’s Invoice – Discounts” on page E-134
                                          Use <Enter> to change from the body area to the footer area. With the manual
                                          entry of the invoice total, the invoice is checked in the system. You can create
                                          the invoice and book it right away or later on.
                                           “Booking of Invoices” on page E-139

                                          Header

                                          Document No. Internal document number of the supplier invoice. You can
                                          specify any number (designation). If you specify a document number or select
                                          one with <F9> for which an invoice has already been created, you can check
                                          and if necessary edit this invoice.
5.00 / 12-2022




                                          Technical info: alphanumeric field, DB field: kauf.exauftrnr




                 A+W Enterprise Purchasing                                                                         E-129
                 Invoices and Credit Notes                                                           Software Reference




                                         Intern (Invoice/Credit Note) Specification whether an invoice or a credit
                                         note was already created. If you have selected a document number for which
                                         one of these document types was already created, the associated number and
                                         document type (invoice/credit note) is displayed. The possibility of editing the
                                         credit notes via the invoice checking requires separate configuration on the
                                         part of A+W Software GmbH.
                                         Technical info: kauf.auftrnr, kauf.vorgang

                                         Doc. Date Date on which the supplier invoice is entered.
                                         Technical info: mandatory field, date field, DB field: kauf.edat

                                         Booking Date Date on which the supplier invoice is booked. The booking
                                         date is pre-populated by the system with the document date.
                                         Technical info: mandatory field, date field, DB field: kauf.bdat

                                         Site Site number. The field is only enabled if the internal client separation is
                                         active.
                                         Technical info: numeric field, DB field: kauf.hausnr

                                         Supplier Supplier number. If you specify a number, the name of the supplier
                                         is displayed in plain text. If you have specified a supplier, you can only select
                                         POs for this supplier in the PO overview. If you do not select a supplier, the
                                         field is pre-populated automatically with the supplier from the first PO.
                                         Technical info: numeric field, DB field: kauf.kunr

                                         Purchase order overview
                                         •   PO number:
                                             Purchase order number on the supplier invoice.Use <F5> to change to the
                                             External No. field where you can specify the PO via the external num-
                                             ber.Use <Ctrl> + <L> to change to the Deliv. Note field where you can spec-
                                             ify the PO via the delivery note number.
                                             Technical info: mandatory field, alphanumeric field, DB field: kauf.auftrnr
                                         •   Reference Doc.:
                                             Reference document for which the internal invoice is created and booked.
                                             – Goods received: The supplier invoice refers to a goods receipt. The de-
                                                 livery is booked for receipt of goods.
                                             – PO:
                                                 The supplier invoice refers to a PO without goods receipt. The delivery
                                                 is not booked in goods receipt.
                                             Technical info: toggle field, DB field: kaufp.refvorgang
                                         •   SubNr.:
                                             Subnumber for partial deliveries of the goods receipt. For complete deliv-
                                             eries, the subnumber 1 is displayed.
                                             Technical info: numeric field, DB field: kaufp.refsubnr
                                         •   Net amount:
                                             Net amount of the supplier invoice from the PO. You can edit the amount.
                                             Depending on the configuration, only a particular deviation is permitted. If
5.00 / 12-2022




                                             the amount entered deviates from the net amount from the PO, a message
                                             is displayed whether the total difference is acceptable.
                                             Technical info: numeric field, DB field: kauf.nettototal


                 E-130                                                                      A+W Enterprise Purchasing
                 Software Reference                                                           Invoices and Credit Notes




                                        •    External No.:
                                             External number that was entered on the Receipt of goods dialog, e.g. or-
                                             der number from sales if the PO was entered with reference.
                                             Technical info: numeric field, DB field: kauf.exaufnr
                                        •    Delivery note:
                                             Supplier OC number that was entered on the Dispatch notification dialog.
                                             Technical info: numeric field, DB field: kauf.lieferschein

                                        Footer

                                        Total Amount Net Total net amount of the supplier invoice that you have to
                                        enter into the system. The system checks the invoice data by comparing the
                                        total net amount of the POs and the total net amount. The result of the invoice
                                        checking is displayed in a message:
                                        • "Total amount is correct.“:
                                            The total of the invoice amounts from the Net amount matches the Total net
                                            amount. The internal invoice is created with [Yes]. In another message, you
                                            can book the invoice.
                                        • "The total amount is not correct.“:
                                            The total of the invoice amounts from the Net amount column does not
                                            match the Total amount. The difference of the values is displayed as
                                            amount and percentage. In the rules, it is not possible to ignore the invoice
                                            difference. In exceptional cases, the system can be configured so that only
                                            an authorized employee may ignore the difference and create the invoice.
                                        Technical info: numerical field, DB field: kauf.nettototal

                                        VAT Amount VAT amount of the POs. If you create the invoice, the field will
                                        be pre-populated by the system. You can edit the amount. Depending on the
                                        configuration, only a particular deviation is permitted. If the amount entered
                                        deviates from the VAT amount from the POs, a message is displayed.If several
                                        VAT rates are specified for a PO, the individual VAT rates are displayed. This
                                        is important for countries where different tax rates are used. The fields are only
                                        displayed if the multi-VAT module is active.
                                        Technical info: numeric fields, DB fields: kauf.mwstbetrag1, kauf.mwstbetrag2,
                                        kauf.mwstbetrag3, kauf.mwstbetrag4

                                        Total Amount Gross Total gross amount of the POs. The system calculate
                                        the gross amount from the total of Total net amount and VAT amount.
                                        Technical info: numerical field, database field: kauf.gesbrutto

                                        Total Qty Total number of pieces of units from all purchase orders.
                                        Technical info: display field

                                        Total Sqft Total area of the articles from the POs in square meters.
                                        Technical info: display field

                                        Total Ser.Mtr. Total length of the articles from the POs in linear meters.
                                        Technical info: display field
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                         E-131
                 Invoices and Credit Notes                                                            Software Reference




                                           Supplier’s Invoice – Detailed View
                                           Purchase > Invoices > Invoice Check > Find Purchase Order > <F2>




                 Fig. E-51   Supplier's invoice — detailed view


                                           The supplier data and supplier details for the selected PO are displayed in
                                           these views.

                                           Header
                                           The header area is described for the Supplier invoice - PO overview dialog;
                                           the fields on the tabs are described in detail for the Purchase Order Entry dia-
                                           log:
5.00 / 12-2022




                                            “Supplier’s Invoice – Purchase Overview” on page E-129
                                            “Purchase Order Entry” on page E-51



                 E-132                                                                       A+W Enterprise Purchasing
                 Software Reference                                                              Invoices and Credit Notes




                                           Supplier’s Invoice – Item Overview
                                           Purchase > Invoices > Invoice Check > Net Amount Field > <F5>




                 Fig. E-52   Supplier’s invoice – item overview


                                           In these views, the item details for the selected PO are displayed.
                                           Use <F2> to change between the tabs.
                                           The following information is displayed in plain text next to the tabs:
                                           •   P.O.:
                                               Purchase order number.
                                           •   (invoice type):
                                               Specification whether a total or partial invoice is created.
                                               – Partial invoice:
                                                   A partial invoice is created for the PO.
                                               – Total invoice:
                                                   A total invoice is created for the PO.
                                           In the upper right part of the tab, the total number of items in the PO and the
                                           currently selected PO items are displayed. For example, 1 of 3 means that the
5.00 / 12-2022




                                           currently the first item of a total of three items in the PO is selected.




                 A+W Enterprise Purchasing                                                                          E-133
                 Invoices and Credit Notes                                                            Software Reference




                                           Header
                                           The header area is described for the Supplier's Invoice - PO Overview dialog:
                                            “Supplier’s Invoice – Purchase Overview” on page E-129

                                           Items, details tab
                                           Use <F2> to change between Items and Details. The fields are described in
                                           detail with the Purchase order entry – items dialog.
                                            “Purchase Order Items - General” on page E-72


                                           Supplier’s Invoice – Discounts
                                           Purchase > Invoices > Invoice Check > Net Amount Field > <Ctrl> + <A>




                 Fig. E-53   Supplier's invoice - discounts


                                           Use this dialog to enter and check supplier invoices, and to create and book
                                           internal invoices.
                                           Use <Enter> to complete the invoice control, create and book the invoice. If
                                           you create or book an invoice, an internal invoice number will be shown. Alter-
                                           natively, you can book an internal invoice subsequently.
                                            “Booking of Invoices” on page E-139
                                           Afterwards, the booking data for FinAcc is generated.

                                           Header
5.00 / 12-2022




                                           The header area is described for the Supplier's Invoice - PO Overview dialog:
                                            “Supplier’s Invoice – Purchase Overview” on page E-129



                 E-134                                                                       A+W Enterprise Purchasing
                 Software Reference                                                               Invoices and Credit Notes




                                           The body area is described for the Purchase Order Entry - Discounts dialog:
                                            “Purchase Order Entry - Discounts Detailed View” on page E-70



                                           Supplier’s Invoice (Automatic)
                                           Purchase > Invoices > Automatic Invoices




                 Fig. E-54   Supplier invoice (automatic)


                                           Use this dialog to create invoices for full deliveries. Book partial deliveries on
                                           the dialog Supplier invoice (manual) dialog. If there is already a delivery plan
                                           for a PO and part of the delivery is on the current day, the partial invoice for
                                           this delivery can also be created and booked on this dialog.
                                           Use <F3> to then book the internal invoice. Alternatively, you can book the in-
                                           ternal invoice later.
                                            “Booking of Invoices” on page E-139
                                           Afterwards, the booking data for FinAcc is generated.

                                           Body
                                           •   P.O.:
                                               Purchase order number.
                                           •   SubNo.:
                                               Sub-number for deliveries. If this is a full delivery, a 1 is always shown. Par-
5.00 / 12-2022




                                               tial numbers reflect the corresponding number of the partial delivery.
                                           •   Deliv.Plan:
                                               Specification whether the delivery plan exists.



                 A+W Enterprise Purchasing                                                                             E-135
                 Invoices and Credit Notes                                                       Software Reference




                                         •   Receipt:
                                             Delivery has already been booked as receipt of goods.
                                         •   Invoice:
                                             Number of the supplier invoice.
                                         •   Doc. Date:
                                             Date when the supplier has created the invoice.
                                         •   Book. Date:
                                             Date when the internal invoice was booked.
                                         •   Cre.:
                                             Selection to create booking of the item.
                                              Create booking.
                                              Do not create booking.

                                         Footer
                                         Name of supplier and invoice amount of delivery.
5.00 / 12-2022




                 E-136                                                                  A+W Enterprise Purchasing
                 Software Reference                                                            Invoices and Credit Notes




                                           Transferred Invoices
                                           Purchase > Invoices > Booking Invoices > Transferred Invoices




                 Fig. E-55   Transferred invoices - overview


                                           On this tab, there is an overview of all invoices that were transferred via the
                                           openTrans interface. On the Details tab, you can see additional invoice fields
                                           for your information.
                                           This function description is not part of the manual and must be requested if
                                           needed.
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                         E-137
                 Invoices and Credit Notes                                                              Software Reference




                                           Supplier's Invoice (Manual)
                                           Purchase > Invoices > Manual Invoices




                 Fig. E-56   Supplier's invoice (manual)


                                           Use this dialog to edit and manually book internal invoices, e.g. if no prices are
                                           maintained in the system and, as a result, you cannot execute automatic in-
                                           voice generation. Afterwards, the booking data for FinAcc is generated.
                                           The fields, columns, and tabs are described with Purchase order entry dialog:
                                            “Purchase Order Entry” on page E-51
                                           In addition, the following fields and columns are displayed:

                                           Header

                                           Invoice No. Invoice number of the supplier invoice.

                                           General tab
                                           •   Invoice:
                                               Quantity of the item that will be invoiced.

                                           Footer

                                           Balance Invoice amount including VAT.
5.00 / 12-2022




                 E-138                                                                        A+W Enterprise Purchasing
                 Software Reference                                                               Invoices and Credit Notes




                                            Supplier's Invoice (Collective Invoice)
                                            Purchase > Invoices > Collective Invoices




                 Fig. E-57   Supplier's invoice (collective invoice)


                                            On this dialog, you can create and book supplier invoices.
                                            In order to create collective invoices, the purchase orders must meet certain
                                            prerequisites:
                                            •   The supplier accepts the partial invoices. This setting is made in the master
                                                data.
                                            •   For purchase orders, the option Collective invoice must be set in the In-
                                                voice type field.
                                                 “Purchase Order Items - Properties” on page E-81
                                            •   The purchase orders must be booked in receipt of goods.
                                                 “Receipt of Goods (Automatic)” on page E-115
                                            Afterwards, the booking data for FinAcc can be generated.
                                            The fields and the footer area are described for the Supplier's Invoice dialog:
                                             “Supplier’s Invoice (Automatic)” on page E-135



                                            Booking of Invoices
5.00 / 12-2022




                                            Purchase > Invoices > Booking of Invoices




                 A+W Enterprise Purchasing                                                                            E-139
                 Invoices and Credit Notes                                                            Software Reference




                 Fig. E-58   Booking of invoices


                                          On this dialog, you can book already created but not yet booked invoices.
                                          Generally you book internal invoices on one of the following dialogs:
                                           “Invoice Check” on page E-128
                                           “Supplier’s Invoice (Automatic)” on page E-135
                                           “Supplier's Invoice (Manual)” on page E-138
                                           “Supplier's Invoice (Collective Invoice)” on page E-139
                                          Afterwards, the booking data for FinAc can be transferred.
                                          The fields are described in Sales section.
                                           Sales, “Booking of Invoices” on page D-348
5.00 / 12-2022




                 E-140                                                                         A+W Enterprise Purchasing
                 Software Reference                                                           Invoices and Credit Notes




                                          Close Purchase Orders
                                          Purchase > Receipt of Goods > Close Purchase Orders
                                          Purchase > Invoices > Close Purchase Orders




                 Fig. E-59   Close purchase orders


                                          In this dialog, you can manually complete open purchase orders, e.g. if a pur-
                                          chase order has only been delivered partially and no further partial deliveries
                                          will follow.
                                          Use <F3> to manually complete purchase orders.

                                             Close purchase orders regularly
                                             You can complete purchase orders regularly after receiving purchase or-
                                             ders from the supplier. You must book the purchase orders, using the two
                                             dialogs Receipt of goods and Supplier invoice so that the program can
                                             complete the purchase orders regularly.

                                          The columns are described here:
                                           “Receipt of Goods (Automatic)” on page E-115
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                        E-141
                 Invoices and Credit Notes                                                           Software Reference




                                           Invoice Log
                                           Purchase > Invoices > Log




                                           Fig. E-60    Invoice log


                                           This dialog displays the invoice log. All documents for the invoices are noted
                                           with specification of the date and time.


                                           Supplier's Credit Note
                                           Purchase > Credit Notes > Enter Credit Notes




                 Fig. E-61   Supplier's credit note
5.00 / 12-2022




                                           Use this dialog to enter and book credit notes that have been sent by suppli-
                                           ers.


                 E-142                                                                      A+W Enterprise Purchasing
                 Software Reference                                                             Invoices and Credit Notes




                                        The tabs and fields are described for the Purchase Order Entry dialog:
                                         “Purchase Order Entry” on page E-51
                                        In addition, the following fields are displayed:

                                        Header

                                        Number Temporary number of the credit note. When saving, the final credit
                                        note number is assigned by the system at the end of entering credit notes.

                                        Ref. Document number that is being referenced. You create credit notes by
                                        using a reference to a document. You must enter the following data in this or-
                                        der:
                                        • Type of reference document:
                                           – Purchase order.
                                           – Purchasing invoice.
                                           – Purchasing credit note.
                                        • Select supplier.
                                        • Select reference document for the supplier, e.g. purchasing invoice num-
                                           ber.

                                        Body
                                        •    Cred.note:
                                             Quantity of the item that will be allocated for the credit note. However, it is
                                             possible to credit only the item number instead of the quantity.
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                           E-143
                 Overviews                                                                          Software Reference




                                          Overviews
                                          There are several overviews available that allow you to check purchase order
                                          documents.
                                          The following information is available on this chapter:
                                           “Document Information” on page E-144
                                           “Overview of Documents” on page E-145
                                           “Purchase Search” on page E-145



                                          Document Information
                                          Purchase > Overview > P.O. Information > Open P.O.
                                          Purchase > P.O. Management > Open P.O. > Items Tab > General Tab >
                                          Quantity Column > <Shift> + <F10>




                 Fig. E-62   Purchase order information


                                          You can have document information displayed for all purchase orders, e.g.
                                          when the receipt of goods has been booked.
                                          The dialog is described in detail in the Sales section.
                                           Sales, “Order Information” on page D-369
5.00 / 12-2022




                 E-144                                                                      A+W Enterprise Purchasing
                 Software Reference                                                                                 Overviews




                                        Overview of Documents
                                        Purchase > Overview > Receipt of Goods: Today, Receipt of Goods: Delayed,
                                        Receipt of Goods: From - To, Delivered - But not Invoiced, Invoiced - But not
                                        Booked, P.O.s not Transferred




                                        Fig. E-63     Example for an overview dialog: Receipt of goods: from - to


                                        These dialogs display the overviews for the following documents:
                                        •    Receipt of goods: today
                                        •    Receipt of goods: delayed
                                        •    Receipt of goods: from – to
                                        •    Delivered - but not invoiced
                                        •    Invoiced - but not booked
                                        •    Purchase orders not transferred
                                        These overview depend on the configuration and must be released separately.
                                        These dialogs can be designed customer-specifically if necessary. Please
                                        contact a service employee of A+W Software GmbH


                                        Purchase Search
                                        Purchase > Search
                                        Use this dialog to search for documents. The results are displayed in a hit list.
                                        This dialog contains the following tabs and views:
                                         “Purchase Search – Search Mode” on page E-146
                                         “Purchase Search – Overview” on page E-147
                                         “Purchase Search – Details” on page E-149
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                             E-145
                 Overviews                                                             Software Reference




                             Purchase Search – Search Mode
                             Purchase > Search




                             Fig. E-64    Purchase search – search mode


                             On this dialog, you enter the criteria for the document search. The results are
                             displayed in the hit list.
                             Use <F3> to start the search.

                             Site (Order) Site/client number of the orders for which the POs were created.

                             Order Order number.

                             Customer Customer number.

                             Cust. Route Date of the route to the customer for direct delivery.

                             Project Number Number of the project for which the goods have been or-
                             dered.

                             Supplier Supplier number.

                             Site (P.O.) Site or client number of purchase order.

                             P.O. Purchase order number.

                             Ordered for Date when the order should be received. Usually, receipt of
                             goods or in the case of direct delivery, e.g. a construction site.

                             Article Article number.

                             Complete Code for filtering by the receipt status.
                             • 0 = List all purchase orders.
                             • 1 = List partially delivered purchase orders.
5.00 / 12-2022




                             • 2 = List all completely delivered purchase orders.

                             Cancel Code for filtering by the cancellation status.
                             • 0 = List all purchase orders.


                 E-146                                                         A+W Enterprise Purchasing
                 Software Reference                                                                         Overviews




                                          •   1 = List only purchase orders not canceled.
                                          •   2 = List all canceled purchase orders.

                                          OC No. Supplier Number of order confirmation from supplier.

                                          Stock Stock number for which the purchase order was entered.

                                          Input Date Date of the purchase order entry.

                                          Entered by Employee who has entered the purchase order.

                                          Remark Text for the item-related remark.

                                          External No. Order number from Sales if the purchase order has been en-
                                          tered with a reference. Depending on the configuration, alternative data can
                                          be shown. The alternative data is described with the Purchase Order Entry di-
                                          alog:
                                           “Cust. Order” on page E-54

                                          Cost Center Cost center for which the purchase order was entered.

                                          Width, Height Dimensions of the item in millimeters.


                                          Purchase Search – Overview
                                          Purchase > Search > Enter Filter Criteria > <F3>
5.00 / 12-2022




                 Fig. E-65   Purchase search – overview




                 A+W Enterprise Purchasing                                                                      E-147
                 Overviews                                                           Software Reference




                             This dialog displays the result of the search.
                             Switch to the Detail view using <F5>.
                             The following columns are displayed:
                             •   Deliv. Date:
                                 Date of delivery at receipt of goods or at the customer.
                             •   Supplier:
                                 Supplier number.
                             •   P.O.:
                                 Purchase order number.
                             •   Itm:
                                 Item number.
                             •   Article:
                                 Article number.
                             •   Order:
                                 Order number for which the purchase order was entered.
                             •   Customer:
                                 Customer number for which the purchase order was entered.
                             •   Customer Route.:
                                 Customer route. Date of the planned delivery of the order.
                             •   Display fields for the status of the purchase order:
                                 – Empty field = no status exists
                                 – C = Canceled.
                                 – Asterisk * = Fully delivered.
                                 – I = Completely invoiced.
5.00 / 12-2022




                 E-148                                                        A+W Enterprise Purchasing
                 Software Reference                                                                                Overviews




                                          Purchase Search – Details
                                          Purchase > Search > Enter Filter Criteria > <F3> > Mark Entry > <F5>




                 Fig. E-66   Purchase search – details


                                          On this dialog, you can display details about an item on the hit list.
                                          Use <F2> to return to the hit list.
                                          The fields are described with the search mode and the hit list.
                                           “Purchase Search – Search Mode” on page E-146
                                           “Purchase Search – Overview” on page E-147
                                          In addition, the following fields are displayed:

                                          Reject Reason Reject reason in plain text, if it is present.

                                          Entry Date of entry for order-related purchase order.

                                          Entered by Employee name of the person who entered the order.

                                          Customer Customer name and location.

                                          Route Number and description of the delivery route.
5.00 / 12-2022




                 A+W Enterprise Purchasing                                                                            E-149
                 Overviews          Software Reference
5.00 / 12-2022




                 E-150       A+W Enterprise Purchasing
Purchasing                E

                    Partindex




             A+W Enterprise
                 Partindex                                                                  Index




                 Index
                 A                                      – Purchase order entry E-72
                 Address                                – Purchase order, details on E-43
                 – Purchase order entry E-58
                 Allocation                             M
                 – Document type E-96                   Miscellaneous
                 Assessment                             – Purchase order entry   E-65
                 – Purchase order entry E-91            Mode
                                                        – Purchase order entry   E-47
                 C
                 Complaint information                  O
                 – order E-65                           Order
                 – Purchase order entry E-65            – complaint information E-65
                 Create                                 – edit delivery address E-59
                 – Purchase order for item E-42         – partial invoice E-63
                 – Purchase order for supplier E-38     – shipping information E-61
                                                        Order information
                 D                                      – Purchase order entry E-87
                 Delivery address                       Overview
                 – edit E-59                            – documents E-145
                 Details                                – Purchasing E-11
                 – Purchase order for item E-43
                 Document                               P
                 – Details on Purchasing E-149          P.O.
                 – Purchasing, Overview of E-147        – Find E-23
                 – Purchasing, Search regarding E-146   P.O. type E-95
                 Document type                          – Invoice E-95
                 – Allocation E-96                      Partial invoice
                 Documents                              – order E-63
                 – overview E-145                       Payment option
                                                        – Purchase order entry E-65
                 F                                      Prices
                 Find                                   – Purchase order entry E-84
                 – Inquiry E-23                         Properties
                 – P.O. E-23                            – Purchase order entry E-60, E-81
                 Form printing                          Purchase order
                 – Form printing E-98                   – Item, Create for E-42
                                                        – Item, details on E-43
                                                        – Purchase order type E-95
                 I
                                                        – Supplier, Create for E-38
                 Inquiries
                                                        Purchase order entry
                 – Search E-23
                                                        – Address E-58
                 Inquiry
                                                        – Assessment E-91
                 – Find E-23
                                                        – Complaint information E-65
                 – Supplier E-50
                                                        – Item E-72
                 Invoice
                                                        – Miscellaneous E-65
5.00 / 12-2022




                 – P.O. type E-95
                                                        – Mode E-47
                 Item
                                                        – Order information E-87
                 – Create purchase order for   E-42
                                                        – Payment option E-65
                 – Order, in E-56


                 A+W Enterprise Purchasing                                                  E-153
                 Index                                                     Partindex




                 – Prices E-84
                 – Properties E-60, E-81
                 – Status E-47, E-88
                 Purchasing
                 – Overview E-11

                 R
                 Reference   E-73

                 S
                 Search
                 – Inquiries E-23
                 – Purchasing, Details on E-149
                 – Purchasing, Document regarding E-146
                 – Purchasing, Overview of E-147
                 Shipping information
                 – order E-61
                 Status
                 – Purchase order entry E-47, E-88
                 Supplier
                 – Create purchase order for E-38
                 – Inquiry E-50
5.00 / 12-2022




                 E-154                                    A+W Enterprise Purchasing

