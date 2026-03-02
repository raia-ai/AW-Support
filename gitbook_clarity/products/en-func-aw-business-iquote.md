---
description: "EN FUNC A+W Business iQuote"
---



# EN FUNC A+W Business iQuote

     Functional Description


A+W iQuote (G)




                              english
1. Content
1.   Content                                                      3
2.   Notes on this Document                                       4
     2.1. Trademarks                                              4
     2.2. Copyrights                                              4
3.   Performance Description                                      5
     3.1. Data                                                    5
     3.2. Description                                             5
     3.3. Requirements                                            5
     3.4. List of functions                                       6
     3.5. Limitations                                             7
     3.6. Notes                                                   8
4.   Contact Address                                              9




A+W Software GmbH              EN-FUNC-A+W Business iQuote.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only be
used and copied according to this license. The contents of the documentation are only informative
and are subject to changes without prior notice. The text and illustrations were compiled with the
utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for
errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2015, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation may only be copied, in whole or in part, saved in
an archiving system, or transferred in any other form only in accordance with our license
agreement. Transmission of the documentation is not allowed, neither electronically, nor
mechanically, nor by recording or in any other way, without the written prior approval of A+W
Software GmbH.

Exclusion of liability
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




A+W Software GmbH                 EN-FUNC-A+W Business iQuote.docx                                 4
3. Performance Description
3.1. Data
 Product                 A+W iQuote (G)
 Module number           200100
 Module
 Brief description       Web configurator for glass products
 Available               V6.4 available as of 08/25/2017


3.2. Description
A+W iQuote (G) is a Web-based configurator for glass products that offers the customer the
opportunity to calculate and enter quotations and orders 24/7 online himself via his homepage.
The creation of quotations and orders and the transformation of a quotation into an order are
supported. The documents are available immediately after entry in the commercial system and
can be scheduled via workflow in production and capacity planning, including sending an order
confirmation automatically via e-mail. The degree of automatic processing is determined by the
workflow.
The customer can inform himself at any time about the documents he has entered, as long as
they have not been processed further and thus blocked for changes. He has insight into the order
status achieved and can thus decide whether a change of the order is still possible or not since it
is already blocked.
Optionally, A+W iQuote can display the document history for quotations and orders that were not
entered in A+W iQuote. Thus the customer maintains an overview of all his documents.
Documents not entered in A+W iQuote can only be displayed.
There is an option to display document attachments, and these available for download by the
user. This also applies for the form printouts that were created and approved with the Crystal
Report service.
This way, A+W iQuote becomes a customer information system for all of the customer's current
business documents.
The info module can be operated regardless of the A+W iQuote configuration


3.3. Requirements
The system can only be installed in Microsoft servers with IIS
The following A+W modules are required:
    •   A+W Business 5.5 or v6 (always the latest patch) on SQL Server database
    •   A+W Infrastructure Reporting Service (for form display)



A+W Software GmbH                 EN-FUNC-A+W Business iQuote.docx                                5
During the configuration, work is required for the:
    •   Creation of the A+W iQuote workflow according to the customer's requirements
    •   Creation of the product images
    •   Reworking of the master data in A+W Business


3.4. List of functions
Browser-based product configuration and ordering of simple glass, LAMI, TG, insulated glass, and
trade products based on a configurable workflow and display of the CAD sketch for glass and
display of stored product images
    •   Price calculation based on the customer terms (standard prices, discount, and individual
        prices) from A+W Business including all price customizing possibilities
    •   Entry of processings for drilling, edges, mitering, facets, rounded corners, corner cut-
        off/cut-outs, edge cut-outs, area cut-outs, and macro (including programmable macros)
    •   Definition of input limits for processing parameters and definition of permissible values
        for rounded corners.
    •   Selection of the permissible processing based on the product or geometry
    •   Explicit release of the products in A+W Business for sale in A+W iQuote
    •   Free sorting of the products displayed by defined sequence number
    •   Selection of the products to be displayed by product number, type, group
    •   Freely-definable graphic selection criteria for products
    •   Display of expl. released stock dimensions and boxes including stock availability indication
        (traffic light system)
    •   Input of the commission and customer item number, as well as the order reference (text)
    •   Entry of additional notes per document
    •   Entry/selection of the delivery address
    •   Selection of a requested delivery date taking into consideration the customer route
    •   Definition of direct collection or delivery time
    •   Storage of the current configuration during entry and thus cancellation and restoration at
        any time on any end user device
Display of the document history for quotations and orders as customer information system.
    •   Display of the document status for all status points released in A+W Business
    •   Display of the item documents including the item price
    •   Display/download of document header attachments from A+W Business (document
        attachment must be released for A+W iQuote)
    •   Display/download of form printouts such as quotation, order confirmation, delivery note,
        and invoice (only with use of the Crystal Report form printout in A+W Business)



A+W Software GmbH                  EN-FUNC-A+W Business iQuote.docx                                 6
Freely-configurable workflow with graphic editor in A+W iQuote. Here, a large selection of
individual activities (functions) is made available, which can be combined in the graphic editor to
form the overall workflow of the configurator. Branches and conditions can be used here.
The workflow is organized in 3 parts:
    •   Check In: Actions that are undertaken before product configuration
    •   Configuration: Actions during product configuration.
    •   Check Out: Completion of the order process with delivery address and requested date
The following functions are available for selection:
    •   Product type selection
    •   Product group selection
    •   Product selection
    •   Stock dimension/box selection
    •   Product color selection
    •   Free selection (according to customer request)
    •   Insulated glass exchange
    •   Geometry entry (shape selection)
    •   Processing entry
    •   Customer reference/commission
    •   Shipping address
    •   Requested date/direct delivery
    •   Order notes


3.5. Limitations
One A+W iQuote is always assigned to precisely one ERP site. A+W iQuote is thus not multi-site
capable. An individual A+W iQuote (own URL) is required for each site. These can then be stored,
e.g. as link on the company home page site-specifically.
The following functions are not available:
    •   A+W iQuote does not support the price calculation by order total quantities; these can
        only be calculated after completion in A+W Business. A+W iQuote always displays the
        price of an individual item.
    •   The exchange in LAMI BOMs is not supported
    •   Entry of muntins is not supported
    •   Hardware with macro entry is not supported
    •   Coating sides cannot be changed
    •   Display of the terms (discount, price per quantity unit)
    •   Display of the explicit BOM prices


A+W Software GmbH                  EN-FUNC-A+W Business iQuote.docx                                   7
    •   No consideration of project prices


3.6. Notes
The installation of A+W iQuote can be done in-house or at a hoster; here it must be noted that
the services must always be installed in-house. This means that the hoster must establish a VPN
connection to the in-house network. If everything is installed in-house, the IIS must be in a DMZ
and be secured with a firewall.




A+W Software GmbH                 EN-FUNC-A+W Business iQuote.docx                                  8
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Business iQuote.docx   9

