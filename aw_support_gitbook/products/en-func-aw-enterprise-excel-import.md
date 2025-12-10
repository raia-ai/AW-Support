---
title: "EN FUNC A+W Enterprise Excel Import"
category: "functional_descriptions"
product: "A+W Enterprise Excel Import"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Enterprise Excel Import"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Enterprise Excel import of items                                    english 1. Contents 1.   Contents                                                                 3 2.   Notes on this Document                                                   4      2.1. Trademarks                                                          4      2.2. Copyrights                                                          4      2.3. Exclusion of liability"
source_file: "EN-FUNC-A+W Enterprise Excel Import.pdf"
---


# EN FUNC A+W Enterprise Excel Import

      Functional Description


A+W Enterprise
Excel import of items




                               english
1. Contents
1.   Contents                                                                 3
2.   Notes on this Document                                                   4
     2.1. Trademarks                                                          4
     2.2. Copyrights                                                          4
     2.3. Exclusion of liability                                              4
3.   Performance description                                                  5
     3.1. Data                                                                5
     3.2. Description                                                         5
     3.3. Requirements                                                        5
     3.4. List of functions                                                   5
     3.5. Restrictions                                                        6
     3.6. Notes                                                               7
4.   Contact Address                                                          8




A+W Software GmbH                  EN-FUNC-A+W Enterprise Excel Import.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The contents of the documentation are only
informative and are subject to changes without prior notice. The text and illustrations were
compiled with the utmost care. However it is not possible to exclude errors completely. A+W
Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to
wilful or grossly negligent action.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2021, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies
and translation. The documentation may only be copied whole or in part, stored in an archiving
system or transmitted in any other form in accordance with the license agreement. The
documentation may not be transmitted electronically, by recording or in any other form without
the prior written permission of A+W Software GmbH.


2.3. Exclusion of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All amendments, extensions, database
queries, reports, analyses, and interface extensions which have been individually created for our
customers and/or machine and software partners as well as all related costs and expenses are to
be borne by the customer (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary to make sure that the commissioned amendments/extensions that
have been made or developed for a version will work flawlessly and can be used in the successor
version.




A+W Software GmbH              EN-FUNC-A+W Enterprise Excel Import.docx                             4
3. Performance description
3.1. Data
 Product                   A+W Enterprise
 Article no.               200018
 Module                    Excel Line Item Import
 Brief description         Import of line items from the MS Excel clipboard
 Available                 Starting with A+W Enterprise v6 QR 04/19


3.2. Description
The Excel Line Item Import module enables the import of order items that are transferred by the
customer as Excel file.
There are 2 types of takeover supported:
    •   Takeover of item dimensions for an article defined in the A+W Enterprise order entry.
    •   Takeover of a complete order with reference to articles or customer article numbers. That
        is, in addition to the dimensions, the article numbers are also included in the Excel file.
The takeover is accomplished in the following steps:
    •   Marking of the data to be taken over in Excel and copying to the clipboard
    •   Assignment of the columns to the fields of the item
        The Excel format used by the customer can be saved and reused for the next import. A
        renewed assignment of the columns to the field of the item is thus no longer necessary
    •   Takeover of the data on the import dialog
    •   If necessary, there can be an addition to/manipulation of the data transferred
    •   Takeover of the items in the order
Analogous to the manual input of the items, prices are calculated and restrictions and dates
checked. If conflicts arise during the takeover of the items, the corresponding items are marked
for reprocessing (Infostatus).




3.3. Requirements
    •   A+W Enterprise (core module)


3.4. List of functions
    •   Transfer of the data from the clipboard to a screen table

A+W Software GmbH             EN-FUNC-A+W Enterprise Excel Import.docx                             5
   •   Editing and selection of the data to be imported on the Import dialog
   •   Generation of the new items in the current document including price calculation and
       restriction check.




3.5. Restrictions
   •   Maximum 900 lines:
       If the clipboard contains more than 900 lines, the import is terminated after 900 lines.
   •   Maximum 80 characters column width:
       If a field contains more than 80 characters, the content is shortened accordingly.
   •   Maximum 10 columns
   •   Empty lines are skipped
   •   The import is restricted to the following fields:
           o   Customer item
           o   Sequential item
           o   Article number (A+W Enterprise - article)
           o   Customer article
           o   Quantity
           o   Width
           o   Height
           o   AIR
           o   AIR2
           o   Reference
   •   The data is expected in the metric system.



A+W Software GmbH             EN-FUNC-A+W Enterprise Excel Import.docx                            6
3.6. Notes




A+W Software GmbH   EN-FUNC-A+W Enterprise Excel Import.docx   7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-Mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH          EN-FUNC-A+W Enterprise Excel Import.docx   8

