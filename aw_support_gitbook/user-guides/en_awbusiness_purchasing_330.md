---
description: "EN AWBusiness Purchasing 3.30"
---



# EN AWBusiness Purchasing 3.30

Purchasing            D




                       English




             A+W Business
                                                                                                              Introduction




                                       Introduction
                                       This part of the documentation contains editorial notes.


                                       Revision Overview
                                       Section          Description
                                       Version/Date

                                       3.30/04-2020     Receipt of goods updated

                                       3.20/11-2019     Software reference: Receipt of goods dialog updated,
                                                        Tutorial: Chapter for boxes moved to the part Box management.

                                       3.10/10-2017     Structural revision, new dialog reorder, dialog OC supplier
                                                        updated.

                                       3.01/01-2017     Product and company names adjusted.

                                       3.00/06-2013     Complete revision of ALFAK documentation and adjustment to
                                                        A+W Business.

                                       2.10/02-2012     Update of the chapters on the receipt of goods

                                       2.00/02-2010     Update and conversion to documentation concept 2010

                                       1.00/10-2008     New Purchasing section
                                                        Separated from section Documents



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
                                       utmost care. Still, errors cannot be totally excluded. A+W Software GmbHcan-
                                       not be held liable for errors or inaccuracies, unless they can be attributed to
                                       wilful or grossly negligent action.
3.30 / 04-2020




                                       This document describes the full scope of A+W Business.




                 A+W Business Purchasing                                                                              D-3
                 Introduction




                                Copyrights
                                © 2020, A+W Software GmbH, all rights reserved, including the right of reprint,
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
3.30 / 04-2020




                 D-4                                                               A+W Business Purchasing
                                                                                                                                                       Contents




                                       Contents
                                       Introduction ............................................................................................................. D-3
                                         Revision Overview ............................................................................................... D-3
                                         Editorial ............................................................................................................... D-3

                                       Tutorial                                                                                                             D-9
                                       Overview ............................................................................................................... D-11
                                         Documentation .................................................................................................. D-12
                                           Tutorial structure ............................................................................................ D-12
                                           Display conventions ....................................................................................... D-13
                                         Menu overview .................................................................................................. D-14
                                       Basic ideas on purchasing .................................................................................... D-17
                                       Master data for purchasing ................................................................................... D-20
                                         Product definition ............................................................................................... D-21
                                           Purchase code ............................................................................................... D-22
                                           Checking a product's master data ................................................................ D-25
                                           Definition of stock sizes ................................................................................. D-27
                                         Suppliers ........................................................................................................... D-29
                                           Market partner supplier ................................................................................. D-30
                                           Checking a supplier's master data ................................................................ D-31
                                           Supplier file amendment ................................................................................ D-32
                                         Purchase prices ................................................................................................. D-34
                                           Price lists ........................................................................................................ D-35
                                           Check price master data ............................................................................... D-36
                                         Document status ............................................................................................... D-38
                                           Status allocation ............................................................................................. D-39
                                           Status allocation ............................................................................................. D-40
                                       Purchase orders ................................................................................................... D-41
                                         P.O. transfer vs. manual purchase order .......................................................... D-42
                                           Document P.O. .............................................................................................. D-43
                                           Checking the default settings for purchase orders ......................................... D-45
                                         P.O. items in the order ...................................................................................... D-48
                                           Customer order ............................................................................................. D-49
                                           Supplier for order item ................................................................................... D-50
                                           Changes in ordered items .............................................................................. D-51
                                           Enter a P.O. item in the order ........................................................................ D-52
                                           Change supplier in order ................................................................................ D-54
                                           Change ordered item ..................................................................................... D-55
                                         P.O. transfer ...................................................................................................... D-58
                                           Order pool ...................................................................................................... D-60
                                           Transfer document to order pool .................................................................... D-66
                                           Changing a P.O. in the order pool ................................................................. D-70
                                           Compare prices in the order pool .................................................................. D-72
                                           Order and P.O. info ........................................................................................ D-76
                                         Manual purchase order ..................................................................................... D-77
                                           Independent P.O.s ......................................................................................... D-78
                                           Entering an independent P.O. ........................................................................ D-79
                                           Enter stock P.O. ............................................................................................. D-81
                                         Supplier's order confirmation ............................................................................. D-84
                                           Supplier's OC ................................................................................................ D-85
                                           Overdue deliveries ........................................................................................ D-86
3.30 / 04-2020




                                           Order confirmation entry ................................................................................ D-87
                                           Enter order confirmation and check prices ................................................... D-91
                                           Remind supplier ............................................................................................. D-95



                 A+W Business Purchasing                                                                                                                      D-5
                 Contents




                              Delivery date check ........................................................................................... D-98
                                Delivery date check and correction ............................................................... D-99
                                Change delivery dates, notify customer ....................................................... D-100
                                Check and change all dates ......................................................................... D-103
                              Inquiry .............................................................................................................. D-108
                                Inquiry for P.O. items or purchase orders ................................................... D-108
                                Create an inquiry for a P.O. item ................................................................ D-110
                                Create a purchase order from an independent inquiry ............................... D-113
                              Exercises ......................................................................................................... D-115
                            Deliveries in receipt of goods .............................................................................. D-117
                              Receipt of goods ............................................................................................. D-118
                                Deliveries ..................................................................................................... D-119
                                Check the default settings for receipt of goods ........................................... D-124
                                Enter receipt of goods .................................................................................. D-125
                                Check receipt of goods ................................................................................ D-131
                              Receipt of boxes .............................................................................................. D-133
                                Dealing with boxes ....................................................................................... D-134
                                Check company data ................................................................................... D-134
                                Checking the settings for ID numbers ......................................................... D-134
                                Enter the receipt of boxes ........................................................................... D-136
                              Price and invoice control ................................................................................. D-141
                                Incoming invoice .......................................................................................... D-142
                                Checking the invoice .................................................................................... D-144
                              Exercises ......................................................................................................... D-147
                            Electronic document exchange ........................................................................... D-148
                              Export/Import (openTRANS) ........................................................................... D-149
                                Document exchange .................................................................................... D-151
                                Document check .......................................................................................... D-154
                                Check the services ....................................................................................... D-157
                                Status allocation ........................................................................................... D-158
                                Check the default settings for data exchange .............................................. D-159
                                Check the currency settings ......................................................................... D-160
                                Check status definitions ............................................................................... D-161
                                Set the data export via openTRANS ........................................................... D-164
                                Check Partner Master Data ......................................................................... D-166
                                Import of electronic documents .................................................................... D-167
                                Check the electronic document .................................................................... D-168
                                Create a partial delivery from an electronic document ................................. D-170
                                Allocate items in electronic documents ........................................................ D-171
                                Allocate surcharges/discounts manually ...................................................... D-172
                              Data export/import (EDI) ................................................................................. D-174
                                Data exchange in ASC format ..................................................................... D-175
                                Check company data ................................................................................... D-175
                                Check the settings ....................................................................................... D-175
                                Exporting of purchase orders ....................................................................... D-179

                            Software Reference                                                                                            D-181
                            Overview ............................................................................................................. D-183
                            Inquiry (menu) ..................................................................................................... D-184
                              Inquiry (document management) .................................................................... D-185
                            Purchase order (menu) ....................................................................................... D-186
                              Purchase order (document management) ....................................................... D-188
                              Replenishment Order ...................................................................................... D-189
3.30 / 04-2020




                              Export (EDI) ..................................................................................................... D-191
                                Functions menu ........................................................................................... D-192
                                Export – export ............................................................................................. D-193
                                Export – pool ................................................................................................ D-194


                 D-6                                                                                         A+W Business Purchasing
                                                                                                                                                       Contents




                                         OC supplier .................................................................................................... D-195
                                           Options menu ............................................................................................... D-195
                                           OC supplier – documents ............................................................................ D-196
                                           OC supplier – items ..................................................................................... D-200
                                           OC Supplier – change delivery dates .......................................................... D-201
                                        Order confirmation ............................................................................................. D-202
                                         Price control .................................................................................................... D-203
                                           Functions menu ........................................................................................... D-203
                                           Options menu ............................................................................................... D-204
                                           Price control – purchase orders ................................................................... D-205
                                           Price control – item ...................................................................................... D-208
                                           Price control – BOM ..................................................................................... D-210
                                         Electronic price control .................................................................................... D-211
                                           Functions menu ........................................................................................... D-212
                                           Options menu ............................................................................................... D-212
                                           Electronic price control – document import ................................................. D-214
                                           Electronic price control – item overview ...................................................... D-217
                                         Selection (prod. no. for balancing item) ........................................................... D-218
                                         Settings for Xternal .......................................................................................... D-219
                                         Manual allocation of items .............................................................................. D-219
                                         Distribution of footer surcharges/discounts ..................................................... D-220
                                         Filter settings ................................................................................................... D-221
                                         Reminder ......................................................................................................... D-223
                                       Receipt of goods ................................................................................................. D-225
                                         Receipt of goods (dialog) ................................................................................ D-225
                                           Functions menu ........................................................................................... D-226
                                           Options menu ............................................................................................... D-226
                                           Print menu .................................................................................................... D-227
                                           Receipt of goods – selection ........................................................................ D-228
                                           Receipt of goods –complete ........................................................................ D-230
                                           Receipt of goods – by item .......................................................................... D-232
                                           Receipt of goods – ID numbers ................................................................... D-235
                                           Receipt of goods – protocol (ID numbers) ................................................... D-237
                                         Settings (ID) .................................................................................................... D-238
                                         Inspection of goods received .......................................................................... D-239
                                           Inspection of goods received – complete P.O.s ........................................... D-239
                                           Inspection of goods received – Qty. discrepancies ...................................... D-241
                                       Invoice ................................................................................................................ D-243
                                         Invoice control ................................................................................................. D-243
                                           Functions menu ........................................................................................... D-244
                                           Options menu ............................................................................................... D-244
                                           Invoice control – Purchase orders ............................................................... D-246
                                           Invoice control – items ................................................................................. D-249
                                           Invoice control – BOM .................................................................................. D-251
                                         Invoice date .................................................................................................... D-253
                                         Electronic invoice control ................................................................................. D-254
                                           Functions menu ........................................................................................... D-254
                                           Options menu ............................................................................................... D-254
                                           Electronic invoice control – document import .............................................. D-257
                                           Electronic invoice control – item overview ................................................... D-260
                                       Invoicing of basic glass ....................................................................................... D-262

                                       Section Index                                                                                                  D-263
3.30 / 04-2020




                                       Index ................................................................................................................... D-265




                 A+W Business Purchasing                                                                                                                      D-7
                 Contents
3.30 / 04-2020




                 D-8        A+W Business Purchasing
Purchasing              D

                    Tutorial




             A+W Business
                 Tutorial                                                                                     Overview




                                       Overview
                                       The tutorial for the Purchasing module deals with the basics of purchasing in
                                       A+W Business. This tutorial is based on existing knowledge of the master data
                                       and on sales.

                                           The functions depend on the enabled modules
                                           Please note that the individual functions are only available if the corre-
                                           sponding modules and interfaces have been installed and enabled.

                                           If you detect functions in this document that are not available in your ver-
                                           sion, please contact A+W Software GmbH.

                                       Subjects
                                       This tutorial offers the following subjects:
                                       •   Basic ideas on purchasing
                                       •   Master data for purchasing
                                       •   Purchase orders
                                       •   Deliveries in receipt of goods
                                       •   Electronic document exchange

                                       Required knowledge
                                       This tutorial is intended for those who process purchase in A+W Business.
                                       Participants must be familiar with the master data concept inA+W Business
                                       and with the Document management dialog.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-11
                 Overview                                                                                   Tutorial




                            Documentation
                            The following documents are available for the Purchasing module:

                            Handout                      Printout of tutorial for training session

                            PDF                          Complete documentation
                                                         • Tutorial
                                                         • Software reference
                                                         • Index

                            Online help <F1>             Context-sensitive dialog help for the A+W Business
                                                         software references and tutorials on the basic version


                            Tutorial structure
                            This tutorial consists of subjects with several training modules each. Each
                            module consists of the following elements:

                            Overview                     Each training module starts with an overview of the
                                                         major topics:
                                                         • Objectives: What knowledge is to be conveyed?
                                                         • Benefit: What can this knowledge be used for?
                                                         • Maxims: Which correlations are to be remembered?

                            Concepts                     First, the concepts and terms of the corresponding
                                                         training module will be explained. This is followed by
                                                         examples and instructions.

                            Exercises                    For some of the modules, exercises with certain tasks
                                                         and suggested solutions are available.

                            Cross-references             At the end of each training module there is a section
                                                         with cross references pointing out additional information
                                                         in the software reference and in other sections.
                                                         This will help you to extend your newly acquired
                                                         knowledge.


                            Reading instructions
                            The contents of a training module are based on the knowledge conveyed in the
                            previous module. We therefore recommend not to skip any modules.
                            If you are already familiar with a subject, you should at least read the summary at the
                            start of the module in order to bring the main details to mind.
3.30 / 04-2020




                 D-12                                                                 A+W Business Purchasing
                 Tutorial                                                                                    Overview




                                       Display conventions
                                       Certain parts of sentences are specially marked. The meanings are:

                                       Italics                 marks character strings describing the software
                                                               elements, e.g. the Number Manager dialog.

                                       Bold                    marks character strings to be entered via the keyboard,
                                                               e.g.: Enter the value 0.

                                       >                       The so-called breadcrumb trail marks the way to open a
                                                               dialog, e.g. Documents > P.O. > Export.

                                       []                      Square brackets mark buttons in a dialog, e.g. [OK] to
                                                               save the data.

                                       <>                      Angle brackets refer to keys or shortcuts on the
                                                               keyboard, e.g. <F1> is used to open the online help.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-13
                 Overview                                                                                      Tutorial




                                        Menu overview
                                        This chapter provides a brief overview of the program sections that will be ad-
                                        dressed in the subjects of this training.
                                        The Documents menu also includes the program sections for handling Sales.
                                        These are described in section Sales.




                 Fig. D-1   Documents module – Purchase order menu


                                        P.O.
                                        Use this section to create and manage purchase orders.
                                         “Purchase orders” on page D-41

                                        Replenishment
                                        Use this dialog you manage orders with ordered parts that are reported as bro-
                                        ken and decide whether they should be reordered, whether a complaint should
                                        be lodged, whether they should be invoiced or deducted from the order quan-
                                        tity.
3.30 / 04-2020




                                         Software Reference, “Replenishment Order” on page D-189




                 D-14                                                                     A+W Business Purchasing
                 Tutorial                                                                                    Overview




                                       Print P.O.
                                       In this dialog you print the purchase orders you are going to send to suppliers.
                                       This function is described in detail in the Sales section.
                                        Sales, “Print” on page C-152

                                       Export
                                       You can use this dialog to export purchase orders in order to transfer them to
                                       the respective supplier via the EDI interface.
                                        “Exporting of purchase orders” on page D-179

                                       Journal
                                       This dialog gives you an overview of the purchase orders. This function is de-
                                       scribed in detail in the Sales section.
                                        Sales, “Journal” on page C-337

                                       OC supplier
                                       In this dialog you enter the order confirmations you have sent to your suppli-
                                       ers.
                                        “Supplier's OC” on page D-85

                                       Order confirmation
                                       In this section you can check the prices in order confirmations.
                                        “Checking the invoice” on page D-144

                                       Receipt of goods
                                       This section is used to check and create receipt of goods for your purchase
                                       orders.
                                        “Receipt of goods” on page D-118

                                       Invoice
                                       This area is used to enter and check invoices from suppliers.
                                        “Check the electronic document” on page D-168

                                       Transfer to financial accounting
                                       This dialog is used to transfer the invoices received to your financial account-
                                       ing system. This function is described in detail in the Sales section.
                                        Sales, “Debit Entry FinAcc” on page C-590

                                       Transfer to archives
                                       This dialog is used to transfer your purchase orders to archives. This function
3.30 / 04-2020




                                       is described in detail in the Sales section.
                                        Sales, “Transfer to Archives” on page C-594




                 A+W Business Purchasing                                                                         D-15
                 Overview                                                                           Tutorial




                            Document data
                            In this dialog you can view lists of purchase orders and the corresponding or-
                            ders and correct dates if necessary. This function is described in detail in the
                            Sales section.
                             Sales, “Document Data” on page C-644

                            Stock search
                            Use this dialog to check product availability and search for stock sizes. This
                            function is described in detail in the Sales section.
                             Sales, “Stock Search” on page C-649

                            Article info
                            In this dialog you can display information on the products entered in
                            A+W Business. You can check the product structure, prices and availability.
                            This function is described in detail in the Sales section.
                             Sales, “Product Information” on page C-521

                            Fax message
                            This dialog allows you to issue and dispatch fax messages to your customers
                            and suppliers directly from A+W Business. This function is described in detail
                            in the Overview section.
                             Einleitung, “Standard-Menüs” auf Seite A-53
3.30 / 04-2020




                 D-16                                                          A+W Business Purchasing
                 Tutorial                                                                  Basic ideas on purchasing




                                         Basic ideas on purchasing
                                         Purchasing is one of the commercial tasks within a company. Purchasing is
                                         typically structured in this or a similar way in A+W Business:




                                                                        Inquiry




                                                         P.O.                         Customer
                                                                                        order

                                                                       Transfer




                                                  OC + price control




                            Stock                 Receipt of goods                               Production




                                                  OC + price control




                  Legend:                 Document                 Section                  optional



                 Fig. D-2    Purchasing scheme in A+W Business


                                         All commercial transactions in A+W Business are based on master data. Pur-
                                         chasing can work properly only if the master data is in order and up to date:
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-17
                 Basic ideas on purchasing                                                                         Tutorial




                                         •   Inquiry:
                                             Inquiries are used to get quotations from your suppliers. If the quotation is
                                             convincing, you can create the purchase order right from the inquiry without
                                             having to enter the data again.
                                              “Inquiry” on page D-108
                                         •   Purchase order:
                                             In a manual purchase order you enter the order items and select the re-
                                             quired supplier.
                                             The reference purchase order is created from the customer order by
                                             means of the order pool.
                                              “Manual purchase order” on page D-77
                                         •   Order confirmation (OC) from the supplier:
                                             Enter the order confirmation number and check the prices and delivery
                                             dates. In case of delays you can notify the customer if necessary. Changed
                                             and confirmed prices can be saved in the PP calculation.
                                              “Order confirmation and delivery date” on page D-85
                                         •   Receipt of goods:
                                             Check the receipt of goods and add stock purchase orders automatically to
                                             the stock on hand. Reference purchase orders are transferred to produc-
                                             tion and/or sales in order to edit the corresponding customer order, or finish
                                             it.
                                              “Enter receipt of goods” on page D-125
                                         •   Invoice control:
                                             Check the invoice and correct the purchase prices if you accept the price
                                             changes. The invoice can now be released for payment.
                                              “Price and invoice control” on page D-141

                                         The purchasing process
                                         Purchasing documents are usually processed on the basis of the following
                                         steps:
                                         •   Create inquiry (optional)
                                         •   Purchase order
                                             – Enter header data
                                             – Enter items
                                             – Edit BOM
                                         •   Print purchase order (send by fax, email, electronically)
                                         •   Enter supplier's order confirmation
                                         •   Check the prices
                                         •   Correct dates and route planning based on feedback
                                         •   Enter receipt of goods
                                         •   Check the invoice
                                         •   Transfer to archives and statistics
                                         •   Delete document from main database
                                         If the purchase order was created by P.O. transfer from a customer order, the
                                         data does not need to be created manually.
3.30 / 04-2020




                 D-18                                                                         A+W Business Purchasing
                 Tutorial                                                                Basic ideas on purchasing




                                           Daily procedure
                                           The easiest way of arranging your daily procedure is by using the Number
                                           Managers. Empty the corresponding Number Manager or create a new one
                                           for that day.
                                           Now create the new documents in this Number Manager. This helps you
                                           keep track of the documents that are new and can or have to be processed.
3.30 / 04-2020




                 A+W Business Purchasing                                                                      D-19
                 Master data for purchasing                                                                    Tutorial




                                         Master data for purchasing
                                         This subject shows you how to adapt the master data for purchasing.
                                         This includes the following training modules:
                                         •    “Product definition” on page D-21
                                         •    “Suppliers” on page D-29
                                         •    “Purchase prices” on page D-34
                                         •    “Document status” on page D-38
3.30 / 04-2020




                 D-20                                                                    A+W Business Purchasing
                 Tutorial                                                                     Master data for purchasing




                                       Product definition
                                       Objectives

                                       • Adapting product master data for purchasing purposes.
                                       • Learning about procurement types for purchase orders.
                                       • Learning about the use of purchase codes in orders.


                                       Benefits

                                       • The purchase code points out products to A+W Business which have to be
                                         ordered.
                                       • By means of the purchase code, a purchase order is automatically created for a
                                         customer order in the order pool. Therefore, the purchase order does not have to
                                         be entered by hand.


                                       Please note:

                                       Procurement type           The code Procurement type defines how the product
                                                                  entered in the order or in the purchase order shall be
                                                                  acquired, e.g. by producing it, taking it from stock, or
                                                                  ordering it.

                                       Purchase code              The following procurement types are called purchase
                                                                  codes:
                                                                  • P.O.
                                                                  • P.O. (complete)

                                       P.O. (complete)            This code is used for products with a bill of materials,
                                                                  which are to be ordered as a whole, e.g. an entire door
                                                                  including the fittings.

                                       P.O.                       This code is used for products for which individual
                                                                  elements are to be ordered, e.g. only the fittings.

                                       Default settings           Master data
                                                                  Product management:
                                                                  • Price/Surcharge tab
                                                                  • Stock/Purchasing tab
                                                                  Company data:
                                                                  •   Stock/PP/EDI tab
                                                                  •   Documents tab
                                                                  •   Parameters tab
                                                                  •   Calculation tab
3.30 / 04-2020




                 A+W Business Purchasing                                                                                D-21
                 Master data for purchasing                                                                            Tutorial




                                         Purchase code
                                         Purchasing refers to the products managed in A+W Business. To buy a prod-
                                         uct, it needs to be entered in a purchase order.
                                         You can define how every product is to be used for pricing, discount calcula-
                                         tion, production, purchasing, etc. Only the appropriate codes permit, for exam-
                                         ple, automatic transfer to interfaces, invoicing, or printing in the documents.
                                         The procurement type requires special attention in connection with purchasing
                                         because it tells A+W Business when a product or a product element has to be
                                         purchased.
                                         •    P.O. item (complete):
                                              The P.O. includes all processing steps defined in the bill of materials. If, for
                                              example, a laminated glass unit consists of float sheet 5 mm, a film layer
                                              and tempered glass 5 mm, the laminated unit will be ordered as a whole.
                                              (Please also note the difference from P.O. items.)
                                         •    P.O. items:
                                              Only the concerned product is ordered, without taking into account the con-
                                              tent of the bill of materials (e.g. processing steps). If, on the other hand, e.g.
                                              a laminated unit consists of a float sheet, a film layer and a tempered sheet
                                              and if the code Purchase article has now been set for the tempered sheet,
                                              only the tempered sheet will be ordered from the supplier. The laminated
                                              unit will be produced in-house.
                                         This purchase code is automatically adopted for the order item. Every item can
                                         be allocated a purchase code in the order itself however.
3.30 / 04-2020




                 D-22                                                                            A+W Business Purchasing
                 Tutorial                                                                       Master data for purchasing




                                             Procurement type
                                             These procurement types for the purchase code are defined in the product
                                             master data. It is used by default when a product is entered in a document. It
                                             can be changed in the order and in the P.O.


                    * = P.O., ** P.O. complete

                                                                                         Float 4 Bronze is arrissed
                      IG 150000                                                          IG is produced
                      • Float_5
                      • AIR
                                                             Float 4 Bronze is
                      • Float_4_Bronze *
                                                             delivered unarrissed
                        -edges arrissed
                      • Step


                      IG 150000                                                          IG is produced
                      • Float_5
                      • AIR
                                                             Float 4 Bronze is
                      • Float_4_Bronze **
                                                             delivered arrissed
                        -edges arrissed
                      • Step


                      IG 150000 **                           IG is delivered complete
                      • Float_5
                      • AIR
                      • Float_4_Bronze
                        -edges arrissed
                      • Step



                 Fig. D-3     Purchase code in BOM


                                             If a main item or a superordinate BOM element is marked with the procure-
                                             ment type P.O. (complete), the corresponding BOM elements will not be with-
                                             drawn from stock if their procurement types are set to Stock withdrawal. The
                                             procurement type cannot be changed for these elements in this case.
3.30 / 04-2020




                 A+W Business Purchasing                                                                              D-23
                 Master data for purchasing                                                                     Tutorial




                                         The procurement type can be defined per Client and/or production prepara-
                                         tion. In this case, please activate the option Activate different procurement
                                         type per client/PS area in the company data.




                                          A

                                         A Different procurement type per client or production preparation.
                                         Fig. D-4      Company data – Parameters tab


                                         Prices and surcharges
                                         Price tables are created for both purchasing and sales. They have to be allo-
                                         cated to every single product to make sure that the corresponding prices are
                                         calculated automatically.
3.30 / 04-2020




                 D-24                                                                          A+W Business Purchasing
                 Tutorial                                                                       Master data for purchasing




                                           Checking a product's master data
                                           For purchasing, in particular all product data that are ordered by default has to
                                           be completely entered.
                                           The Master data section describes in detail how to define the master data for
                                           your products. The following description therefore only deals with the peculiar-
                                           ities you have to consider in connection with purchasing.


                                            How to check a product's master data
                                           1 Select Master Data > Products > Articles > Articles.
                                              The Product management dialog appears.
                                               Master Data, “Product Management – Stock / Purchasing” on page B-598
                                           2 Search the product you want to check and go to the Price/surcharge tab.




                                                                                                                         A


                                                                                                                         B




                    A Pricing for sales purposes                          B Pricing for purchasing purposes
                    Fig. D-5     Product management – Price/surcharge


                                           3 Check whether price tables and the checkboxes Price relevant for sales(A)
                                             and purchasing (B) are correctly selected.
3.30 / 04-2020




                                              Checkbox Price relevant PP has to be ticked only if you are using purchase
                                              price calculation.




                 A+W Business Purchasing                                                                              D-25
                 Master data for purchasing                                                                    Tutorial




                                              For more information on prices, please see:
                                               “Purchase prices” on page D-34
                                          4 Go to the Stock/Purchasing tab.




                                                                                                                    A




                                                                                                                    B




                    A Choosing the procurement type                      B Selection for divergent codes
                    Fig. D-6    Product management – Stock/purchasing


                                          5 Check whether the procurement type (A) has been set correctly.
                                              You can select the following entries for P.O. items:
                                              •   P.O.(complete):
                                                  Product with BOM and product which is ordered as a whole, e.g. an en-
                                                  tire door including the fittings.
                                              •   P.O.:
                                                  Product without BOM and product which is ordered as BOM elements
                                                  (partly or completely).
                                          6 Go to the menu Start > Save to save the data.
                                              Data is saved.
3.30 / 04-2020




                 D-26                                                                         A+W Business Purchasing
                 Tutorial                                                                          Master data for purchasing




                                             Definition of stock sizes
                                             For correct pricing, you can define stock sizes for the products, e.g. glass with
                                             fixed sizes. If a product is to be kept on stock as well, you also have to enter it
                                             in stock management. For details, please refer to the Stock management sec-
                                             tion.


                                              How to define stock sizes in master data
                                             1 Select Master data > Products > Articles > Stock sizes
                                                The Product management – stock sizes dialog appears.
                                                 Master Data, “Stock Sizes” on page B-626
                                             2 Go to the menu Start > New to switch to the input mode.


                                         B                 A




                 C

                 D




                 A Lite size                                          C Set price tables for sales and purchasing
                 B Content for boxes                                  D Pricing in stock
                 Fig. D-7    Fields for stock size are released


                                             3 Enter the size (A) an.
                                                If you have already entered a corresponding stock article in stock manage-
3.30 / 04-2020




                                                ment, enter the same width and height.
                                             4 If the stock size is managed as a box, enter the number of sheets (B) in the
                                               box.


                 A+W Business Purchasing                                                                                  D-27
                 Master data for purchasing                                                                         Tutorial




                                          5 You can make the following, different settings:
                                              •   Price keys (C) for sales and purchasing.
                                              •   Description and short description (matchcode), e.g. for better identifica-
                                                  tion of the stock article.
                                              •   Procurement type, e.g. stock withdrawal for stock sizes, which are also
                                                  available as stock articles.
                                              If you want to enter the stock size as a stock article as well, you have to
                                              decide whether pricing shall also be done on stock.
                                          6 Tick the checkbox Search stock PP (D) if the stock size is to be included in
                                            pricing.




                    Fig. D-8    New stock size for pricing.


                                          7 Go to the menu Start > Save to save the data.
                                              The data is saved. Next, the system will want to know whether you want to
                                              define this stock size as a stock article as well.
                                          8 Choose [Yes] if the stock size is also be managed as a stock article.
                                              The Stock management dialog appears. The creation of stock articles is
                                              described in detail in the Stock management section.
3.30 / 04-2020




                                               Inventory Management, “Create a Stock Article” on page G-66




                 D-28                                                                          A+W Business Purchasing
                 Tutorial                                                                       Master data for purchasing




                                       Suppliers
                                       Objectives

                                       • Creating suppliers as market partners.
                                       • Allocating a standard supplier.
                                       • Learning about the supplier file.


                                       Benefits

                                       • Purchase orders can be directly sent to the supplier by means of the defined
                                         communication channels.
                                       • Standard suppliers are automatically entered in the purchase order. They can be
                                         changed however if necessary.
                                       • Based on the delivery time, the dates for purchase orders and reference orders are
                                         calculated.


                                       Please note:

                                       Market partner              All suppliers are entered in the Partner management
                                                                   dialog.

                                       Supplier file               The supplier file specifies which products or product
                                                                   groups are delivered by the individual suppliers. This
                                                                   information is also required for the transfer of order items
                                                                   to Purchasing, among other things.

                                       Standard supplier           A standard supplier is defined if several suppliers have
                                                                   been entered for a product or a product group.

                                       Default settings            Master data:
                                                                   • Supplier data (market partners)
                                                                   • Supplier file
3.30 / 04-2020




                 A+W Business Purchasing                                                                                 D-29
                 Master data for purchasing                                                                         Tutorial




                                         Market partner supplier
                                         Suppliers are entered in A+W Business for the automatic processing of pur-
                                         chase orders. When you enter orders and purchase orders, the supplier data
                                         therefore does not have to be defined specifically.
                                         Like customers, suppliers are entered in the Partner management dialog. The
                                         data for communication must be correctly entered in supplier master data to
                                         make sure that documents can be directly sent from A+W Business.

                                         Supplier file
                                         The supplier file specifies which products or product groups are delivered by
                                         the individual suppliers. If a product and the corresponding product groups are
                                         entered for a supplier, transfer to purchasing will handle this product with pri-
                                         ority.
                                         The details from the supplier file will be ignored if an alternative supplier is en-
                                         tered for an item or a BOM element in the document header.
                                         If several suppliers have been entered for a product, transfer to purchasing
                                         can trigger a comparison of prices. The delivery time is displayed at the same
                                         time so that stored delivery times can be taken into account as well.

                                         Standard supplier
                                         If a standard supplier has been defined, the purchase order does not have to
                                         be sent via the order pool. The standard supplier gets rank number 1 while all
                                         other suppliers are numbered in the sequence matching their importance for
                                         purchasing.
                                         Every product has just one standard supplier. If large quantities of a certain
                                         product are ordered however, which the standard supplier is unable to pro-
                                         duce, a standard supplier for serial orders can be defined as well. In this case,
                                         you will enable the document type Serial order at order entry. With the P.O.
                                         transfer, the system will automatically select the supplier defined for serial or-
                                         ders.
3.30 / 04-2020




                 D-30                                                                          A+W Business Purchasing
                 Tutorial                                                                      Master data for purchasing




                                           Checking a supplier's master data
                                           To ensure that orders are settled correctly, you have to set up the master data
                                           of a supplier and the allocation of products to suppliers.
                                           The Master data tutorial describes in detail how to define the master data for
                                           your partners. The following description therefore only deals with the peculiar-
                                           ities you have to consider in connection with purchasing.


                                            How to check the master data of your suppliers
                                           1 Go to the menu Master data > Market partners > Supplier > Suppliers.
                                           2 Search for the supplier whose data you want to check.




                                                                                                                              B




                    A




                    A Email address of the supplier                  B Language to be used for form printout
                    Fig. D-9     Master data – Suppliers


                                           3 Check in the Address tab whether the data for written correspondence and
                                             communication is complete and up to date.
                                               The email address can also be used for the exchange of electronic docu-
                                               ments, e.g. PDF files. Make sure that the spelling is correct and complete.
3.30 / 04-2020




                 A+W Business Purchasing                                                                             D-31
                 Master data for purchasing                                                                         Tutorial




                                           4 Go to the Order tab and check whether document dispatch has been set
                                             correctly.




                                                     A       B
                                               A Fax P.O.                             B Email inquiry
                                               Fig. D-10     Fax and email dispatch (example settings)


                                           5 Go to the menu Start > Save to save the changes made.
                                               The data is saved.


                                           Supplier file amendment
                                           The supplier file is used to define the suppliers for the individual products or
                                           product groups as well as the corresponding delivery times.


                                            How to check the supplier file
                                           1 Select the menu Master data > Market partner > Supplier > File.
                                               The Supplier file dialog opens on the Products tab.
                                           2 Go to the menu Start > Filter to switch to the search mode.




                    A
                    B
3.30 / 04-2020




                    A   Product option                            B Selection of variants
                    Fig. D-11    Supplier file – Product search


                 D-32                                                                            A+W Business Purchasing
                 Tutorial                                                                          Master data for purchasing




                                               3 Select the Product (A) option and enter the number of the product.
                                               4 To start the search, go to the menu Start > Search.
                                                  The Product – Suppliers section lists all suppliers who can provide the se-
                                                  lected product. Rank 1 marks the standard supplier.




                    A

                    B




                                                               C                      D
                    A Different descriptions                        C Rank 1 = standard supplier
                    B Delivery time                                 D Change priority
                    Fig. D-12    Supplier file – Products


                                               5 Enter the number (B) of days to be used to calculate the delivery time.
                                                  The delivery time will be taken into account when prices are compared
                                                  upon P.O. transfer, and for checking delivery dates.
                                               6 Check the priority of the suppliers and correct it if required by selecting an
                                                 entry and moving it up or down by means of the arrow keys (D).
                                                  Rank 1 (C) marks the standard supplier. It will be automatically used for
                                                  purchase orders that are not checked in the order pool.
                                               7 If your supplier uses different product names, enter them (A).
                                                  These descriptions are listed in the purchase order and help avoid misun-
                                                  derstandings.
                                               8 Go to the menu Start > Save to save the data.
3.30 / 04-2020




                                                  To check whole product groups, go to the Product groups tab and proceed
                                                  in the same way.




                 A+W Business Purchasing                                                                                 D-33
                 Master data for purchasing                                                                            Tutorial




                                         Purchase prices
                                         Objectives

                                         • Learning about price years, keys, and rates for purchase prices (PP).
                                         • Editing purchase prices.


                                         Benefits

                                         • Purchase prices are calculated at order and P.O. entry so that the contribution
                                           margin can be determined automatically.
                                         • Purchase prices can be changed in the purchase order.


                                         Please note:

                                         Price list                  Price years, keys, and rates are the basis for the price
                                                                     lists.

                                         Individual prices           Individual supplier prices can be defined with all
                                                                     reference values which also apply to the general price
                                                                     lists and surcharges.

                                         Default settings            Master data:
                                                                     •   Year
                                                                     •   Key
                                                                     •   Rates
                                                                     •   Prices
                                                                     Company data:
                                                                     • Stock/ PP / EDI tab
                                                                     • Pricing tab
                                                                     • FinAcc tab
                                                                     References:
                                                                     • VEGLA price import
                                                                     Utilities:
                                                                     • Import of price lists
