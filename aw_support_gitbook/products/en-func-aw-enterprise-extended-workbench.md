---
title: "EN FUNC A+W Enterprise Extended Workbench"
category: "functional_descriptions"
product: "A+W Enterprise Extended Workbench"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Enterprise Extended Workbench"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Enterprise – Extended Workbench                                   english 1. Content 1.   Content                                                               3 2.   Notes on this Document                                                4      2.1. Trademarks                                                       4      2.2. Copyrights                                                       4      2.3. Disclaimer of liability"
source_file: "EN-FUNC-A+W Enterprise Extended Workbench.pdf"
---


# EN FUNC A+W Enterprise Extended Workbench

     Functional Description


A+W Enterprise – Extended
Workbench




                              english
1. Content
1.   Content                                                               3
2.   Notes on this Document                                                4
     2.1. Trademarks                                                       4
     2.2. Copyrights                                                       4
     2.3. Disclaimer of liability                                          4
3.   Performance Description                                               5
     3.1. Data                                                             5
     3.2. Description                                                      5
     3.3. Requirements                                                     5
     3.4. List of functions                                                5
     3.5. Restrictions                                                     6
          3.5.1. A+W Enterprise                                            6
          3.5.2. A+W Production                                            7
          3.5.3. Master Data                                               8
     3.6. Notes                                                            8
4.   Contact Address                                                       9




A+W Software GmbH         EN-FUNC-A+W Enterprise Extended Workbench.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The content of the documentation serves only as
information and can be changed without prior notice at any time. The text and illustrations were
compiled with the utmost care. However it is not possible to exclude errors completely. A+W
Software GmbH assumes no liability for errors or imprecise statements unless these can be traced
back to intentional or negligent actions.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2018, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation can be copied, completely or in part, saved in
an archiving system, or transferred in any other form only in accordance with our license
agreement. Transmission of the documentation is not allowed, neither electronically, nor
mechanically, nor by recording or in any other way, without the written prior approval of A+W
Software GmbH.


2.3. Disclaimer of liability
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




A+W Software GmbH         EN-FUNC-A+W Enterprise Extended Workbench.docx                            4
3. Performance Description
3.1. Data

 Product                A+W Enterprise
 Module number
 Module                 Extended workbench
 Brief description      Ordered processings in A+W Enterprise
 Available              A+W Enterprise 6 / A+W Production 6


3.2. Description
At many companies, there are individual processings that the company cannot do itself. Things
begin with production, then the goods are transported to a processor who does the processing.
After that, the goods are transported back and the further processing is done in-house at the
company.
This process was already supported in the earlier version in ALCIB-PMS. Now the "extended
workbench" is also available in some cases to an extended extent in interplay between A+W
Enterprise and A+W Production.


3.3. Requirements
   •   A+W Enterprise and A+W Production Version 6.3 are assumed.
   •   The module variable in A+W Enterprise must be activated.
   •   The use of the A+W processing type catalog is assumed (described below as STD
       processing).
   •   The use assumes particular master data.


3.4. List of functions
The extended workbench serves in interplay between A+W Enterprise and A+W Production to
transfer individual or several processings to another processor without generating individual
orders for these and including the following steps:
   •   Triggering of a correctly-scheduled purchase order
   •   Organization of the transport out and back via the dispatch control
   •   Goods receipt in A+W Enterprise / A+W Production -> continuation of production
The procedure has the advantages:
   •   There is only one order in production



A+W Software GmbH        EN-FUNC-A+W Enterprise Extended Workbench.docx                         5
    •   The relationship between the BOM parts provided and the goods receipt after successful
        processing can be traced easily in A+W Production
    •   The work plan for the order can be regarded as a whole so that the scheduling and
        backlog tracing happen with the same tools as for production orders


3.5. Restrictions
3.5.1. A+W Enterprise
Order entry
For the person entering the order, little changes with the extended workbench. Adjusting the
procurement types of glass in the order and thus triggering purchase orders is one of the basic
functions of our ERP system.
In the past, the procurement type of a processing could be changed in order to order the
processing outside the site, for example.
For such processing, the glass to be provided is also incorporated into the order generation. Here,
an important restriction should be noted:
All externally ordered processings per BOM level must absolutely be ordered from only one
supplier. The glass itself, as well as other subparts from the entire BOM can, if necessary, be
ordered elsewhere.
This results in the important characteristics:
    •   Within the BOM level, you can have any processings performed externally, as long as you
        specify the same supplier
    •   The sequence of entry plays no role here
    •   The external processings must be done in a block
