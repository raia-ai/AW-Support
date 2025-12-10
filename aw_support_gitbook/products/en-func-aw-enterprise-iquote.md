---
description: "EN FUNC A+W Enterprise iQuote"
---



# EN FUNC A+W Enterprise iQuote

     Functional Description


A+W Enterprise - iQuote




                              english
1. Content
1.   Content                                                            3
2.   Notes on this Document                                             4
     2.1. Trademarks                                                    4
     2.2. Copyrights                                                    4
     2.3. Exclusion of liability                                        4
3.   Performance Description                                            5
     3.1. Data                                                          5
     3.2. Description                                                   5
     3.3. Requirements                                                  5
     3.4. List of functions                                             6
     3.5. Limitations                                                   7
     3.6. Notes                                                         7
4.   Contact Address                                                    8




A+W Software GmbH                  EN-FUNC-A+W Enterprise iQuote.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The contents of the documentation are only
informative and is subject to changes without prior notice. The text and illustrations were
compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH
assumes no liability for errors or imprecise statements unless these can be traced back to
intentional or negligent actions.


2.1. Trademarks
All hardware and software names mentioned in this documentation might also be registered
trademarks or other property rights of third parties. The property rights of third parties must be
observed.


2.2. Copyrights
© 2020, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation must be copied, completely or in part, saved, or
transferred only in accordance with our license agreement. Transmission of the documentation is
not allowed, neither electronically, nor mechanically, nor by recording or in any other way,
without the written prior approval of A+W Software GmbH.


2.3. Exclusion of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions which have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions which
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH                EN-FUNC-A+W Enterprise iQuote.docx                                  4
3. Performance Description
3.1. Data
Product               A+W Enterprise
Module number 200100
Module                A+W iQuote (G)
Brief                 Web configurator for glass products
description
Available             Starting with A+W Enterprise v6 - 2019


3.2. Description
A+W iQuote (G) is a Web-based configurator for glass products that offers the customer the
opportunity to calculate and enter quotations and orders online via homepage. The documents
entered with A+W iQuote are available as "classic" A+W Enterprise orders or quotations in A+W
Enterprise after entry. For all orders/quotations in AWE, the same functionalities are available
regardless of whether they were entered manually, via EDI or using A+W iQuote.
The customer can inform himself at any time about the documents he has entered. He has insight
into the order status achieved and can thus see, for example, whether a change to the order is
still possible or for which date delivery is planned.
A+W iQuote can also display all the customer's orders and quotations that were not entered in
A+W iQuote. This way, the customer receives an overview of all orders and quotations that exist
in A+W Enterprise.
This information module is available as a stand-alone module without the A+W iQuote entry
functionality.


3.3. Requirements
The A+W iQuote can only be installed in Microsoft servers with IIS.
The following A+W modules are required:
    •   A+W Enterprise v6 on Linux Redhat ES 6 with Informix database.
    •   A+W Enterprise v6 on AIX with Informix database.

During the configuration, work is required for the:
    •   Creation of the A+W iQuote workflow according to the customer's requirements
            o   A standard workflow is included.
    •   Creation and assignment of the product images.
    •   Addition of the master data in A+W Enterprise.


A+W Software GmbH                EN-FUNC-A+W Enterprise iQuote.docx                                5
3.4. List of functions
Web browser-based product configuration and ordering of simple glass, LSG, TG, insulated glass,
and trade products based on a configurable workflow and display of the CAD sketch for glass and
display of stored product images
   •   Price calculation based on the customer terms (standard prices, discount, and individual
       prices) from A+W Enterprise.
   •   Entry of processings for drilling, edges, mitering, facets, rounded corners, corner cut-
       off/cutouts, edge cutouts, area cutouts, and macro (including programmable macros)
   •   Evaluation of the standard restrictions that are stored in A+W Enterprise.
   •   Explicit release of the products and processings in A+W Enterprise for sale in A+W iQuote.
   •   Freely-definable graphic selection criteria for products (workflow).
   •   Input of the commission and customer item number, as well as the order reference (text)
   •   Entry of additional notes per document
   •   Selection/entry of the delivery address.
   •   Selection of a requested delivery date taking into consideration the customer route
   •   Definition of direct collection or delivery time.
   •   Intermediate storage of the current shopping cart to avoid data loss (automated).
   •   Re-activation of saved entries at any time and on any end user devices.
   •   Display of the quotations and orders in the customer information system (only orders
       entered with A+W iQuote and quotations or all of the customer's A+W Enterprise orders
       and quotations).
   •   Display of the processing status via the customer information system.
   •   Freely-configurable workflow with graphic editor in A+W iQuote. Here, a large selection of
       individual activities (functions), branches, and conditions is made available, which can be
       combined in the graphic editor to form the overall workflow of the configurator.
           o   The workflow is organized as follows:
                       Configuration: Actions during product configuration.
                       Check Out: Completion of the order process with delivery address and
                        requested date
           o   Product type selection.
           o   Product group selection.
           o   Product selection.
           o   Product color selection.
           o   Free selection (according to customer request).
           o   Insulated glass exchange.
           o   Geometry entry (shape selection).
           o   Processing entry.

A+W Software GmbH                EN-FUNC-A+W Enterprise iQuote.docx                                  6
    •   Customer reference/commission.
    •   Shipping address.
    •   Requested date/direct delivery.
    •   Order notes.
    •   A+W iQuote shopping cart individual items displayed with respect to price.
    •   In the check-out area, before saving the order/quotation, all discounts/surcharges are
        displayed.
    •   Installation positions of the glass in the insulated glass exchange can be changed.
    •   Filter for AIR and colors during frame exchange of the insulated glass.
    •   Gas exchange for the insulated glass.
    •   Entry of symmetrical muntins.


3.5. Limitations
The following functionalities are not available:
    •   The exchange in laminated glass BOMs.
    •   Entry of non-symmetrical muntins.
    •   Stepped entry.
    •   No project assignment, therefore, no project prices possible.
    •   Display/download of form printouts such as quotation, order confirmation, delivery note,
        and invoice.
    •   Display/download of document attachments from A+W Enterprise (document attachment
        must be released for A+W iQuote)
    •   Box selection.
    •   Customer information system: Orders/quotations, not entered with A+W iQuote have no
        CAD sketches in the detailed view.


3.6. Notes
The installation of A+W iQuote can be done in-house or at a hoster; here it must be noted that
the services must always be installed in-house. This means that the hoster must establish a VPN
connection to the in-house network. If everything is installed in-house, the IIS must be in a DMZ
and be secured with a firewall.




A+W Software GmbH                 EN-FUNC-A+W Enterprise iQuote.docx                                7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Enterprise iQuote.docx   8