3.30 / 04-2020




                 D-34                                                                           A+W Business Purchasing
                 Tutorial                                                                     Master data for purchasing




                                       Price lists
                                       Pricing in A+W Business consists of flexible modules covering all pricing op-
                                       tions. A suitable pricing method can be allocated to every product.
                                       Price years, keys, and rates are the basis for the price lists. The amounts to
                                       be used in the documents are defined in the price tables.
                                       Prices can be defined as standard price lists or price lists for certain customer
                                       or supplier groups, for individual customers or suppliers.
                                       Purchasing is usually based on just one price key, e.g. the PP key. You can of
                                       course use different price keys for purchasing if required.
                                       Prices are calculated based on the following hierarchy:
                                       •   Manual price input in the order or quotation (top priority)
                                       •   Project-related agreements
                                       •   Customer-/supplier-related agreements
                                       •   Group-related agreements
                                       •   General agreements
                                       Within these hierarchy levels, you can enter general prices, special conditions
                                       for product groups and individual products, alternative prices and surcharges
                                       for shapes and Georgian bars.

                                       Individual prices
                                       For the definition of individual prices for customers and suppliers, you can use
                                       all the reference values that apply to the general price lists and surcharges.
                                       You can either enter price tables for individual customers or suppliers, or adapt
                                       the prices in the document as agreed.

                                       Import of price lists
                                       You can import price lists from your suppliers, e.g. if they are available as a file.

                                           History of price changes
                                           If you are using a Gupta database, you can trace the history of price chang-
                                           es. This function is described in the Master data section.
3.30 / 04-2020




                 A+W Business Purchasing                                                                              D-35
                 Master data for purchasing                                                                             Tutorial




                                              Check price master data
                                              In P.O.s, prices can only be calculated if the purchase prices are correct. The
                                              Master data section describes in detail how to define the master data for your
                                              prices. The following description therefore only deals with the peculiarities you
                                              have to consider in connection with purchasing.


                                               How to check the master data of your price lists
                                              1 Go to the menu Master data > Prices > Prices and check whether year, key,
                                                and rate of the purchase prices (PP) have been defined correctly.
                                              2 Switch to the Prices dialog and view the table and the PP rates.
                                                 If you do not restrict your search, all price tables will be listed.


                                         A                                     B




                 A Unit price                                             B Price table
                 Fig. D-13      Purchase price tables – Price selection


                                              3 Select the price table (B) that you want to check and go to the tab in which
                                                the price is defined.
3.30 / 04-2020




                                                 In this example, the unit price (A) is checked.




                 D-36                                                                               A+W Business Purchasing
                 Tutorial                                                                       Master data for purchasing




                                                               A      B                               C




                    A Price                            B Price unit                      C Currency
                    Fig. D-14   Price selection – Unit price


                                              The overview lists all rates of the selected price table. The non-defined pric-
                                              es are written in red letters.
                                           4 Check whether the price is up to date, and correct it if necessary. To do this,
                                             position the cursor on the Price field and overwrite the entry.
                                           5 Go to the menu Start > Save to save the data.
                                              The data is saved.


                                           Additional information
                                            Master Data, “Price Master Data” on page B-208
                                            Master Data, “Define Unit Prices” on page B-233
                                            Master Data, “Company Data – Calculation” on page B-952
3.30 / 04-2020




                 A+W Business Purchasing                                                                               D-37
                 Master data for purchasing                                                                           Tutorial




                                         Document status
                                         Objectives

                                         • Learning about the status changes in reference documents.
                                         • Checking the status allocation.


                                         Benefits

                                         • Status allocations for reference documents are maintained in addition to the status
                                           allocations for independent documents. The status therefore tells you whether a
                                           purchase order has a reference.
                                         • Goods received for a purchase order will change the status of the reference order.
                                           The order therefore shows the current status.


                                         Please note:

                                         Status allocations          Status allocations for reference documents have to have
                                                                     the same minimum status.

                                         Change of status            The status of the reference order is changed upon
                                                                     receipt of goods for a purchase order.

                                         Default settings            Master data:
                                                                     • Status allocation
3.30 / 04-2020




                 D-38                                                                           A+W Business Purchasing
                 Tutorial                                                                   Master data for purchasing




                                       Status allocation
                                       The purchase documents go through several program items from entry to ar-
                                       chiving, each of which are identified by a status. Conditions and locks can be
                                       linked to this status.
                                       The definition of status points and allocations ultimately depends on the busi-
                                       ness processes in your company. The Master data section offers a detailed de-
                                       scription.




                                                                                                                       A




                                                                                                                       B




                                       A Status for an order with reference P.O. B Corresponding status for the P.O.
                                       Fig. D-15    Status allocation for reference documents


                                       Status allocations for reference documents and independent documents are
                                       set up separately, e.g. for receipt of goods.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-39
                 Master data for purchasing                                                                            Tutorial




                                         Status allocation
                                         The status of documents is generally changed when a purchase order is
                                         changed, sent, etc. A differentiation is made between whether the purchase
                                         order is generated by an order or independently.

                                              Examples

                                              for orders                             for purchase orders

                                              30 - Transfer order to Purchasing

                                              31 - OC supplier partly/order          62 - OC supplier partly/purchase order

                                              32 - OC supplier complete/order        63 - OC supplier complete/purchase order

                                              33 - Partial receipt of goods/order    64 - Partial receipt of goods/purchase
                                                                                     order

                                              34 - Complete receipt of goods/order   65 - Complete receipt of goods/purchase
                                                                                     order

                                                                                     66 - Invoice control


                                         The status of the purchase order changes when the supplier's order confirma-
                                         tion (OC) number is entered upon receipt of goods.
                                         If receipt of goods is booked for a purchase order based on a customer order
                                         (reference P.O.) for which there are still other, open purchase orders, the sta-
                                         tus of the order is set to Partial receipt of goods/order.


                                         Additional information
                                          Sales, “Status” on page C-183
                                          Master Data, “Handling of Business Processes” on page B-413
                                          Master Data, “Status Allocation” on page B-872
3.30 / 04-2020




                 D-40                                                                            A+W Business Purchasing
                 Tutorial                                                                               Purchase orders




                                       Purchase orders
                                       This subject shows you how to create purchase orders and check dates.
                                       This includes the following training modules:
                                       •   “P.O. transfer vs. manual purchase order” on page D-42
                                       •   “P.O. items in the order” on page D-48
                                       •   “P.O. transfer” on page D-58
                                       •   “Manual purchase order” on page D-77
                                       •   “Supplier's order confirmation” on page D-84
                                       •   “Delivery date check” on page D-98
                                       •   “Inquiry” on page D-108
                                       Normally, you enter a purchase order in the following steps:
                                       •   Create inquiry (optional)
                                       •   Enter purchase order
                                       •   Send purchase order to supplier
                                       •   Enter supplier's order confirmation
                                           – Check the prices
                                           – Correct dates and route planning based on feedback
                                           – Inform customer of changed dates
                                       •   Remind supplier of order confirmation
                                       This sequence more or less matches the sequence of dialogs in
                                       A+W Business. Some of the steps however can be executed via several dia-
                                       logs however. This is why they have been summed up in one training session.
                                       Prices can be checked in the supplier's order confirmation. In practice, it is not
                                       unusual that the order confirmation and delivery are received together with the
                                       invoice. As the dialogs for price control and invoice control are identical, the
                                       concept of price and invoice control is explained in the Receipt of goods sub-
                                       ject.
                                        “Incoming invoice” on page D-142
                                       An inquiry is obviously issued before the purchase order but it is not strictly re-
                                       quired. This tutorial deals with inquiries after the purchase orders because you
                                       will be familiar with the details of purchase orders by then.
3.30 / 04-2020




                 A+W Business Purchasing                                                                            D-41
                 Purchase orders                                                                              Tutorial




                                   P.O. transfer vs. manual purchase order
                                   Objectives

                                   • Learning about the difference between automatic (reference) and independent
                                     purchase orders.


                                   Benefits

                                   • Order items which have to be ordered, can be automatically passed on to a
                                     (reference) P.O.
                                   • The stock is topped up by stock P.O.s. These are entered manually. They can also
                                     be created when the stock falls below the defined minimum. (This function is
                                     described in the Stock management tutorial.)


                                   Please note:

                                   P.O. based on order        Order items to be ordered are transferred to Purchasing
                                                              by means of the order pool. Transfer automatically
                                                              creates a purchase order.

                                   Reference P.O.             An order item passed on to Purchasing is turned into a
                                                              reference P.O. with its own document number.

                                   Independent P.O.           Independent purchase orders are entered manually.
                                                              In case of independent purchase orders, the stock will
                                                              not be updated when receipt of goods is booked.

                                   Stock P.O.                 Stock P.O.s serve to replenish the stock. They can be
                                                              entered manually.

                                   Default settings           Master data:
                                                              • Supplier data (market partners)
                                                              • Supplier file
                                                              Company data:
                                                              • Documents tab
                                                              • Parameters tab
                                                              • Stock/PP/EDI tab
3.30 / 04-2020




                 D-42                                                                   A+W Business Purchasing
                 Tutorial                                                                                   Purchase orders




                                               Document P.O.
                                               Purchase orders can be entered independently or based on an order:
                                               •   Independent (reference) purchase orders refer to an item in the customer
                                                   order. They are created by the P.O. transfer. In the order pool,
                                                   A+W Business suggests a supplier based on the data entered in the sup-
                                                   plier file.
                                               •   Independent purchase orders usually do not serve to replenish the stock
                                                   because receipt of goods will not automatically update the stock – receipt
                                                   of goods is entered manually.
                                               •   Stock P.O.s serve to replenish the stock. They can be entered manually or
                                                   by the stock falling below the defined minimum.




                     Order-dependent P.O.
                                                                                             Order

                                                                Receipt of goods
                     Independent
                     P.O.




                     Manual stock P.O.


                                                                Receipt of goods
                     Automatic stock P.O.




                                                              Stock
                                                              • Float 3
                             Minimum stock                    • Float 4
                                                              • Float 5
                                                              • …




                 Fig. D-16     Types of P.O.


                                               This simplified example shows you what the different orders are created for.
                                               The following units will describe order-dependent and independent P.O. orders
                                               in detail.
                                               Stock P.O.s are described in detail in the Stock management section.
                                               All purchase orders are individual documents with their own number ar-
3.30 / 04-2020




                                               ea.They are shown in the document management dialog and can be edited in-
                                               dependently of how they were created.



                 A+W Business Purchasing                                                                               D-43
                 Purchase orders                                                                         Tutorial




                                   A




                                   B




                                   C




                                   A Delivery by the                 C Document type:
                                     supplier                          - <n.s.>: automatic or manual
                                   B Additional information, e.g.        P.O.
                                     reference to the order            - Stock P.O.

                                   Fig. D-17     Document P.O.


                                   Purchase orders must be sent to the supplier. Apart from faxing and emailing,
                                   this can also be done by means of interfaces.
3.30 / 04-2020




                 D-44                                                                A+W Business Purchasing
                 Tutorial                                                                                          Purchase orders




                                              Checking the default settings for purchase orders
                                              For the P.O.s, you have to check the default settings for the company data.
                                              The Master data section describes in detail how to define the master data for
                                              your company. The following description therefore only deals with the peculiar-
                                              ities you have to consider in connection with purchasing.

                                                  Reboot A+W Business
                                                  After changing company data, reboot A+W Business.


                                               How to check the settings for purchase orders
                                              1 Select Master data > Company > Company data
                                                  The Company data dialog appears.
                                              2 Go to the Documents tab and check the settings for sending faxes and
                                                emails.




                 A
                 B                                                                                                                C




                 A Fax dispatch, individually or collectively per supplier/ B Email dispatch individually or collectively per supplier/
                   customer                                                   customer
                                                                            C File format that is sent as an email attachment.
                 Fig. D-18     Company data > Documents
3.30 / 04-2020




                                              3 Go to the Parameters tab and check the settings as shown in the following
                                                illustration.


                 A+W Business Purchasing                                                                                        D-45
                 Purchase orders                                                                                   Tutorial




                                                                                                                         D
                                                                                                                         C

                                                                                                                         B


                    A




                   A Adopt changes to items in the reference documentC Automatically mark items with sizes that exceed the
                   B Adopt order texts from the customer order for the   stock sizes as a P.O.
                     openTRANS exchange                                D Virtual item numbers for the receipt of boxes
                   Fig. D-19    Company data – Parameters


                                             The settings are described in detail in separate units.
                                             •   Checkbox A:
                                                  “Change ordered item” on page D-55
                                             •   Checkboxes B and D:
                                                  “Dealing with boxes” on page D-134
                                                  “Export/Import (openTRANS)” on page D-149
                                             •   Stock P.O.s (C) are described in detail in the Stock management sec-
                                                 tion.
3.30 / 04-2020




                 D-46                                                                         A+W Business Purchasing
                 Tutorial                                                                               Purchase orders




                                           4 Go to the Stock/PP/EDI tab and check the setting in the Purchasing sec-
                                             tion.




                    A
                    B




                    A Purchase code for IG units which include        B Show items from stock P.O.s even though they are
                      processing                                        not inventory items
                    Fig. D-20    Company data – Inventory/Purchasing/EDI


                                           5 Tick the checkbox IG as P.O. item (process. steps as in-house prod.) (A).
                                              If the BOM of an IG unit includes processing steps of the procurement type
                                              Production (in-house), these can be ordered as well. This setting is useful
                                              if you order IG units only in case of production bottlenecks.
                                           6 Go to the menu Start > Save to save the data.
                                              The data is saved.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-47
                 Purchase orders                                                                                  Tutorial




                                   P.O. items in the order
                                   Objectives

                                   •   Entering P.O. items and allocating codes
                                   •   Changing the supplier of an order item
                                   •   Changing the supplier for the entire order
                                   •   Change ordered item


                                   Benefits

                                   • Order items can be turned into purchase orders without the need to enter the items
                                     again in a purchase order.


                                   Please note:

                                   P.O. item                     P.O. items from orders create a separate P.O. per
                                                                 standard supplier.

                                   Purchase code                 The following procurement types are called purchase
                                                                 codes:
                                                                 • P.O.
                                                                 • P.O. (complete)

                                   P.O. (complete)               This code is used for products with a bill of materials,
                                                                 which are to be ordered as a whole, e.g. an entire door
                                                                 including the fittings.

                                   P.O.                          This code is used for products for which individual
                                                                 elements are to be ordered, e.g. only the fittings.

                                   Default settings              Master data:
                                                                 • Supplier data (market partners)
                                                                 • Supplier file
                                                                 Company data:
                                                                 • Documents tab
                                                                 • Parameters tab
                                                                 • Stock/PP/EDI tab
3.30 / 04-2020




                 D-48                                                                       A+W Business Purchasing
                 Tutorial                                                                                Purchase orders




                                         Customer order
                                         Customer orders can include items that have to be ordered for different rea-
                                         sons, e.g. because the product is not kept on stock or because production bot-
                                         tlenecks put the delivery date at risk, so that the entire item has to be ordered.
                                         Therefore, basically any item of an order can be ordered.
                                         Purchase orders for order items can be issued from the orders. For this pur-
                                         pose, at least one BOM element or the whole item must be marked as a P.O.
                                         Purchase orders are not automatically transferred to Purchasing. You can de-
                                         fine that a message is issued upon closing item entry should an order include
                                         purchase articles.




                                A                                                B
                 A BOM component shall be ordered                   B Procurement type of the component changed in the
                                                                      purchase order
                 Fig. D-21   Purchase code for BOM element


                                         A new document is generated for the P.O. items in an order: a purchase order.
                                         This document is generated by transferring the order to Purchasing. The P.O.
                                         transfer is described in a separate unit.
                                          “P.O. transfer” on page D-58
                                         If an order includes several purchase items, the system creates as many pur-
                                         chase orders as different standard suppliers are found in the supplier file.
3.30 / 04-2020




                 A+W Business Purchasing                                                                             D-49
                 Purchase orders                                                                            Tutorial




                                   Supplier for order item
                                   Please make sure that you select the appropriate supplier for P.O. items in the
                                   order. You have the following options:
                                   •   Document entry – Terms tab:




                                       This setting applies for all items of the present order unless they are
                                       changed (afterwards) on item or BOM level.
                                   •   Item entry – Supplement tab:




                                       The setting applies only to the selected item.
                                   •   Item entry – BOM tab:




                                       The setting applies only to the selected BOM element.
                                   •   P.O. transfer:
                                       If no entries are made for the above options, the standard supplier will be
                                       used by default.
                                       The settings from the order and/or product master data can be changed in
                                       the order pool.
                                       The P.O. transfer is described in a separate unit.
3.30 / 04-2020




                 D-50                                                                   A+W Business Purchasing
                 Tutorial                                                                             Purchase orders




                                       Changes in ordered items
                                       Order items that have already been ordered or blocked from further process-
                                       ing. They can only be changed later in item entry of the order (or P.O.) if the
                                       lock is removed manually. Changes may involve, e.g. prices, quantities or siz-
                                       es. The rate can be changed in spite of the lock.
                                       The changes to purchase orders have to be saved in the reference orders. If
                                       you change the size or quantity of an ordered item, you can enter the changes
                                       in the original P.O. The P.O. must then be sent to the supplier again, informing
                                       him of the changes.
                                       The changed order must then again be transferred to Purchasing by way of
                                       the order pool.
3.30 / 04-2020




                 A+W Business Purchasing                                                                         D-51
                 Purchase orders                                                                                Tutorial




                                           Enter a P.O. item in the order
                                           Elements or entire items can be entered in an item position from which a P.O
                                           has to be generated. To this end, the correct procurement type (purchase
                                           code) has to be assigned.


                                            How to enter an item for the P.O. in the order
                                           1 Enter the order header and go to the Items tab.
                                           2 Enter the product your customer requires.




                 A


                 B




                 A Procurement type for the selected item           B Order item created
                 Fig. D-22    Purchase item in the order


                                           3 Check the correct settings of the procurement type (A).
                                           4 Go to the menu Start > Save to save the data.
                                           5 Enter another item which includes only one BOM element.
                                           6 Go to the BOM tab.
3.30 / 04-2020




                 D-52                                                                        A+W Business Purchasing
                 Tutorial                                                                                   Purchase orders




                 A




                 B

                 C




                 A BOM element to be ordered                              C Procurement type
                 B Supplier for the element
                 Fig. D-23   Procurement type for BOM element


                                         7 Select the element (A) that is to be ordered.
                                         8 Choose the procurement type (C) and the supplier (B).
                                         9 Go to the menu Start > Save to save the changes.
                                               You can now enter more items or change the entered items.
                                               If you want to order all P.O. items from the same supplier, select the new
                                               supplier in the order header in the Terms tab.
                                                “How to change the supplier for all P.O. items” on page D-54
                                         10 Close item entry.
                                               If no default supplier was specified for the P.O. items, the supplier has to
                                               be specified in the P.O. transfer – Order pool dialog.
                                                “How to create a purchase order for a customer order” on page D-66
3.30 / 04-2020




                 A+W Business Purchasing                                                                              D-53
                 Purchase orders                                                                                    Tutorial




                                             Change supplier in order
                                             You can choose a different supplier for the purchase orders in the order head-
                                             er. This supplier will be used for all P.O. items of this order.

                                                 Change purchase code in the Number Manager
                                                 If you need to change the purchase code in several orders, you can collect
                                                 these orders in a new Number Manager. You can use the menu Functions
                                                 > Change code in this Number Manager to change the procurement type
                                                 and the supplier for all documents in one step.


                                              How to change the supplier for all P.O. items
                                             1 Open the order with all purchase items.
                                             2 Go to the Terms tab.




                                                                                                                         A




                 A Supplier for all P.O. items
                 Fig. D-24     Order header – Terms tab


                                             3 Choose the desired supplier (A).
3.30 / 04-2020




                                             4 Go to the menu Start > Save to save the data.
                                                 A question appears: Set purchase code for all items?



                 D-54                                                                          A+W Business Purchasing
                 Tutorial                                                                              Purchase orders




                                       5 Select
                                           •   [Yes]: The entire order is transferred to Purchasing to be ordered from
                                               the selected supplier.
                                           •   [No]: Only the P.O. items are transferred to Purchasing.
                                       6 Close the order.
                                           You can now transfer the P.O.s to Purchasing.
                                            “How to create a purchase order for a customer order” on page D-66


                                       Change ordered item
                                       You can change an ordered item in the order afterwards and issue a new pur-
                                       chase order. Do not forget to tell your supplier which purchase order is the new
                                       one, and which of the previous purchase orders it replaces.

                                           Change ordered item
                                           You can change an ordered item as long as no supplier's order confirmation
                                           or receipt of goods has been entered, or a lock status has been reached.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-55
                 Purchase orders                                                                                        Tutorial




                                               How to change an ordered item
                                              1 Open the document in which you want to change an ordered item, and go
                                                to item entry.
                                              2 Select the item you want to change.




                                                                                                                             A




                                                                                                                             B




                 A Product structure locked                                 B Item locked, only price can be changed
                 Fig. D-25    Procurement type of BOM element


                                                 The fields (A) for the ordered items are locked. The respective text is shown
                                                 in the Remark column (B).
                                              3 Go to the menu Functions > Group item > Change locked item.
                                                 The fields will be enabled.
                                              4 Enter your changes, e.g. the quantity.
                                              5 Go to the menu Start > Save to save the changes.
                                                 The changes are saved. You can enter more changes.
                                              6 Close item entry.
                                                 The P.O. transfer – Order pool dialog appears; you can transfer the pur-
3.30 / 04-2020




                                                 chase orders to Purchasing.
                                                  “How to create a purchase order for a customer order” on page D-66



                 D-56                                                                            A+W Business Purchasing
                 Tutorial                                                                                  Purchase orders




                 Fig. D-26   P.O. transfer – Order pool


                                           7 Transfer the changed P.O. as described in Transfer to Purchasing.
                                                “Transfer document to order pool” on page D-66

                                               Inform supplier
                                               Do not forget to tell your supplier of the change if you have already forward-
                                               ed the original P.O. to him.
3.30 / 04-2020




                 A+W Business Purchasing                                                                               D-57
                 Purchase orders                                                                                     Tutorial




                                   P.O. transfer
                                   Objectives

                                   •   Transferring an order with P.O. items to the order pool
                                   •   Checking P.O. items in the order pool
                                   •   Changing supplier and delivery dates
                                   •   Transferring P.O. items to Purchasing


                                   Benefits

                                   • Order items can be passed directly on to Purchasing. The P.O. items do not have
                                     to be checked in the P.O. pool.
                                   • Prices can be compared in the order pool in order to select the most favorable (or
                                     fastest) supplier.
                                   • Dates, prices, and suppliers of purchase orders can be checked before the transfer
                                     is made.


                                   Please note:

                                   P.O. transfer                 The P.O. transfer creates purchase orders from the order
                                                                 items.
                                                                 The transfer of a purchase order must be triggered
                                                                 manually. Only order items with a purchase code will be
                                                                 transferred from the order pool to Purchasing.

                                   Order pool                    The order pool is filled by hand. It lists all documents
                                                                 from the selected Number Manager.

                                   P.O.s                         Purchase orders from different orders can be combined
                                                                 in a collective P.O. if the supplier and the delivery date
                                                                 are identical for these items.

                                   Supplier                      If several items with purchase codes were entered in an
                                                                 order, a separate purchase code will be issued for every
                                                                 supplier.

                                   Price comparison              Before transferring the purchase order, you can compare
                                                                 the prices of suppliers who can provide the required
                                                                 product. For this purpose, the supplier file must be kept
                                                                 updated.

                                   Change of date                If the delivery date at the customer is changed in the
                                                                 order pool, this change will be applied to the reference
                                                                 order as well.

                                   Send P.O.                     Purchase orders created by means of the order pool
                                                                 have to be printed and sent to the supplier via the Form/
                                                                 label printing dialog.
3.30 / 04-2020




                 D-58                                                                        A+W Business Purchasing
                 Tutorial                                                                         Purchase orders




                                       Please note:

                                       Default settings   P.O. transfer > Options menu:
                                                          • Order-related transfer:
                                                            Purchase orders are transferred by order. Collective
                                                            P.O.s can be created if this option is disabled.
                                                          • P.O. number = order number:
                                                            This option is only available if the option Order-related
                                                            transfer has been enabled. This setting may not be
                                                            enabled if different suppliers are entered for an order.
                                                          Master data:
                                                          • Number areas
                                                          • Supplier file
                                                          Company data:
                                                          • Production tab (profit center invoicing)
                                                          • Stock/PP/EDI tab (include spacers in the P.O.)
3.30 / 04-2020




                 A+W Business Purchasing                                                                       D-59
                 Purchase orders                                                                                  Tutorial




                                           Order pool
                                           Purchase orders are automatically created from customer orders.


                        A    B         C                D           E               F              G    H




                 A Order number                      D Product description              G Document number after transfer
                 B Item number from the order        E Issue P.O.                       H Show BOM
                 C (Standard) supplier               F Generate inquiry
                 Fig. D-27   P.O. items in the order pool


                                           The order items are transferred to Purchasing by way of an order pool. Order
                                           items without P.O. items will not be processed further. The document status
                                           tells the program which items can be transferred to purchasing.
                                           Customer order check in the order pool only applies to products with the pro-
                                           curement type P.O. or P.O. (complete).
3.30 / 04-2020




                 D-60                                                                         A+W Business Purchasing
                 Tutorial                                                                                      Purchase orders




                              Order




                            Order pool




                             Check for
                             purchased



                                              no                                      no         Subordinate components
                            Main item                                 BOM
                                                                    elements


                                   yes                                    yes                                  yes


                                                              One P.O. per supplier



                 Fig. D-28       Process of the order check in the order pool


                                               Components with one of the two procurement types are searched for in the
                                               customer orders – first at the level of the main component and then at the BOM
                                               level. The products are distinguished by simple purchased elements and pur-
                                               chased elements for which all sub-products have to be ordered as well.
                                               If a customer order contains several items to be ordered from different suppli-
                                               ers, a separate P.O. will be created for each supplier.
                                               If a customer order states stock articles in a quantity which exceeds the cur-
                                               rent stock on hand, these stock articles have to be ordered by means of a
                                               (manual) stock P.O.

                                               Checks
                                               You can activate various checks via the Options menu, e.g.:
                                               •   Check delivery date:
                                                   The delivery date is checked automatically. The system will inform you if
                                                   you have changed a delivery date which falls on a day that is not a route
                                                   day.
                                               •   Consider supplier's route:
                                                   If the delivery date for the P.O. is not a route day, a message to that effect
                                                   will be issued. This requires that supplier's routes have been defined in the
                                                   master data.
                                               •   Determine lead days based on PGR combinations:
3.30 / 04-2020




                                                   If lead days have been defined for PGR combinations, these shall be used
                                                   to calculate the delivery date.
                                                    Master Data, “Lead days” on page B-560



                 A+W Business Purchasing                                                                                   D-61
                 Purchase orders                                                                             Tutorial




                                   •   Product names as per the supplier file:
                                       The names of the ordered products are adopted from the supplier file.
                                   •   No saving of costs:
                                       Costs are not written back to the purchase prices of the order.
                                   •   Consider size surcharges:
                                       Size surcharges shall be transferred with the P.O.

                                   P.O. transfer
                                   You can select the mode prior to transferring the P.O. items.




                                   Fig. D-29     Order mode




                                                           NM
                                                          Orders


                                                P.O. transfer
                                                • Direct inquiry                 Generate inquiry
                                                • Direct order
                                                • Fill pool                      Issue P.O.




                                                      Order pool                 Date OK
                                                                                 Supplier OK


                                       Price comparison         Date problems



                                                 Change supplier




                                   Fig. D-30     Change supplier in order pool


                                   With the option Direct order, P.O.s are generated without transferring them to
                                   the order pool. In the order pool, the dates and the suppliers can be changed.

                                   Supplier selection and price comparison
                                   If a date is at risk, you can choose other suppliers. These will be loaded from
3.30 / 04-2020




                                   the supplier file. If prices are also defined by supplier there, prices can be com-
                                   pared so that you can choose the most favorable supplier, irrespective of date
                                   problems.


                 D-62                                                                   A+W Business Purchasing
                 Tutorial                                                                                Purchase orders




                                                             Price comparison
                                                             Change supplier


                   NM                                  Order pool


                   Orders                 P.O. items             Standard                   Collective P.O.s
                   • 12301                                       supplier
                   • 12302
                                          • 12301 - 2            • 4004               Supplier 4004    • 12301 - 3
                   • 12303
                                                  -3             • 5001                                • 12304 - 3
                   • 12304
                   • …                    • 12304 - 1            • 7890
                                                  -3             • 4004               Supplier 5001    • 12304 - 1
                                                  -5             • 6731                                        -5

                                                                                      Supplier 2468    • 12301 - 2

                                                             Date problems
                                                             Change supplier


                 Fig. D-31   Change supplier in order pool


                                          Delivery dates
                                          To be able to calculate delivery dates, the delivery times of all suppliers must
                                          be kept in the supplier file. When customer orders are transferred, the delivery
                                          date is checked with the customer. The program also shows whether the de-
                                          livery time defined for this supplier will allow him to supply the goods on time.
                                          The supplier's delivery date in the order pool is determined by means of the
                                          shipping date minus the lead days defined for the corresponding product
                                          group.
                                          Weekdays and the route will be taken into account. If no lead days were en-
                                          tered, the shipping date is adopted as the delivery date.
                                          Delivery dates requested in the order that cannot be kept for the P.O. due to
                                          the delivery days defined in the supplier file are marked by a special color in
                                          the order pool.
                                          The supplier and/or delivery date can be changed in the order pool in this
                                          case. The changes will be saved in the order.

                                          Generated purchase orders
                                          Once the transfer is completed, a report shows the number of documents that
                                          could not be transferred (processed).
3.30 / 04-2020




                 A+W Business Purchasing                                                                             D-63
                 Purchase orders                                                                         Tutorial




                                   Fig. D-32    Faulty documents


                                   These have to be checked, one by one, and corrected if necessary. The fol-
                                   lowing errors are possible:
                                   •   No purchase code found.
                                   •   Order is still open.
                                   •   Status does not allow transfer.
                                   From the order items with a purchase code, purchase orders were created
                                   which can be opened and checked in the P.O. document management. These
                                   purchase orders can be sent to the supplier in the usual way.
                                   The status of all transferred items is changed. The status is also changed in
                                   the reference orders.

                                   P.O. numbers
                                   Automatically created purchase orders usually get numbers from the corre-
                                   sponding number area. At the transfer you can also decide whether the order
                                   number shall be used as the P.O. number as well.
3.30 / 04-2020




                 D-64                                                                A+W Business Purchasing
                 Tutorial                                                                             Purchase orders




                                       Collective orders per supplier
                                       Purchase orders from different orders placed with the same supplier are
                                       summed up in collective orders. The system will stick to the sequence in which
                                       the entries appear in the order pool. The order number must not be used as a
                                       P.O. number in this case however.
                                       When you have selected all items to be ordered from the same supplier in the
                                       order pool, you can combine them in a collective P.O.
                                       The following requirements must be met for this:
                                       •   Identical supplier
                                       •   Identical delivery date
                                       •   The code for collective orders has to be set in the supplier master data (Or-
                                           der tab).
                                       The Functions > Marking options menu can be used to define the supplier for
                                       which a collective P.O. shall be issued.




                                       Fig. D-33     Marking options for collective orders


                                       With the marking options, all corresponding items in the order pool will be se-
                                       lected automatically. To generate the collective order, disable the menu Op-
                                       tions > Group transfer > Order-related transfer.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-65
                 Purchase orders                                                                                  Tutorial




                                        Transfer document to order pool
                                        Orders are collected in a Number Manager for the transfer. The order pool ac-
                                        cesses the Number Manager selected by you. A new Number Manager can
                                        be created with the P.O. transfer in which successful purchase orders are
                                        transferred. The P.O.s can only be generated if the orders are closed prior to
                                        transfer.


                                         How to create a purchase order for a customer order
                                        1 Go to Documents > Order > P.O. transfer.


                                                                                                 A




                    B




                    C                                                                                                    D

                   A Number Manager with orders for B Transfer mode                     D Target number area
                     transfer                       C Target Number Manager
                   Fig. D-34   Transfer orders from the Number Manager


                                        2 Select the mode(B):
                                            •   Fill pool:
                                                Use this option to display the orders on the Order pool tab where they
                                                can be checked before the transfer and amended if necessary.
3.30 / 04-2020




                                            •   Direct order:
                                                Use this option to transfer the data immediately to the standard supplier.
                                                This option is useful if you do not want to check prices or delivery dates
                                                first.


                 D-66                                                                        A+W Business Purchasing
                 Tutorial                                                                                  Purchase orders




                                                  You can print the purchase orders afterwards and send them to the sup-
                                                  plier in the usual way, e.g. as an email attachment.
                                              •   Direct inquiry:
                                                  Use this option to transfer the data immediately as an inquiry to the stan-
                                                  dard supplier.
                                              In this example, the orders are first checked in the order pool.
                                          3 Select the Number Manager (A) that contains the orders with the P.O.
                                            items.
                                          4 Select the target Number Manager (C) to which the generated P.O.s shall
                                            be moved.
                                              You can enter a new name and thus create a new Number Manager. If you
                                              select another user, the Number Manager will be allocated to him/her.
                                          5 Choose a different target number area (D) if required.
                                          6 To move the orders to the order pool, go to the menu Start > Execute.




                    Fig. D-35   Order items in the order pool


                                              The order pool is filled. The P.O. items are shown per order.
3.30 / 04-2020




                 A+W Business Purchasing                                                                               D-67
                 Purchase orders                                                                                Tutorial




                                         7 Select the items to be transferred to Purchasing.
                                            Double-click on the corresponding line header.




                   Fig. D-36   Transfer marked order items


                                            Only items marked with an X have been selected.
                                         8 To start the action, go to the menu Start > Execute.
                                            The activated checks will be executed. Depending on the number of or-
                                            ders, this may take some time. Confirm the corresponding informative mes-
                                            sages by selecting [Yes] or [No] to proceed with the checks. When all
                                            checks have been completed, the corresponding purchase orders will be
                                            created and thus transferred to Purchasing.
                                            The transferred items are removed from the order pool.
                                            The order status is raised. The order history shows the P.O. number as a
                                            reference.
3.30 / 04-2020




                 D-68                                                                          A+W Business Purchasing
                 Tutorial                                                                               Purchase orders




                    Fig. D-37   P.O. numbers after transfer


                                              When the items have been transferred, the P.O. number for the order is dis-
                                              played.
                                              You can open and edit the purchase orders in Documents > P.O. Print the
                                              new purchase order and send it to the supplier.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-69
                 Purchase orders                                                                                   Tutorial




                                         Changing a P.O. in the order pool
                                         If difficulties regarding a date are shown for an item, you can select another
                                         supplier from the order pool. You can also open the dialog to change the sup-
                                         plier without date difficulties to select a different supplier other than the stan-
                                         dard supplier.


                                          How to change the delivery date and the supplier
                                         1 Go to Documents > Order > P.O. transfer.
                                         2 Move the orders to the order pool.
                                             This procedure is described in the previous unit.
                                              “Transfer document to order pool” on page D-66
                                         3 Select the item for which you want to change the delivery date.
                                             Double-click on the corresponding line header.




                   Fig. D-38   Item for the change of supplier is marked


                                             Only items marked with an X have been selected.
                                         4 Go to the menu Functions > Change supplier/delivery dates.
3.30 / 04-2020




                 D-70                                                                           A+W Business Purchasing
                 Tutorial                                                                            Purchase orders




                                           You can now change the following information:
                                           •   the supplier
                                           •   the delivery date of the supplier
                                           •   the date of delivery at the customer
                                       5 Click [OK] to accept the change.
                                           The Change supplier and delivery dates dialog closes. The purchase order
                                           pool shows the order item with the new date and/or supplier.
                                       6 To transfer the item to Purchasing, go to the menu Start > Execute.
                                           The activated checks will be executed. Depending on the number of or-
                                           ders, this may take some time. Confirm the corresponding informative mes-
                                           sages by selecting [Yes] or [No] to proceed with the checks. When all
                                           checks have been completed, the corresponding purchase orders will be
                                           created and thus transferred to Purchasing.
                                           The changed dates are saved in the order.
                                           When the items have been transferred, the P.O. number for the order is dis-
                                           played.
                                           You can open and edit the generated purchase orders in Documents > P.O.
                                           Print the new purchase order and send it to the supplier.
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-71
                 Purchase orders                                                                                Tutorial




                                         Compare prices in the order pool
                                         If several suppliers have been entered for a product, you can compare prices
                                         in the order pool and select another supplier if required.


                                          How to compare prices in the order pool
                                         1 Go to Documents > Order > P.O. transfer.
                                         2 Move the orders to the order pool.
                                            This procedure is described in the previous unit.
                                             “Transfer document to order pool” on page D-66
                                         3 Select the item for which you want to compare purchase prices.
                                            Double-click on the corresponding line header.




                   Fig. D-39   Item for price comparison is marked


                                            Only items marked with an X have been selected.
                                         4 Go go the menu Functions > Supplier prices.
