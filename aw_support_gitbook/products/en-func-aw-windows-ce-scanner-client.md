---
title: "EN FUNC A+W Windows CE Scanner Client"
category: "functional_descriptions"
product: "A+W Windows CE Scanner Client"
doc_type: "Functional Description"
language: "EN"
tags: ["FUNC", "A+W Windows CE Scanner Client"]
version: "1.0"
last_updated: "2025-12-10"
description: "Functional Description   A+W Windows CE Scanner Client                                     english 1. Content 1.   Content                                                              3 2.   Notes on this Document                                               4      2.1. Trademarks                                                      4      2.2. Copyrights                                                      4      2.3. Disclaimer of liability                                         4 3."
source_file: "EN-FUNC-A+W Windows CE Scanner Client.pdf"
---


# EN FUNC A+W Windows CE Scanner Client

     Functional Description


A+W Windows CE Scanner Client




                                english
1. Content
1.   Content                                                              3
2.   Notes on this Document                                               4
     2.1. Trademarks                                                      4
     2.2. Copyrights                                                      4
     2.3. Disclaimer of liability                                         4
3.   Performance Description                                              5
     3.1. Data                                                            5
     3.2. Description                                                     5
     3.3. Requirements                                                    5
          3.3.1. Software                                                 5
          3.3.2. Hardware (Scanner)                                       6
     3.4. List of functions                                               6
     3.5. Limitations                                                     8
          3.5.1. Hardware                                                 8
          3.5.2. Software                                                 8
     3.6. Notes                                                           8
4.   Contact Address                                                      9




A+W Software GmbH            EN-FUNC-A+W Windows CE Scanner Client.docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only be
used and copied according to this license. The content of the documentation serves only as
information and can be changed without prior notice at any time. The text and illustrations were
compiled with the utmost care. However it is not possible to exclude errors completely. A+W
Software GmbH assumes no liability for errors or imprecise statements unless these can be traced
back to intentional or negligent actions.


2.1. Trademarks
All hardware and software designations mentioned in the documentation can also be registered
trademarks or other industrial property rights of third parties. The property rights of third parties
must be observed.


2.2. Copyrights
© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation may only be copied whole or in part, stored in
an archiving system or transmitted in any other form in accordance with the license agreement.
Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by
recording or in any other way, without the written prior approval of A+W Software GmbH.


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




A+W Software GmbH           EN-FUNC-A+W Windows CE Scanner Client.docx                             4
3. Performance Description
3.1. Data
 Product               A+W Production
 Module number 872505
 Module                CIM Barcoding Client
 Brief                 Web-based scanner application for bookings in production
 description
 Available             Starting with A+W Production v6


3.2. Description
The CIM-Barcoding Client is a Web-based scanner application. The application supported by A+W
Production offers the following advantages:
    •   The application works regardless of the scanner hardware
    •   All you need is a WLAN connection and Internet-Explorer 6 on the scanner
    •   Easy configuration: Only a shortcut is required on the desktop, no software must be
        installed on the scanner)
    •   Also saves the data in Offline mode
    •   Direct reporting in case of booking errors


3.3. Requirements
3.3.1. Software
In order to be able to work with the CIM-Barcoding Client, the following infrastructure setups
must be installed anywhere in the network (normally the process server). The "A+W
Infrastructure Process Server" contains these setups.
    •   A+W Infrastructure 6 Collector Services
    •   A+W Infrastructure 6 Middleware
    •   A+W Infrastructure 6 Service Locator
    •   A+W Infrastructure 6 Services
    •   A+W Infrastructure 6 Web
    •   A+W Infrastructure 6 Workflow Studio
In addition, the following setups must be installed to run the scanner software (usually also on the
process server):


A+W Software GmbH           EN-FUNC-A+W Windows CE Scanner Client.docx                            5
    •   A+W Infrastructure 6 Collector Services
    •   A+W Infrastructure 6 Middleware
    •   A+W CIM 6 Barcoding Services
    •   A+W CIM 6 Web
    •   A+W Planning 6 Job Services


3.3.2. Hardware (Scanner)
The Windows CE scanners used must fulfill at least the following minimum requirements:
    •   Windows CE 6.0
    •   Internet Explorer 6.0
    •   Display: 240 x 320 pixels
    •   WiFi-capable


3.4. List of functions
The interface of the CIM-Barcoding Client presents itself as follows on the scanner:




The fields above the dotted line display the booking results, the fields below the last scanned bar
code.


 Symbol                         Description

                                    • Black field: number of non-processed bookings (of
                                      AlcimBooking)
                                    • Green field: number of successfully processed bookings
                                    • Red field: number of incorrect bookings




A+W Software GmbH           EN-FUNC-A+W Windows CE Scanner Client.docx                                6
                                Number of entries saved in the scanner as a result of Offline
                                mode

                                Last scanned barcode


                                Currently registered person


                                Dynamic, either the registration point, the rack or the status



During the booking, the CIM-Barcoding Client checks directly whether the booking sequence was
adhered to correctly. If that is the case, the CIM-Barcoding Client indicates this after a complete
booking sequence with a green screen background. In case of incorrect booking sequence, the
error icon appears.




                  = impermissible booking sequence.
Examples of an incorrect booking sequence:
    •   No person was logged in on the scanner
    •   Impermissible bookings such as <Begin><Person>.
Additional icons on the display provide the user with information about correct or incorrect
operation:




               = Barcode is transferred to the server




             = Connection to Barcoding Service interrupted




A+W Software GmbH           EN-FUNC-A+W Windows CE Scanner Client.docx                                7
3.5. Limitations
3.5.1. Hardware
The CIM-Barcoding Client was tested with the following devices:

    •   Datalogic Memor X3 (A+W Standard)
    •   Motorrola Psion Omnii XT15
    •   Motorola MC9190G


3.5.2. Software
    •   In order to prevent possible data loss, we recommend not doing more than 50 scans in
        offline mode.
    •   Breakage bookings are not possible with the use of the A+W Serial Manager with the CIM-
        Barcoding Client .


3.6. Notes
A database license is required per scanner.
A+W employees will be glad to tell you about possible accessories (docking station, battery, etc.).




A+W Software GmbH           EN-FUNC-A+W Windows CE Scanner Client.docx                            8
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH        EN-FUNC-A+W Windows CE Scanner Client.docx   9