To simplify and for a better overview, adherence to a sensible processing sequence in A+W
Production is recommended.
An additional processing intermediate packaging can be inserted in front of these processings if it
is necessary for the cost calculation. However, this is not necessary for the sequence.
In order to generate a correct purchase order, you need appropriate master data.
The order processing including order generation in the background is now handled by the
background process INTAUF. Here no new item per processing is created; instead, there is an
attempt to combine the processings ordered per sheet. For this reason, the sequence of the
processings entered plays a decisive role. This order item includes the complete branch of the
BOM beginning with the processed glass up to the last ordered processing from the same
supplier. All elements of the BOM that are not on procurement type=purchase order will be
marked as included. The item ordered takes over the item number from the table 'bestbeaartzu'
and the designation from the processed glass from the order
A direct delivery from one supplier to another can also be guaranteed by the process. This is
controlled via the delivery address.
In the shipping control, the purchase order for the external processings can also be booked. The
manner of these bookings depends on the system settings:


A+W Software GmbH         EN-FUNC-A+W Enterprise Extended Workbench.docx                           6
There are 4 possibilities:
    •   only goods receipt
    •   outgoing goods + goods receipt. outgoing goods for all that have a date for the supplier
    •   only incoming goods, but only for items with ordered processings
    •   outgoing goods + goods receipt only for items with ordered processings
The date for goods delivery to the supplier is reported from production and accepted by A+W
Enterprise.
Goods receipt for the glass delivered back including the processings orders is done in shipping
control. After successful missing quantity check, a complete goods receipt can be reported for the
purchase order.
With the key combination <Shift+F8> it is possible to visualize the components in shipping.
Printing dispatch papers
It is intended that in dispatch, you should be able to output both loading lists as well as advance
delivery notes using the normal interfaces. For the reports required for this, please ask your A+W
contact person. The report adjustments are not included in the scope of the module.


3.5.2. A+W Production
Scheduling
The order information, such as procurement type and supplier number, is required for scheduling
in production and machine assignment.
Depending on the BOM configuration, additional processings are generated, insofar as they were
not entered in the order.
    •   Packaging for external processing in order to provide the glass to be processed
    •   Packaging for an externally generated processing in order to provide glass for contract
        tempering, contract lamination, and contract insulation
    •   Optional: goods receipt after external processing in order to indicate that a product
        returns after processing and should be quality checked.
Then the scheduling runs and the dates found are reported back to A+W Enterprise.
Before glass can be processed further externally, it must be provided and packed for transport if
necessary.
Previously, both delivery work processes (packaging and shipping) as well as goods receipt were
processes mastered in production as start point of the production. New is now that glass returns
again to production after shipping and the glass is processed before goods receipt.
The existing process for ignoring the BOM for purchased glass and reporting of the 'shipping' as
progress report for the shipping control is retained in A+W Production now as before.
A new processing type '1805 - intermediate packing for external processing' was included in the
A+W processing catalog. It offers the following technical possibilities:
    •   Query of date pairs for provision and return of the glass and consideration in the
        scheduling



A+W Software GmbH            EN-FUNC-A+W Enterprise Extended Workbench.docx                           7
    •   Consideration of the provision date for the purchase order proposal generation
    •   Display of provision dates in the shipping control
    •   Reporting of glass as 'provided' from production to shipping control
The processing 'intermediate packing for external processing' can be transferred with the order or
generated artificially in A+W Production. In both cases, the processing sequence is not
determined by the item master data, but corrected by A+W Capacity Planner before scheduling so
that the provision processing takes place immediately before the fits external processing. If a
generated processing should be produced externally (contract tempering, contract lamination,
contract insulation), intermediate packing is generated as last processing on the BOM level below.
Processing sequences
The processing sequence is specified in A+W Production based on the master data of the
processing item and (if nothing was found there) from the processing types. Only after that is the
entry sequence of the ERP considered in order to map specialties such as screen printing
sequences.
For the management of ordered processings, it must be considered that for a sequence, either all
processing items are ordered or all processing items themselves are worked through. The
background of this limitation is that the processing 'intermediate packaging' has a sequence that
is 1 smaller than the first ordered processing by BOM branch.


3.5.3. Master Data
For successful work with the "extended workbench" module, appropriate master data and some
system settings are required both in A+W Enterprise and in A+W Production. They include:
    •   Configuration of ordered processings
    •   Adjustments in the item master data (procurement type and supplier details for
        processings to be ordered externally)
    •   Adjustment in MZO
    •   New processing types and items
    •   Checking of the transfer times for goods receipts
    •   New text operations and formulas
    •   New work processes for external processing
For detailed configuration including master data adjustment, contact the responsible A+W
employee.


3.6. Notes




A+W Software GmbH        EN-FUNC-A+W Enterprise Extended Workbench.docx                              8
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH      EN-FUNC-A+W Enterprise Extended Workbench.docx   9