3.30 / 04-2020




                 D-72                                                                          A+W Business Purchasing
                 Tutorial                                                                                      Purchase orders




                                                         A

                                    B
                                    C
                                    D

                    A !!! For all text colors:                         C Text in green:
                      Delivery date is at risk                           most favorable supplier in terms of price
                    B Text color red:                                  D Text in blue:
                      Standard supplier                                  Standard supplier is most favorable supplier in terms of
                                                                         price
                    Fig. D-40     Price comparison for item


                                             5 Tick the checkbox left from the supplier to whom the purchase order for this
                                               item is to be sent.
                                             6 Click [OK] to accept the change.
                                                 The Price comparison dialog closes. The order pool shows the order item
                                                 with the new supplier.
                                             7 Select the orders or order items you want to transfer to Purchasing.
                                                 Double-click on the corresponding line header.
3.30 / 04-2020




                 A+W Business Purchasing                                                                                   D-73
                 Purchase orders                                                                             Tutorial




                   Fig. D-41   Item with changed supplier


                                            Only items marked with an X have been selected.
                                         8 To start the transfer, go to the menu Start > Execute.
                                            The activated checks will be executed. Depending on the number of or-
                                            ders, this may take some time. Confirm the corresponding informative mes-
                                            sages by selecting [Yes] or [No] to proceed with the checks. When all
                                            checks have been completed, the corresponding purchase orders will be
                                            created and thus transferred to Purchasing.
                                            Transferred items are removed from the order pool.
3.30 / 04-2020




                 D-74                                                                      A+W Business Purchasing
                 Tutorial                                                                                  Purchase orders




                    A




                    B




                    A First P.O. number                               B Second P.O. number
                    Fig. D-42   P.O. numbers after transfer


                                              When the items have been transferred, the old and the new P.O. number
                                              for this order are shown.
                                              You can open and edit the purchase orders in Documents > P.O. Print the
                                              new purchase order and send it to the supplier.
                                              Do not forget to inform the former supplier of the change.
3.30 / 04-2020




                 A+W Business Purchasing                                                                            D-75
                 Purchase orders                                                                                   Tutorial




                                           Order and P.O. info
                                           The reference documents for every order and every P.O. can be displayed in
                                           a list. This function is available for purchase orders (header data) in the menu
                                           Function > Order/P.O. info.




                 Fig. D-43   Order and P.O. info – List of reference documents


                                           This dialog is described in the Sales section.
                                            Sales, “Order/P.O. Info” on page C-486
3.30 / 04-2020




                 D-76                                                                         A+W Business Purchasing
                 Tutorial                                                                                  Purchase orders




                                       Manual purchase order
                                       Objectives

                                       • Entering a purchase order manually.
                                       • Learning about the document type Stock P.O.


                                       Benefits

                                       • Stock P.O.s serve to maintain the stock on hand. Apart from stock articles, they can
                                         also include articles which are not kept on stock.


                                       Please note:

                                       Manual purchase order       Purchase orders which do not have to be created from
                                                                   an order item by means of P.O. transfer, have to be
                                                                   entered manually.

                                       Independent P.O.            Independent P.O.s serve to enter all products that can be
                                                                   purchased.
                                                                   Independent P.O.s do not refer to an order.

                                       Stock P.O.s                 Stock P.O.s are a separate document type. They serve to
                                                                   replenish the stock.

                                       Default settings            Master data:
                                                                   • Supplier file
                                                                   Suppliers
                                                                   • Order tab
                                                                   • Finance tab
                                                                   • Balance tab
                                                                   Company data:
                                                                   • Parameters tab
                                                                   • Stock/PP/EDI tab
3.30 / 04-2020




                 A+W Business Purchasing                                                                               D-77
                 Purchase orders                                                                          Tutorial




                                   Independent P.O.s
                                   All purchase orders for products which do not have the Purchase order or Pur-
                                   chase order (complete) purchase code and have not been created from an or-
                                   der must be entered manually.
                                   All products needed for production or sales can be entered in purchase orders.
                                   A distinction is made between articles that can be booked as stock articles and
                                   those that are kept on stock but do not appear on any stock list. Purchase or-
                                   ders for stock articles and boxes have to have the document type Stock P.O.
                                   to make sure that receipt of goods can be booked correctly.
                                   When you enter the corresponding terms for your suppliers, the purchase or-
                                   ders will show the current purchase prices right away. They serve for checking
                                   the prices in order confirmations (OC) and invoices received from your suppli-
                                   ers.

                                   Stock P.O.s
                                   Stock P.O.s are entered as a separate document type; the items can include
                                   all purchase articles, stock sizes, boxes, and special sizes that are kept as
                                   stock articles. Receipts of goods for inventory items from inventory P.O.s are
                                   booked directly into the stock on hand.
                                   If you enter stock P.O.s with items which are not recorded as stock articles,
                                   they will not be displayed at receipt of goods. You can however enable the cor-
                                   responding option in the company data.
                                   Stock P.O.s are described in detail in the Stock management section.

                                   Purchase prices
                                   The purchase price is loaded from the purchase price lists. The corresponding
                                   prices are displayed when you enter P.O. items, and are updated when chang-
                                   es are made.
3.30 / 04-2020




                 D-78                                                                A+W Business Purchasing
                 Tutorial                                                                                   Purchase orders




                                              Entering an independent P.O.
                                              All products defined in master data can be entered in an independent P.O.

                                                 Working with Number Managers
                                                 Configure the Number Managers for purchase orders in such a way that
                                                 documents can be compiled in accordance with unambiguous criteria, e.g.
                                                 by supplier, by date, stock P.O.s, or completely delivered orders.


                                               How to enter an independent P.O.
                                              1 Go to the menu Documents > P.O. > P.O.
                                                 The Document management dialog opens.
                                              2 Go to the menu Functions > Select NM and check if the right Number Man-
                                                ager has been set, and correct the setting if necessary.
                                              3 Enter the document header by selecting the supplier.




                                                                                                                           A




                                                                                                                           B




                 A Supplier's delivery date                             B Document type
                 Fig. D-44    Entering an independent P.O.
3.30 / 04-2020




                                              4 Check the delivery date (A).
                                                 This is the date on which you expect the delivery to arrive at your premises.



                 A+W Business Purchasing                                                                                D-79
                 Purchase orders                                                                           Tutorial




                                   5 Go to the field Type (B) and select the entry <n.s.>.
                                      If you set the type to <n.s.>, the receipt of goods will not be added to the
                                      stock.
                                      The stock P.O. is described in a separate unit.
                                   6 Enter the items as described in chapter P.O. items included in the order.
                                   7 Print and send the purchase order.
                                      Now the purchase order is in the Number Manager you have defined. The
                                      supplier's order confirmation and/or receipt of goods can be added later.
                                       “Enter receipt of goods” on page D-125
3.30 / 04-2020




                 D-80                                                                   A+W Business Purchasing
                 Tutorial                                                                            Purchase orders




                                       Enter stock P.O.
                                       You can also use a stock P.O. to order items which cannot be booked as stock
                                       items. A message will make you aware of these order items upon saving.
                                       These items are not automatically added to stock upon receipt of goods.
                                       The following guideline shows how to enter a stock P.O. for boxes. These box
                                       P.O.s can be processed further in the Dealing with boxes subject.


                                        How to enter a stock P.O. with boxes
                                       1 Enter the document as described in the section Independent P.O.
                                            “How to enter an independent P.O.” on page D-79
                                       2 Go to field Type and select the entry Stock P.O.




                                           If you set the type to <n.s.>, goods received cannot be automatically added
                                           to stock.
                                       3 Go to the Items tab.
                                       4 Enter the product number, e.g. 1005.
                                           You can specify the number after selecting the stock article. You do not
                                           need to enter sizes as they are taken from the stock article.
                                       5 Go to the menu Start > Stock search to open the Stock info dialog.
                                           You can also open this dialog by pressing <F3>.
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-81
                 Purchase orders                                                                                     Tutorial




                    A




                    B




                   A Product number of glass type                        B Box (without ID)
                   Fig. D-45   Stock info – Stock search


                                             The Stock info dialog opens providing a list of all boxes and stock sizes. For
                                             boxes, the entry in column Cont. is greater than 1.
                                         6 Select the required box without box ID and accept it by a double click.
                                             The dialog is closed and you will find yourself back at item entry. In the input
                                             line, you will find that all fields from Quantity onwards are locked for boxes.
                                             The price fields are updated.
3.30 / 04-2020




                 D-82                                                                          A+W Business Purchasing
                 Tutorial                                                                   Purchase orders




                                      A             B
                    A Amount                                               B Quantity
                    Fig. D-46   Box at item entry


                                          7 Enter the amount required.
                                              The display of details is updated.
                                          8 Repeat steps 4 to 7 to enter all P.O. items.
                                          9 Go to the menu Start > Save to save the data.
                                              The data is saved.
                                          10 Print and send the purchase order.
3.30 / 04-2020




                 A+W Business Purchasing                                                             D-83
                 Purchase orders                                                                                 Tutorial




                                   Supplier's order confirmation
                                   Objectives

                                   •   Enter supplier's order confirmation (OC)
                                   •   Enter OC per item
                                   •   Check prices in the OC
                                   •   Send reminder for overdue order confirmations


                                   Benefits

                                   • The supplier's order confirmation is allocated to the purchase order. The delivery
                                     date is confirmed or amended without having to open the purchase order itself.
                                     Changed dates will be applied to the reference documents.
                                   • The status of reference orders is automatically changed together with the status of
                                     the purchase order.
                                   • OCs for confirmation of partial quantities can be entered without having to enter
                                     the data anew.
                                   • The Number Manager can be filtered for overdue purchase orders in order to send
                                     reminders to the suppliers in question.


                                   Please note:

                                   Partial confirmation        If your supplier confirms delivery of the ordered quantity
                                                               in several partial quantities, you can enter order
                                                               confirmations (OC) for the individual items or partial
                                                               quantities.

                                   Status                      The status of the reference documents is raised when
                                                               you enter the supplier's order confirmation in one of the
                                                               documents.

                                   Document lock               Reference documents are locked for other users while
                                                               the price and invoice control is run.

                                   Send reminder               The reminder is sent to the supplier via the same
                                                               channel as the P.O.

                                   Default settings            Supplier master data
                                                               • Fax and email dispatch
3.30 / 04-2020




                 D-84                                                                     A+W Business Purchasing
                 Tutorial                                                                             Purchase orders




                                       Supplier's OC
                                       Your supplier acknowledges receipt of your purchase order by an order confir-
                                       mation (OC). You can enter the number of this order confirmation and allocate
                                       it to the corresponding purchase order. At the same time, you can check the
                                       dates and prices and amend them in your documents if necessary.
                                       When you enter an order confirmation, you can move the purchase order and/
                                       or corresponding customer order to a target Number Manager for further pro-
                                       cessing.

                                       Partial deliveries
                                       It may happen that for larger orders, your supplier does not confirm all items
                                       or the entire quantity for the desired date but announces a certain number of
                                       partial deliveries. You can confirm a part of the purchase order in this case
                                       without having to create a new document.

                                       Status
                                       The status of all reference documents is changed when the order confirmation
                                       number has been acknowledged. The reference documents are displayed
                                       when the order or P.O. number is entered. For independent purchase orders,
                                       the corresponding fields are locked.

                                       Order confirmation and delivery date
                                       The supplier's order confirmations can be entered in different ways:
                                       •   Order confirmation with or without receipt of goods. You can check the de-
                                           livery dates and notify your customer in case of a delay.
                                       •   Confirmation for individual P.O. items.
                                       •   Order confirmation and price control. You can check and correct the pur-
                                           chase prices and the delivery date and enter a partial delivery for an or-
                                           dered quantity if required. You can find a description of this variant under:
                                            “Price and invoice control” on page D-141
                                       Based on a customer order, several purchase orders can be created for differ-
                                       ent suppliers. The different order confirmation numbers are saved for the cor-
                                       responding order items.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-85
                 Purchase orders                                                                          Tutorial




                                   Overdue deliveries
                                   You can send reminders for overdue order confirmations or deliveries.The
                                   search for open orders can be restricted to a date, to certain suppliers and/or
                                   Number Managers.
                                   The reminder is sent to the supplier by the same communication channel as
                                   for the purchase order. The rule is:
                                   •   Fax:
                                       A+W Business transfers the purchase orders directly to a fax machine, to
                                       be passed on to the supplier.
                                   •   Regular mail:
                                       A+W Business sends the purchase orders directly to a printer.
                                   The reminder is always issued for all purchase orders selected by means of
                                   the search criteria. Purchase orders for the same supplier are compiled in one
                                   reminder.
3.30 / 04-2020




                 D-86                                                                 A+W Business Purchasing
                 Tutorial                                                                            Purchase orders




                                       Order confirmation entry
                                       For a P.O., you enter the order confirmation (OC) of your supplier and thus
                                       raise the status of the P.O.
                                       The following instructions exist for this training module:
                                       •   “How to enter an order confirmation for an entire P.O.” on page D-87
                                       •   “How to enter an order confirmation for a P.O. item” on page D-89


                                        How to enter an order confirmation for an entire P.O.
                                       1 Go to Documents > P.O. >OC supplier.

                                            A               B




                                           A Search mode                         B Document number
                                           Fig. D-47   Enter the OC of the supplier


                                       2 Choose the option (A) which which you would like to use to search for the
                                         open purchase orders, e.g. P.O. number.
                                       3 Enter the purchase order number (B) and press <Tab> to jump to the next
                                         field.
                                           The data will be loaded and displayed.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-87
                 Purchase orders                                                                             Tutorial




                                   A

                                   B




                                   C

                                   D




                                   A Target Number Manager                    C Delivery date as per the order
                                   B Book complete receipt of goods             confirmation
                                                                              D Order confirmation number
                                       Fig. D-48    OC supplier – Documents


                                   4 Select the target Number Manager (A) for orders or purchase orders if the
                                     corresponding documents are to be transferred to other Number Manag-
                                     ers.
                                   5 Tick the checkbox Book receipt of goods (B) only if you want to book the
                                     complete receipt of goods for this purchase order at the same time.
                                       With this setting, you cannot book a partial receipt of goods. The receipt of
                                       goods is explained in a separate unit.
                                   6 Check the dates (C) in sections P.O. data and Order data and correct them
                                     if necessary.
                                   7 Enter the number of the order confirmation (D) received from your supplier.
                                   8 Go to the menu Start > Execute to save the data.
                                       The data is saved. The order confirmation number appears in the overview.
                                       If you book a receipt of goods at the same time, the status of the purchase
                                       order is changed accordingly.
3.30 / 04-2020




                 D-88                                                                  A+W Business Purchasing
                 Tutorial                                                                              Purchase orders




                                        How to enter an order confirmation for a P.O. item
                                       1 Fill in the fields as described in steps 2 to 6 of the previous process.
                                       2 Go to the Items tab.




                                       A




                                       B




                                       A Item numbers                            B Date of partial delivery
                                       Fig. D-49    OC supplier – Items


                                       3 Enter the item number(s) (A) for which you have received an order confir-
                                         mation.
                                           If you do not have an unbroken sequence of numbers, you have to individ-
                                           ually repeat the steps for each item, e.g. for item 1, 3 and 7.
                                       4 Enter the date of delivery of the items in the field Partial delivery date.
                                       5 Go to the menu Start > Execute to save the data.
3.30 / 04-2020




                 A+W Business Purchasing                                                                            D-89
                 Purchase orders                                                                     Tutorial




                                                                                A        B
                                   A OC number                              B Confirmed date
                                   Fig. D-50   OC supplier – Partial delivery


                                   The data is saved. The OC number and the partial delivery date are shown
                                   in the overview.
3.30 / 04-2020




                 D-90                                                               A+W Business Purchasing
                 Tutorial                                                                                     Purchase orders




                                            Enter order confirmation and check prices
                                            Prices can be checked based on the supplier's order confirmation or based on
                                            the supplier's invoice. The Price control and Invoice control dialogs have the
                                            same structure.
                                            Your supplier's order confirmation may cover several purchase orders. These
                                            can be collected in the Price control dialog to be checked together.
                                            The following instructions exist for this training module:
                                            •   “How to enter an order confirmation from your supplier, and check the pric-
                                                es” on page D-91
                                            •   “How to enter a collective order confirmation from your supplier” on
                                                page D-93
                                            Price and invoice control is described in detail in a separate unit.
                                             “Checking the invoice” on page D-144


                                             How to enter an order confirmation from your supplier, and check the
                                              prices
                                            1 Go to the menu Documents > P.O.s > Order confirmation > Price control.




                    A                                                                                                      D



                    B
                    C




                    A Data stated in the order confirmation              C Display mode for prices
                    B Confirmed total                                    D Search P.O.(s)
                    Fig. D-51    Enter an order confirmation number from your supplier and check the prices
3.30 / 04-2020




                                            2 Enter your supplier's order confirmation number (A) and the confirmed de-
                                              livery date.
                                            3 Enter the P.O. number (D) and use <Tab> to go to the next field.


                 A+W Business Purchasing                                                                               D-91
                 Purchase orders                                                                                 Tutorial




                                             The purchase order is displayed in the P.O.s overview.
                                             If an order confirmation includes several purchase orders, you can enter
                                             the P.O. numbers one by one. The following guideline describes this.
                                          4 Enter the amount confirmed by your supplier in the field OC total (B).
                                             The amount must be identical with the amount loaded from the purchase
                                             order. If the supplier has stated a different amount which you are going to
                                             accept, you have to change the prices in the purchase order. These chang-
                                             es can be entered on the Items tab.
                                             Please make sure that the mode (C) for displaying the amounts has been
                                             set correctly.

                                             Currency
                                             If you are using just one currency (EUR), the entry in field Exchange rate
                                             must be 1.


                                             A                B




                   A OC total                                           B Amount from the P.O.
                   Fig. D-52    Enter an order confirmation number from your supplier and check the prices


                                          5 To confirm the entry, go to the menu Start > Execute.
                                             The amount will be checked and the Items tab appears.
3.30 / 04-2020




                 D-92                                                                           A+W Business Purchasing
                 Tutorial                                                                                  Purchase orders




                                                               A




                                                                                                                     B


                    A Item price                                         B Difference across all items
                    Fig. D-53      Check P.O. item prices


                                                If you need to change an item price, change the amount in the correspond-
                                                ing item (A). The change will be saved in the purchase order.
                                             6 If no (more) differences are shown, go to the menu Start > Execute. (B).
                                                The data will be saved, and the P.O. status is changed. You will find your-
                                                self back on P.O.s tab where you can enter the next order confirmation. The
                                                price control for this purchase order cannot be performed again.


                                              How to enter a collective order confirmation from your supplier

                                                Collect purchase orders
                                                You can collect the purchase orders stated on the supplier's order confir-
                                                mation in a Number Manager which can be selected in the P.O. data sec-
                                                tion.
                                                Alternatively, you can compile the purchase orders in the Price control dia-
                                                log. This process is described in the following instruction.

                                             1 Use the Price control dialog to enter your supplier's order confirmation
                                               number and the delivery date as described above.
                                                If you have compiled the purchase orders in a Number Manager, select the
3.30 / 04-2020




                                                Number Manager and proceed with step 5.
                                             2 Enter the number of the first purchase order and wait until it is loaded.



                 A+W Business Purchasing                                                                              D-93
                 Purchase orders                                                                                Tutorial




                                         3 Enter the number of the next purchase order stated on the order confirma-
                                           tion.
                                            The purchase order is displayed in the P.O.s overview. You can only com-
                                            bine purchase orders with the same tax rate however.
                                         4 Repeat this step until all purchase orders are listed in the overview.
                                            To remove a purchase order from the overview, select it and press <Del>.




                   Fig. D-54   Enter an order confirmation number from your supplier and check the prices


                                         5 Now enter the amount confirmed by your supplier.
                                            This amount must match the total of the listed purchase orders.
                                         6 To confirm the entry, go to the menu Start > Execute.
                                            The amount will be checked and the Items tab appears. If you need to
                                            change an item price, change the amount in the corresponding item. The
                                            change will be saved in the purchase order.
                                         7 If no (more) differences are shown, go to the menu Start > Execute.
                                            The data will be saved, and the status of the purchase orders is changed.
3.30 / 04-2020




                 D-94                                                                          A+W Business Purchasing
                 Tutorial                                                                               Purchase orders




                                       Remind supplier
                                       Order confirmations and deliveries are recorded to ensure the proper process-
                                       ing of your purchase orders. You can remind suppliers that are late.

                                           Collect purchase orders
                                           You can collect the purchase orders stated on the supplier's order confir-
                                           mation in a Number Manager.


                                        How to remind a supplier
                                       1 Go to the menu Documents > P.O.s > Order confirmation > Reminder.

                                                         A         B      C         D




                                                                                                                        E

                                                                                                                        F




                                       A Supplier                                   D (Do not) remind supplier again
                                       B Number Manager with overdue P.O.s          E Entry date of purchase order
                                       C Restricting the selection to a status area F Modes of dispatch of P.O. order
                                       Fig. D-55    Remind supplier


                                       2 Filter the view:
                                           •   by supplier (A)
                                           •   by a Number Manager (B)
                                       3 Use the fields Minimum status and Status below (C) to define a status area
                                         for the purchase orders about whose delivery you want to remind the sup-
                                         plier.
3.30 / 04-2020




                                           One criterion for the minimum status could be that the purchase order has
                                           been printed or that the order confirmation has been entered.




                 A+W Business Purchasing                                                                            D-95
                 Purchase orders                                                                             Tutorial




                                      The criterion for the other status should lie before the status Receipt of
                                      goods.
                                   4 Restrict the selection of purchase orders to a date (E).
                                      The current date is displayed by default.
                                   5 If you do not want to send another reminder to a supplier who has already
                                     received a reminder, tick off the checkbox (C) for this criterion.
                                      Suppliers who have already received a reminder will not appear on this list.
                                      If the checkbox is ticked, these suppliers are shown in red. They will be re-
                                      minded again of the overdue deliveries.
                                   6 Select the method of dispatch (F) used for the purchase orders.
                                      If you are using different modes of dispatching purchase orders to your
                                      suppliers, observe the communication path for the selected supplier.
                                      Option All is useful if you are using different methods of sending purchase
                                      orders to your suppliers, and the selection is not restricted to a certain sup-
                                      plier.
                                   7 To start the search, go to the menu Start > Search.




                                      Fig. D-56    Selection of suppliers to be reminded


                                      The open purchase orders appear on the overview.
                                   8 Choose the required output media in the Print menu.
                                      The reminder is issued.
3.30 / 04-2020




                 D-96                                                                      A+W Business Purchasing
                 Tutorial                                                                             Purchase orders




                                           Fig. D-57   Reminders created


                                           All entries on the overview are shown in red afterwards.
3.30 / 04-2020




                 A+W Business Purchasing                                                                       D-97
                 Purchase orders                                                                                 Tutorial




                                   Delivery date check
                                   Objectives

                                   • Checking the delivery dates for reference documents.
                                   • Change dates.
                                   • Inform the customer of the change.


                                   Benefits

                                   • Dates have to be changed in only one of the reference documents.
                                   • Delivery dates can be changed in various dialogs. Purchase orders or orders which
                                     have been compiled in a separate Number Manager can be changed without the
                                     need to open the individual documents.


                                   Please note:

                                   Changing dates in          All amendments of purchase orders are saved in the
                                   reference documents        reference orders. This also works vice versa.

                                   Customer information       This dialog can be used to change the delivery date and
                                   dialog                     notify the customer.

                                   Document data dialog       This dialog is used to adapt all dates in the orders and in
                                                              reference purchase orders. You can also change the
                                                              routes for orders, and change several documents at the
                                                              same time.

                                   Default settings           Customer master data (fax or email dispatch)
3.30 / 04-2020




                 D-98                                                                     A+W Business Purchasing
                 Tutorial                                                                             Purchase orders




                                       Delivery date check and correction
                                       Your supplier will confirm or correct the dates stated in your purchase orders.
                                       Order confirmations and delivery dates conveyed by the supplier are allocated
                                       to the purchase orders by creating supplier OCs. Changed dates will be auto-
                                       matically adopted for the reference documents.


                                       You can also use the options in the Customer information dialog or the Com-
                                       munication menu to inform the customer, or just call them.
                                       You can change the delivery date itself in various dialogs:
                                       •   Document management (order, purchase order)
                                       •   Document data
                                       •   Customer information (delivery date check)
                                       •   OC supplier
                                       •   Inspection of goods received
                                       Dates are usually corrected in the purchase orders upon which they are saved
                                       in the reference orders.

                                       Customer information
                                       You can use the Customer information dialog to inform the customer of a delay
                                       in delivery (Delivery date check). An email address must have been entered
                                       in the customer's master data for this purpose. In the order itself, the checkbox
                                       Email must be ticked in the Address section.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-99
                 Purchase orders                                                                                Tutorial




                                         Change delivery dates, notify customer
                                         You have to check and correct the delivery dates of purchase orders and ref-
                                         erence orders and, if necessary, notify the customer if the delivery dates can-
                                         not be met. This can be done via the Customer information dialog.
                                         You can open it as follows:
                                         •   Order or P.O. > Functions > Group document > Check delivery dates
                                         •   Documents > Customer information
                                         Use the Document data dialog to check and correct the production dates as
                                         well.


                                          How to change the delivery date
                                         1 Open the order, the dates of which you want to check or have changed.
                                         2 Select Documents > Customer information.




                                                                                                                      B
                    A




                   A Search mode                                       B Scheduled delivery date
                   Fig. D-58   Change the date of delivery to the customer
3.30 / 04-2020




                 D-100                                                                       A+W Business Purchasing
                 Tutorial                                                                                 Purchase orders




                                           3 Select the option (A) Orders or P.O.s and the Number Manager if required.
                                              If the Number Manager includes very many documents, you can restrict the
                                              view to the originally scheduled delivery date (B).
                                           4 To import the data, go to the menu Start > Search.




                    A




                                                                                    B                 C
                    A Customer has not been informed of the new date   B Scheduled delivery date stated in the order
                      yet                                              C New delivery date
                    Fig. D-59    Check delivery dates


                                           5 Select the order for which you want to change the date of delivery to the
                                             customer and go to the Postponement tab.
3.30 / 04-2020




                 A+W Business Purchasing                                                                               D-101
                 Purchase orders                                                                                 Tutorial




                    A




                    B




                   A New delivery date at the customer's site.            B Order for which the change applies
                   Fig. D-60    Change the date of delivery to the customer


                                           6 Select the order (B) for which the customer date is to be postponed.
                                              You can select several orders if they all have the same delivery date and
                                              route.
                                           7 Enter the new date (A) and change the route if necessary.
                                           8 Go to the menu Start > Save to save the changes.
                                              You can print the new date for the customer and dispatch it via the usual
                                              communication channel.
                                           9 Go to the Print menu and select the printer.
                                              The notification is created and can be dispatched. If you have changed sev-
                                              eral dates, a notification will be issued for each customer.
3.30 / 04-2020




                 D-102                                                                         A+W Business Purchasing
                 Tutorial                                                                               Purchase orders




                                          Check and change all dates
                                          The Document data dialog can be used to view all purchase orders and orders
                                          in order to check the delivery dates as well as the production dates and
                                          change them if necessary. You can compile orders, e.g. in order to change the
                                          dates in several orders at the same time.
                                          The following instructions exist for this training module:
                                          •   “How to check and change document data” on page D-103
                                          •   “How to collect documents for common changes” on page D-106


                                           How to check and change document data
                                          1 Go to Documents > Document data.


                                  A                                  B




                    A Document type                                      B Number of the searched document
                    Fig. D-61   Check dates for orders containing purchase items
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-103
                 Purchase orders                                                                                Tutorial




                                         2 Select the document type, e.g. order or purchase order.
                                            You can also view all documents from one Number Manager. In this exam-
                                            ple, one single order is to be checked.
                                            You can change the dates for several orders and/or purchase orders that
                                            are not in a collective Number Manager.
                                             “How to collect documents for common changes” on page D-106
                                         3 Enter the order number and adopt the data by pressing <Enter>.




                    A




                    B




                   A Customer dates                                   B New date of supplier
                   Fig. D-62   Check dates for orders containing purchase items


                                            The fields in the Order area show the data from the order header. The P.O.
                                            data appears in the fields in the P.O. area.
                                         4 Adapt the supplier date (B) and customer dates (A).
                                            If you select the dates from the calendar, you can take the customer's route
                                            days into account.
                                         5 Go to the menu Start > Save to save the data.
                                            The new dates are saved and adopted for the corresponding documents.
3.30 / 04-2020




                 D-104                                                                         A+W Business Purchasing
                 Tutorial                                                                      Purchase orders




                    Fig. D-63   Changed dates


                                            You can inform the customer of the new date now.
3.30 / 04-2020




                 A+W Business Purchasing                                                               D-105
                 Purchase orders                                                                               Tutorial




                                          How to collect documents for common changes
                                         1 Go to Documents > Document data.


                                   A                                B         C




                   A Document type                                      C Do not mark the Number Manager
                   B Number of the searched document
                   Fig. D-64   Check dates for orders containing purchase items


                                         2 Select the document type, e.g. order (A).
                                         3 Make sure that the checkbox (C) Number Manager is unchecked.
                                         4 Enter the order number (B) and adopt the data by pressing <Enter>.
                                            The order data is shown on the overview. The section P.O. lists the refer-
                                            ence purchase orders.
                                         5 Repeat this step until you have compiled all orders to be changed together.
                                            Make sure that all orders with the same route can be delivered and that
                                            they have the same delivery date.
3.30 / 04-2020




                 D-106                                                                      A+W Business Purchasing
                 Tutorial                                                                               Purchase orders




                    A




                    B




                    A Order dates                                      B P.O. dates
                    Fig. D-65   Orders for collective date change


                                              The list shows all orders.
                                          6 Select all listed orders by keeping the <Ctrl> key pressed.
                                          7 Change the dates (A, B).
                                          8 Check the route and change it if necessary.
                                          9 Go to the menu Start > Save to save the data.
                                              The new dates will be applied to all listed orders and the reference pur-
                                              chase orders. You can notify the customer now.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-107
                 Purchase orders                                                                                 Tutorial




                                   Inquiry
                                   Objectives

                                   • Obtaining inquiries from suppliers
                                   • Generating a P.O. from an inquiry
                                   • Obtaining inquiries for an order item


                                   Benefits

                                   • To agree on dates and capacities, inquiries can be made via the order pool.
                                   • An inquiry can be turned into a purchase order without having to enter the data
                                     again.


                                   Please note:

                                   Inquiries                   Like purchase orders, inquiries can be entered manually
                                                               or can be created from a customer order by means of the
                                                               order pool.

                                   P.O.                        Purchase orders can be created from any type of inquiry.

                                   References                  References to order items are kept in the inquiry and in
                                                               the purchase order if these are created from the order
                                                               pool.
                                                               If a purchase order is created by copying an inquiry, the
                                                               reference exists only between these two documents.

                                   Default settings            Master data:
                                                               • Supplier > Order tab



                                   Inquiry for P.O. items or purchase orders
                                   Inquiries are created and sent to the supplier in the same way as purchase or-
                                   ders. When the quotation comes in and is accepted, you can turn the inquiry
                                   into a purchase order without having to enter the data once more. You can use
                                   the function Copy document for this purpose.
                                   You can also create inquiries for P.O. items from a customer order.
3.30 / 04-2020




                 D-108                                                                    A+W Business Purchasing
                 Tutorial                                                                                      Purchase orders




                   Order             P.O. transfer         Inquiry           Copy to       P.O.          no reference
                   No. 1167         Direct inquiry                                                       to order 1167




                                      Order pool           Inquiry        Reference to
                   Order                                                  order 1167
                   No. 1167                                                                P.O.           Reference to
                                                                                                          order 1167




                                     Independent inquiry                     Copy to           Independent P.O.




                 Fig. D-66    Inquiry – P.O.


                                               If the option Direct inquiry was selected during the P.O. transfer, inquiries from
                                               a customer order are also generated. If this is done by means of the order pool,
                                               you can even create inquiries for individual order items and select a certain
                                               supplier.
                                               Of course, these inquiries can also be turned into purchase orders. The refer-
                                               ence to the order will be kept only if the resulting purchase orders are created
                                               by means of the order pool as well.
                                               Independent inquiries are created in the same way as orders and purchase or-
                                               ders. The Documents module offers the Inquiries menu for this purpose.
3.30 / 04-2020




                 A+W Business Purchasing                                                                                  D-109
                 Purchase orders                                                                                  Tutorial




                                          Create an inquiry for a P.O. item
                                          You can create an inquiry for a P.O. item, e.g. to find out whether the supplier
                                          can offer the necessary capacity. Every inquiry can be turned into a purchase
                                          order by means of the order pool.
                                          The following instructions exist for this training module:
                                          •   “How to create an inquiry based on a customer order” on page D-110
                                          •   “How to create a P.O. from a reference inquiry” on page D-111


                                           How to create an inquiry based on a customer order
                                          1 Go to Documents > Order > P.O. transfer.


                                                           A                                      B




                    C

                   A Transfer mode                                    C Target Number Manager
                   B Number Manager with orders for transfer
                   Fig. D-67    Transfer orders from the Number Manager


                                          2 Select the mode Direct inquiry (A) and the Number Manager (B) you used
                                            to collect the orders with P.O. items.
3.30 / 04-2020




                 D-110                                                                        A+W Business Purchasing
                 Tutorial                                                                             Purchase orders




                                           3 Select the target Number Manager (C) to which the inquiries shall be made.
                                              You can enter a new name and thus create a new Number Manager. If you
                                              select another user, the Number Manager will be allocated to him/her.
                                           4 Choose the Client and the OM area in the section Target number area if re-
                                             quired.
                                           5 To transfer the items, go to the menu Start > Execute.
                                              Confirm the positive report.
                                              An inquiry has been created for every P.O. item. You can use Documents
                                              > Inquiry to open and print the inquiries and send them to the supplier.


                                            How to create a P.O. from a reference inquiry
                                           1 Open the P.O. transfer dialog.


                            A                                                                   B




                    C

                    A Transfer mode                                   C Target Number Manager
                    B Number Manager with orders for transfer
                    Fig. D-68    Transfer orders from the Number Manager
3.30 / 04-2020




                                           2 Select the Number Manager (B) that includes the orders for which you have
                                             created inquiries.
                                           3 Choose the option Fill pool (A).


                 A+W Business Purchasing                                                                        D-111
                 Purchase orders                                                                                Tutorial




                                           4 To move the orders to the order pool, go to the menu Start > Execute.
                                              The P.O. items are imported and the display changes to the Order pool tab.


                                                                         A                      B




                    C

                   A P.O. mode                                        C Target Number Manager
                   B Inquiries generated for the displayed order
                   Fig. D-69    Create P.O.s for orders


                                              The document numbers of the inquiries are shown for the inquiry items
                                              from the order.
                                           5 Select the option P.O.s (A) and the target Number Manager (C) for P.O.s.
                                           6 Select the items for which a purchase order is to be created.
                                              Double-click on the corresponding line header. Only items marked with an
                                              X have been selected.
3.30 / 04-2020




                 D-112                                                                      A+W Business Purchasing
                 Tutorial                                                                                   Purchase orders




                                           7 To generate purchase orders, go to the menu Start > Execute.
                                               Purchase orders have been created. The transferred items are removed
                                               from the order pool.
                                               You can use Documents > P.O. to open and print the purchase orders and
                                               send them to the supplier.


                                           Create a purchase order from an independent inqui-
                                           ry
                                           You can create a purchase order from any inquiry with the copy function, no
                                           matter whether the inquiry is referenced or not. References to customer orders
                                           will not be adopted however.
                                           The copy function is described in detail in the Sales section.


                                            How to enter a purchase order for an inquiry
                                           1 Open the inquiry for which you want to enter a purchase order.
                                           2 Select the menu Functions > Document group > Copy documents.


                                                                   B                                         C




                    A




                    A Target document type                             C Target Number Manager
