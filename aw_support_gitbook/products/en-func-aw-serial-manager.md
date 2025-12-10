---
title: "EN FUNC A+W Serial Manager"
category: "functional_descriptions"
product: "A+W Serial Manager"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Serial Manager"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Serial Manager                                   english 1. Notes on this Document This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The content of the documentation serves only as information and can be changed without prior notice at any time. The greatest care was used in compiling the texts and figures. However it is not possible to exclude errors completely. A+W S"
source_file: "EN-FUNC-A+W Serial Manager.pdf"
---


# EN FUNC A+W Serial Manager

     Functional Description


A+W Serial Manager




                              english
1. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The content of the documentation serves only as
information and can be changed without prior notice at any time. The greatest care was used in
compiling the texts and figures. However it is not possible to exclude errors completely. A+W
Software assumes no liability for errors or imprecise statements unless these can be traced back
to intentional or negligent actions.


1.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


1.2. Copyrights
© 2016, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies
and translation. The documentation may only be copied whole or in part, stored in an archiving
system or transmitted in any other form in accordance with the license agreement. Without the
prior written permission of A+W Software GmbH, the documentation may not be transmitted
electronically, by recording or in any other form.


1.3. Exclusion of liability
A+W Software GmbH assumes no liability for data errors that rely on basic principles of the
standard functions made available by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to change software data, structure, and interfaces as part
of program expansions without prior announcement. All adjustments, expansions, database
queries, reports, analyses, and interface expansions that were created individually for our
customers and/or machines and software partners as well as all costs and efforts associated with
these were borne by the client (customers, machine and software partners). This includes also any
necessary long-term costs and efforts for the expansion and adjustment of subsequent program
versions. This is necessary in order to ensure that the adjustments/expansions commissioned that
were undertaken/developed for a version will also work perfectly and be used in the subsequent
version.




A+W Software GmbH                  EN-FUNC-A+W Serial Manager.docx                                  3
2. Contents
1.   Notes on this Document                                          3
     1.1. Trademarks                                                 3
     1.2. Copyrights                                                 3
     1.3. Exclusion of liability                                     3
2.   Contents                                                        4
3.   Performance Description                                         5
     3.1. Data                                                       5
     3.2. Description                                                5
     3.3. Requirements                                               5
     3.4. List of functions                                          5
     3.5. Limitations                                                6
     3.6. Notes                                                      6
4.   Contact Address                                                 7




A+W Software GmbH                  EN-FUNC-A+W Serial Manager.docx       4
3. Performance Description
3.1. Data
 Product                  A+W Production
 Module number            220017
 Module                   A+W Serial Manager
 Brief description        It is possible to execute serial bookings with the A+W
                          Barcode Manager
 Available                Starting with A+W Production 5.1


3.2. Description
In the FDC for individual lites, each lite of a BOM is assigned a unique barcode. In contrast to this,
in the quantity FDC for a BOM element, only a single barcode is assigned. The advantage of the
quantity FDC is that the data quantity in the database is reduced drastically for orders with large
quantities. Thus the performance during the initialization after the scheduling and during
bookings is improved considerably. FDC for individual lites and quantity FDC can be used in
combination, in that only orders starting with a configurable quantity are handled with the
quantity FDC.


3.3. Requirements
FDC bookings must be set off with a quantity, the specification of the label is not sufficient. For
this an A+W Production Terminal Order is required, here the quantity to be booked can be
entered for a quantity label.


3.4. List of functions
With the installation of the A+W Production Terminal, a station of the A+W Production Terminal
Order is available, which is suitable for the quantity FDC. Here a batch, an order number or a
quantity label can be entered. The production progress is displayed and the quantity to be
produced can be entered and booked. It is displayed how many lites of a quantity label have
already booked which processings.
The FDC display in A+W Production is also suitable for quantity FDC.
Orders with quantity FDC can be processed in the A+W Realtime Optimizer with the standard
Panorama cutting and the A+W Realtime Optimizer Light without limitation.




A+W Software GmbH                  EN-FUNC-A+W Serial Manager.docx                                    5
3.5. Limitations
The quantity FDC is only supported by A+W Production Terminal Order, not by other versions of
the A+W Production Terminal.
The quantity FDC is not supported by scanners (A+W Barcode Manager).
For bookings it is only specified how many lites of a part are produced or reported broken. It is
not specified where the lites to be booked are located. Therefore, in contrast to FDC for individual
lites, no reliable information is possible about how many lites of a part are currently at which
registration point and on which rack.
For DynOpt 2, no orders with quantity FDC can be processed in the A+W Realtime Optimizer since
for the quantity FDC no unique lite barcode is assigned. Similarly, processing is not possible if in
the A+W Realtime Optimizer a Panorama model that deviates from the standard one is stored,
which executes a precise-to-the-lite identification via the barcode.
Due to the different depiction of orders for the quantity FDC and orders of the FDC for individual
lites in the database, joint evaluations with reports are only possible to a limited extent.


3.6. Notes




A+W Software GmbH                 EN-FUNC-A+W Serial Manager.docx                                    6
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Serial Manager.docx   7

