---
title: "EN FUNC A+W Smart Terminal"
category: "functional_descriptions"
product: "A+W Smart Terminal"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Smart Terminal"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Smart Terminal                                   english 1. Contents 1.   Contents                                                         3 2.   Notes on this Document                                           4      2.1. Trademarks                                                  4      2.2. Copyrights                                                  4      2.3. Disclaimer of liability                                     4 3.   Performance Description"
source_file: "EN-FUNC-A+W Smart Terminal.pdf"
---


# EN FUNC A+W Smart Terminal

     Functional Description


A+W Smart Terminal




                              english
1. Contents
1.   Contents                                                         3
2.   Notes on this Document                                           4
     2.1. Trademarks                                                  4
     2.2. Copyrights                                                  4
     2.3. Disclaimer of liability                                     4
3.   Performance Description                                          5
     3.1. Data                                                        5
     3.2. Description                                                 5
     3.3. Requirements                                                5
     3.4. List of functions                                           6
     3.5. Limitations                                                 7
     3.6. Notes                                                       7
4.   Contact Address                                                  8




A+W Software GmbH                   EN-FUNC-A+W Smart Terminal.docx       3
2. Notes on this Document
This documentation and the software described in it are only licensed and may only be used and
copied pursuant to this license. The contents of the documentation are for information purposes
only and are subject to changes without prior notice. The text and illustrations were compiled with
the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be
held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent
action.


2.1. Trademarks
All hardware and software names mentioned in this documentation may also be registered
trademarks or other industrial property rights held by third parties. Copyrights of third parties
must be complied with.


2.2. Copyrights
© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation can be copied, completely or in part, saved in
an archiving system, or transferred in any other form only in accordance with our license
agreement. Transmission of the documentation is not allowed, neither electronically, nor
mechanically, nor by recording or in any other way, without the written prior approval of A+W
Software GmbH.


2.3. Disclaimer of liability
A+W Software GmbH does not assume any liability for data errors resulting from the basics of the
standard functions provided by Microsoft, Unix or other software and hardware suppliers.
A+W Software GmbH reserves the right to perform changes to software data, structure and
interfaces as part of program extensions without prior notice. All amendments, extensions,
database queries, reports, analyses, and interface extensions which have been individually
created for our customers and/or machine and software partners as well as all related costs and
expenses are to be borne by the customer (customers, machine and software partners). This also
includes possibly necessary long-term costs and expenses for amending and extending
subsequent program versions. This is necessary to make sure that the commissioned
amendments/extensions which have been made or developed for a version will work flawlessly
and can be used in the successor version.




A+W Software GmbH                  EN-FUNC-A+W Smart Terminal.docx                                  4
3. Performance Description
3.1. Data
 Product                   A+W Production
 Module number             220090
 Module                    A+W Smart Terminal
 Brief description         Web-based interface for bookings in production
 Available                 Starting with A+W Production v6


3.2. Description
The A+W Smart Terminal is a Web-based interface and allows the user to make simple bookings:
frame to a registration point or sheet on rack. Here it is possible to search through the existing
frame/registration points/states. After entry of the first character, you can select from a menu.
The A+W Smart Terminal can be operated on a suitable mobile device.




                                                                   .


3.3. Requirements
The A+W Smart Terminal requires the following components:
    •   SOA infrastructure service
    •   CIM Barcoding Service
    •   CIM Web
    •   Production Booking Engine / Service

A+W Software GmbH                 EN-FUNC-A+W Smart Terminal.docx                                    5
   •   Current browser with activated Javascript and cookies


3.4. List of functions
The following bookings are possible and must be selected accordingly:

 Symbol            Description




                   Unit to rack




                   Unit to registration point




                   Rack to registration point




                   Status to registration point




                   Status to unit




A+W Software GmbH                   EN-FUNC-A+W Smart Terminal.docx     6
                    Status to rack




After selecting the booking type, the corresponding data are entered in the respective fields and
booking is made.
The three fields in the top section of the dialog show the booking results:




Black field: number of non-processed bookings (of AlcimBooking)
Green field: number of successfully processed bookings
Red field: number of incorrect bookings


3.5. Limitations
Data must be entered here manually and can NOT be scanned.
A+W Smart Terminal does NOT support the A+W Serial Manager!


3.6. Notes
The minimum resolution for mobile devices (tablets) is 385 x 420 pixels. Smartphones are not
suitable for this application.




A+W Software GmbH                    EN-FUNC-A+W Smart Terminal.docx                                7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH               EN-FUNC-A+W Smart Terminal.docx   8