3.30 / 04-2020




                    B Copy mode
                    Fig. D-70    Creating a P.O. from an inquiry




                 A+W Business Purchasing                                                                            D-113
                 Purchase orders                                                                       Tutorial




                                   3 Select the document type P.O. (A).
                                      The Target area automatically shows the first Number Manager for pur-
                                      chase orders.
                                   4 Choose a different target Number Manager (C) if required.
                                   5 Check the other settings.
                                   6 To generate the purchase order, go to the menu Start > Execute.
                                      The items are checked and copied. The purchase order is saved.
                                   7 Close the dialog.
                                      The Copy documents dialog disappears and is replaced by the Document
                                      management dialog.
                                      The inquiry and P.O. history shows the reference. You can use Documents
                                      > P.O. to open and print the generated purchase order and send it to the
                                      supplier.
3.30 / 04-2020




                 D-114                                                             A+W Business Purchasing
                 Tutorial                                                                           Purchase orders




                                       Exercises
                                       The structure of the exercises is such that every aspect of purchasing is con-
                                       veyed. This means that the purchase orders created by means of these exer-
                                       cises can be processed further in the next subject.

                                           Checking prerequisites and master data
                                           When working with your own system please make sure that the settings in
                                           master data meet the requirements for the smooth entry of documents and
                                           goods received.
                                           Please also make sure that the document status is changed correctly if the
                                           documents are to be processed further, e.g. in the order pool.

                                       Enter a P.O. item in the order
                                       Enter a customer order with the following items:
                                       •   Items with different purchase codes.
                                       •   Items which can be provided by different suppliers.
                                       •   Items which do not have to be ordered.

                                           Tip
                                           Create 2-3 copies of the orders and of the manual purchase orders so that
                                           you can check the different effects of amendments, e.g. change of supplier
                                           on different levels.

                                       Enter a manual P.O.
                                       Enter a purchase order with the following items:
                                       •   Items with stock articles and products which are not kept on stock.
                                       •   Items with different boxes.
                                       •   At least five boxes per item

                                       Transfer the order to Purchasing
                                       Transfer the orders to Purchasing:
                                       •   at least one order directly (without order pool).
                                       •   at least one order via the order pool.
                                       •   Now check the new purchases order for differences.

                                       Enter order confirmation and check prices
                                       Enter an order confirmation for at at least one reference and one manual pur-
                                       chase order each.
3.30 / 04-2020




                 A+W Business Purchasing                                                                         D-115
                 Purchase orders                                                                            Tutorial




                                   Check and amend delivery dates, notify customer
                                   Enter the following changes:
                                   •   Enter a larger amount in an item in a reference order and transfer the item
                                       again.
                                   •   Select another supplier because he cannot keep the originally confirmed
                                       dates.
                                   •   Change the delivery date in a purchase order, then inform the customer of
                                       the delay.

                                   Remind supplier
                                   Search for purchase orders for which you have not entered an order confirma-
                                   tion yet, and send a reminder to the supplier.


                                   Additional information
                                    “Supplier file” on page D-30
                                    “Deliveries in receipt of goods” on page D-117
                                    “Dealing with boxes” on page D-134
                                    “Receipt of boxes” on page D-133
                                    “Electronic document exchange” on page D-148

                                   Sales section
                                    Sales, “Copy Documents” on page C-206
                                    Sales, “Copy Documents” on page C-461
                                    Sales, “Order/P.O. Info” on page C-486
                                    Sales, “Document Data” on page C-644

                                   Master data section
                                    Master Data, “Product” on page B-139
                                    Master Data, “Currencies” on page B-450
                                    Master Data, “Stock Sizes” on page B-626
                                    Master Data, “Prices” on page B-701
                                    Master Data, “Customers, Suppliers” on page B-745
                                    Master Data, “Company Data” on page B-900
                                    Master Data, “Show items w/o stock code at receipt of goods on stock” on
                                     page B-933

                                   Stock management section
                                    Inventory Management, “Stock Management” on page G-60
                                    Inventory Management, “Stock P.O. (automatic)” on page G-107
                                    Inventory Management, “Stock Management – Stock Articles” on page G-198
                                    Inventory Management, “Stock Movement – Dispatch, Addition” on page G-208
3.30 / 04-2020




                 D-116                                                                 A+W Business Purchasing
                 Tutorial                                                               Deliveries in receipt of goods




                                       Deliveries in receipt of goods
                                       This subject shows you how to check the prices and invoices and enter the re-
                                       ceipt of goods.
                                       This includes the following training modules:
                                       •   “Receipt of goods” on page D-118
                                       •   “Receipt of boxes” on page D-133
                                       •   “Price and invoice control” on page D-141
                                       Receipt of goods usually includes the following steps:
                                       •   Enter a delivery as receipt of goods
                                       •   Check receipt of goods for outstanding or incomplete deliveries
                                       •   Check the invoice.
                                       •   Transfer documents to archives and statistics.
                                       •   Delete document from main database.
                                       This sequence more or less matches the sequence of dialogs in
                                       A+W Business. Some of the steps can be executed in different dialogs how-
                                       ever. This is why they have been summed up in one training session.
                                       The prices on the order confirmation are naturally checked prior to the receipt
                                       of goods. This tutorial describes price control and invoice control together be-
                                       cause the corresponding dialogs are structured in the same way.
                                       Archiving of documents has already been introduced in the Sales tutorial
                                       which is why we are not going to deal with this again at this point.
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-117
                 Deliveries in receipt of goods                                                                          Tutorial




                                           Receipt of goods
                                           Objectives

                                           • Learning about the Receipt of goods dialog.
                                           • Learning about the difference between goods received for stock P.O.s and for
                                             reference P.O.s.
                                           • Checking received goods for completeness
                                           • Being able to add omitted 'goods received' bookings


                                           Benefits

                                           • Deliveries must be entered so that customer order can be completed and shipped.
                                           • The stock is updated when goods received for stock are entered so that you
                                             always have a good idea of the actual stock on hand.
                                           • Receipt of goods can be entered even if the ordered quantity differs from the
                                             quantity delivered.


                                           Please note:

                                           Incomplete delivery        Partial receipt of goods can be entered if the delivered
                                                                      quantity does not match the quantity ordered.

                                           Surplus quantities         If the stock articles delivered (with a stock ID) exceeds
                                                                      the number of stock articles ordered, this quantity will be
                                                                      booked on stock.
                                                                      The receipt of goods of surplus quantities will only be
                                                                      booked if you have ticked the Accept checkbox.
                                                                      Surpluses for customers orders must be permitted and
                                                                      restricted in the master data.

                                           Default settings           Company data:
                                                                      • Parameters tab
                                                                      • Stock/PP/EDI tab
                                                                      Master data (surplus):
                                                                      • Customer, supplier
                                                                      • Product
3.30 / 04-2020




                 D-118                                                                            A+W Business Purchasing
                 Tutorial                                                                     Deliveries in receipt of goods




                                             Deliveries
                                             When entering goods received, a distinction is made between the receipt of
                                             boxes, stock P.O.s, independent, and reference purchase orders.


                   Receipt of goods                                             Booking, status



                   Stock P.O.                                                    Booking in stock on hand

                                                        Assignment of IDs
                   Box                                                           Booking in stock on hand
                                                                                 Status in ref. documents


                   Reference P.O.                                                Booking in stock on hand only for stock
                                                                                 articles


                   Independent P.O.                                              No booking in stock on hand



                 Fig. D-71      Receipt of goods and stock bookings


                                             This distinction helps Stock Management to maintain the stock data.
                                             After booking the receipt of goods, all automatic surcharges for the purchase
                                             order are recalculated and saved.

                                             Receipt of goods for stock P.O.s
                                             Booking the receipt of goods for stock P.O.s updates the stock on hand. The
                                             Stock info dialog shows the reserved quantities in addition to the stock on
                                             hand. This gives you a proper idea of the current and the future stock on hand
                                             even at item entry.
                                             Even stock P.O. items that include articles without stock codes are displayed
                                             at receipt of goods, and can be booked. These bookings will not change the
                                             stock on hand however.
3.30 / 04-2020




                 A+W Business Purchasing                                                                               D-119
                 Deliveries in receipt of goods                                                                    Tutorial




                 A




                 B



                 C




                 D




                 A Delivery date of the selected P.O.                 C Points out a lock status
                 B Completely booked receipt of goods in blue         D Reference order for the selected P.O.
                 Fig. D-72    Receipt of goods – Purchase orders in the Number Manager


                                           P.O. item for production
                                           If you have entered a P.O. item in a customer order which is necessary for pro-
                                           ducing this order, it can be processed further only after receipt of goods. When
                                           you enter the receipt of goods, production must be informed so that the order
                                           can be produced.
                                           You can enable an option in receipt of goods which automatically triggers the
                                           transfer as soon as the receipt of this item has been entered.
                                           For order items with the code P.O.(complete), the status is changed and
                                           passed on to the order so that the order can be shipped.
3.30 / 04-2020




                 D-120                                                                        A+W Business Purchasing
                 Tutorial                                                                  Deliveries in receipt of goods




                                       Items without stock codes
                                       If you enter stock P.O.s with items which are not recorded as stock items, they
                                       will not be displayed at receipt of goods. You can however enable the corre-
                                       sponding option in the company data.




                                       A


                                       A Activate the display in receipt of goods
                                       Fig. D-73     Company data – Stock/PP/EDI tab


                                       Partial receipt of goods
                                       Receipt of goods can be booked in full or partially. Partial receipt of goods can
                                       apply to individual items as well as to partial deliveries for individual items, e.g.
                                       items 5 and 7 of a purchase order or 15 pcs. of an item for which 30 pcs. had
                                       been ordered. The status of the purchase order and/or the order will be set ac-
                                       cordingly afterwards.

                                       Receipt of goods for BOM elements
                                       BOM elements are not listed individually in receipt of goods but belong to the
                                       corresponding main product. The article description shows the BOM elements
                                       separated by "/".
3.30 / 04-2020




                 A+W Business Purchasing                                                                            D-121
                 Deliveries in receipt of goods                                                                      Tutorial




                                           Deliveries with surpluses
                                           If a supplier delivers more pieces of an item than have been ordered (surplus),
                                           you can enter this delivery at receipt of goods. In case of stock articles (with a
                                           stock ID) from a document of the type Stock P.O., the delivered quantity is add-
                                           ed to stock. In the P.O. itself, the quantity is changed accordingly.
                                           The same applies to shortfalls which are rather infrequent in practice however.
                                           The surpluses and shortfalls are defined in the following dialogs:
                                           •   Per customer and per product: Relative amount of divergence.




                                           •   Per product: Relative amount of divergence.




                                           •   Per order item: also divergent quantity
3.30 / 04-2020




                 D-122                                                                         A+W Business Purchasing
                 Tutorial                                                                   Deliveries in receipt of goods




                                       Inspection of goods received
                                       The Inspection of goods received dialog offers a quick overview of open or in-
                                       complete deliveries.

                                               A                             B        C    D




                                       A P.O. number                                  C Delivered quantity
                                       B Ordered quantity                             D Receipt of goods complete
                                       Fig. D-74    Control of the receipt of goods


                                       You can make up for the booking of purchase orders or P.O. items for which
                                       the receipt of goods has not yet been entered although they have been deliv-
                                       ered.
3.30 / 04-2020




                 A+W Business Purchasing                                                                            D-123
                 Deliveries in receipt of goods                                                                   Tutorial




                                            Check the default settings for receipt of goods
                                            The default settings for the receipt of goods have to be made in company data.
                                            The corresponding parameters and options are found on the following tabs:
                                            •   Parameters
                                            •   Stock/PP/EDI




                                                                                                                  A




                 A Virtual item numbers for the receipt of boxes
                 Fig. D-75    Company data – Parameters tab


                                            Virtual item numbers are created so that the boxes received can be booked
                                            correctly. This function is described in the unit on the receipt of boxes.
                                             “Receipt of boxes” on page D-133
3.30 / 04-2020




                 D-124                                                                        A+W Business Purchasing
                 Tutorial                                                                Deliveries in receipt of goods




                                       Stock on hand
                                       To be able to update the stock on hand based on the booked receipts, the res-
                                       ervation option and the stock management on BOM level have to be enabled
                                       in company data.


                                                                                            A
                                       B




                                       A Reservation and updating of stock on B Stock management on BOM level
                                         hand
                                       Fig. D-76    Company data – Stock/PP/EDI tab


                                       Enter receipt of goods
                                       You can use receipt of goods to enter the supplier's order confirmation (OC)
                                       number and change the delivery date. You can book partial deliveries by en-
                                       tering the quantity delivered for an item, or by just marking individual items as
                                       completely delivered.

                                           Entry in receipt of goods
                                           Generally the document numbers are entered via the barcode scanner.
                                           They are entered manually for the following examples. All other steps are
                                           identical for both variants.

                                       The following instructions exist for this training module:
                                       •   “How to enter complete receipt of goods” on page D-126
                                       •   “How to enter partial receipt of goods” on page D-128
3.30 / 04-2020




                 A+W Business Purchasing                                                                         D-125
                 Deliveries in receipt of goods                                                               Tutorial




                                            How to enter complete receipt of goods
                                           1 Go to the menu Documents > P.O.> Receipt of goods > Receipt of goods.




                 A




                                                          B
                 A Selection by Number Manager                       B Selecting the Number Manager
                 Fig. D-77    Receipt of goods – Selection by Number Manager


                                           2 Go to Selection area and choose the option by Number Manager.
                                           3 To import the data, go to the menu Start > Execute.
                                              The display switches to the Complete tab where the purchase orders from
                                              the Number Manager are displayed.
3.30 / 04-2020




                 D-126                                                                     A+W Business Purchasing
                 Tutorial                                                                      Deliveries in receipt of goods




                 A




                 B




                                  C                                                                        D
                 A Delivery date and order confirmation for the selected C Checkbox for complete receipt of goods
                   P.O.                                                  D Indicates that the P.O. includes boxes
                 B Points out a lock status
                 Fig. D-78    Receipt of goods – Purchase orders


                                               The fields in section Delivery date (A) are locked if an order confirmation
                                               from the supplier has been entered for this purchase order.
                                            4 Select the purchase order for which you want to enter receipt of goods.
                                               The fields in Delivery date (A) area are accessible now. Normally, the de-
                                               livery date and the OC number of the supplier have already been created.
                                               You can however add this data if it is missing.
                                            5 Tick the checkbox book completely (C).
3.30 / 04-2020




                 Fig. D-79    Receipt of goods – Report P.O. completed




                 A+W Business Purchasing                                                                             D-127
                 Deliveries in receipt of goods                                                                       Tutorial




                                           6 To enter the receipt of goods, go to the menu Start > Execute.
                                               The data will be saved, and the P.O. status is changed. The stock on hand
                                               is updated if the P.O. includes stock articles. For reference P.O.s, receipt of
                                               goods is passed on to production and/or sales so that the corresponding
                                               customer order can be processed or completed.


                                            How to enter partial receipt of goods
                                           1 Go to the menu Documents > P.O.> Receipt of goods > Receipt of goods.
                                           2 Go to Selection area and choose the option by P.O. number (A) then enter
                                             the P.O. number (B).


                                                             B




                 A




                 A Selection by P.O. number                            B P.O. number
                 Fig. D-80    Receipt of goods – Selection


                                           3 To import the data, go to the menu Start > Execute.
                                               Data will be loaded; the display switches to the Complete tab.
                                               Should you frequently select by P.O. or order number, you can define in the
                                               Options menu that after loading the document, the display should switch to
                                               the By item tab.
                                           4 Go to the By item tab if required.
3.30 / 04-2020




                 D-128                                                                           A+W Business Purchasing
                 Tutorial                                                                         Deliveries in receipt of goods




                                          C                        D   E                                       F




                 B




                 A




                 A Book item completely                                    D Quantity already delivered
                 B Storage place for stock articles                        E Accept surplus or shortfall
                 C Enter partial quantity as receipt of goods              F Order confirmation number
                 Fig. D-81     Receipt of goods – Report partial quantity for the P.O.


                                                 All P.O. items will be displayed. You can enter partial receipt of goods as
                                                 follows:
                                                 •   Complete booking of one of the P.O. items (A).
                                                 •   Enter part (C) of the ordered quantity for an item.
                                                 If for instance the quantity delivered for a stock P.O. does not exactly match
                                                 the ordered quantity, you can accept a surplus or a shortfall (E), thus book-
                                                 ing complete receipt of goods for an item.
                                              5 Select the item for which you want to enter receipt of goods.
                                              6 Go to field Quantity received (C) and enter the number of items received or
                                                tick the checkbox Book completely (A) to report the entire item as complete.
                                              7 Enter the supplier's order confirmation number (F) if required.
                                              8 For stock articles, choose the storage place (B).
3.30 / 04-2020




                 A+W Business Purchasing                                                                                D-129
                 Deliveries in receipt of goods                                                                       Tutorial




                                          C                        D   E                                     F




                 B




                 A




                 A Book item completely                                    D Quantity already delivered
                 B Storage place for stock articles                        E Accept surplus or shortfall
                 C Enter partial quantity as receipt of goods              F Order confirmation number
                 Fig. D-82     Receipt of goods – Report partial quantity for the P.O.


                                              9 Go to the menu Start > Execute to save the data.
                                                 Partial receipt of goods will be booked.
                                                 The P.O. items are shown in blue if the purchase order/item has been de-
                                                 livered in full.
                                                 Changes are adopted for the purchase order and the reference customer
                                                 order if required.
                                                 A surplus will be saved in the purchase order while a reference order will
                                                 remain unaffected. On stock, the surplus will be booked automatically only
                                                 for stock articles from stock P.O.s. The same applies to shortfalls theoreti-
                                                 cally; in practice however one would rather create a partial delivery and re-
                                                 mind the supplier of the missing quantity.
3.30 / 04-2020




                 D-130                                                                              A+W Business Purchasing
                 Tutorial                                                                 Deliveries in receipt of goods




                                       Check receipt of goods
                                       You have to check deliveries for completeness in order to determine which or-
                                       ders can be processed further. If you know that the delivery has actually ar-
                                       rived you can enter the receipt of goods. You can check the following facts:
                                       •   Complete purchase orders per Number Manager
                                       •   Quantity discrepancies per P.O. item


                                        How to check the receipt of goods
                                       1 Go to the menu Documents > P.O.> Receipt of goods > Incoming control.




                                           Fig. D-83    Inspection of goods received – Complete P.O.


                                       2 Go to the Complete P.O.s tab and select the Number Manager for the pur-
                                         chase orders.
                                           In the Receipt of goods complete overview, all P.O.s are listed, whose P.O.s
                                           have been entered completely.
                                       3 Go to the Qty.discrepancies tab to display the incomplete items.
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-131
                 Deliveries in receipt of goods                                                                     Tutorial




                                                                                               A B
                                              A Quantity partially delivered          B Book complete receipt of goods
                                              Fig. D-84     Inspection of goods received – Qty. discrepancies


                                              The overview lists all purchase orders for which no receipt has been
                                              booked, or incomplete receipt of goods.
                                              If you have moved the purchase order to a target Number Manager when
                                              booking the entire receipt of goods, no discrepancies should be shown
                                              here.
                                           4 Catch up on any overdue bookings by ticking the checkbox OK (B).
                                              Please note that you can add only complete receipt of goods. To enter par-
                                              tial quantities, go to the Receipt of goods dialog.
                                           5 To start the booking of the receipt of goods, go to the menu Start > Execute.
                                              Receipt of goods will be booked. Completely booked purchase orders are
                                              removed from the list.


                                           Additional information
                                            Master Data, “Show items w/o stock code at receipt of goods on stock” on
                                             page B-933
                                            Master Data, “Stock control mode” on page B-933
                                            Sales, “Stock Info” on page C-650
                                            Software Reference, “Receipt of goods” on page D-225
3.30 / 04-2020




                 D-132                                                                          A+W Business Purchasing
                 Tutorial                                                                     Deliveries in receipt of goods




                                       Receipt of boxes
                                       Objectives

                                       • Learning the meaning of the dummy box
                                       • Learning about the assignment of IDs
                                       • Learning about the settings for the automatic assignment of box IDs


                                       Benefits

                                       • Upon receipt, every box gets an ID so that it can be clearly identified on stock, and
                                         can be reserved for an order.
                                       • IDs can be assigned manually or automatically. You can also adopt the supplier's
                                         box ID.


                                       Please note:

                                       Virtual item numbers         If the quantity of a box item is over 1, a sub-item will be
                                                                    created for every box. These sub-items will get virtual
                                                                    item numbers consisting of the item number and the
                                                                    number of boxes, e.g. 1.1, 1.2 or 3.1, 3.2 etc.

                                       ID                           When you enter receipt of goods, the box of every sub-
                                                                    item is assigned a separate ID.

                                       Box identification           Only a box with an ID can be booked as stock on hand
                                                                    and/or allocated to an order item.

                                       Default settings             Master data:
                                                                    • Product Management
                                                                    Company data:
                                                                    • Parameters tab
                                                                    • Stock/PP/EDI tab
3.30 / 04-2020




                 A+W Business Purchasing                                                                                 D-133
                 Deliveries in receipt of goods                                                                    Tutorial




                                           Dealing with boxes
                                           Boxes are usually assigned ID numbers which may originate from the supplier
                                           or are maintained in your own system. These IDs are entered when boxes are
                                           received. Every box is booked with its own box ID by which it is kept on stock.
                                           Even if the number of boxes of a P.O. item is over 1, every box is booked as a
                                           separate receipt of goods. The system automatically creates sub-items (virtual
                                           items) for the original item and allocates just one box to each of these items.
                                           This function must be enabled in company data.
                                           An individual box ID must be allocated to each sub-position so that the stock
                                           on hand of the boxes can be maintained. These box IDs can be automatically
                                           assigned based on the values you define. An ID can also be entered manually,
                                           e.g. when adopting the box ID from the supplier's delivery note.
                                           As part of the receipt of goods, a production date can also be specified in the
                                           automatic box ID dialog. For coated glass, this can be used for calculating the
                                           expiry date so that boxes can be handled according to the FiFo principle (FiFo
                                           = First in - First out).
                                           When the IDs have been assigned, you can use the print function to print box
                                           labels with the IDs as barcodes, then stick them to the appropriate boxes.
                                           Box barcodes are usually scanned upon issue of stock or when a box is bro-
                                           ken up. This does not only serve to keep the number of boxes up to date but
                                           also for identifying the boxes.


                                           Check company data
                                           The Master data section describes in detail how to define the master data for
                                           your company. The following description therefore only deals with the peculiar-
                                           ities you have to consider in connection with the receipt of boxes.

                                              Reboot A+W Business
                                              After changing company data, reboot A+W Business.


                                            How to check company data
                                           1 Go to the menu Master data > Company > Company data and check the
                                             setting for the checkbox Use virtual item numbers on the Parameters tab.
                                              This setting is already explained in the unit on Receipt of goods.
                                               “Company data – Parameters tab” on page D-124
                                           2 Go to the menu Start > Save to save the changes.
                                              The data is saved.


                                           Checking the settings for ID numbers
                                           If you want to enter the boxes with a separate box ID, this ID can be assigned
3.30 / 04-2020




                                           automatically. You have to define the necessary settings. These settings can
                                           be adapted before every receipt of boxes, e.g. to add a code for the supplier
                                           to the ID.



                 D-134                                                                        A+W Business Purchasing
                 Tutorial                                                                Deliveries in receipt of goods




                                       You can use a maximum of 20 characters which are automatically completed
                                       by a 5-digit number. The entered string is kept until it is changed manually. If
                                       you add a code for the supplier to the box ID, you have to make sure to change
                                       the ID before you enter the receipt of boxes for another supplier.


                                        How to check the settings for the automatic allocation of ID numbers
                                       1 Go to the menu Documents > P.O.> Receipt of goods > Receipt of goods.
                                           The Receipt of goods dialog opens.
                                       2 Go to the menu Options > Group > ID number allocation > Settings.




                                       3 Enter the code.
                                           Please avoid overwriting the dummies (X) for the numbers.
                                       4 Click on [OK] to save the changes.
                                           The dialog closes. The settings are saved and will be kept until they are
                                           changed again manually.
                                       5 Go to the menu Options > Group ID number allocation > Automatic alloca-
                                         tion.
                                           Automatic allocation of box IDs has been set now.
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-135
                 Deliveries in receipt of goods                                                                   Tutorial




                                           Enter the receipt of boxes
                                           When you enter the receipt of boxes, the box of every sub-item is assigned a
                                           separate ID. Then the respective labels are printed.
                                           The following instructions exist for this training module:
                                           •   “How to enter receipt of boxes with automatic IDs” on page D-136
                                           •   “How to enter box IDs manually” on page D-139
                                           •   “How to print box labels” on page D-140


                                            How to enter receipt of boxes with automatic IDs
                                           1 Go to the menu Documents > P.O.> Receipt of goods > Receipt of goods.


                                                           B




                 A




                 A Search option                                      B P.O. number
                 Fig. D-85    Receipt of boxes – by Number Manager


                                               Please make sure that automatic allocation of box IDs is active.
                                           2 Choose the option (A) which which you would like to search for the open
                                             purchase orders, e.g. by P.O. number.
                                           3 Enter the P.O. number (B).
                                           4 To import the data, go to the menu Start > Execute.
3.30 / 04-2020




                                               You will find yourself on the Complete tab. You can check the data again.
                                           5 Go to the ID tab.



                 D-136                                                                         A+W Business Purchasing
                 Tutorial                                                                     Deliveries in receipt of goods




                 A



                 B

                 C




                 D




                 A Selected P.O.                                       C Storage place
                 B Enter supplier's box ID                             D One line per box (sub-item)
                 Fig. D-86    Receipt of boxes – Enter receipt


                                                If the quantity of the ordered item is larger than 1, the Box items overview
                                                lists a separate line for every box.
                                                You can select several boxes at once to book them in one step.
                                             6 Select a line that shows no virtual item number yet.
                                             7 Go to field Supplier ID (B) and enter the supplier's box ID or scan the box
                                               ID and use <Tab> to go to the next field.
                                                If more than one box was selected and the supplier ident numbers entered,
                                                the system calculates the box ident numbers for all marked entries.
                                             8 Choose the storage place, check the contents and price and correct them
                                               if necessary.
3.30 / 04-2020




                 A+W Business Purchasing                                                                             D-137
                 Deliveries in receipt of goods                                                                    Tutorial




                 A




                 B




                 A Supplier's box ID                                     B Book receipt of goods for this box
                 Fig. D-87    Receipt of boxes – Data for the selected line


                                                The input is adopted for the selected line.
                                            9 In the menu, go to Start > Execute in order to confirm the entries and to
                                              book the receipt of goods.




                 A

                                                                                B
                 A Virtual item number (booked sub-item)                       B (Automatic) box ID
                 Fig. D-88    Receipt of boxes – New, virtual item number created


                                                The box is booked and moved to the end of the Box items list together with
                                                the next virtual item number.
                                            10 Repeat steps7 to 9 until you have entered all receipt of goods.
                                                When you have entered all boxes you can start to print the box labels and
3.30 / 04-2020




                                                the protocol.
                                                 “How to print box labels” on page D-140




                 D-138                                                                            A+W Business Purchasing
                 Tutorial                                                                    Deliveries in receipt of goods




                                             How to enter box IDs manually
                                            1 Go to the menu Documents > P.O.> Receipt of goods > Receipt of goods.
                                            2 Disable in the menu Options > Group ID number allocation > Automatic al-
                                              location.
                                            3 Make the preparations to enter the receipt of goods as described in the
                                              steps 2 to 7 of the previous sequence.


                 A



                 B
                 C




                 D




                 A Selected P.O.                                      C Manual box ID
                 B Supplier's box ID                                  D One line per box (sub-item)
                 Fig. D-89    Receipt of boxes – Enter receipt


                                               If the quantity of the ordered item is larger than 1, the Box items overview
                                               lists a separate line for every box.
                                            4 Enter the box ID (C) by which the box shall be booked on stock.
                                               You can adopt the supplier's ID by moving the cursor to the field and scan-
                                               ning the supplier ID again.
                                            5 Choose the storage place, check the contents and price and correct them
                                              if necessary.
                                               These entries are only valid for box items selected from the list.
3.30 / 04-2020




                                            6 To confirm the entries, go to the menu Start > Execute.
                                               The box is booked and moved to the end of the Box items list together with
                                               the next virtual item number.


                 A+W Business Purchasing                                                                            D-139
                 Deliveries in receipt of goods                                                                     Tutorial




                                           7 Repeat steps4 to 6 until you have entered all receipt of goods.
                                              When you have entered all boxes you can start to print the box labels in
                                              order to print labels with the manually allocated IDs.


                                            How to print box labels
                                           1 After entering the boxes of a shipment, go to the menu Print > Printer > La-
                                             bels.
                                              If you select the entry Labels and protocol, a protocol is also printed, which
                                              you can also view in the Protocol (IDs) tab.




                                                                                              A

                                                                                              B




                                              A Quantity                             B Printer
                                              Fig. D-90    Print box labels


                                           2 Select the printer (B) and the number (A) of copies required.
                                           3 Click [OK] to start printing.
                                              The dialog closes and the labels are printed. All booked boxes and box IDs
                                              are listed in the protocol.


                                           Additional information
                                            Master Data, “Use virtual item numbers” on page B-919
                                            Software Reference, “Settings (ID)” on page D-238
3.30 / 04-2020




                 D-140                                                                           A+W Business Purchasing
                 Tutorial                                                                    Deliveries in receipt of goods




                                       Price and invoice control
                                       Objectives

                                       • Entering the supplier's order confirmation.
                                       • Check prices.
                                       • Entering a collective order confirmation for several purchase orders.


                                       Benefits

                                       • You can check the prices together with the order confirmation.
                                       • The prices of several purchase orders can be checked in a collective order
                                         confirmation.


                                       Please note:

                                       Status                      After checking the prices and invoices, the document
                                                                   status is raised. This is why price and/or invoice control
                                                                   cannot be repeated in connection with a lock status.

                                       Differences                 You can complete the price or invoice control only if
                                                                   there is no difference between the defined total and the
                                                                   total of the purchase orders displayed.

                                       Quick entry                 If you enable the menu Options > Quick entry, the cursor
                                                                   switches directly to field Invoice total or OC total when
                                                                   you enter the P.O. number. You can use this option if you
                                                                   usually enter just one P.O. number.

                                       Document lock               Reference documents are locked for other users while
                                                                   the price and invoice control is run.

                                       Default settings            Company data:
                                                                   •   Tax tab
                                                                   •   Pricing tab
                                                                   •   Print tab
                                                                   •   Stock/PP/EDI tab
3.30 / 04-2020




                 A+W Business Purchasing                                                                               D-141
                 Deliveries in receipt of goods                                                                     Tutorial




                                           Incoming invoice
                                           Prices can be checked based on the supplier's order confirmation or based on
                                           the supplier's invoice. The Price control and Invoice control dialogs have the
                                           same structure. This allows you to correct the prices and update your pur-
                                           chase prices (PP) in the documents.
                                           During price/invoice control, access of the respective purchase order will be
                                           blocked for other users. In order to be able to amend the purchase order dur-
                                           ing the price or invoice control, the document can be opened directly. This per-
                                           mits you e.g. to enter missing surcharges without leaving price and invoice
                                           control.
                                           The prices and invoices in electronically exchanged documents can also be
                                           checked. This function is described in connection with Electronic document
                                           exchange:
                                            “Export/Import (openTRANS)” on page D-149

                                           Price corrections
                                           You can complete price or invoice control only if there is no difference between
                                           the defined total and the total of the purchase orders displayed. Such differ-
                                           ences can e.g. be attributed to different prices, surcharges that have not been
                                           entered, or incorrect entries.
                                           If the amount entered does not match the purchase order or the total of pur-
                                           chase orders, prices have to be corrected in the items or in the BOM – or return
                                           the order confirmation/invoice and ask for correction.
                                           After invoice control, the purchase orders get the appropriate status and are
                                           now ready for to be released and transferred to financial accounting.
                                           The status of the purchase order is changed accordingly after checking, cor-
                                           recting and confirming the prices.

                                           Purchase prices in the order
                                           The PP of a reference order can only be updated for the amount of time al-
                                           lowed by the locking status. The status of the purchase order is raised after the
                                           invoice control is complete. Price or invoice control cannot be run again after-
                                           wards.
3.30 / 04-2020




                 D-142                                                                         A+W Business Purchasing
                 Tutorial                                                                Deliveries in receipt of goods




                                       Footer surcharges and discounts
                                       The footer The footer surcharges/discounts of a purchase order, e.g. an ener-
                                       gy surcharge, are saved in the costs of the order. The footer surcharges/dis-
                                       counts are distributed to the individual items and are shown in document
                                       management. This way, the contribution margin shown at item entry is always
                                       up to date, even for ordered items.
                                       As an option, the item Delivery fee per P.O. can be added during invoice con-
                                       trol. This way, you do not have to enter it manually later in the purchase order.

                                       Foreign currency
                                       If you are using several currencies, you can confirm the prices and invoices in
                                       foreign currency. The prices of the P.O. items are saved in national currency.
                                       The purchase prices are updated on the basis of the currency conversion.

                                       Collective order confirmation and collective invoice
                                       If your supplier has collected several purchase orders in an order confirmation
                                       or invoice, this can be checked and accepted only if all purchase orders show
                                       the same VAT rate and the same currency.
                                       If one of your suppliers usually issues collective invoices, it may be useful to
                                       define a special Number Manager for purchase orders sent to this supplier.

                                       Save purchase price
                                       The purchase price is saved in the reference orders if it has been changed dur-
                                       ing price or invoice control and/or when booking the receipt of goods. The
                                       amended purchase prices are used to calculate the contribution margin, to
                                       evaluate the stock, or for stock P.O.s.
                                       The corresponding option to determine the purchase price must be enabled in
                                       company data, and the purchase price tables must be maintained appropriate-
                                       ly.




                                       Fig. D-91    Company data – Stock/PP/EDI tab
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-143
                 Deliveries in receipt of goods                                                                     Tutorial




                                            Checking the invoice
                                            Prices can be checked in the order confirmation as well as in the supplier's in-
                                            voice. Two dialogs are available for this purpose which are identical in struc-
                                            ture and function:
                                            •   Price control
                                            •   Invoice control
                                            Price control has already been introduced in the unit Enter order confirmation
                                            and check prices. Just like with price control, you can check the supplier in-
                                            voice and release for payment.

                                                Define cursor position
                                                If you enable the menu Options > Quick entry, the cursor switches directly
                                                to field Invoice total or OC total when you enter the P.O. number. You can
                                                use this option if you usually enter just one P.O. number.


                                             How to check a received supplier's invoice
                                            1 Go to the menu Documents > P.O.s > Invoice > Invoice control.




                 A                                                                                                    D
                 B

                 C

                                                                                                                      E




                 A Invoice number                                       D Purchase order number(s)
                 B Invoice date                                         E Exchange rate
                 C Invoice amount (net/gross)
                 Fig. D-92    Invoice control
3.30 / 04-2020




                                            2 Enter the invoice number (A), the date (B), and the P.O. number (D) and
                                              use <Tab> to go to the next field.
                                                The purchase order is displayed in the P.O.s overview.


                 D-144                                                                         A+W Business Purchasing
                 Tutorial                                                                       Deliveries in receipt of goods




                                                  If an invoice covers several purchase orders, you can enter the P.O. num-
                                                  bers one by one. The P.O.s are the added to the list. You can only combine
                                                  purchase orders with the same tax rate however.
                                                  To remove a purchase order from the overview, select it and press <Del>.
                                              3 Enter the invoice total (C).

                                                  Currency
                                                  If you are using just one currency (EUR), the entry in field Rate (E) must
                                                  be 1.

                                              4 To confirm the entry, go to the menu Start > Execute.
                                                  The amount will be checked and the Items tab appears.




                                                                                                                    A




                                                                                                                    B


                 A Item price                                              B Difference across all items
                 Fig. D-93      Invoice control – Items


                                                  You can level out price differences by changing an item price. Amended
                                                  amounts will be saved in the reference documents.
3.30 / 04-2020




                 A+W Business Purchasing                                                                                D-145
                 Deliveries in receipt of goods                                                                      Tutorial




                                           5 If no (more) differences are shown, go to Start > Execute.
                                              The data is saved, and the status of the purchase order(s) changed. In-
                                              voice control cannot be run again for this document after that.
                                              Purchase price calculation is corrected in the corresponding purchase or-
                                              ders and orders if this option has been enabled in the menu Options >
                                              Group >Settings.


                                           Additional information
                                            Software Reference, “Price control” on page D-203
                                            Software Reference, “Invoice control – Purchase orders” on page D-246
3.30 / 04-2020




                 D-146                                                                        A+W Business Purchasing
                 Tutorial                                                                 Deliveries in receipt of goods




                                       Exercises
                                       The structure of the exercises is such that every aspect of purchasing is con-
                                       veyed. This means that you are going to further edit the purchase orders from
                                       the previous subject now.

                                       Enter receipt of goods
                                       Enter all receipt of goods for a reference P.O. and check if the status of the or-
                                       der has changed.

                                       Enter partial receipt of goods
                                       Enter a partial delivery for a reference P.O. and for a manual P.O.
                                       Enter receipt of goods for a stock P.O. and for an item that includes products
                                       which are not kept on stock (partly or completely).

                                       Enter receipt of boxes
                                       Enter the partial or complete receipt of boxes.

                                       Check deliveries for completeness
                                       Search for purchase orders, for which items or sub-items have not been deliv-
                                       ered yet.
                                       Make up for the entry of the receipt of goods by making a complete booking.

                                       Check the invoice
                                       Enter the invoice for the receipt of goods.
3.30 / 04-2020




                 A+W Business Purchasing                                                                         D-147
                 Electronic document exchange                                                                     Tutorial




                                            Electronic document ex-
                                            change
                                            This subject shows you how to adapt A+W Business for electronic document
                                            exchange, and how to export and import documents.
                                            You can exchange documents electronically with your suppliers/customers.
                                            To exchange purchase orders, data is saved in an ASC file. In order to ex-
                                            change invoices or order confirmations, data must be available in openTRANS
                                            format (XML format).



                                                                    EDI
                              Customer order = purchase order                      P.O.




                             Customer                           A+W Business                           Supplier

                         A+W Business                                                              A+W Business


                              Order confirmation (OC)                              Order confirmation (OC)
                              Invoice                            openTRANS         Invoice


                 Fig. D-94    Data export and import


                                            Purchase orders can be exchanged via EDI. From the customer's point of
                                            view, the customer order is a purchase order while for A+W Business, it is an
                                            order.
                                            Order confirmations and invoices can be exchanged in openTRANS format.
                                            This requires that all parties involved are using A+W Business. This function
                                            will be explained in detail in the following chapters.
3.30 / 04-2020




                 D-148                                                                        A+W Business Purchasing
                 Tutorial                                                                  Electronic document exchange




                                       Export/Import (openTRANS)
                                       Objectives

                                       •   Learning about the functional principle of electronic document exchange
                                       •   Learning about the settings and how to adapt them
                                       •   Learning about mandatory fields in documents
                                       •   Dispatch and import of electronic documents


                                       Benefits

                                       • Electronic document exchange can be used to import documents from your
                                         customers and suppliers without having to enter the individual data.
                                       • Data import helps to reduce input errors.


                                       Please note:

                                       Prerequisite                 The supplier/customer has to have the same
                                                                    A+W Business version as yourself, at least
                                                                    A+W Business 5.
                                                                    The necessary services must be installed and started.

                                       Data format                  Electronic documents can be exchanged in openTRANS
                                                                    and in XML format.

                                       Data import                  Data can be sent as files by email or saved on a shared
                                                                    drive on a server.

                                       Data export                  Whenever an order confirmation or an invoice is printed,
                                                                    the program checks whether there are documents with
                                                                    the code for the export flag. These documents will be
                                                                    automatically sent to the defined email address.

                                       References                   Document references are created from the following
                                                                    fields:
                                                                    • In the order header, field P.O. text1
                                                                    • At item entry, field Customer item
                                                                    These fields always have to be filled in.
                                                                    If these references cannot be established in imported
                                                                    documents, allocation has to be done later by hand,
                                                                    when checking the electronic document.

                                       Partial deliveries           Partial deliveries can be created from an electronic order
                                                                    confirmation.

                                       Rounding differences         At price and invoice control, rounding differences of just
                                                                    a few cents are acceptable if a so-called balancing item
                                                                    has been defined in product management to which
                                                                    differences can be booked.

                                       Collective invoices          For collective invoices issued by the supplier, a
3.30 / 04-2020




                                                                    surcharge which appears just once can be distributed to
                                                                    all items of the purchase orders or P.O. items involved.




                 A+W Business Purchasing                                                                               D-149
                 Electronic document exchange                                                            Tutorial




                                        Please note:

                                        Document lock      Reference documents are locked for other users while
                                                           the price and invoice control is run.

                                        Default settings   Master data:
                                                           •   Product data
                                                           •   Customer/supplier data
                                                           •   Status definition
                                                           •   Status allocation
                                                           •   Currencies
                                                           Company data:
                                                           • Parameters tab
                                                           Master data:
                                                           • B2B customer/supplier
3.30 / 04-2020




                 D-150                                                                  A+W Business Purchasing
                 Tutorial                                                               Electronic document exchange




                                       Document exchange
                                       Order confirmations and invoices can be exported and imported in open-
                                       TRANS format. This format has been extended for A+W Business. Docu-
                                       ments can also be imported in standard format and XML files however.
                                       Exchanging data in openTRANS format requires that the customer/supplier
                                       has the same A+W Business versions installed as you have, at least
                                       A+W Business 5. The parameters in the interface management have to be de-
                                       fined in the same way at the customer/supplier as in your A+W Business sys-
                                       tem.

                                       Document export
                                       The export of order confirmations and invoices are configured separately for
                                       each customer/supplier in the module Master data > B2B. You have to define
                                       whether and which documents are to be exported, and which mode is to be
                                       used.

                                                                                   C




                                       B
                                       A




                                                                                            D
                                       A Export mode                            C Selection of documents
                                       B Export format                          D Settings for email mode
                                       Fig. D-95    Settings for electronic data exchange


                                       Export mode (A):
                                       •   Automatic email dispatch:
                                           There has to be an email server in the network for this purpose. The email
3.30 / 04-2020




                                           address defined in customer/supplier master data will be used by default.
                                           Different email addresses can be defined for order confirmations and in-
                                           voices.



                 A+W Business Purchasing                                                                      D-151
                 Electronic document exchange                                                                  Tutorial




                                        •   Saving in a certain directory (on the server):
                                            These files can be transferred manually afterwards.
                                        Whenever an order confirmation or an invoice is printed, the program checks
                                        whether there are documents with the code for the export flag. The actual ex-
                                        port is performed at regular intervals by a service in the background. The cor-
                                        responding documents are shown in the Export dialog for control purposes.
                                        The following files are created as part of the export process:
                                        •   RESPONSExxxx.awotres for order confirmations.
                                        •   DISPATCHxxxx.awotdis for a delivery notification.
                                        •   INVOICExxxx.awotinv for invoices.
                                        File names are case sensitive.

                                        Document references
                                        Document references on item level are necessary for the automatic allocation
                                        (reference) of order items and the corresponding P.O. items (referencing). At
                                        manual order entry, these document references are automatically created
                                        from the fields P.O. text1 in the order header and Customer item at item entry.




                                                       A           B


                                        A Header data – Document               B Items – Item tab
                                        Fig. D-96    Reference for data exchange


                                        Plus, this requires that the option Adopt P.O. text1 and customer item for doc-
                                        ument references is active in company data in the Parameters tab.




                                        Fig. D-97    Company data – Parameters
3.30 / 04-2020




                 D-152                                                                     A+W Business Purchasing
                 Tutorial                                                                Electronic document exchange




                                       Document import
                                       Order confirmations and invoices in openTRANS format are imported by
                                       means of the A+W openTRANS ImportTool. It is installed on the
                                       A+W Business client by default.
                                       This is why there are different import options:
                                       •   Double-click on the saved file.
                                       •   Double-click on the file sent as an email attachment.
                                       Double clicking imports the data into the database where it can be displayed
                                       in A+W Business's import dialogs.
                                       If the files are stored on the hard disk, you can use the context menu to start
                                       the option Display and display a generic view of the document.

                                       XML files
                                       XML files cannot be imported directly from the email client. These files have to
                                       be saved first. After that, they can be imported by means of the context menu,
                                       or displayed as a generic view.
                                       When a document has been successfully imported, it is available in the Electr.
                                       price control or Electr. invoice control dialog.
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-153
                 Electronic document exchange                                                                         Tutorial




                                             Document check
                                             The Price control and Invoice control dialogs have the same structure.




                 A




                 B



                 C




                                                                                D
                 A Imported document                                    C Status
                 B Display and filter settings                          D Referenced documents
                 Fig. D-98     Electronic invoice control


                                             In both dialogs, all documents (D) that are linked with the imported document
                                             (A) are shown – including possible partial deliveries. For every purchase order,
                                             there is an optical signal (C) which tells you whether the links between the pur-
                                             chase order and imported document are complete. Only completely refer-
                                             enced documents can be accepted.
                                             When the imported document has been accepted, the status of the reference
                                             purchase orders is changed accordingly. Price or invoice control cannot be run
                                             again afterwards.

                                             Booking types
                                             When you check the imported documents, the options Accept, Create partial
                                             delivery, and Reject are offered depending on the status.
                                             Booking type Accept is only available if an imported document is complete and
                                             correctly referenced. If only the ordered quantities are not fully referenced
                                             while the document is otherwise complete, a partial delivery can be automati-
3.30 / 04-2020




                                             cally created with this booking type.




                 D-154                                                                           A+W Business Purchasing
                 Tutorial                                                              Electronic document exchange




                                       Item allocation
                                       If the P.O. references are incorrect or missing from an openTRANS document,
                                       the system cannot automatically link document and P.O. items. These (un-
                                       linked) items are marked on the item list and have to be linked manually.
                                       In an invoice, the reference with an item can be missing or incorrect for in-
                                       stance. Based on the product names, you can set these references in the
                                       Manual item allocation dialog.

                                       Footer surcharges/discounts
                                       Footer surcharges or discounts are usually not entered in the purchase order.
                                       They do appear on the order confirmation or on the invoice however. To per-
                                       form invoice control, these items have to be subsequently added to the pur-
                                       chase orders. P.O. entry can be accessed from the Invoice control dialog for
                                       this purpose. After the surcharge has been entered in the P.O., it has to be al-
                                       located in the invoice.
                                       If your supplier has collected several purchase orders in one invoice in which
                                       the footer surcharge/discount appears just once, this item can be distributed
                                       to all linked purchase orders. Based on the surcharge basis, the program tries
                                       to find – and suggests – reasonable values for the proportional amounts.
                                       These values can be changed.
                                       Based on the product number, the footer surcharges/discounts can also be al-
                                       located automatically for this supplier. The allocation of the supplier's product
                                       number to your own product number will be saved.

                                       Collective invoices in A+W Business
                                       If collective invoices are issued in A+W Business, the footer surcharges/dis-
                                       counts are shown as individual items for every order. Since direct manual al-
                                       location is often difficult, you can collect several document items in this case,
                                       and allocate them to the P.O. items. In the item overview, it is then only listed
                                       as a combined document item.
3.30 / 04-2020




                 A+W Business Purchasing                                                                         D-155
                 Electronic document exchange                                                                    Tutorial




                                        Differing amounts
                                        You can usually accept an invoice only if no differences are found. If you (are
                                        to) expect different amounts from a supplier, you can handle this in various
                                        ways:
                                        •   You can reject the invoice and inform the supplier of the discrepancies (by
                                            phone).
                                        •   Different amounts can also be caused by different rounding methods. Op-
                                            tion Accept different amounts allows for invoice control to be performed de-
                                            spite such discrepancies. The difference may only be a matter of cents. You
                                            should use the option Notification of price difference/balancing item to be
                                            made aware of this.
                                            Rounding differences in the scope of cents can be accepted automatically.
                                            You have to create a so-called balancing product to which the difference
                                            can be booked.
                                        •   The function Prod.no. for balancing item can be used to select a product to
                                            which the rounding differences (if they are just a matter of cents) are to be
                                            booked.
3.30 / 04-2020




                 D-156                                                                      A+W Business Purchasing
                 Tutorial                                                                 Electronic document exchange




                                         Check the services
                                         The following services must be installed and running:
                                         •   A+W Business 6 Interface Service
                                             This service is usually installed on a separate computer. When it is installed
                                             by a member of the A+W Software GmbH service team, the function Inter-
                                             face Service handles B2B documents must be enabled.
                                         •   AWProtocolService
                                             This service can be found in System control > Management > Services.
                                         •   ERP-WebService
                                             This service is found in System control > Computer management > Servic-
                                             es and applications > Sites > Default web site.




                    Fig. D-99   Check ERP service


                                         The services are usually installed together with A+W Business. They are set
                                         to the start mode Automatically. They should start automatically when you turn
                                         on your computer.
                                         If the data exchange does not work, you should check the services and start
                                         them manually if necessary. Instructions for this can be found in the operating
                                         system's online help.
                                         You will also need the A+W openTRANS ImportTool which is automatically in-
                                         stalled by the A+W Business setup.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-157
                 Electronic document exchange                                                                        Tutorial




                                        Status allocation
                                        The status of the documents is also changed during import and export. For
                                        this, the following status points need to be assigned.

                                           Status Points

                                           for import                              for export

                                           61 - Do not accept order confirmation   830 - Invoice export

                                           64 - Do not accept invoice              840 - Export of order confirmations


                                        During import, the status is changed manually and during export it is changed
                                        automatically.
                                        The status points and status allocations are described in detail in the Master
                                        data section. This unit therefore only deals with the peculiarities you have to
                                        consider in connection with the electronic exchange of documents.
3.30 / 04-2020




                 D-158                                                                          A+W Business Purchasing
                 Tutorial                                                              Electronic document exchange




                                          Check the default settings for data exchange
                                          The settings for exchanging product data have to be made correctly in compa-
                                          ny data. Documents can be imported correctly only if the corresponding prod-
                                          uct data has been entered and allocated.

                                             Reboot A+W Business
                                             After changing company data, reboot A+W Business.


                                           How to check company data
                                          1 Select the menu Master data > Company > Company data and go to the
                                            Parameters tab.




                                                                                                             A




                 A Adopt P.O. text
                 Fig. D-100   Company data – Parameters


                                          2 Tick the checkbox Adopt P.O. text1 and customer item into document ref-
                                            erences.
                                          3 Go to the menu Start > Save to save the changes.
3.30 / 04-2020




                                             The data is saved.




                 A+W Business Purchasing                                                                         D-159
                 Electronic document exchange                                                                     Tutorial




                                        Check the currency settings
                                        The international currency code must be stored for the currencies used in the
                                        orders and purchase orders. You have to check the settings if you are using
                                        several currencies.


                                         How to check currency settings
                                        1 Select Master data > Finances > Currency.

                                                                  A                            B




                                           A Exchange rate to convert prices      B International currency code
                                           Fig. D-101   International currency code


                                           Every currency has to be assigned an international currency code (B).
                                        2 Select the line of the currency that you want to assign the code to.
                                        3 Open the combo box in the column Internat. code and select the appropri-
                                          ate code from the list.
                                        4 Check each exchange rate (A) entered and update them if required.
                                        5 Go to the menu Start > Save to save the changes.
                                           The data is saved.
3.30 / 04-2020




                 D-160                                                                     A+W Business Purchasing
                 Tutorial                                                              Electronic document exchange




                                       Check status definitions
                                       Status points 61, 64, 830, 840 must be defined and assigned in order to pro-
                                       cess electronic documents. These status points are required for the following
                                       actions:
                                       •   Import and export of documents.
                                       •   Rejecting or accepting an imported document.
                                       For instructions on this subject, please see:
                                       •   “How to check the status points” on page D-161
                                       •   “How to check the status management” on page D-161
                                       •   “How to check the status allocation” on page D-163


                                        How to check the status points
                                       1 Select the menu Master data > Order > Status points.




                                           Fig. D-102   Status points


                                       2 Check whether status points 61, 64, 830 and 840 exist.
                                           The numbers of the status points are stated in the Code column.
                                           Status points are normally created during installation. They always have to
                                           be allocated manually.
                                       3 If not all of these status points exist, enter the missing ones.
                                       4 Go to the menu Start > Save to save the changes.
                                           The data is saved. The status points must be assigned a corresponding
                                           user status.
3.30 / 04-2020




                                        How to check the status management
                                       1 Select the menu Master Data > Order > Status management.



                 A+W Business Purchasing                                                                       D-161
                 Electronic document exchange                                                                   Tutorial




                                           Fig. D-103   Status management


                                           If the user status 61/64 and 830/840 do not exist in full, enter the missing
                                           ones.
                                        2 Go to the menu Start > Save to save the changes.
                                           Then check whether all allocations are available and complete.
3.30 / 04-2020




                 D-162                                                                     A+W Business Purchasing
                 Tutorial                                                                Electronic document exchange




                                        How to check the status allocation
                                       1 Select the menu Master data > Order > Status allocation.




                                                                                                                       A

                                                                                                                       B

                                                                                                                       C




                                       A Status point                            C Allocated user status
                                       B Document type
                                       Fig. D-104    Status allocation


                                       2 Check whether status points 61, 64, 830 and 840 are allocated.
                                           If you select a status point in the Status allocation table, the status alloca-
                                           tion must at least show the user status (C).
                                           If this status points have not been allocated in full, catch up on the alloca-
                                           tions.
                                       3 Go to the menu Start > New to switch to the input mode.
                                       4 Select the appropriate entries in the fields Status point, Document type,
                                         and User status.
                                       5 Go to the menu Start > Save to save the changes.
                                           The data is saved.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-163
                 Electronic document exchange                                                                    Tutorial




                                        Set the data export via openTRANS
                                        You must define how data should be exchanged in the module Master data
                                        >B2B.


                                         How to define the export type for openTRANS
                                        1 Go to Master Data > B2B > Customer > Document export.
                                            The openTRANS document export dialog opens with the Selection tab.
                                        2 Go to the menu Start > Search to import the customers.
                                            The customers are listed in the Table tab.
                                        3 Select the customer (C) with whom documents shall be exchanged in open-
                                          TRANS format.
                                        4 Go to the Selection tab.
                                            •   If the information for the customer is correct, you can proceed to the
                                                next customer.
                                            •   If there is no information, you must enter it.

                                                                                   D                     E




                                        C


                                        B
                                        A




                                        A Export type by file or email           D Selection of document type
                                        B Transfer type                          E Email addresses for different document
                                        C Customer number                          types

                                        Fig. D-105    openTRANS document export
3.30 / 04-2020




                 D-164                                                                      A+W Business Purchasing
                 Tutorial                                                                 Electronic document exchange




                                       5 Go to the field Type (B) and select the entry Standard (openTRANS-
                                         based).
                                           With this setting, documents intended for this customer will automatically
                                           obtain the code for openTRANS exchange.
                                       6 Go to the field Export type (A) and define how the files shall be exchanged.
                                           •   Export to a file:
                                               This setting means that the data will be saved in a file. The fields for the
                                               target path are released. You can select a directory or enter the path
                                               manually.
                                           •   Export via email:
                                               This setting means that the data will be attached to an email. You have
                                               to check whether the email address has been defined correctly in the
                                               customer master data.
                                       7 Define whether order confirmations and/or invoices (D) shall be exported.
                                       8 If the data is sent by email, different email addresses (E) can be entered for
                                         order confirmations, invoices and/or delivery notifications.
                                       9 Go to the menu Start > Save to save the changes.
                                           The data is saved.
                                       10 Repeat the steps 3 to 9 for all customers with whom you exchange data.
                                           No additional settings are required for importing order confirmations and in-
                                           voices from your suppliers.
3.30 / 04-2020




                 A+W Business Purchasing                                                                            D-165
                 Electronic document exchange                                                                   Tutorial




                                          Check Partner Master Data
                                          The communication details must be correctly defined in supplier/customer
                                          master data to make sure that documents can be directly dispatched from
                                          A+W Business.


                                           How to check supplier/customer data
                                          1 Go to the menu Master data > Market partners > Supplier, customer > Sup-
                                            pliers, customers.




                    A




                   A Email address for document exchange
                   Fig. D-106   Partner data - address


                                          2 Check whether the email address of the supplier/customer is correct.
                                               If your supplier or customer has more than one email address, you can en-
                                               ter alternative email addresses in the document exchange settings.
                                                “Set the data export via openTRANS” on page D-164
                                          3 Go to the Order tab and check whether the external number has been en-
                                            tered.




                                                                                                                  A


                   A Specify external number
                   Fig. D-107   Partner data – order
3.30 / 04-2020




                 D-166                                                                       A+W Business Purchasing
                 Tutorial                                                                Electronic document exchange




                                           This number has the following meaning in the customer and supplier data:
                                           •   Supplier data:
                                               You can get the external customer number from your supplier. It has to
                                               be entered even if it is the same as your internal number.
                                           •   Customer data:
                                               In the customer master data, this field must show the number your cus-
                                               tomer uses for you as a supplier.
                                       4 Go to the menu Start > Save to save the changes.


                                       Import of electronic documents
                                       You can receive electronic documents in two different formats: as an open-
                                       TRANS file or as an XML file. Depending on the settings in your company,
                                       these files are saved in a certain directory on the server or are available as an
                                       email attachment.


                                        How to import an openTRANS document
                                       1 Open the directory with the sent files or the email to which the file had been
                                         attached.
                                           An openTRANS file has the suffix *.awotdis, *.awotres or *.awotinv.
                                       2 Double-click on the file to start the import.
                                           The data will be loaded and will appear in the dialogs for electronic price or
                                           invoice control.


                                        How to import an XML document
                                       1 Open the directory with the sent files or the email to which the file had been
                                         attached.
                                       2 Save the XML file on your computer.
                                       3 Select the file in the Explorer and open the context menu.
                                       4 Select the option Import as openTRANS document.
                                           The data will be loaded and will appear in the dialogs for electronic price or
                                           invoice control.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-167
                 Electronic document exchange                                                                            Tutorial




                                            Check the electronic document
                                            In documents imported from your suppliers, you can check the prices in both
                                            the order confirmation and in the invoice. Two dialogs are available for this pur-
                                            pose which are identical in structure and function:
                                            •   Electronic price control
                                            •   Electronic invoice control
                                            We are going to describe the steps now, using electronic invoice control as an
                                            example.


                                             How to check and accept an imported supplier's invoice
                                            1 Go to the menu Documents > P.O.s > Invoice > Electr. invoice control.




                 A




                 B




                 C




                                                        D    E                     F
                 A Options for the booking type                              D Information on discrepancies
                 B Restriction of the display                                E Filtering the shown documents
                 C Status of the selected document                           F Referenced documents
                 Fig. D-108   Electronic invoice control – Document import


                                            2 Restrict the view if too many documents are shown:
                                                •   Select the entry (B) to view Only open documents.
                                                •   Click on the (E) button and set the desired filters. From the Filter settings
                                                    dialog you can select several suppliers and accept them by pressing
                                                    [OK].
3.30 / 04-2020




                                                     Software Reference, “Filter settings” on page D-221
                                            3 Select one of the displayed invoices.



                 D-168                                                                             A+W Business Purchasing
                 Tutorial                                                                    Electronic document exchange




                                               The list P.O.s/partial deliveries (F) shows all purchase orders which belong
                                               to this invoice.
                                               The section Document status (C) tells you whether references are missing
                                               and/or if there are differences in price or quantity.
                                               •   If you are not going to accept price differences, select the option Do not
                                                   accept (A) and return the invoice to the sender.
                                                   The document will be marked as rejected and can be archived.
                                               •   The following steps explain how to correct differences.
                                               •   Establish the missing references.
                                                    “How to allocate items in an imported invoice” on page D-171
                                           4 Go to the Item overview tab if required in order to check the differences in
                                             the purchase prices of individual items.
                                               If there are divergences due to different rounding methods, you can accept
                                               them in general via the menu Options > Accept different amounts. In this
                                               case, you can choose the booking type Select or Reject.




                    Fig. D-109   Electronic invoice control – Item overview


                                               You cannot correct the item prices and quantities directly.
                                           5 Select the item you want to correct.
                                           6 Select the menu Functions > Open P.O. creation and correct the quantity.
                                               When you close a P.O. entry after correcting and saving the differences, the
3.30 / 04-2020




                                               new values will appear in the electronic invoice control.




                 A+W Business Purchasing                                                                              D-169
                 Electronic document exchange                                                                   Tutorial




                                           You do not need to correct price differences manually. You can just accept
                                           the document despite these differences. The program will make the neces-
                                           sary corrections automatically.
                                        7 When all errors have been corrected, select the option Accept.
                                        8 Go to the menu Start > Save to close the invoice control.
                                           The data is saved, and the status of the purchase order(s) changed. In-
                                           voice control cannot be run again for this document after that.


                                        Create a partial delivery from an electronic docu-
                                        ment
                                        You can create a partial delivery if the imported document includes only part
                                        of the P.O. items or of the ordered quantities.


                                         How to create a partial delivery for an imported supplier's invoice
                                        1 Go to the menu Documents > P.O.s > Invoice > Electr. invoice control.
                                        2 Select the invoice for which you want to create a partial delivery.
                                           You can create a partial delivery if the document status does not show any
                                           other errors except quantity differences. The option Create partial delivery
                                           is available only if this is the case.
                                           The process of creating missing references is described in:
                                            “How to allocate items in an imported invoice” on page D-171
                                        3 Select the option Create partial delivery.
                                        4 Go to the menu Start > Execute to generate the partial delivery.
                                           This creates a partial delivery with the invoice number, the delivered quan-
                                           tity and the prices from the imported document. The status of the original
                                           purchase order is changed accordingly.
                                           The original purchase order can be reallocated until all items have been de-
                                           livered in full and referenced.
3.30 / 04-2020




                 D-170                                                                      A+W Business Purchasing
                 Tutorial                                                                  Electronic document exchange




                                            Allocate items in electronic documents
                                            The item cannot be allocated if the references in the electronic document are
                                            not clear. You can make up for this allocation when checking the document.
                                            If an item is completely missing from the purchase order, e.g. an energy sur-
                                            charge, you have to enter this item in the corresponding purchase order first.
                                            You can open the purchase order from price/invoice control for this purpose.
                                            When you have entered and saved the item, proceed with invoice control.


                                             How to allocate items in an imported invoice
                                            1 Go to the menu Documents > P.O.s > Invoice > Electr. invoice control.
                                                The (Electr.) Invoice control dialog opens and the imported invoices are
                                                displayed.
                                            2 Mark the invoice for which you would like to allocate items.
                                            3 Go to the Item overview tab.
                                                You can add an item to the purchase order at a later stage by opening the
                                                document via the menu Functions > Open P.O. entry. When you have en-
                                                tered and saved the item, proceed with the invoice control, step 4.




                 Fig. D-110   Electronic invoice control – Item overview


                                            4 Select the item that could not be allocated and go to the menu Functions >
                                              Allocate items manually.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-171
                 Electronic document exchange                                                                              Tutorial




                 A                                                                                                   D




                 B
                 C

                 A Item from the invoice                                     C Save the allocation of the footer surcharge for all
                 B Retain allocation of the footer surcharge for the current   future imports
                   session                                                   D Item in the purchase order
                 Fig. D-111    Electronic invoice control – Allocate items


                                             5 From the left and the right list, select the items (A, D) you want to be allo-
                                               cated.
                                             6 Click on [OK] to save the allocation.
                                             7 Repeat the process until all items have been allocated.
                                                 If you have allocated footer surcharges/discounts you can use the check-
                                                 boxes (B, C) to define whether the allocation shall be maintained for this in-
                                                 voice and/or this supplier.
                                                 How you distribute a footer surcharge/discount to several purchase orders,
                                                 is described in:
                                                  “Allocate surcharges/discounts manually” on page D-172
                                             8 Click [End] if all allocations are correct.
                                                 All booking types are available in the Electr. invoice control dialog.
                                             9 Select the desired booking type, e.g. Accept.
                                             10 To start the activity, go to the menu Start > Execute.


                                             11 Go to the menu Start > Save to save the data.
                                                 The data is saved, and the status of the purchase order(s) changed.


                                             Allocate surcharges/discounts manually
                                             If an invoice shows just one footer surcharge/discount for several purchase or-
                                             ders, you can distribute it manually to the individual purchase orders and/or
3.30 / 04-2020




                                             P.O. items. The surcharge/discount will be calculated proportionately and
                                             saved in the purchase orders.




                 D-172                                                                               A+W Business Purchasing
                 Tutorial                                                              Electronic document exchange




                                        How to distribute the footer surcharge/discount to purchase orders
                                       1 Go to the menu Documents > P.O.s > Invoice > Electr. invoice control.
                                           The Electr. Invoice Control dialog opens and the imported invoices are dis-
                                           played.
                                       2 Select the invoice from which the footer surcharge/discount is to be distrib-
                                         uted.




                                           The list P.O.s/Partial deliveries shows all reference documents.
                                       3 Go to the menu Functions > Distribute footer surcharges/discounts to
                                         P.O.s.
                                       4 Hold down the <Ctrl> key and select all of the items which you would like
                                         the surcharge/discount to be distributed to.
                                       5 Click on [OK] to save the distribution.
                                           The data is saved in the respective purchase orders. The purchase prices
                                           in the purchase orders will be updated.
                                       6 Close the dialog using [End] and proceed with invoice control.
                                            “How to check and accept an imported supplier's invoice” on page D-168


                                       Additional information
                                        Software Reference, “Electronic price control” on page D-211
                                        Software Reference, “Electronic invoice control” on page D-254
                                        Software Reference, “Manual allocation of items” on page D-219
                                        Master Data, “Handling of Business Processes” on page B-413
                                        Master Data, “Company Data – Parameters” on page B-914
3.30 / 04-2020




                 A+W Business Purchasing                                                                         D-173
                 Electronic document exchange                                                                           Tutorial




                                        Data export/import (EDI)
                                        Objectives

                                        • Learning about the function of the external interface
                                        • Learning about the default settings for data exchange via the EDI interface


                                        Benefits

                                        • Thanks to data exchange via EDI interfaces, documents do not have to be entered
                                          manually.


                                        Please note:

                                        EDI                         EDI = Electronic Data exchange, electronic data
                                                                    exchange via ASCII file

                                        Interfaces                  Interfaces have to be implemented for customers and
                                                                    suppliers.

                                        Default settings            Company data:
                                                                    • Stock/PP/EDI tab
                                                                    B2B:
                                                                    • Customer, supplier
3.30 / 04-2020




                 D-174                                                                         A+W Business Purchasing
                 Tutorial                                                             Electronic document exchange




                                       Data exchange in ASC format
                                       The EDI interface serves for exchanging quotations, orders, purchase orders,
                                       and credit notes. The data is saved in an ASC file (ascii). Define the path for
                                       this file for each customer and each supplier.
                                       The data of the file to be transferred are automatically converted to ANSI for-
                                       mat by default, e.g. ä becomes ae.


                                       Check company data
                                       In company data (in the Stock/PP/EDI tab), you have to check the default set-
                                       tings which refer to the conversion.




                                       Fig. D-112   Company data – Stock/PP/EDI tab


                                       OEM/ANSI conversion should be disabled only if the interface you are using
                                       requires this specifically.


                                       Check the settings
                                       If you exchange orders and purchase orders in the ASC format with your sup-
                                       pliers/customers, you must set the parameters for each individual supplier/
                                       customer.


                                        How to check the settings for data export via EDI
                                       1 Select the menu Master data > B2B > Supplier > Supplier.
                                           For data import via EDI, select Master data > B2B > Customer > Customer.
                                           The following steps apply likewise.
                                       2 To start the search, go to the menu Start > Search.
                                           The list of matches is shown on the Table tab.
                                       3 Select the supplier who shall receive purchase orders via the EDI interface.
3.30 / 04-2020




                 A+W Business Purchasing                                                                       D-175
                 Electronic document exchange                                                                          Tutorial




                                              4 Go to the Selection tab.




                                                                                                             B




                                                                                                             C
                                                                                                             D

                 A




                 A Interface type                                        C Specifications for the log file
                 B Specifications for the target file                    D Path for the backup file
                 Fig. D-113    Interface management


                                              5 Enter the directories and file names (B) of the export file and the backup file
                                                (D).
                                              6 Select the interface version (A) your system uses.
                                                  If you also want to transfer order confirmations and invoices electronically
                                                  (openTRANS-Format) you have to choose the version you have been us-
                                                  ing so far for transferring the data. The version is defined when
                                                  A+W Business is installed.
3.30 / 04-2020




                 D-176                                                                              A+W Business Purchasing
                 Tutorial                                                              Electronic document exchange




                                       Fig. D-114   Settings for EDI document export


                                       7 Go to the menu Start > Save to save the data.
                                           The data is saved.
                                       8 Go to the Parameters tab.
3.30 / 04-2020




                 A+W Business Purchasing                                                                    D-177
                 Electronic document exchange                                                                               Tutorial




                                                                                                           A
                                                                                                           B




                                                                                                                               A
                                                                                                                               B




                                                                                                                               C



                 A Compulsory referencing                                 C Parameters for EDI import of orders (only for
                 B Access lock and time of lock                             customers)

                 Fig. D-115   Parameter for EDI exchange


                                           9 Mark the checkboxes for export:
                                                  •   Compulsory referencing (A):
                                                      If an item without a reference is transferred to an (external) product, this
                                                      item can be ignored. An error report will be made in the logbook in this
                                                      case.
                                                      If this checkbox is not marked, the product number is imported from the
                                                      master data to the interface file. This is useful, for example, if the send-
                                                      ing and the receiving system use the same product master data. In this
                                                      case it is not necessary to enter data in the reference tables
                                                  •   Locking active and Maximum lock time (B):
                                                      With this setting, you prevent that only one program can access the
                                                      same interface during the specified period.
                                                  •   Import from customer orders (C):
                                                      When you set up data for customers, you can also define extra settings
                                                      for import.
3.30 / 04-2020




                                           10 Repeat the steps for all suppliers with whom you exchange data via EDI.




                 D-178                                                                              A+W Business Purchasing
                 Tutorial                                                                 Electronic document exchange




                                       11 Now go to the menu Master data > B2B > Customer > Customer and repeat
                                          the steps for all customers with whom you exchange data via EDI.


                                       Exporting of purchase orders
                                       When you export purchase orders, the data is saved in an ASC file. This file is
                                       then saved in a defined directory. The file is then transferred to the supplier via
                                       the EDI interface.


                                        How to export a purchase order
                                       1 Go to the menu Documents > P.O.s > Export.
                                           The Export dialog is opened and the purchase orders in the current Num-
                                           ber Manager are shown.




                                           Fig. D-116   Export of purchase orders


                                       2 To start the export, go to the menu Start > Execute.
                                           Export begins. The progress report shows which purchase order is being
                                           transferred.
                                       3 Go to the Pool tab to check the export status.
                                           You can update the view by means of [Queries].


                                       Additional information
                                        Sales, “Document Import” on page C-330
                                        Master Data, “Interface Service” on page B-995
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-179
                 Electronic document exchange                    Tutorial
3.30 / 04-2020




                 D-180                          A+W Business Purchasing
Purchasing                  D

             Software Reference




              A+W Business
                 Software Reference                                                                          Overview




                                       Overview
                                       In document management you can enter and edit all documents required for
                                       purchasing, e.g. inquiries about shipments and orders. You can also enter re-
                                       ceipt of goods, check and correct delivery dates and verify suppliers' invoices.
                                       The Software Reference provides information on the following subjects:
                                       •   Inquiry (menu)
                                       •   Purchase order (menu)
                                       •   Order confirmation
                                       •   Receipt of goods
                                       •   Invoice
                                       •   Invoicing of basic glass
                                       The following dialogs are the same for all document types and are therefore
                                       explained just once, in the Sales section:
                                       •   Transfer to financial accounting
                                       •   Transfer to archives
                                       •   Search

                                           Dialogs are accessible from different points
                                           Please note that many of the functions and overviews in the field of pur-
                                           chasing can be accessed from different dialogs in A+W Business. The cor-
                                           responding dialogs will only be described once in this document.

                                           Dialogs which are also required for sales are described in detail in the
                                           Sales section.


                                       Dialog descriptions in the Sales section
                                        Software Reference, “Document Management” on page C-359
                                        Software Reference, “Overviews and References concerning Header Data” on
                                         page C-454
                                        Software Reference, “Item Data” on page C-385
                                        Software Reference, “Overviews and References concerning Items” on page C-503
                                        Software Reference, “Number Manager” on page C-540
                                        Software Reference, “Printing” on page C-548
                                        Software Reference, “Transfer to Archives” on page C-594
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-183
                 Inquiry (menu)                                                                Software Reference




                                  Inquiry (menu)
                                  Documents > Inquiry
                                  You can access the following program items via the Inquiry menu:
                                  •   NM inquiry:
                                      The Number Manager function is the same for all documents. It is de-
                                      scribed in detail with the orders.
                                       Sales, “Number Manager” on page C-540
                                  •   Inquiry:
                                      Document input is the same for all document types. It is described in detail
                                      with the orders.
                                       Sales, “Document Management” on page C-359
                                       Sales, “Item Data” on page C-385
                                  •   Print inquiry:
                                      Form and label print is the same for all documents. It is described in detail
                                      with the orders.
                                       Sales, “Printing” on page C-548
                                  •   Journal:
                                      Printing of journals is the same for all documents. It is described in detail
                                      with the orders.
                                       Sales, “Journal” on page C-632
                                  •   Transfer to archives:
                                      Transfer to archives is the same for all documents. It is described in detail
                                      with the orders.
                                       Sales, “Transfer to Archives” on page C-594
                                  •   Search:
                                      Search is identical for all documents. It described in detail with the orders.
                                       Sales, “Search Document” on page C-455
3.30 / 04-2020




                 D-184                                                                 A+W Business Purchasing
                 Software Reference                                                                        Inquiry (menu)




                                          Inquiry (document management)
                                          Documents > Inquiry > Inquiry




                 Fig. D-117   Document management – Inquiry


                                          This dialog is used to enter and edit inquiries for your suppliers. Inquiries can
                                          either be created manually or they are created during the P.O. transfer, provid-
                                          ed the option Inquire immediately is selected in the order pool.
                                           Tutorial, “Inquiry” on page D-108
                                           Sales, “P.O. Transfer – P.O. Numbers” on page C-568
                                          The fields in the Document management dialog and at item entry are the same
                                          for all document types. They are described in detail with the orders:
                                           Sales, “Document – Header Data” on page C-365
                                           Sales, “Document – Items” on page C-394
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-185
                 Purchase order (menu)                                                                Software Reference




                                         Purchase order (menu)
                                         Documents > Purchase order
                                         You can access the following program items via the Purchase order menu:
                                         •   NM purchase order:
                                             The number manager function is the same for all documents. It is described
                                             in detail with the orders.
                                              Sales, “Number Manager” on page C-540
                                         •   Purchase order:
                                             Document input is the same for all document types. It is described in detail
                                             with the orders.
                                              Sales, “Document Management” on page C-359
                                              Sales, “Item Data” on page C-385
                                         •   Partial delivery:
                                             Creation of partial deliveries is the same for all document types. It is de-
                                             scribed in detail with the orders.
                                              Verkauf, “Teillieferungen” auf Seite C-603
                                         •   Replenishment order:
                                             Use this dialog to re-order, complain, invoice purchased parts that have
                                             been reported broken or to reduce the order quantity.
                                              “Replenishment Order” on page D-189
                                         •   Print purchase order:
                                             Form and label print is the same for all documents. It is described in detail
                                             with the orders.
                                              Sales, “Printing” on page C-548
                                         •   Export (EDI):
                                             You can use this dialog to export purchase orders via the EDI interface.
                                              “Export (EDI)” on page D-191
                                         •   Journal:
                                             Printing of journals is the same for all documents. It is described in detail
                                             with the orders.
                                              Sales, “Journal” on page C-632
                                         •   OC supplier:
                                             This dialog lets you create and check your suppliers' order confirmations
                                             (OC).
                                              “OC supplier” on page D-195
3.30 / 04-2020




                 D-186                                                                        A+W Business Purchasing
                 Software Reference                                                             Purchase order (menu)




                                       •   Order confirmation:
                                           – Price control:
                                              Use this dialog to check the order confirmations of your suppliers and
                                              correct prices if required.
                                               “Order confirmation” on page D-202
                                           – Electr. price control:
                                             You can use this dialog to check the prices and references in electroni-
                                             cally transferred order confirmations.
                                               “Order confirmation” on page D-202
                                           – Reminder:
                                             You can use this dialog to create reminders for outstanding deliveries.
                                               “Reminder” on page D-223
                                       •   Receipt of goods
                                           – Receipt of goods:
                                             Use this dialog to create receipts of goods for purchase orders and
                                             stock purchase orders.
                                               “Receipt of goods” on page D-225
                                           – Incoming control:
                                             Use this dialog to check whether the receipts of goods are complete.
                                               “Inspection of goods received” on page D-239
                                       •   Invoice:
                                           – Invoice control:
                                              Use this dialog to check the invoices of your suppliers and correct prices
                                              if required.
                                               “Invoice control – Purchase orders” on page D-246
                                           – Electr. invoice control:
                                             Use this dialog to check the prices and references in electronically
                                             transferred invoices.
                                               “Electronic invoice control” on page D-254
                                       •   Transfer to FinAc:
                                           Transfer to financial accounting is the same for all documents. It is ex-
                                           plained using an order as an example.
                                            Sales, “Transfer to FinAcc” on page C-588
                                       •   Transfer to archive:
                                           Transfer to archives is the same for all documents. It is described in detail
                                           with the orders.
                                            Sales, “Transfer to Archives” on page C-594
                                       •   Search:
                                           Search is identical for all documents. It described in detail with the orders.
                                            Sales, “Search Document” on page C-455
                                       •   Single glass settlement:
                                           Use this to manage internal profit center calculations. Basic glass calcula-
                                           tion is only released for specific customers.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-187
                 Purchase order (menu)                                                               Software Reference




                                          Purchase order (document manage-
                                          ment)
                                          Documents > Purchase order > Purchase order




                 Fig. D-118   Document management - P.O.


                                          This dialog is used to enter and edit purchase orders.
                                           Tutorial, “Manual purchase order” on page D-77
                                          The Document management dialog and the corresponding menus are the
                                          same for all document types. We are going to describe it in connection with an
                                          Order.
                                           Sales, “Document – Header Data” on page C-365
                                           Sales, “Document – Items” on page C-394

                                             Enter purchase order
                                             You can create purchase orders in the same way as an order. Make sure
                                             to select the correct document type:
3.30 / 04-2020




                                             •   Stock P.O.:
                                                 This setting lets you order stock articles. The delivered items are
                                                 booked into Stock automatically upon receipt of goods.


                 D-188                                                                       A+W Business Purchasing
                 Software Reference                                                                Purchase order (menu)




                                                  You must select the stock purchase orders in this purchase order with
                                                  the stock search <F3>. The Stock P.O. type is shown in the Type field.
                                              •   <n.s.>:
                                                  Use this setting to order all products which are not booked through
                                                  stock.
                                               Sales, “Type” on page C-369
                                               Tutorial, “Entering an independent P.O.” on page D-79
                                              If you enter a stock P.O. with products which are not recorded as stock ar-
                                              ticles, the receipt of goods for these products cannot be booked into stock
                                              automatically. A message to that effect will be issued when entering the
                                              purchase order.

                                              Items without stock codes
                                              If you enter stock P.O.s with items which are not recorded as stock items,
                                              they will not be displayed at receipt of goods. You can however activate the
                                              corresponding option in the company data.

                                               Master Data, “Show items w/o stock code at receipt of goods on stock” on
                                                page B-933



                                          Replenishment Order
                                          Document > P.O. > Replenishment Order




                 Fig. D-119   Replenishment
3.30 / 04-2020




                                          Use this dialog you manage orders with ordered parts that are reported as bro-
                                          ken from production. You can reorder the ordered parts, make a complaint, in-
                                          voice them or reduce the order quantity.


                 A+W Business Purchasing                                                                             D-189
                 Purchase order (menu)                                                               Software Reference




                                         Selection

                                         Order from, to Restrict the search to an order or a sequence of orders.

                                         Delivery date from, to Restrict the search to a specific delivery date or set of
                                         delivery dates.

                                         Documents
                                         The list shows all orders with breakage matching the search criteria.
                                         •   Order:
                                             Order number.
                                         •   Order item:
                                             Item number from the order.
                                         •   Delivery date:
                                             Delivery date shown in the order header
                                         •   P.O.:
                                             Purchase order number.
                                         •   Purchase Item
                                             Item number from the purchase order.
                                         •   Supplier:
                                             Name of the supplier from the purchase order.
                                         •   Product:
                                             Number and name of the product.
                                         •   Order quantity:
                                             Quantity from the order.
                                         •   Purchase qty.:
                                             Quantity that is ordered.
                                         •   Breakage Quantity:
                                             Quantity reported broken.
                                         •   Feedback date:
                                             Date of breakage report.
                                         •   Action:
                                             Selection of the action:
                                             – Replenishment order:
                                                 The purchase order is created and moved to the selected Number Man-
                                                 ager.
                                             – Complaint:
                                                 A complaint is created for the ordered parts. If this option is selected,
                                                 the reason and cause of the complaint can be specified.
                                             – Booking in terms of value:
                                                 The purchase order is created with a negative item quantity. Thus, the
                                                 broken quantity is booked out and the value of the broken quantity is off-
                                                 set against the value of the order.
                                             – Reduce order quantity:
                                                 The original order is reduced by the broken quantity. This excludes the
                                                 possibility of reordering.
3.30 / 04-2020




                                         •   Complaint reason:
                                             The complaint reason is specified only if Complaint is selected as the ac-
                                             tion.


                 D-190                                                                        A+W Business Purchasing
                 Software Reference                                                           Purchase order (menu)




                                       •   Complaint cause:
                                           The complaint cause is specified only if Complaint is selected as the ac-
                                           tion..
                                       •   Comment:
                                           You can enter comments, e. g. agreements in connection with this replen-
                                           ishment or complaint.
                                       •   Label:
                                           Number of the label from production. The number can not be changed.

                                       Goal

                                       Number Manager Number Manager to which the replenishment orders shall
                                       be moved.


                                       Export (EDI)
                                       Documents > Purchase order > Export
                                       Export (EDI):
                                       You can use this dialog to export P.O.s in order to transfer them to the respec-
                                       tive supplier via the EDI interface.
                                        Tutorial, “Data export/import (EDI)” on page D-174

                                           Prerequisite
                                           For this purpose, the parameters for the interface have to be defined for
                                           each individual supplier/customer with whom you would like to exchange
                                           documents via the external interface. These parameters have to be config-
                                           ured in the menu Master data > B2B.

                                       This chapter provides information on the following subjects:
                                       •   “Functions menu” on page D-192
                                       •   “Export – export” on page D-193
                                       •   “Export – pool” on page D-194
3.30 / 04-2020




                 A+W Business Purchasing                                                                       D-191
                 Purchase order (menu)                                                            Software Reference




                                         Functions menu
                                         Documents > P.O. > Export > Functions menu
                                         Use this menu to open other dialogs without closing the Export dialog.

                                         Edit group
                                         •   Copy:
                                             Opens the Copy number manager dialog to create a new number manager.
                                              Sales, “Copy Number Manager” on page C-545
                                         •   Status change:
                                             Opens the Status change dialog to change the status manually and to
                                             amend the Number Manager.
                                              Sales, “Status Change” on page C-479

                                         Documents group
                                         •   Show document:
                                             Opens the Document view dialog and provides a print preview.
                                              Sales, “Complaint” on page C-510
                                         •   History:
                                             Opens a list of status changes for the selected document.
                                              Sales, “History” on page C-478
                                         •   Document data:
                                             Opens the Document data dialog to correct the dates and the status if nec-
                                             essary.
                                              Sales, “Document Data” on page C-646
                                         •   Document entry:
                                             Opens the Document management dialog to create or change documents.
                                              Sales, “Document Management” on page C-359

                                         Document copy group
                                         •   Copy documents:
                                             Opens the Copy documents dialog to copy a document to the same or an-
                                             other document type.
                                              Sales, “Copy Documents” on page C-461
                                         •   Partial delivery:
                                             Opens the Copy documents dialog to enter a partial delivery.
                                              Sales, “Copy Documents” on page C-461
3.30 / 04-2020




                 D-192                                                                      A+W Business Purchasing
                 Software Reference                                                              Purchase order (menu)




                                       Export – export
                                       Documents > P.O.> Export > Export tab




                                       Fig. D-120   Export – Export


                                       This tab is used to export purchase orders. The data is saved in an ASC file.
                                       This file is then saved in a defined directory. The file is then transferred to the
                                       supplier via the EDI interface.
                                       The settings for the export are defined by supplier in the module Master data
                                       > B2B.
                                        Tutorial, “Data export/import (EDI)” on page D-174

                                       Select by

                                       Employee Name of the employee logged in to A+W Business.

                                       Number manager Choose the Number Manager that the Export dialog is to
                                       access.

                                       [Logbook] Button that opens the system logbook.

                                       Documents
                                       A list of all documents included in the selected Number Manager. They shall
                                       be sent to the supplier by way of interfaces.
                                       •   Number:
                                           Number of the document
3.30 / 04-2020




                                       •   Cust./suppl. number:
                                           Customer or supplier number
                                       •   Customer/supplier:
                                           Customer or supplier name


                 A+W Business Purchasing                                                                           D-193
                 Purchase order (menu)                                                               Software Reference




                                         •   Status:
                                             Status of the document
                                         •   Input date:
                                             Date on which the document was entered
                                         •   Delivery date:
                                             Delivery date
                                         •   OC date:
                                             Date of order confirmation
                                         •   Lock code:
                                             Code indicating whether the document is locked – the lock code is rarely
                                             set for purchase orders


                                         Export – pool
                                         Documents > P.O. > Export > Pool tab




                                         Fig. D-121   Export – Pool


                                         Use this tab to transfer the listed purchase orders via the EDI interface (elec-
                                         tronically).

                                         Transfer pool
                                         The list shows all purchase orders to be transferred electronically.

                                         [Delete] This button is only enabled if an error has occurred during the trans-
                                         fer. This button allows you to delete an entry from the transfer pool.

                                         [Enable] This button is only enabled if an error has occurred during the trans-
3.30 / 04-2020




                                         fer. You can correct the data and resubmit it for transfer if an error was found.
                                         You can start the transfer process with the [Enable] button.




                 D-194                                                                       A+W Business Purchasing
                 Software Reference                                                            Purchase order (menu)




                                       [Queries] Use this button to update the display to check the transfer status.


                                       OC supplier
                                       Documents > P.O.> OC supplier
                                       This dialog allows you to enter the order confirmation which your supplier sent
                                       for a purchase order. You can also enter the corresponding receipt of goods
                                       and/or check the dates for purchase orders and deliveries and correct them if
                                       required.
                                       This chapter provides information on the following subjects:
                                       •   “Options menu” on page D-195
                                       •   “OC supplier – documents” on page D-196
                                       •   “OC supplier – items” on page D-200
                                       •   “OC Supplier – change delivery dates” on page D-201


                                       Options menu
                                       Documents > P.O.> OC supplier > Options menu
                                       This menu allows you to define the default settings for the dialog. The options
                                       can be enabled or disabled. The settings will not be reset when you close the
                                       dialog.
                                       The following entries are displayed:
                                       •   Stock booking date = Delivery date:
                                           The delivery date from the P.O. is automatically taken as the booking date.
                                           If this option is disabled, the current date will be used by default.
                                       •   Check OC number:
                                           This setting outputs a message if the number of the order confirmation has
                                           not been entered by the supplier.
                                       •   ID number assignment:
                                           This setting is only needed for the receipt of boxes and stockplates.
                                           – Manually:
                                                Use this option to assign the ID manually. The checkbox Assign ID(s) in
                                                the Options area is released.
                                               “Options” on page D-196
                                           – Automatic:
                                             Use this option for automatic assignment of IDs. A default can be de-
                                             fined. If this option is disabled, you have to enter the ID by hand.
                                           – Settings:
                                             Opens the Settings dialog which lets you enter the settings for the auto-
                                             matic assignment of IDs.
                                               “Settings (ID)” on page D-238
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-195
                 Purchase order (menu)                                                                 Software Reference




                                          OC supplier – documents
                                          Documents > P.O.> OC Supplier > Documents tab




                 Fig. D-122   OC supplier – Documents


                                          Use this tab to create an order confirmation from the supplier and/or the cor-
                                          responding receipt of goods. You can also check the dates for purchase orders
                                          and deliveries and correct them if required.
                                          All the data entered on this tab also applies to all items shown on the P.O. list.
                                          Go tothe Items tab to enter data for individual items.
                                           Tutorial, “Supplier's OC” on page D-85

                                          Documents
                                          Select the option to define which document type you would like to create the
                                          order confirmation for. Use the magnifier to search for the P.O. or order.
                                          •   P.O. number:
                                              Selection of a purchase order. The purchase order input field is released.
                                          •   Order number:
                                              Selection of a customer order used to generate a purchase order. The or-
                                              der number input field is released.

                                          Options

                                          Fill order NM When booking an order confirmation from your supplier and –
                                          if applicable – also the receipt of goods for the P.O., the corresponding (cus-
3.30 / 04-2020




                                          tomer) order can be automatically moved to another Number Manager.
                                          ☐The reference (customer) order is not moved to another Number Manager.
                                          ☑The reference (customer) order is moved to the selected Number Manager.


                 D-196                                                                         A+W Business Purchasing
                 Software Reference                                                             Purchase order (menu)




                                       Fill P.O. NM When you book an order confirmation from your supplier and –
                                       if applicable – the receipt of goods for this P.O., the corresponding P.O. can be
                                       automatically moved to another Number Manager.
                                       ☐The purchase order is not moved to another Number Manager.
                                       ☑The purchase order is moved to the selected Number Manager.

                                       Book goods received You can enter the entire receipt of goods if your sup-
                                       plier has delivered the goods together with the OC.
                                       ☐ Receipt of goods is not booked.
                                       ☑ Receipt of goods is booked as complete. If the delivery contains boxes, you
                                       have to check the settings for the box ID.

                                           Enter partial receipt of goods
                                           The complete receipt of goods for individual items can be entered on the
                                           Items tab. To enter partial receipt of goods for an item, go to the Receipt of
                                           goods dialog.

                                            “Receipt of goods (dialog)” on page D-225

                                       Assign ID number(s) This checkbox is enabled or disabled by means of the
                                       ID number assignment setting. IDs are usually assigned to boxes. You can set
                                       a default ID for booking the receipt of goods on stock.
                                       The checkbox is enabled only if you have selected Manually in the Options
                                       menu.
                                       ☐ The checkbox is disabled if you have selected Manual in the Options menu.
                                       The ID must be entered manually.
                                       ☑ The checkbox is active if you have selected Automatic in the Options menu.
                                        “Settings (ID)” on page D-238

                                       P.O. data

                                       Supplier The supplier name from the P.O or customer order.

                                       Status Status of the selected document.

                                       Total quantity Total quantity of all items in the selected document.

                                       Confirmed delivery date Date of delivery by the supplier. The date is adopt-
                                       ed from the P.O. You can change it if required. The changed date will be saved
                                       in the P.O. and – if applicable – in the reference order.
                                        “OC Supplier – change delivery dates” on page D-201

                                       Partial delivery date Delivery date specified in the supplier's order confir-
                                       mation.

                                       OC number Order confirmation number provided by the supplier. This num-
                                       ber is entered for all items shown on the P.O. list.
                                       If the order confirmation number is to apply to one item only, go to the Items
3.30 / 04-2020




                                       tab.
                                        “OC supplier – items” on page D-200




                 A+W Business Purchasing                                                                          D-197
                 Purchase order (menu)                                                               Software Reference




                                         Order data
                                         The data in this section is displayed only if an order or a P.O. for an order has
                                         been selected. The fields are empty for a stock P.O. (without an order).

                                         Customer Name of the customer for whom the P.O. was created.

                                         Status Status of the customer order.

                                         Total quantity Total quantity of all items in the customer order.

                                         Delivery date at the customer Delivery date at the customer. The date is
                                         adopted from the order.You can change it if required.The changed data will be
                                         saved in the P.O. and – if applicable – in the reference order.
                                          Sales, “Delivery Date Check (Delivery Date Control)” on page C-489
                                          Tutorial, “Change delivery dates, notify customer” on page D-100
                                          “OC Supplier – change delivery dates” on page D-201

                                         Planned Originally planned delivery date at the customer.

                                         Shipping date Date on which the shipment is dispatched to the customer.
                                         This date is usually the same as the delivery date. The shipping date must be
                                         earlier than the delivery date only if the delivery takes longer than one day.

                                         Route Selection of the route by which the goods will be shipped to the cus-
                                         tomer.
3.30 / 04-2020




                 D-198                                                                       A+W Business Purchasing
                 Software Reference                                                            Purchase order (menu)




                                       P.O. items
                                       List of all items of this P.O. If the purchase order was created from a customer
                                       order, the purchased items can be the items of the referenced order at the
                                       same time.
                                       •   Item:
                                           P.O. item number. For a customer order, this can also be the item number
                                           from the order.
                                       •   Product description:
                                           Number and description of the ordered item.
                                       •   Qty:
                                           Quantity of the ordered item.
                                       •   Width / Height:
                                           Dimensions of the ordered item.
                                       •   Supplier OC:
                                           Number of the supplier's order confirmation. If you have entered the order
                                           confirmation number for the entire P.O., the same number is shown for all
                                           items.
                                       •   Partial delivery data:
                                           Delivery date for partial deliveries.
                                       •   Pr./PU:
                                           PU price per price unit of the ordered item.
                                       •   Pr./PU total:
                                           Total price per price unit of the ordered item.
                                       •   List/key:
                                           Price list and key which apply for the underlying purchase price (PU).
                                       •   Disc.:
                                           Discount applied to the PP.
                                       •   Net/item:
                                           Item price without a discount and/or surcharges.
                                       •   Net/item total:
                                           Price of all items of purchase order without a discount and/or surcharges.
                                       •   Price unit qty.:
                                           Quantity in displayed prise unit.
                                       •   Price unit:
                                           Price unit that applies to the displayed price.
                                       •   Unit price:
                                           Unit price for the selected item including all components. It is calculated
                                           based on the price unit, surcharges and discounts.
                                       •   Order:
                                           Order number.
                                       •   Description:
                                           Product name from the referenced order. You can enter a different supplier
                                           description in the purchase order.
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-199
                 Purchase order (menu)                                                                  Software Reference




                                           OC supplier – items
                                           Documents > P.O. > OC supplier > Items tab




                 Fig. D-123   OC supplier – Items


                                           You can enter the same data on this tab as on the Documents tab. The entered
                                           data only refer to the defined items.
                                           These fields in this tab are described in detail in connection with the Docu-
                                           ments tab.
                                            “OC supplier – documents” on page D-196

                                           Items from – to Item numbers for which you want to book an OC number
                                           and/or receipt of goods. This will indicate the items as delivered in full. The or-
                                           der number appears on the P.O. list only for the entered items.
                                           Go to the Receipt of goods dialog to book partial delivery/receipt of goods for
                                           individual items.
                                            Tutorial, “Enter receipt of goods” on page D-125
                                            “Receipt of goods (dialog)” on page D-225
3.30 / 04-2020




                 D-200                                                                          A+W Business Purchasing
                 Software Reference                                                               Purchase order (menu)




                                           OC Supplier – change delivery dates
                                           Documents > P.O.> OC supplier > Change delivery dates tab




                 Fig. D-124   OC supplier – Change delivery dates


                                           In this tab, you can change the supplier's delivery dates.
                                           The fields in this tab are described in detail in connection with the Documents
                                           tab.
                                            “OC supplier – documents” on page D-196
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-201
                 Order confirmation                                                             Software Reference




                                          Order confirmation
                                      Documents > P.O. > Order confirmation > Price control
                                      You can check supplier prices before accepting an order confirmation. If a sup-
                                      plier fails to adhere to the agreed dates, you can send a reminder.
                                      This chapter provides information on the following subjects:
                                      •   “Price control” on page D-203
                                      •   “Electronic price control” on page D-211
                                      •   “Selection (prod. no. for balancing item)” on page D-218
                                      •   “Settings for Xternal” on page D-219
                                      •   “Manual allocation of items” on page D-219
                                      •   “Distribution of footer surcharges/discounts” on page D-220
                                      •   “Filter settings” on page D-221
                                      •   “Reminder” on page D-223
3.30 / 04-2020




                 D-202                                                                  A+W Business Purchasing
                 Software Reference                                                                  Order confirmation




                                       Price control
                                       Documents > P.O. > Order confirmation > Price control
                                       You can check the prices confirmed by your suppliers and correct them if re-
                                       quired.
                                        Tutorial, “Enter order confirmation and check prices” on page D-91

                                           Collective invoice
                                           If your supplier pools several orders in a collective order, this can be
                                           checked and accepted only if the same VAT rate and currency have been
                                           defined in all purchase orders.

                                       This chapter provides information on the following subjects:
                                       •   “Functions menu” on page D-203
                                       •   “Options menu” on page D-204
                                       •   “Price control – purchase orders” on page D-205
                                       •   “Price control – item” on page D-208
                                       •   “Price control – BOM” on page D-210


                                       Functions menu
                                       Documents > P.O.> Order confirmation > Price control > Functions menu
                                       This menu can be used to open other dialogs without closing Price control.
                                       The following entries are displayed:
                                       •   Create partial delivery:
                                           Opens the Copy documents dialog to enter a partial delivery.
                                            Sales, “Copy Documents” on page C-461
                                       •   Enter shipping fee:
                                           The shipping fee is automatically entered as an item on the Items tab. If the
                                           purchase order already contains a shipping fee, the option is omitted.
                                       •   Open P.O. input:
                                           All listed P.O.s are locked for editing (by other users) during price control.
                                           This function allows you to open the Document management dialog in or-
                                           der to edit one of the displayed purchase orders. Changed values are ad-
                                           opted for the price control.
                                            Sales, “Document – Header Data” on page C-365
                                       •   Update order data:
                                           This function directly saves the changed values in the purchase order.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-203
                 Order confirmation                                                                 Software Reference




                                      Options menu
                                      Documents > P.O. > Order confirmation > Price control > Options menu
                                      This menu allows you to define the default settings for the dialog. The options
                                      can be enabled or disabled. The settings will not be reset when you close the
                                      dialog.

                                      Standard group
                                      •   Net VAT:
                                          Net amounts are shown incl. VAT.
                                      •   Gross VAT:
                                          Gross amounts are shown incl. VAT.
                                      •   Net:
                                          Net amounts are shown without VAT.

                                      Behavior group
                                      •   Quick input:
                                          This option means that when you enter a P.O. number, the cursor directly
                                          goes to the Order total field. This setting is saved in relation to the user.
                                      •   Invoice date restriction:
                                          Opens the Invoice date dialog in order to set the deviation in days.
                                           “Invoice date” on page D-253
                                      •   Fill target NM:
                                          Releases the fields in the Target Number Manager section to select a user
                                          and the corresponding Number Manager.

                                      Settings group
                                      •   Freeze discount:
                                          This option fixes the discount. You should enable this option if you have de-
                                          fined new discounts but want to keep the old discounts for your old pur-
                                          chase orders. In this case, prices will not be recalculated after price control.
                                      •   No correction of order costs in statistics:
                                          The purchase prices are corrected in the reference order only if the order
                                          still exists in the main database, and has not yet been transferred to statis-
                                          tics.
                                      •   Notification for exceeded delivery date:
                                          A message is shown if the confirmed delivery date is later than the desired
                                          delivery date of the P.O.
3.30 / 04-2020




                 D-204                                                                      A+W Business Purchasing
                 Software Reference                                                                      Order confirmation




                                           Xternal group
                                           •   Create Xternal XML file:
                                               This option is active only for defined customers.
                                           •   Settings for Xternal:
                                               Opens the Settings dialog in order to set XML export defaults. This function
                                               is available only if the Create Xternal XML file option is active.


                                           Price control – purchase orders
                                           Documents > P.O. > Order confirmation > Price control > P.O.s tab




                 Fig. D-125   Price control – Purchase orders


                                           Choose a P.O. on this tab to check the prices in the corresponding order con-
                                           firmation. The data will be displayed only after the P.O. number fields or the
                                           Number Manager fields in the section P.O. data have been filled, and the cur-
                                           sor is moved to another field.
                                            Tutorial, “Enter order confirmation and check prices” on page D-91

                                           OC data

                                           OC number Mandatory field. You have to enter the supplier's order confir-
                                           mation number.

                                           Confirmed delivery date Mandatory field. Date shown on the order confir-
3.30 / 04-2020




                                           mation. You can select the date from the calendar or enter it manually.




                 A+W Business Purchasing                                                                            D-205
                 Order confirmation                                                                 Software Reference




                                      P.O. data
                                      Selecting the option will release the corresponding fields in order to select the
                                      purchase order(s) for which you want to check the prices.
                                      •   P.O. number, to:
                                          If you enter the same number in both fields, just this purchase order will be
                                          imported. If several purchase orders belong to an order confirmation, you
                                          can enter several P.O. numbers and add them to the view. For this, all P.O.s
                                          must belong to the same supplier and have the same VAT rate.
                                      •   Number manager:
                                          When you have selected a Number Manager, the P.O.s section shows all
                                          purchase orders of this Number Manager.

                                      Totals
                                      You can switch to another tab only after you have entered the amount from the
                                      supplier's order confirmation and have confirmed it with [Execute].

                                      OC Total/VAT Mandatory field. Total amount of the confirmed delivery and
                                      VAT. The VAT amount will not be displayed if the Net mode has been selected.

                                      Mode Your selection here will determine whether the VAT is shown or not.
                                      You can set the default mode in the menu Options > Standard group.
                                      • Net incl. VAT:
                                         The total amount will be evaluated as net; the VAT amount is shown.
                                      • Gross with VAT:
                                         The total amount will be evaluated as gross; the VAT amount is shown.
                                      • Net:
                                         The total amount is evaluated as net; the VAT amount is not shown.

                                      Currency Selection of the currency if you are working with several curren-
                                      cies.
                                      The combo box offers a selection of all currencies defined in the master data.
                                      If you select a currency other than Euro, the overview will list the order and
                                      VAT amounts in the selected currency as well.
                                       Master Data, “Currencies” on page B-450

                                      Rate If you are using more than one currency, the exchange rate defined in
                                      the master data is shown here. It can be changed. If you are using only Euro
                                      as a currency, the entry in this field must be 1.

                                          Fix exchange rate
                                          You can define a different exchange rate for each purchase order. This will
                                          be used automatically for price control calculations. You can only change it
                                          if it has not been fixed in the purchase order.

                                           Sales, “Rate fixed for invoicing” on page C-379

                                      Target number manager
3.30 / 04-2020




                                      These two fields are released only if the option Fill target NM is enabled.
                                       “Options menu” on page D-204


                 D-206                                                                        A+W Business Purchasing
                 Software Reference                                                                Order confirmation




                                       Employee Name of the employee allocated to the target Number Manager.

                                       Number manager Number Manager to which the purchase orders shall be
                                       moved after checking.

                                       Purchase orders
                                       The list shows all purchase orders included in the Number Manager. If you
                                       have used the purchase order numbers as a filter in the P.O. data section, only
                                       the corresponding purchase orders will be displayed.
                                       The VAT and foreign currency amount columns are displayed only if a mode
                                       with VAT and/or a foreign currency has been selected.

                                       Total Display of the totals of the listed purchase orders and the total VAT
                                       amount.

                                       Underlying VAT record Shows the VAT rate stated in the purchase order.
                                        Sales, “Tax rate” on page C-453
3.30 / 04-2020




                 A+W Business Purchasing                                                                       D-207
                 Order confirmation                                                                      Software Reference




                                            Price control – item
                                            Documents > P.O. > Order confirmation > Price control > Item tab




                 Fig. D-126   Price control – Item


                                            This tab shows the prices of the P.O. items.
                                            This tab appears only if the mandatory fields on the P.O.s tab have been filled
                                            and confirmed with [Execute].
                                             Tutorial, “Enter order confirmation and check prices” on page D-91

                                            P.O. items
                                            This list shows all items of the purchase order, for which you want to check the
                                            prices and invoice total.
                                            •   P.O. no.:
                                                Number under which the purchase order is saved in the database.
                                            •   Item:
                                                P.O. item number.
                                            •   Article:
                                                Name of the ordered item.
                                            •   Width / Height:
                                                Dimensions of the ordered item.
3.30 / 04-2020




                 D-208                                                                           A+W Business Purchasing
                 Software Reference                                                                   Order confirmation




                                       •   Euro net:
                                           Price of the item in the national currency (Euro in this case). If you are using
                                           a different currency, the name will change accordingly. If you are using two
                                           currencies, a second column with the appropriate amount is added for the
                                           second currency.
                                       •   VAT (Euro):
                                           VAT amount in the national currency (Euro in this case). This column is not
                                           displayed if the option Net is selected on the P.O.s tab.
                                           Display of VAT in a multi-currency system is identical with the display of the
                                           amount.
                                       •   BOM-based entry:
                                           This column shows whether you have corrected the price differences on
                                           the BOM element level, or on the item level.
                                           – Inactive:
                                              The price was not changed or the price of the entire item was changed.
                                           – Active:
                                              The price was changed for a BOM element.
                                       •   Supplier:
                                           Supplier number and name.
                                       •   Qty:
                                           Quantity ordered.
                                       •   Customer delivery date:
                                           Date of delivery at the customer.
                                       •   Order no.:
                                           Number of the reference order.

                                       Total amount Display of the sum of the (entered) item amounts.

                                       Total quantity Total of the item quantities.

                                       Difference Display of the difference between the invoice total in the P.O.s tab
                                       and the total of the (entered) item amounts. In this case, the price cannot be
                                       confirmed before the item prices or the BOM prices have been changed.

                                           Difference
                                           A difference is also shown if you have entered the wrong order confirmation
                                           total on the P.O. table or if the exchange rate is incorrect.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-209
                 Order confirmation                                                                     Software Reference




                                           Price control – BOM
                                           Documents > P.O. > Order confirmation > Price control > BOM tab




                 Fig. D-127   Price control – BOM


                                           This tab serves to display the price of an item on the BOM level, and on the
                                           BOM element level. This tab is active only if an item including a bill of materials
                                           has been marked on the Items tab.
                                            Tutorial, “Enter order confirmation and check prices” on page D-91

                                           BOM structure
                                           This field shows the BOM of the item marked on the Items tab.

                                           Prices
                                           The contents of the fields depends on the selected BOM element.
                                           You can correct the prices on the main level or for the BOM elements. You can
                                           change the replacement surcharges and prices for the individual elements.

                                           Price / PU Shows the price and the price unit from the purchase order.

                                           Discount Shows the discount stated in the purchase order. This value can-
                                           not be changed.
3.30 / 04-2020




                                           Net / Item quantity Shows the price and the quantity from the purchase or-
                                           der if the main item has been selected. This entry cannot be changed.




                 D-210                                                                          A+W Business Purchasing
                 Software Reference                                                               Order confirmation




                                       Net / BOM total Shows the price and the quantity from the purchase order if
                                       an element has been selected. This entry cannot be changed.

                                       Net total Shows the item price from the purchase order if the main item is se-
                                       lected. This entry can be changed.

                                       Net total / Item quantity Shows the price of the element and the quantity if
                                       an element has been selected. This entry can be changed.

                                       Total sum Shows the element price per item if an element has been selected.
                                       This entry can be changed.


                                       Electronic price control
                                       Documents > P.O. > Order confirmation > Electr. price control
                                       If you receive electronic order confirmations from your supplier (openTRANS
                                       format), you can check the allocation of items to your purchase orders as well
                                       as the prices and dates. The dialog Order confirmation – Electr. price control
                                       can be used for this purpose.
                                       This chapter provides information on the following subjects:
                                       •   “Functions menu” on page D-212
                                       •   “Options menu” on page D-212
                                       •   “Electronic price control – document import” on page D-214
                                       •   “Electronic price control – item overview” on page D-217
3.30 / 04-2020




                 A+W Business Purchasing                                                                      D-211
                 Order confirmation                                                                 Software Reference




                                      Functions menu
                                      Documents > P.O. > Order confirmation > Electr. price control > Functions
                                      menu
                                      This menu can be used to open other dialogs without closing Electronic price
                                      control.
                                      The following entries are displayed:
                                      •   Enter shipping fee:
                                          The shipping fee is automatically entered as an item on the Items tab. If the
                                          purchase order already contains a shipping fee, the option is omitted.
                                      •   Open P.O. input:
                                          All listed P.O.s are locked for editing (by other users) during price control.
                                          This function allows you to open the Document management dialog in or-
                                          der to edit one of the displayed purchase orders. Changed values are ad-
                                          opted for the price control.
                                           Sales, “Document – Header Data” on page C-365
                                      •   Manual item allocation:
                                          Opens the Manual item allocation dialog in order to allocate items from the
                                          electronic document to the appropriate items of the purchase order(s).
                                           “Manual allocation of items” on page D-219
                                      •   Distribute footer surcharges/discounts to purchase orders:
                                          Opens the Distribute footer surcharges/discounts to purchase orders dia-
                                          log in order to distribute the surcharge/discount from the electronic docu-
                                          ment to the allocated purchase orders.
                                           “Distribution of footer surcharges/discounts” on page D-220
                                      •   Remove manual item allocation:
                                          Removes the manual allocation of the selected invoice/purchase order
                                          items.
                                      •   Remove all item allocations:
                                          Removes all manual allocations of invoice and purchase order items.


                                      Options menu
                                      Documents > P.O. > Order confirmation > Electr. price control > Options menu
                                      This menu allows you to define the default settings for the dialog. The options
                                      can be enabled or disabled. The settings will not be reset when you close the
                                      dialog.
3.30 / 04-2020




                 D-212                                                                      A+W Business Purchasing
                 Software Reference                                                                     Order confirmation




                                       General group
                                       •   Different amounts:
                                           Different amounts which can be due to rounding are generally acceptable
                                           in connection with electronic price control.
                                       •   Notification of different amounts/balancing item:
                                           If differences caused by rounding are automatically allocated to a balanc-
                                           ing item, a notification will be shown.
                                       •   Freeze discount:
                                           This option fixes the discount. You should enable this option if you have de-
                                           fined new discounts but want to keep the old discounts for your old pur-
                                           chase orders. In this case, prices will not be recalculated after price control.
                                       •   Correct order PP only up to statistics:
                                           The purchase prices are corrected in the reference order only if the order
                                           still exists in the main database, and has not yet been transferred to statis-
                                           tics.
                                       •   Prod.no. for balancing item:
                                           Opens the Selection dialog from which you can select a balancing item for
                                           rounding differences.
                                            “Selection (prod. no. for balancing item)” on page D-218

                                       Settings group
                                       •   Notification of delivery delay:
                                           A message appears if the planned delivery is delayed.
                                       •   Suppress automatic allocation:
                                           You can enable the checkbox for automatic allocation in the Manual item
                                           allocation dialog so that the footer surcharges/discounts from the order
                                           confirmation are automatically allocated to a A+W Business product. You
                                           can suppress this automatic allocation.
                                            “Resolve footer surcharges/discounts automatically in future” on page D-220
                                           If this option has been changed, the currently imported document must be
                                           reimported.
                                            Tutorial, “How to import an openTRANS document” on page D-167
                                       •   Trust referencing supplier's product numbers:
                                           If a A+W Business product number has been entered as a reference in the
                                           imported document, the allocation can be made automatically.

                                       Xternal group
                                       •   Create Xternal XML file:
                                           This option is active only for defined customers.
                                       •   Xternal settings:
                                           Opens the Settings dialog to set XML export defaults. This function is avail-
                                           able only if the Create Xternal XML file option is enabled.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-213
                 Order confirmation                                                                     Software Reference




                                            Electronic price control – document import
                                            Documents > P.O. > Order confirmation > Electr. price control > Document im-
                                            port tab




                 Fig. D-128   Electronic price control – Document import


                                            Use this tab to check the imported order confirmations. The price control can
                                            be completed successfully only if the document status is free of errors.
                                             Tutorial, “Check the electronic document” on page D-168

                                            Booking type
                                            By choosing one of the options, you define how the electronic document is to
                                            be processed. The options released are based on the document status.
                                            •   Reject:
                                                Choose this option to reject the documents. No price control will be con-
                                                ducted.
                                            •   Accept:
                                                Choose this option to confirm the price control. Order confirmation number,
                                                prices, and delivery dates from the imported document will be saved in the
                                                purchase orders. Document history is updated.
3.30 / 04-2020




                 D-214                                                                          A+W Business Purchasing
                 Software Reference                                                                  Order confirmation




                                       •   Create partial delivery:
                                           A (new) partial delivery is created for the items in this document, and is
                                           booked in the same way as with Accept. The remaining items are kept in
                                           the original purchase order. The status of this purchase order is adapted
                                           accordingly.
                                           In the case of a dispatch notification, a partial order is generated with this
                                           booking type.

                                       Order confirmations
                                       This list shows all imported order confirmations. These can originate from dif-
                                       ferent suppliers.
                                       If you select an entry, the reference documents will appear on the P.O.s / par-
                                       tial deliveries list.
                                       •   OC number:
                                           OC number stated by the supplier.
                                       •   Supplier:
                                           Name of the supplier.
                                       •   Delivery date confirmed:
                                           Delivery date stated in the supplier's order confirmation.
                                       •   Net:
                                           Total amount of the delivery.
                                       •   Currency:
                                           Currency of the amount stated in the order confirmation. This is only of in-
                                           terest if you are using a multi-currency system.

                                       Display You can restrict the display of documents.

                                       Filter settings You can set filters for displaying imported documents.
                                        “Filter settings” on page D-221

                                       Document status
                                       The red or green mark indicates whether inconsistencies were found or not.
                                       The options in the Booking type section are blocked or released accordingly.
                                       •   No document selected:
                                           The document status display cannot be updated because no document has
                                           been selected from the list. This entry does not appear if an order confir-
                                           mation has been selected.
                                       •   At least one footer surcharge/discount of a P.O. could not be allocated to
                                           the document:
                                           This entry appears only if an order confirmation has been selected which
                                           shows this kind of error.
                                       •   P.O.s completely referenced:
                                           A red mark means that at least one of the reference items does not fully
                                           match the imported order confirmation. Purchase orders with incomplete
                                           references are marked on the list.
3.30 / 04-2020




                                       •   Missing article items in P.O.s:
                                           The order confirmation contains items which are not listed in the purchase
                                           orders.



                 A+W Business Purchasing                                                                          D-215
                 Order confirmation                                                               Software Reference




                                      •   Missing footer surcharges/discounts in P.O.s:
                                          Footer surcharges/discounts are not included in the order. Since they are
                                          shown on the order confirmation however, they must exist as P.O. items for
                                          price control purposes. Missing footer surcharges/discounts must be en-
                                          tered in the purchase order manually.
                                      •   Price difference:
                                          The totals of the purchase order and order confirmation differ. The appro-
                                          priate fields show the difference as an amount and as a percentage.
                                      •   Quantity difference:
                                          The item quantities of the purchase order and order confirmation differ.

                                      [Show document] Opens the document view of the selected document.

                                      P.O.s / partial deliveries
                                      This list shows the reference documents if you have selected an entry in the
                                      Order confirmations section. Partial deliveries are shown in blue letters.
                                      •   P.O. number:
                                          Number of the purchase order created by A+W Business.
                                      •   Delivery date requested:
                                          Date from the stock P.O. or the customer order.
                                      •   Net:
                                          P.O. total or order total.
                                      •   Currency:
                                          Currency shown on the P.O. This is only of interest if you are using a multi-
                                          currency system.
                                      •   Order no.:
                                          Order number.
                                      •   Customer delivery date:
                                          Date of delivery at the customer.
                                      •   Remark:
                                          If the link between the P.O. and the imported document is incomplete, this
                                          remark may indicate the error.
3.30 / 04-2020




                 D-216                                                                    A+W Business Purchasing
                 Software Reference                                                                        Order confirmation




                                            Electronic price control – item overview
                                            Documents > P.O. > Order confirmation > Electr. price control > Item overview
                                            tab




                 Fig. D-129   Electronic price control – Item overview


                                            This tab lets you check the items of the order confirmation (OC) received from
                                            your supplier. You can correct the item prices. The corrections are saved in the
                                            reference purchase orders.
                                            The options in the Booking type section are described in connection with the
                                            Document import tab.
                                             “Electronic price control – document import” on page D-214

                                            Item overview
                                            This list shows all items of the order confirmation. If you select an item, the de-
                                            tails are shown in the Document item and P.O. item sections.
                                            •   Item No.:
                                                Item number from the order confirmation.
                                            •   P.O. number:
                                                Number of the reference purchase order.
                                            •   P.O. item:
                                                Item number from the purchase order.
3.30 / 04-2020




                                            •   Net documents / Net 1 P.O.:
                                                Item price from the imported order confirmation and purchase order.
                                            •   Quantity document / Qty. 1 P.O.:
                                                Item quantity from the imported order confirmation and purchase order.


                 A+W Business Purchasing                                                                               D-217
                 Order confirmation                                                               Software Reference




                                      •   Dimensions document / Dimension 1 P.O.:
                                          Item sizes from the imported order confirmation and purchase order.
                                      •   Price difference:
                                          Difference between the columns Net documents and Net P.O.
                                      •   Difference 1 price %:
                                          Price difference in percent.
                                      •   Difference 2 qty.:
                                          Difference between the columns Quantity documents and Quantity P.O.
                                      •   Order no.:
                                          Order number.
                                      •   Customer delivery date:
                                          Date of delivery at the customer.

                                      Document item, P.O. item
                                      These two sections show details on the item selected in the item overview.


                                      Selection (prod. no. for balancing item)
                                      Documents > P.O.> Order confirmation > Electr. price control > Options menu
                                      > Prod. no. for balancing item
                                      Documents > P.O. > Invoice > Electr. invoice control > Options menu > Prod.
                                      no. for balancing item




                                      Fig. D-130   Selection


                                      Use this dialog to enter the product number used to book rounding differences.
                                      This dialog is accessible only during electronic price/invoice control.
                                       Tutorial, “Differing amounts” on page D-156
                                       Tutorial, “Check the electronic document” on page D-168

                                          Prerequisite
                                          In product management, a product must have been defined to which round-
                                          ing differences can be booked.

                                      Article number Number of the product to which the price difference is to be
                                      booked.
3.30 / 04-2020




                 D-218                                                                    A+W Business Purchasing
                 Software Reference                                                                         Order confirmation




                                             Settings for Xternal
                                             This function and the dialog are released only for certain customers.
                                             During invoice control, an XML file can be sent to the Xternal interface. It in-
                                             cludes an excerpt from the header and item data of the purchase orders in
                                             question.


                                             Manual allocation of items
                                             Documents > P.O. > Order confirmation > Electr. price control > Functions
                                             menu > Allocate items manually
                                             Documents > P.O.> Invoice > Electr. invoice control > Functions menu > Allo-
                                             cate items manually




                 Fig. D-131   Manually allocate items in electr. price control or invoice control


                                             This dialog lets you allocate the items of the imported document to the items
                                             of the purchase order(s). This dialog can be accessed only if automatic allo-
                                             cation has been disabled in the Functions menu.
                                              “Functions menu” on page D-212
                                              Tutorial, “Allocate items in electronic documents” on page D-171

                                             Document items/P.O. items
                                             Both these sections list the items from the imported document and from the
                                             corresponding purchase order. To allocate these items to one another, select
                                             the corresponding entries and confirm the allocation by pressing [OK]. The al-
                                             located items are no longer displayed afterwards.
                                             You can cancel the allocations by selecting the entry Remove all item alloca-
                                             tions in the Functions menu.
3.30 / 04-2020




                                              “Functions menu” on page D-212




                 A+W Business Purchasing                                                                               D-219
                 Order confirmation                                                               Software Reference




                                      Maintain product allocation of the footer surcharge/discount This
                                      checkbox is released only if you have allocated a footer surcharge/discount.
                                      You can save this allocation for the current session. Saving is invalid if you re-
                                      start document import.
                                      ☐The allocation only applies to this document and the corresponding pur-
                                      chase orders.
                                      ☑ The allocation applies to all other documents selected by the import filter.

                                      Resolve footer surcharges/discounts automatically in future This
                                      checkbox is released only if the Maintain product allocation of the footer sur-
                                      charge/discount checkbox is selected.
                                      If you have allocated a footer surcharge/discount, you can save this allocation
                                      for all future imports.
                                      ☐The allocation only applies to this document and the corresponding pur-
                                      chase orders.
                                      ☑ Allocation is automatically made for all other documents imported from this
                                      supplier.


                                      Distribution of footer surcharges/dis-
                                      counts
                                      Documents > P.O. > Order confirmation > Electr. price control > Functions
                                      menu > Distribute footer surcharges/discounts to P.O.s
                                      Documents > P.O. > Invoice > Electr. invoice control > Functions menu > Dis-
                                      tribute footer surcharges/discounts to P.O.s




                                      Fig. D-132   Distribute footer surcharges/discounts to P.O.s.


                                      This dialog lets you allocate the footer surcharge/discount in an electronic doc-
                                      ument to several purchase orders.
                                      This list shows all P.O. items belonging to the imported document.
                                       Tutorial, “Footer surcharges/discounts” on page D-155
3.30 / 04-2020




                                       Tutorial, “Allocate surcharges/discounts manually” on page D-172




                 D-220                                                                    A+W Business Purchasing
                 Software Reference                                                                     Order confirmation




                                       You can resolve the allocation via the Options menu.
                                        “Options menu” on page D-254



                                       Filter settings
                                       Documents > P.O. > Order confirmation > Electr. price control > Filter settings
                                       button
                                       Documents > P.O.> Invoice > Electr. invoice control > Functions menu > Filter
                                       settings button




                                       Fig. D-133   Filter settings for displaying imported documents


                                       This dialog serves to define the purchase orders that are to be displayed for
                                       the imported documents. The filters can refer to the user and/or to the supplier.

                                       By user
                                       You can define whose purchase orders can be displayed for the imported doc-
                                       ument.

                                       All You can view all purchase orders for the imported documents.
                                       ☐ Display of the purchase orders shall be restricted by means of the other fil-
                                       ters. The checkboxes Only own and Fix are available.
                                       ☑The display of purchase orders is not restricted by user or Number Manager.
                                       The checkboxes Only own and Fix are blocked.

                                       Only own This checkbox is blocked if the checkbox All is ticked.
                                       ☐The display is not restricted to own purchase orders.
                                       ☑ The display is restricted to purchase orders you have entered yourself. If
                                       you select a Number Manager as well, only your own purchase orders from
3.30 / 04-2020




                                       the selected Number Manager will be displayed.




                 A+W Business Purchasing                                                                           D-221
                 Order confirmation                                                                Software Reference




                                      Fix This checkbox is blocked if the checkbox All is ticked.
                                      ☐The display of purchase orders is not restricted to a single Number Manager.
                                      ☑Only purchase orders from the displayed Number Manager will be shown. If
                                      you have ticked the checkbox Only own as well, you will see only your own
                                      purchase orders in the selected Number Manager.

                                      By supplier
                                      You can restrict the display of purchase orders to one or several suppliers.

                                      Supplier You can select one or more suppliers.

                                      Buttons You can use the buttons to adopt the selected supplier for the over-
                                      view, or remove an entry from the overview.
                                       Tutorial, “Buttons in search dialogs” on page C-39

                                      Overview
                                      The overview shows all suppliers that can be used as a filter for displaying pur-
                                      chase orders.

                                         Save settings
                                         The settings will be saved when leaving the dialog and will apply until they
                                         are altered or reset.
3.30 / 04-2020




                 D-222                                                                       A+W Business Purchasing
                 Software Reference                                                                 Order confirmation




                                       Reminder
                                       Documents > P.O.> Order confirmation > Reminder




                                       Fig. D-134   Remind supplier


                                       This dialog can be used to search for open purchase orders overdue for deliv-
                                       ery. The search can be restricted to a date, to certain suppliers and/or Number
                                       Managers.
                                        Tutorial, “Remind supplier” on page D-95

                                       Functions menu
                                       •   Delete reminder code:
                                           Deletes the reminder code from the displayed purchase orders.

                                       Selection

                                       Supplier from, to Restrict the search to a supplier or a sequence of suppli-
                                       ers.

                                       Number manager Display of the purchase orders in a Number Manager.

                                       Minimum status, status below Restrict the search to purchase orders that
                                       are in a certain status range.

                                       Options

                                       Up to entry date Specification of the entry date for which the open purchase
                                       orders are to be searched for. The current date is selected by default. This set-
3.30 / 04-2020




                                       ting also shows, if applicable, purchase orders which cannot have been deliv-
                                       ered at all.



                 A+W Business Purchasing                                                                        D-223
                 Order confirmation                                                              Software Reference




                                      Remind suppliers who have been reminded once again If you have is-
                                      sued a reminder for a delivery, the respective order receives a reminder code.
                                      ☐Purchase orders for which reminders have been issued already will not be
                                      displayed.
                                      ☑Open purchase orders will be displayed even if a reminder has already been
                                      issued. A new reminder can be issued.

                                      Fax dispatch / mail dispatch / all The search can be restricted to purchase
                                      orders dispatched by fax or regular mail. Regular mail also includes PDF files
                                      attached to emails.
                                      If you do not want to restrict the search, choose the option All.
                                      The reminders will be dispatched in the way that has been defined as a stan-
                                      dard for purchase orders to the corresponding supplier.

                                      Table
                                      This list includes all suppliers for which there are open purchase orders match-
                                      ing the filter criteria. Suppliers which have already been sent a reminder are
                                      shown in red.
                                      •   P.O. number:
                                          Number of the open purchase order.
                                      •   Stat.:
                                          Status of the open purchase order.
                                      •   Supplier:
                                          Supplier to whom the purchase order was sent.
                                      •   Entry date:
                                          Entry date of the purchase order.
                                      •   Delivery date:
                                          Scheduled and/or confirmed delivery date as per the purchase order.
3.30 / 04-2020




                 D-224                                                                   A+W Business Purchasing
                 Software Reference                                                                   Receipt of goods




                                       Receipt of goods
                                       Documents > P.O. > Receipt of goods > Receipt of goods
                                       You can enter the receipt of goods and the supplier's order confirmation, check
                                       the delivered items and correct them if required.
                                       This chapter provides information on the following subjects:
                                       •   “Receipt of goods (dialog)” on page D-225
                                       •   “Inspection of goods received” on page D-239


                                       Receipt of goods (dialog)
                                       Documents > P.O. > Receipt of goods > Receipt of goods
                                       This dialog serves to enter the goods received for individual purchase orders
                                       or for the purchase orders in a Number Manager.
                                       For booking stock on hand, you can define ID numbers to be automatically as-
                                       signed if the stock P.O. includes items with a quantity of larger than 1. The ID
                                       numbers are assigned for boxes and glass (stockplates).

                                           Prerequisite
                                           The checkbox for the virtual assignment of item numbers must be ticked in
                                           company data.

                                            Master Data, “Use virtual item numbers” on page B-919
                                       This chapter provides information on the following subjects:
                                       •   “Functions menu” on page D-226
                                       •   “Options menu” on page D-226
                                       •   “Print menu” on page D-227
                                       •   “Receipt of goods – selection” on page D-228
                                       •   “Receipt of goods –complete” on page D-230
                                       •   “Receipt of goods – by item” on page D-232
                                       •   “Receipt of goods – ID numbers” on page D-235
                                       •   “Receipt of goods – protocol (ID numbers)” on page D-237
3.30 / 04-2020




                 A+W Business Purchasing                                                                       D-225
                 Receipt of goods                                                              Software Reference




                                    Functions menu
                                    Documents > P.O. > Receipt of goods > Receipt of goods > Functions menu
                                    This menu can be used to open other dialogs without closing Receipt of goods.
                                    The following entries are displayed:
                                    •   Show document:
                                        Opens the Document view dialog and provides a print preview.
                                         Sales, “Complaint” on page C-510
                                    •   Document data:
                                        Opens the Document data dialog to correct the dates and the status if nec-
                                        essary.
                                         Sales, “Document Data” on page C-646
                                    •   Stock search:
                                        Opens the Stock Info dialog to show the current stock on hand.
                                         Sales, “Stock Info” on page C-650
                                    •   Article Info:
                                        Opens the Article info dialog in order to gather detailed information on the
                                        current product.
                                         Sales, “Product Information” on page C-521


                                    Options menu
                                    Documents > P.O. > Receipt of Goods > Receipt of Goods > Options menu
                                    This menu allows you to define the default settings for the dialog. The options
                                    can be enabled or disabled. The settings will not be reset when you close the
                                    dialog.
                                    The following entries are displayed:
                                    •   Item view if a single document is selected:
                                        Use this option to go to the tab By item and view a single document.
                                    •   ID number assignment:
                                        This setting is only needed for the receipt of boxes and stockplates.
                                        – Automatic allocation:
                                           Use this option for automatic assignment of IDs. A default can be de-
                                           fined. If this option is disabled, you have to enter the ID by hand.
                                        – Settings:
                                           Opens the Settings dialog which lets you enter the settings for the auto-
                                           matic assignment of IDs.
                                            “Settings (ID)” on page D-238
                                    •   Show storage location for ID numbers from the item:
                                        This option is used to suggest the storage location, which was specified in
                                        the previously booked item.
3.30 / 04-2020




                 D-226                                                                  A+W Business Purchasing
                 Software Reference                                                                    Receipt of goods




                                       •   Stock booking date = Delivery date:
                                           The delivery date from the P.O. is automatically taken as the booking date.
                                       •   Check OC number:
                                           This setting outputs a message if the number of the order confirmation has
                                           not been entered by the supplier.


                                       Print menu
                                       Documents > P.O. > Receipt of goods > Receipt of goods > Print menu
                                       Use this menu to start the print function.
                                       The following entries are displayed:
                                       •   Receipt of goods:
                                           Starts printout of a list containing all orders and reference orders listed in
                                           the dialog.
                                       •   Labels:
                                           Starts the printout of box labels.
                                       •   Protocol:
                                           Starts the printout of a protocol containing all box items and the assigned
                                           box IDs.
                                       •   Labels and protocol (only group printer):
                                           Starts the printout of the box labels and a protocol containing all assigned
                                           box IDs.
                                       •   Settings:
                                           Opens the printer settings.
3.30 / 04-2020




                 A+W Business Purchasing                                                                          D-227
                 Receipt of goods                                                                       Software Reference




                                           Receipt of goods – selection
                                           Documents > P.O. > Receipt of goods > Receipt of goods > Selection tab




                 Fig. D-135   Receipt of goods – Selection


                                           This tab is used to filter the selection and display of documents for which re-
                                           ceipt of goods shall be checked and/or entered.
                                            Tutorial, “Receipt of goods” on page D-118

                                           Selection
                                           By choosing the option, you define how the purchase orders shall be filtered.
                                           Open purchase orders are displayed after the search in the Complete tab so
                                           that receipt of goods can be booked.
                                           •   By P.O. number:
                                               The input field for the P.O. number is released. The Complete tab shows
                                               the required purchase order and all reference orders.
                                           •   By order number:
                                               The input field for the order number is released. The Complete tab shows
                                               all purchase orders issued for the defined order number.
                                           •   By supplier:
                                               The input field for the supplier number is released. The Complete tab
                                               shows all purchase orders placed with the selected supplier.
                                           •   By delivery note number/dispatch notification, total quantity delivered:
3.30 / 04-2020




                                               The input field for the delivery note or dispatch notification number and the
                                               field for entering the total quantity are released. If a dispatch notification
                                               has been imported, the actually received quantities must be entered.



                 D-228                                                                          A+W Business Purchasing
                 Software Reference                                                                 Receipt of goods




                                       •   By supplier delivery date:
                                           The input field for the delivery date is released. The Complete tab shows
                                           all purchase orders to be delivered by the selected date.
                                       •   By Number Manager:
                                           The combo box for selecting the Number Manager is released. The Com-
                                           plete tab shows all purchase orders in the selected Number Manager.
                                       •   By scanner / document:
                                           The fields for the barcode of the P.O. number or a P.O. item are released.

                                       Target Number Manager

                                       Target Number Manager After booking the receipt of goods, the stock P.O.s
                                       can be automatically transferred to a different Number Manager.
                                       ☐The stock P.O.s are not moved to a different Number Manager.
                                       ☑The fields in the Target Number Manager section are released. The stock
                                       P.O.s will be moved to the selected Number Manager.

                                       Employee Name of the employee allocated to the target Number Manager.

                                       Number manager Number Manager to which the stock P.O.s with (complete)
                                       receipt of goods should be moved.
3.30 / 04-2020




                 A+W Business Purchasing                                                                      D-229
                 Receipt of goods                                                                     Software Reference




                                           Receipt of goods –complete
                                           Documents > P.O.> Receipt of goods > Receipt of goods > Complete tab




                 Fig. D-136   Receipt of goods – Complete


                                           This tab shows all purchase orders matching the search criteria. Select a pur-
                                           chase order to list all reference orders.
                                            Tutorial, “Enter receipt of goods” on page D-125

                                           Delivery date

                                           Supplier's delivery date Shows the current date. You can change it to enter
                                           a delivery received before that date. The date will be adopted only for the doc-
                                           uments selected in the list.

                                           OC supplier You can also enter the supplier's order confirmation number for
                                           the goods received.
3.30 / 04-2020




                 D-230                                                                          A+W Business Purchasing
                 Software Reference                                                                  Receipt of goods




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
                                           ☐Receipt of goods is incomplete. Some deliveries have yet to be made.
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

                                       Delivery at the customer This date is adopted from the reference order.
                                       You can change it if the originally scheduled date cannot be adhered to.
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-231
                 Receipt of goods                                                                    Software Reference




                                           Receipt of goods – by item
                                           Documents > P.O. > Receipt of goods > Receipt of boxes > By item tab




                 Fig. D-137   Receipt of goods – By item


                                           This tab serves to enter the receipt of goods by item for a purchase order se-
                                           lected on the Complete tab.

                                           Goods received/issued

                                           Quantity received Quantity already delivered for the selected item.

                                           Quantity ordered, already delivered, quantity announced These fields
                                           show the corresponding quantities for the item selected. The fields are updat-
                                           ed after input.

                                           Storage location You can select a storage location for the selected item, to
                                           which the stock article is to be booked to. Please note that stock articles can
                                           also be booked to the storage location <n.s.>. The storage location from the
                                           P.O. can be shown via the Options menu.
                                            “Options menu” on page D-226
3.30 / 04-2020




                 D-232                                                                        A+W Business Purchasing
                 Software Reference                                                                      Receipt of goods




                                       Accept surplus or shortfall The quantity delivered can differ from the quan-
                                       tity ordered. You can accept deviating quantities and thus declare delivery of
                                       the item as complete.
                                       ☐Do not accept surplus or shortfall.
                                       ☑ The quantity entered is accepted; the item is booked as complete.
                                       • If a stock article has been delivered, the stock on hand is updated based
                                            on the quantity delivered. The changed quantity is saved in the purchase
                                            order.
                                       • If the delivery was ordered for an order, the new quantities are entered in
                                            the order as surplus- or shortfall.
                                            – If the order is already in production, the quantity change is transferred
                                               to the production system.
                                            – If the order is not yet in production, the over/excess quantity is reported
                                               to the production system with the production transfer.
                                           For this, in the company data, the check box Change purchase order and
                                           order if under/over-delivery is accepted must be activated.
                                            Master Data, “Company Data – Stock/Purchasing/EDI” on page B-931

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
                                           ☐Receipts of goods is incomplete.
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
3.30 / 04-2020




                                       •   Delivered:
                                           Quantity already delivered for this item. For partial deliveries, this is the to-
                                           tal of the quantities delivered so far for this purchase order.


                 A+W Business Purchasing                                                                            D-233
                 Receipt of goods                                                                 Software Reference




                                    •   Receipt:
                                        Quantity already delivered for the selected item..
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
                                    •   Storage location:
                                        Standard storage location for this stock article. Please note that stock arti-
                                        cles can also be booked to storage location <n.s.>.
                                    •   Article description 2 + 3:
                                        Descriptions of the ordered product that are stored in the master data. For
                                        float glass, usually only description 1 is stored, which is displayed in the Ar-
                                        ticle column.

                                    Appended orders
                                    The list shows the reference orders for the items. The fields are explained in
                                    connection with the Complete tab.
                                     “Receipt of goods –complete” on page D-230
3.30 / 04-2020




                 D-234                                                                    A+W Business Purchasing
                 Software Reference                                                                      Receipt of goods




                                           Receipt of goods – ID numbers
                                           Documents > P.O.> Receipt of goods > Receipt of goods > ID numbers tab




                 Fig. D-138   Receipt of goods – ID numbers


                                           This tab shows the items belonging to a purchase order that includes boxes.
                                           For every box in a P.O. item, a sub-item (virtual item number) is created which
                                           can be assigned a box with a special ID number (identification number). You
                                           can define the default for the ID.
                                            “Settings (ID)” on page D-238

                                              Prerequisite
                                              The checkbox for assigning virtual item numbers must be ticked in the com-
                                              pany data.

                                               Master Data, “Use virtual item numbers” on page B-919

                                           Box data

                                           Supplier ID number Box ID assigned to the delivery item by the supplier.
                                           When you enter the number, the ID numbers filed shows the automatic box ID.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-235
                 Receipt of goods                                                               Software Reference




                                    ID numbers The automatic box ID appears when you enter the supplier ID.
                                    For every box in a P.O. item, a separate box ID is created when you enter the
                                    receipt of goods. If, for example, 5 boxes of float 5 à 1200 x 800 mm are or-
                                    dered and delivered, the IDs XXXX00001, XXXX00002, …, XXXX00005 are
                                    assigned. You can define the presetting for XXXX yourself.
                                     “Settings (ID)” on page D-238

                                    Storage location Each item can be assigned a separate storage location.
                                    Please note you can also assign storage location <n.s.>.

                                    Remark Comments can be entered here in case of peculiarities, e.g. regard-
                                    ing the allocation of storage locations or in connection with reservations.

                                    Contents Contents of the box selected in the list. This entry can be changed
                                    if required.

                                    Prod. date Date by which the production of the ordered goods should be fin-
                                    ished. This date is important for the stock withdrawal in accordance with the
                                    FiFo principle, e.g. for coated glass.

                                    PP / QU Purchase price and price unit of the ordered item. If you change the
                                    price, the amendment will be saved in the purchase order.

                                    Box items
                                    You can select several boxes at once to book them in one step. If more than
                                    one box was selected and the supplier ident numbers entered, the system cal-
                                    culates the box ident numbers for all marked entries.
                                    •   Item
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
                                        Production date as defined in section Box data
                                    •   Pr./QU:
                                        Purchase price per quantity unit as defined in the Box data section.
3.30 / 04-2020




                                    •   Pr. unit:
                                        Price unit that applies to the displayed price.



                 D-236                                                                  A+W Business Purchasing
                 Software Reference                                                                   Receipt of goods




                                           Receipt of goods – protocol (ID numbers)
                                           Documents > P.O.> Receipt of goods > Receipt of goods > Protocol tab (ID
                                           numbers)




                 Fig. D-139   Receipt of goods – Protocol (ID numbers)


                                           This tab gives you an overview of the allocated box IDs.
3.30 / 04-2020




                 A+W Business Purchasing                                                                       D-237
                 Receipt of goods                                                                Software Reference




                                    Settings (ID)
                                    Documents > P.O. > Receipt of goods > Receipt of goods > Options menu >
                                    ID allocation group > Settings




                                    Fig. D-140   Settings


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

                                        Master Data, “Use virtual item numbers” on page B-919

                                    Stock ID number

                                    Default You can enter text (or numbers) of max. 15 characters which is com-
                                    pleted by XXXXX. XXXXX represents the automatically assigned number. The
                                    text is retained until you change it.
                                    If you buy boxes from different suppliers and want to mark them separately,
                                    you have to amend the default before entering the receipt of goods.
3.30 / 04-2020




                 D-238                                                                   A+W Business Purchasing
                 Software Reference                                                                 Receipt of goods




                                       Inspection of goods received
                                       Documents > P.O. > Receipt of goods > Inspection of goods received
                                       You can use the Inspection of goods received dialog to check which purchase
                                       orders have been completely delivered, and which are incomplete.
                                       If you have entered a target Number Manager when booking receipt of goods,
                                       the P.O.s will be moved there automatically.
                                        “Target Number Manager” on page D-229
                                       This dialog offers the following tabs:
                                       •   “Inspection of goods received – complete P.O.s” on page D-239
                                       •   “Inspection of goods received – Qty. discrepancies” on page D-241


                                       Inspection of goods received – complete P.O.s
                                       Documents > P.O. > Receipt of goods > Inspection of goods received > Com-
                                       plete P.O.s tab




                                       Fig. D-141   Inspection of goods received – Complete P.O.s


                                       This tab lets you display all purchase orders of a specific Number Manager
                                       and check whether they have been delivered in full.
                                        Tutorial, “Check receipt of goods” on page D-131
3.30 / 04-2020




                 A+W Business Purchasing                                                                       D-239
                 Receipt of goods                                                                Software Reference




                                    Number manager

                                    P.O. Number Manager The Number Manager in which the purchase orders
                                    (and receipt of goods) are administered. Only the Number Managers defined
                                    in the menu Purchase order > NM purchase order will be offered for selection.

                                    Receipt of goods complete
                                    The list shows all purchase orders from the selected Number Manager.
                                    •   No.:
                                        Purchase order number.
                                    •   Supplier:
                                        Name of the supplier to which the purchase order was sent.
                                    •   Status:
                                        Status of the purchase order. The status is changed when the purchase or-
                                        der has been entered completely.

                                        Old purchase orders in the Number Manager
                                        Purchase orders are usually deleted from the main database after ar-
                                        chiving. The corresponding settings are found in the company data.

                                         Master Data, “Company Data – Archives” on page B-938
                                        If the Number Manager for purchase orders for which goods have been re-
                                        ceived gets too full, you should empty it from time to time, or create a new
                                        one.
                                         Sales, “How to clear a number manager” on page C-149
3.30 / 04-2020




                 D-240                                                                 A+W Business Purchasing
                 Software Reference                                                                      Receipt of goods




                                       Inspection of goods received – Qty. discrepancies
                                       Documents > P.O.> Receipt of goods > Inspection of goods received > Qty.
                                       discrepancies tab




                                       Fig. D-142    Inspection of goods received – Qty. discrepancies


                                       This tab can be used to view all items for purchase orders whose receipt of
                                       goods has not been booked in full.
                                       You can book purchase orders as complete. Partial deliveries can only be en-
                                       tered in the Receipt of goods dialog.
                                        “Receipt of goods (dialog)” on page D-225

                                       Quantity discrepancies
                                       This list shows all purchase orders with items for which the receipt of goods is
                                       incomplete.
                                       •   No.:
                                           Purchase order number.
                                       •   Item:
                                           Number of the P.O. item for which there are still goods to be received.
                                       •   Product:
                                           Name of the item.
                                       •   Purch. quantity:
                                           Quantity of the ordered item.
                                       •   Deliv. quantity:
3.30 / 04-2020




                                           Quantity delivered for this item. For partial deliveries, this value can differ
                                           from the ordered quantity.




                 A+W Business Purchasing                                                                           D-241
                 Receipt of goods                                                              Software Reference




                                    •   OK:
                                        If the remaining part of the delivery has arrived in the meantime, you can
                                        make up for the Complete booking by ticking the checkbox.
                                    •   Del. date:
                                        The delivery date is adopted from the P.O. If it was changed for partial re-
                                        ceipts of goods, the new date is displayed here as well.
                                    •   Supplier:
                                        Name of the supplier to which the purchase order was sent.
3.30 / 04-2020




                 D-242                                                                  A+W Business Purchasing
                 Software Reference                                                                               Invoice




                                       Invoice
                                       Documents > P.O.> Invoice > Invoice control
                                       You can enter and check the invoices of your suppliers in A+W Business be-
                                       fore transferring them to your accounting and/or financial accounting (FinAcc)
                                       department. The Invoice control dialog is used for this purpose.
                                       This chapter provides information on the following subjects:
                                       •   “Invoice control – Purchase orders” on page D-246
                                       •   “Invoice date” on page D-253


                                       Invoice control
                                       Documents > P.O.> Invoice > Invoice control
                                       Use this dialog to enter and control supplier invoices and transfer them to a
                                       corresponding Number Manager in FinAcc.
                                       Only purchase orders that have reached the defined minimum status will be
                                       displayed, e.g. Receipt of goods complete.
                                        Tutorial, “Price and invoice control” on page D-141

                                           Collective invoice
                                           If your supplier combines multiple P.O.s in a collective invoice, this can only
                                           be checked and accepted if the same VAT rate and the same currency is
                                           given in all P.O.s.

                                       This chapter provides information on the following subjects:
                                       •   “Functions menu” on page D-244
                                       •   “Options menu” on page D-244
                                       •   “Invoice control – Purchase orders” on page D-246
                                       •   “Invoice control – items” on page D-249
                                       •   “Invoice control – BOM” on page D-251
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-243
                 Invoice                                                                Software Reference




                           Functions menu
                           Documents > Purchase Order > Invoice > Invoice Control > Functions menu
                           This menu allows to open other dialogs without closing invoice control.
                           The following entries are displayed:
                           •   Create partial delivery:
                               Opens the Copy documents dialog to enter a partial delivery.
                                Sales, “Copy Documents” on page C-461
                           •   Enter shipping fee:
                               The shipping fee is automatically entered as an item on the Items tab. If the
                               purchase order already contains a shipping fee, the option is omitted.
                           •   Open P.O. input:
                               All listed P.O.s are locked for editing (by other users) during price control.
                               This function allows you to open the Document management dialog in or-
                               der to edit one of the displayed purchase orders. Changed values are ad-
                               opted for the price control.
                                Sales, “Document – Header Data” on page C-365
                           •   Update order data:
                               This function directly saves the changed values in the purchase order.


                           Options menu
                           Documents > P.O. > Invoice > Invoice Control > Options menu
                           This menu allows you to define the default settings for the dialog. The options
                           can be enabled or disabled. The settings will not be reset when you close the
                           dialog.

                           Standard group
                           •   Net VAT:
                               Net amounts are shown incl. VAT.
                           •   Gross VAT:
                               Gross amounts are shown incl. VAT.
                           •   Net:
                               Net amounts are shown without VAT.

                           Behavior group
                           •   Quick input:
                               This option means that when you enter a P.O. number, the cursor directly
                               goes to the Order total field. This setting is saved in relation to the user.
                           •   Invoice date restriction:
                               Opens the Invoice date dialog in order to set the divergence in days.
                                “Invoice date” on page D-253
                           •   Fill target NM:
                               Releases the fields in the Target Number Manager section to select a user
3.30 / 04-2020




                               and the corresponding Number Manager.




                 D-244                                                          A+W Business Purchasing
                 Software Reference                                                                                Invoice




                                       Settings group
                                       •   Freeze discount:
                                           This option fixes the discount. You should enable this option if you have de-
                                           fined new discounts but want to keep the old discounts for your old pur-
                                           chase orders. In this case, prices will not be recalculated after price control.
                                       •   No correction of order costs in statistics:
                                           The purchase prices are corrected in the reference order only if the order
                                           still exists in the main database, and has not yet been transferred to statis-
                                           tics.
                                       •   Notification of delivery delay:
                                           A message is shown when the delivery date at the customer cannot be ad-
                                           hered to.

                                       Xternal group
                                       •   Create Xternal XML file:
                                           This option is enabled only for defined customers.
                                       •   Xternal settings:
                                           Opens the Settings dialog to set XML export defaults. This function is avail-
                                           able only if the Create Xternal XML file option is enabled.
3.30 / 04-2020




                 A+W Business Purchasing                                                                           D-245
                 Invoice                                                                              Software Reference




                                           Invoice control – Purchase orders
                                           Documents > P.O. > Invoice > Invoice control > P.O.s tab




                 Fig. D-143   Invoice control – Purchase orders


                                           This tab is used to enter supplier invoices and transfer them to another Num-
                                           ber Manager to be passed on to Financial accounting.
                                            Tutorial, “Checking the invoice” on page D-144

                                           Invoice data

                                           Invoice number Mandatory field. You have to enter the supplier's invoice
                                           number.

                                           Invoice date Mandatory field. Date shown on the invoice. The last assigned
                                           invoice date is suggested by default. You can select the date from the calendar
                                           or enter it by hand, e.g. 16052013.
3.30 / 04-2020




                 D-246                                                                        A+W Business Purchasing
                 Software Reference                                                                             Invoice




                                       P.O. data
                                       Choose one of the two options to release the corresponding fields for selecting
                                       the purchase order(s), for which you want to check the invoices.
                                       •   P.O. number, to:
                                           If you enter the same number in both fields, just this purchase order will be
                                           displayed in the P.O.s section. If several purchase orders belong to an or-
                                           der confirmation, you can enter several P.O. numbers in succession and
                                           add them to the overview. All of the purchase orders must belong to the
                                           same supplier and have the same VAT rate.
                                       •   Number Manager:
                                           When you have selected a Number Manager, the P.O.s section shows all
                                           purchase orders of this Number Manager.

                                       Totals
                                       You can switch to another tab only after you have entered the amount from the
                                       supplier's invoice and have confirmed it with [Execute].

                                       Invoice total, VAT Mandatory field. Invoice and VAT total. The VAT amount
                                       will not be displayed if the Net mode has been selected.

                                       Mode Your selection here will determine whether the VAT is shown or not.
                                       You can set the default mode in the menu Options > Standard group.
                                       • Net incl. VAT:
                                          The total amount will be evaluated as net; the VAT amount is shown.
                                       • Gross with VAT:
                                          The total amount will be evaluated as gross; the VAT amount is shown.
                                       • Net:
                                          The total amount will be evaluated as net; the VAT amount will not be
                                          checked.

                                       Currency You can select another currency only if you are using more than
                                       one currency.
                                       The combo box offers a selection of all currencies defined in the master data.
                                       If you select a currency other than Euro, the overview will list the order and
                                       VAT amounts in the selected currency as well.
                                        Master Data, “Currencies” on page B-450
3.30 / 04-2020




                 A+W Business Purchasing                                                                         D-247
                 Invoice                                                                Software Reference




                           Exchange rate If you are using more than one currency, the exchange rate
                           defined in the master data is shown here. It can be changed. If you are using
                           only Euro as a currency, the entry in this field must be 1.

                              Fix exchange rate
                              You can define a different exchange rate for each purchase order. This will
                              be used automatically for price control calculations. You can only change it
                              if it has not been fixed in the purchase order.

                               Sales, “Rate fixed for invoicing” on page C-379

                           Target Number Manager
                           These two fields are released only if the option Fill target NM is enabled. In-
                           voices will be moved to the defined Number Manager after invoice control, e.g.
                           in order to release them for payment.
                            “Options menu” on page D-204

                           Employee Name of the employee allocated to the target Number Manager.

                           Number manager Number Manager to which the invoices shall be moved af-
                           ter the check.

                           Purchase orders
                           The list shows all purchase orders included in the Number Manager. If you
                           have used the purchase order numbers as a filter in the P.O. data section, only
                           the corresponding purchase orders will be displayed.
                           The VAT and foreign currency amount columns are displayed only if a mode
                           with VAT and/or a foreign currency has been selected.

                           Total These fields show the totals of the listed purchase orders and the total
                           VAT amount.

                           Underlying VAT record This field shows the percentage for VAT calculation
                           defined in the purchase order which belongs to this invoice.
                            Sales, “Tax rate” on page C-453
3.30 / 04-2020




                 D-248                                                            A+W Business Purchasing
                 Software Reference                                                                                  Invoice




                                            Invoice control – items
                                            Documents > P.O. > Invoice > Invoice control > Items tab




                 Fig. D-144   Invoice control – Items


                                            This tab is used to check the items of all purchase orders for which you have
                                            entered a supplier invoice.
                                            This tab appears only if the mandatory fields on the P.O.s tab have been filled
                                            and confirmed with [Execute].
                                             Tutorial, “Checking the invoice” on page D-144

                                            P.O. items
                                            This list includes all items of the purchase orders to which this invoice refers.
                                            •   P.O. no.:
                                                Number under which the purchase order is saved in the database.
                                            •   Item:
                                                P.O. item number.
                                            •   Article:
                                                Name of the ordered item.
                                            •   Width / Height:
                                                Dimensions of the ordered item.
3.30 / 04-2020




                 A+W Business Purchasing                                                                              D-249
                 Invoice                                                                 Software Reference




                           •   Euro net:
                               Price of the item in the national currency (Euro in this case). If you are using
                               a different currency, the name will change accordingly. If you are using two
                               currencies, a second column with the appropriate amount is added for the
                               second currency.
                           •   VAT (Euro):
                               VAT amount in the national currency (Euro in this case). This column is not
                               displayed if the option Net is selected on the P.O.s tab.
                               Display of VAT in a multi-currency system is identical with the display of the
                               amount.
                           •   BOM-based entry:
                               This column shows whether you have corrected the price differences on
                               the BOM element level, or on the item level.
                               – Inactive:
                                  The price was not changed or the price of the entire item was changed.
                               – Active:
                                  The price was changed in the BOM.
                           •   Qty:
                               Quantity delivered.
                           •   Supplier:
                               Supplier number and name.

                           Total amount Display of the sum of the (entered) item amounts.

                           Total quantity Total of the item quantities.

                           Difference Display of the difference between the invoice total in the P.O.s tab
                           and the total of the (entered) item amounts. In this case, the price cannot be
                           confirmed before the item prices or the BOM prices have been changed.

                               Difference
                               A difference is also shown if you have accidentally entered the wrong in-
                               voice total on the P.O.s tab or if the exchange rate is incorrect.
3.30 / 04-2020




                 D-250                                                           A+W Business Purchasing
                 Software Reference                                                                                   Invoice




                                           Invoice control – BOM
                                           Documents > P.O.> Invoice > Invoice control > BOM tab




                 Fig. D-145   Invoice control – BOM


                                           This tab serves to display the price of an item on the BOM level, and on the
                                           BOM element level. This tab is active only if an item including a bill of materials
                                           has been marked on the Items tab.
                                            Tutorial, “Checking the invoice” on page D-144

                                           BOM structure
                                           This field shows the BOM of the item marked on the Items tab.

                                           Prices
                                           The contents of the fields depend on the selected BOM element.
                                           You can correct the prices on the main level or for the BOM elements. You can
                                           change the replacement surcharges and prices for the individual elements.

                                           Price / PU Shows the price and the price unit from the purchase order.

                                           Discount Shows the discount stated in the purchase order. This value can-
                                           not be changed.
3.30 / 04-2020




                                           Net / Item quantity Shows the price and the quantity from the purchase or-
                                           der if the main item has been selected. This entry cannot be changed.




                 A+W Business Purchasing                                                                               D-251
                 Invoice                                                            Software Reference




                           Net / BOM quantity Shows the price and the quantity from the purchase or-
                           der if an element has been selected. This entry cannot be changed.

                           Net total Shows the item price from the purchase order if the main item is se-
                           lected. This entry can be changed.

                           Net total / Item quantity Shows the price of the element and the quantity if
                           an element has been selected. This entry can be changed.

                           Total sum Shows the element price per item if an element has been selected.
                           This entry can be changed.
3.30 / 04-2020




                 D-252                                                       A+W Business Purchasing
                 Software Reference                                                                          Invoice




                                       Invoice date
                                       Documents > P.O.> Order confirmation > Price control > Options menu >
                                       Group behavior > Invoice date restrictions
                                       Documents > P.O.> Invoice > Invoice control > Options menu > Group behav-
                                       ior > Invoice date restrictions




                                       Fig. D-146    Invoice date restrictions


                                       You can use this dialog to specify the maximum divergence in days between
                                       the invoice date and the current date. This prevents incorrect date entries.
                                       This setting is only useful for invoice control.

                                       Divergence

                                       in days This value specifies the maximum divergence in days between the
                                       invoice date and the current date. If the allowed period is exceeded due to an
                                       incorrect date entry, the maximum date permitted will be inserted automatical-
                                       ly.

                                           Example

                                           Displayed: August 24 – 10 days are allowed
                                           Entry: August 13 – Correction to August 14


                                       You can switch off this function by entering a 0 (zero).
3.30 / 04-2020




                 A+W Business Purchasing                                                                      D-253
                 Invoice                                                                 Software Reference




                           Electronic invoice control
                           Documents > P.O. > Invoice >Electr. invoice control
                           If you receive invoices from your suppliers in electronic format, you can check
                           the allocation of items to your purchase orders as well as the prices and dates.
                           Electronic invoice control is used for this purpose.
                            Tutorial, “Export/Import (openTRANS)” on page D-149
                            Tutorial, “Check the electronic document” on page D-168
                           This chapter provides information on the following subjects:
                           •   “Functions menu” on page D-254
                           •   “Options menu” on page D-254
                           •   “Electronic invoice control – document import” on page D-257
                           •   “Electronic invoice control – item overview” on page D-260


                           Functions menu
                           Documents > P.O.> Invoice > Electr. invoice control > Functions menu
                           This menu lets you open other dialogs without closing electronic invoice con-
                           trol.
                           The following entries are displayed:
                           •   Enter shipping fee:
                               The shipping fee is automatically entered as an item on the Items tab. If the
                               purchase order already contains a shipping fee, the option is omitted.
                           •   Open P.O. input:
                               All listed P.O.s are locked for editing (by other users) during invoice control.
                               This function allows you to open the Document management dialog in or-
                               der to edit one of the displayed purchase orders. Changed values are ad-
                               opted for the invoice control.
                                Sales, “Document – Header Data” on page C-365
                           •   Manual allocation of items:
                               Opens the Manual allocation of items dialog to allocate the items of the
                               electronic document to the items of the purchase order(s).
                                “Manual allocation of items” on page D-219
                           •   Distribute footer surcharges/discounts to purchase orders:
                               Opens the Distribute footer surcharges/discounts to purchase orders dia-
                               log in order to distribute the surcharge/discount from the electronic docu-
                               ment to the allocated purchase orders.
                                “Distribution of footer surcharges/discounts” on page D-220
                           •   Remove manual item allocation:
                               Removes the manual allocation of the selected invoice/purchase order
                               items.
                           •   Remove all item allocations:
                               Removes all manual allocations of invoice and purchase order items.
3.30 / 04-2020




                           Options menu
                           Documents > P.O. > Invoice > Electr. invoice control > Options menu


                 D-254                                                           A+W Business Purchasing
                 Software Reference                                                                              Invoice




                                       This menu allows you to define the default settings for the dialog. The options
                                       can be enabled or disabled. The settings will not be reset when you close the
                                       dialog.

                                       General group
                                       •   Accept different amounts:
                                           Different amounts which can be due to rounding are generally acceptable
                                           in connection with electronic invoice control.
                                       •   Notification of different amounts/balancing item:
                                           If differences caused by rounding are automatically allocated to a balanc-
                                           ing item, a notification will be shown.
                                       •   Freeze discount:
                                           This option fixes the discount. You should enable this option if you have de-
                                           fined new discounts but want to keep the old discounts for your old pur-
                                           chase orders. In this case, prices will not be recalculated after invoice
                                           control.
                                       •   Correct order PP only up to statistics:
                                           The purchase prices are corrected in the reference order only if the order
                                           still exists in the main database, and has not yet been transferred to statis-
                                           tics.
                                       •   Prod.no. for balancing item:
                                           Opens the Selection dialog to allocate a balancing item for rounding differ-
                                           ences.
                                            “Selection (prod. no. for balancing item)” on page D-218
3.30 / 04-2020




                 A+W Business Purchasing                                                                         D-255
                 Invoice                                                                Software Reference




                           Settings group
                           •   Notification of delivery delay:
                               A message appears if the planned delivery is delayed.
                           •   Suppress automatic allocation:
                               You can enable the checkbox for automatic allocation in the Manual item
                               allocation dialog so that the footer surcharges/discounts from the order
                               confirmation are automatically allocated to a A+W Business product. You
                               can suppress this automatic allocation.
                                “Resolve footer surcharges/discounts automatically in future” on page D-220
                               If this option has been changed, the currently imported document must be
                               reimported.
                                Tutorial, “How to import an XML document” on page D-167
                           •   Trust referencing supplier product numbers:
                               If a A+W Business product number has been entered as a reference in the
                               imported document, the allocation can be made automatically.

                           Xternal group
                           •   Create Xternal-XML file:
                               An XML file is created for electronic data exchange.
                           •   Xternal settings:
                               Opens the Settings dialog to set XML export defaults. This function is avail-
                               able only if the Create Xternal XML file option is enabled.
3.30 / 04-2020




                 D-256                                                          A+W Business Purchasing
                 Software Reference                                                                                     Invoice




                                            Electronic invoice control – document import
                                            Documents > P.O. > Invoice > Electr. invoice control > Document import tab




                 Fig. D-147   Electronic invoice control – Document import


                                            Use this tab to check the imported invoices. Invoice control can only be com-
                                            pleted successfully if the document status has no errors.
                                             Tutorial, “Export/Import (openTRANS)” on page D-149
                                             Tutorial, “Check the electronic document” on page D-168

                                            Booking type
                                            By choosing one of the options, you define how the electronic document is to
                                            be processed. The options released are based on the document status.
                                            •   Reject:
                                                Choose this option to reject the documents. Invoice control will not be car-
                                                ried out.
                                            •   Accept:
                                                This option causes the invoice control to be accepted. Order confirmation
                                                number, prices, and delivery dates from the imported document will be
                                                saved in the purchase orders. Document history is updated.
                                            •   Create partial delivery:
                                                A (new) partial delivery is created for the items in this document (partial in-
                                                voice) and is booked in the same way as with Accept. The remaining items
3.30 / 04-2020




                                                stay in the original P.O. The status of this P.O. is adapted accordingly. In the
                                                case of a dispatch notification, a partial delivery is generated with this book-
                                                ing type.


                 A+W Business Purchasing                                                                                D-257
                 Invoice                                                                 Software Reference




                           Invoices
                           This list shows all imported invoices. These can also originate from different
                           suppliers.
                           If you select an entry, the reference documents will appear on the P.O.s / par-
                           tial deliveries list.
                           •   Invoice number:
                               Invoice number provided by the supplier.
                           •   Supplier:
                               Name of the supplier.
                           •   Net:
                               Total amount of the delivery.
                           •   VAT:
                               Total VAT for this invoice
                           •   Currency:
                               Currency in which the invoice amount is stated. This is only of interest if you
                               are using a multi-currency system.

                           Display You can restrict the display of documents.

                           Filter settings You can set filters for displaying imported documents.
                            “Filter settings” on page D-221

                           Document status
                           The red or green mark indicates whether inconsistencies were found or not.
                           The options in the Booking type section are blocked or released accordingly.
                           •   No document selected:
                               The document status display cannot be updated because no document has
                               been selected from the list. This entry is not displayed if an invoice has
                               been selected.
                           •   At least one footer surcharge/discount of a P.O. could not be allocated to
                               the document:
                               This entry appears only if an invoice has been selected which shows this
                               kind of error.
                           •   P.O. completely referenced:
                               A red mark means that at least one of the reference items does not fully
                               match the imported invoice. Purchase orders with incomplete references
                               are marked on the list.
                           •   Missing article items in P.O.s:
                               The invoice contains items which are not listed in the purchase order.
                           •   Missing footer surcharges/discounts:
                               Footer surcharges/discounts are not included in the order. Since they are
                               shown on the invoice however, they must exist as P.O. items for invoice
                               control purposes. Missing footer surcharges/discounts must be entered in
                               the purchase order manually.
                           •   Price difference:
3.30 / 04-2020




                               The totals of the purchase order and the invoice are different. The differ-
                               ence is shown as an amount and a percentage in the corresponding fields.




                 D-258                                                           A+W Business Purchasing
                 Software Reference                                                                             Invoice




                                       •   Quantity difference:
                                           The purchase order and invoice contain different item quantities.

                                       [Show document] Opens the document view of the selected document.

                                       P.O.s / partial deliveries
                                       This list shows the reference documents if you have selected an entry in the
                                       Invoices section. Partial deliveries are shown in blue letters.
                                       •   P.O. number:
                                           Number of the purchase order created by A+W Business.
                                       •   Net:
                                           Purchase order total.
                                       •   VAT:
                                           Total VAT for this purchase order.
                                       •   Currency:
                                           Currency shown on the P.O. This is only of interest if you are using a multi-
                                           currency system.
                                       •   Order no.:
                                           Number of the reference order.
                                       •   Customer delivery date:
                                           Date of delivery at the customer.
                                       •   Remark:
                                           If the link between the P.O. and the imported document is incomplete, this
                                           remark may indicate the error.
3.30 / 04-2020




                 A+W Business Purchasing                                                                        D-259
                 Invoice                                                                                 Software Reference




                                            Electronic invoice control – item overview
                                            Documents > P.O.> Invoice > Electr. invoice control > Item overview tab




                 Fig. D-148   Electronic invoice control – Item overview


                                            This tab lets you check the items of the invoice received from your supplier.
                                            The options in the Booking type section are described in connection with the
                                            Document import tab.
                                             “Electronic invoice control – document import” on page D-257

                                            Item overview
                                            The overview lists all items of the invoice. If you select an item, the details are
                                            shown in the Document item and P.O. item sections.
                                            •   Item No.:
                                                Item number from the order confirmation.
                                            •   P.O. number:
                                                Number of the reference purchase order.
                                            •   P.O. item:
                                                Item number from the purchase order.
                                            •   Net documents / Net 1 P.O.:
                                                Item price from the imported order confirmation and purchase order.
                                            •   Quantity document / Qty. 1 P.O.:
3.30 / 04-2020




                                                Item quantity from the imported order confirmation and purchase order.
                                            •   Dimensions document / Dimension 1 P.O.:
                                                Item sizes from the imported order confirmation and purchase order.



                 D-260                                                                           A+W Business Purchasing
                 Software Reference                                                                         Invoice




                                       •   Price difference:
                                           Difference between the columns Net documents and Net P.O.
                                       •   Difference 1 price %:
                                           Price difference in percent.
                                       •   Difference 2 qty.:
                                           Difference between the columns Quantity documents and Quantity P.O.
                                       •   Order no.:
                                           Number of the reference order.
                                       •   Customer delivery date:
                                           Date of delivery at the customer.

                                       Document item, P.O. item
                                       These two sections show details on the item selected in the item overview.
3.30 / 04-2020




                 A+W Business Purchasing                                                                    D-261
                 Invoicing of basic glass                                                              Software Reference




                                            Invoicing of basic glass
                                            Documents > P.O. > Invoicing of basic glass
                                            This function is released only for certain customers.
                                            For basic glass invoicing, the actual surface of model lites is transferred and
                                            calculated instead of the invoiced surface.
3.30 / 04-2020




                 D-262                                                                         A+W Business Purchasing
Purchasing               D

                Section Index




             A+W Business
                 Section Index                                                                    Index




                 Index
                 A                                       – Change supplier D-54
                 A+W B2B Purchasing Service D-157        – Create inquiry D-110
                 Amount difference                       – Enter P.O. item D-52
                 – Electronic document D-156             – Generate P.O. D-66
                 AW CommonBase Service D-157             – Purchase order D-49
                 AWProtocolService D-157
                                                         D
                 B                                       Data exchange D-148
                 Balancing item D-218                    – Document D-149
                 Book                                    – External interface management D-175
                 – Receipt of goods D-125                – Import openTRANS document D-167
                 Booking                                 – Import XML file D-167
                 – Partial delivery D-214                Data export
                 Booking type                            – EDI D-174
                 – Document import D-154                 Date monitoring D-99
                 – Electronic price control D-214        Delivery
                 – Price control D-214                   – Book D-125
                 Box                                     – Partial quantity D-233
                 – Box ID D-235                          – Receipt of goods D-119
                 – Create receipt of goods D-136         – Receipt of goods with OC D-197
                 – Print label D-140                     Delivery date D-85
                 – Receipt of goods D-134, D-228         – Change D-100, D-103
                 – Virtual item number D-236             – Change in order pool D-70
                 Box ID D-134                            – Change in several documents D-106
                 – Settings D-238                        – Check D-103
                 Box P.O.                                – Control and correction D-99
                 – Virtual item number D-45, D-134       – Inform customer D-100
                                                         – OC Supplier D-201
                                                         Difference
                 C
                                                         – Invoice control D-249
                 Change ordered item D-55
                                                         Display
                 Check supplier file D-32
                                                         – Filter in electr. document D-221
                 Company data
                                                         Display conventions D-13
                 – References D-159
                                                         Document D-43
                 – Settings for receipt of goods D-124
                                                         Document exchange D-148
                 – Virtual item number D-45, D-134
                                                         – openTRANS D-149
                 Control
                                                         – References D-152
                 – Check electronic document D-168
                                                         – Services D-157
                 – Check Supplier prices D-144
                                                         – XML file D-149
                 – Incomplete deliveries D-241
                                                         Document import D-153
                 – Quantity discrepancies D-241
                                                         – Booking type D-154
                 – Receipt of Goods D-131
                                                         – Footer surcharges/discounts D-155
                 – Receipt of goods D-239
                                                         – Import openTRANS file D-167
                 – Supplier invoice D-243
                                                         – Import XML file D-167
                 Currency
                                                         – Item allocation D-155
                 – Electronic data exchange D-160
                                                         – Rounding difference D-156
3.30 / 04-2020




                 Customer
                                                         Document status D-215
                 – Individual price D-35
                                                         Documentation
                 Customer order
                                                         – Types D-12


                 A+W Business Purchasing                                                         D-265
                 Index                                                                    Section Index




                 Documents                               I
                 – Order request D-184                   ID number
                 – Purchase Order D-186                  – Box ID D-235
                 – Purchasing D-183                      – Settings D-238
                                                         ID numbers
                 E                                       – In receipt of goods D-134
                 EDI                                     Import document
                 – Data export settings D-175            – Booking type D-214, D-257
                 – Export D-174                          – Check D-168
                 – External interface management D-175   – Document status D-215
                 Electr. document                        – Filter setting D-221
                 – Status D-158                          – Invoice control D-257
                 Electronic data exchange                – Item allocation D-219
                 – Currencies D-160                      – Items D-217
                 – Display D-221                         – P.O.s D-216
                 – Document status D-215                 – Price control D-211
                 – EDI interface (settings) D-175        Individual price D-35
                 – Filter settings D-221                 Inquiry
                 – Interface management D-164            – Create for customer order D-110
                 – Invoice control D-254                 – Create independent P.O. D-113
                 – openTRANS settings D-164              – Create via order pool D-111
                 – Price control D-211                   – For customer item D-108
                 – References D-159                      – Reference D-108
                 Electronic document                     Inquiry (menu) D-184
                 – Allocate item D-171                   Inspection of goods received
                 – Amount difference D-156               – Control
                 – Check D-168                              – Complete deliveries D-239
                 – Create partial delivery D-170         Interface management
                 – Distribute surcharge/discount D-173   – Check supplier data D-175
                 Electronic document exchange D-148      Invoice
                 – Allocate item D-219                   – Check D-144
                 – Company data D-159                    – Different date D-253
                 – Partner master data D-166             Invoice control D-243, D-257
                 – Services D-157                        – BOM D-251
                 – Status definition D-161               – Booking type D-257
                 Electronic invoice control D-254        – Correction D-142
                 ERP WebService D-157                    – Currency D-247
                 Export                                  – Difference D-249
                 – Data export via EDI D-191             – Document status
                 – Document (openTRANS) D-151               – Import document
                 – EDI settings D-175                                  Document status D-258
                 – Purchase order D-193                  – Electr. document D-254
                 – Transfer pool D-194                   – Exchange rate D-247
                 External customer number D-166          – Footer surcharges D-143
                 External interface                      – Imported document D-257
                 – Export (EDI) D-191                    – Item overview D-249, D-260
                 – Transfer pool D-194                   – P.O.s D-246
                                                         – Partial delivery D-257
                 F                                       – Purchasing D-142
3.30 / 04-2020




                 Footer surcharge/discount               Item
                 – Distribute to P.O.s D-220             – Allocate in electr. document D-171, D-219
                 – Import document D-155                 – references D-155



                 D-266                                                        A+W Business Purchasing
                 Section Index                                                                       Index




                 L                                            Order types
                 Label                                        – Reference orders D-43
                 – Print for box   D-140                      – Stock P.O. D-78
                                                              Overview
                                                              – Open deliveries D-241
                 M
                                                              – Receipt of goods D-131
                 Master data
                 – Check company data D-45, D-134, D-159
                 – Check currency D-160                       P
                 – Check price data D-36                      P.O.
                 – Check product data D-25                    – Change supplier D-70
                 – Check status for electr. documents D-161   – Complete receipt of goods D-239
                 – Enter stock size D-27                      – Create from independent inquiry D-113
                 master data                                  – Create independent purchase order D-79
                 – Check supplier data D-31                   – Create stock P.O. D-81
                 Module                                       – Date monitoring D-99
                 – function D-11                              – Delivery date D-63
                                                              – Electr. invoice control D-254
                                                              – Enter box D-81
                 O
                                                              – Independent P.O. D-78
                 OC see also Order confirmation
                                                              – Inspection of goods received D-123
                 OC Supplier D-195
                                                              – Invoice control D-246
                 – Delivery date D-201
                                                              – Price control D-205
                 – Order data D-198
                                                              – Quantity discrepancies D-241
                 – P.O. data D-197
                                                              – Reminder D-86
                 – P.O. items D-199
                                                              – Transfer D-66
                 – Receipt of goods D-196
                                                              P.O. data
                 – Receipt of goods per item D-200
                                                              – OC Supplier D-197
                 openTRANS D-149
                                                              P.O. item
                 – Document export D-151
                                                              – Create OC D-89
                 – Document import D-153
                                                              – Enter in order D-52
                 – Price control D-154
                                                              – Production D-120
                 – Settings D-164
                                                              P.O. order
                 – XML file D-153
                                                              – Order pool D-60
                 Order
                                                              – Price comparison D-62
                 – Supplier per item D-50
                                                              P.O. types
                 Order confirmation
                                                              – Independent P.O. D-78
                 – BOM prices D-210
                                                              Partial delivery
                 – Check prices D-144
                                                              – Create from electr. document D-170
                 – Electr. price control D-211
                                                              – Create receipt of goods D-128
                 – Enter for item D-89
                                                              – Receipt of goods D-121
                 – Enter supplier D-87
                                                              Partial invoice D-257
                 – Price control D-202
                                                              Price
                 – Price per item D-208
                                                              – Check in OC D-91
                 – Purchasing D-85
                                                              – Check invoice D-144
                 – Supplier D-195
                                                              – Individual price D-35
                 Order data
                                                              Price control D-143
                 – OC Supplier D-198
                                                              – BOM D-210
                 Order pool D-60
                                                              – Electr. document D-211
                 – Change supplier D-70
                                                              – Electr. file D-211
                 – Collective purchase order D-65
3.30 / 04-2020




                                                              – Imported document D-214
                 – Compare prices D-72
                                                              – Invoice date D-253
                 – Create inquiry D-111
                                                              – Item D-208
                 Order request D-184


                 A+W Business Purchasing                                                            D-267
                 Index                                                                          Section Index




                 – Item overview D-217                          Q
                 – Order confirmation D-202                     Quantity discrepancies
                 – P.O.s D-205                                  – Check D-131
                 Process
                 – Purchasing D-18
                                                                R
                 Production
                                                                Receipt of goods D-225
                 – Message at receipt of goods D-120
                                                                – Box D-134, D-228
                 Purchase
                                                                – Check default settings D-124
                 – Replenishment D-189
                                                                – Check quantity discrepancies D-131
                 Purchase code
                                                                – Complete D-231
                 – Purchasing, Purchasing
                                                                – Complete P.O.s D-239
                   – Purchase code D-22
                                                                – Control D-131
                 Purchase order D-43, D-85
                                                                – Create D-125
                 – Automatic D-58
                                                                – Create box D-136
                 – Change ordered item D-51, D-55
                                                                – Create partial delivery D-128
                 – Collective purchase order D-65
                                                                – Display incomplete deliveries D-131
                 – Customer order D-49
                                                                – Enter completely D-126
                 – Electr. price control D-211
                                                                – Enter with automatic box ID D-136
                 – Enter manually D-79
                                                                – ID for box D-235
                 – Enter mixed P.O. D-81
                                                                – Inspection of goods received D-123
                 – Export (document) D-191
                                                                – Partial delivery D-121
                 – Foreign currency D-143
                                                                – Partial quantity D-233
                 – Manual D-43
                                                                – Production date D-134
                 – Order confirmation D-85
                                                                – Quantity discrepancies D-241
                 – Partial delivery D-257
                                                                – Search for open purchase orders D-126
                 Purchase Order (menu) D-186
                                                                – Setting for ID D-134
                 Purchase order from customer order D-49
                                                                – Status D-119
                 Purchasing
                                                                – Stock P.O. D-119
                 – Basic Ideas D-17
                                                                – Sub-item (boxes) D-235
                 – Check company data D-159
                                                                – Surplus D-122
                 – Check company data (boxes) D-134
                                                                – With manual box ID D-139
                 – Check company data for purchase order D-45
                                                                – Without stock code D-121
                 – Check currency master data D-160
                                                                receipt of goods
                 – Check interface management D-175
                                                                – Status D-40
                 – Check process master data D-36
                                                                Reference order D-43
                 – Check product master data D-25
                                                                References
                 – Check status for electr. documents D-161
                                                                – Upon document import D-152
                 – Check supplier master data D-31
                                                                Remind supplier D-223
                 – Delivery date D-85
                                                                Reminder
                 – Documents D-183
                                                                – Delivery D-95
                 – Inquiry D-108, D-184
                                                                Rounding difference D-156
                 – Invoice control D-142
                                                                – Product allocation D-218
                 – Menu overview D-14
                 – P.O. transfer from order D-58
                 – Price controls D-141                         S
                 – Price lists D-35                             Save purchase price D-143
                 – Process D-18                                 Services
                 – Procurement type D-23                        – A+W B2B Purchasing Service D-157
                 – Purchase order D-188                         – AW CommonBase Service D-157
                                                                – AWProtocolService D-157
3.30 / 04-2020




                 – Scheme D-17
                 – Status D-39                                  – ERP WebService D-157
                 – Status allocation D-39                       Settings
                                                                – Box ID D-238


                 D-268                                                               A+W Business Purchasing
                 Section Index                               Index




                 Standard supplier D-32
                 Status
                 – Allocation at receipt of goods D-40
                 – Assignment for electr. documents D-158
                 – Electronic document exchange D-161
                 – Puchase orders D-39
                 – Receipt of goods D-119
                 Stock article
                 – Stock size D-27
                 Stock evaluation D-143
                 Stock P.O.
                 – Box D-134, D-228
                 – Receipt of goods D-119
                 Stock size
                 – Enter in master data D-27
                 – Stock article D-27
                 Sub-item
                 – Receipt of boxes D-235
                 Supplier
                 – Change in order pool D-70
                 – Change in P.O. item D-54
                 – Check price in OC D-91
                 – Compare prices D-72
                 – Create collective OC D-93
                 – Create OC D-87
                 – For order item D-50
                 – Issue reminder for delivery D-95
                 – Master data D-30
                 – Price comparison D-62
                 Supplier file D-30
                 – Standard supplier D-32
                 Supplier invoice
                 – Check D-144
                 – Check imported invoice D-168
                 – Control D-243
                 Surcharge/discount
                 – Allocation D-155
                 – Distribute to P.O.s D-173
                 Surplus
                 – Receipt of goods D-122

                 T
                 Total difference
                 – Product allocation   D-218
                 Transfer
                 – P.O. D-66

                 V
                 Virtual item number D-134, D-236
3.30 / 04-2020




                 – Company data D-45, D-134




                 A+W Business Purchasing                    D-269
                 Index              Section Index
3.30 / 04-2020




                 D-270   A+W Business Purchasing

