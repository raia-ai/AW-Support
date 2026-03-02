---
description: "EN FUNC A+W Barcode Manager (EL)"
---



# EN FUNC A+W Barcode Manager (EL)

     Functional Description


A+W Barcode Manager (EL)




                              english
1. Content
1.   Content                                                               3
2.   Notes on this Document                                                4
     2.1. Trademarks                                                       4
     2.2. Copyrights                                                       4
     2.3. Exclusion of liability                                           4
3.   Performance Description                                               5
     3.1. Data                                                             5
     3.2. Description                                                      5
     3.3. Requirements                                                     5
     3.4. List of functions                                                6
     3.5. Limitations                                                      7
     3.6. Notes                                                            7
4.   Contact Address                                                       8




A+W Software GmbH                  EN-FUNC-A+W Barcode Manager (EL).docx       3
2. Notes on this Document
This documentation and the software it describes is only distributed with a license and may only
be used and copied according to this license. The contents of the documentation are only
informative and are subject to changes without prior notice. The text and illustrations were
compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH
assumes no liability for errors or imprecise statements unless these can be traced back to
intentional or negligent actions.


2.1. Trademarks
All hardware and software names mentioned in this documentation might also be registered
trademarks or other property rights of third parties. The property rights of third parties must be
observed.


2.2. Copyrights
© 2019, A+W Software GmbH, all rights reserved, including the right of reprint, the production of
copies and of the translation. The documentation may only be copied whole or in part, stored in
an archiving system or transmitted in any other form in accordance with the license agreement.
Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by
recording or in any other way, without the written prior approval of A+W Software GmbH.


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




A+W Software GmbH              EN-FUNC-A+W Barcode Manager (EL).docx                                 4
3. Performance Description
3.1. Data
 Product                   A+W Business / A+W Business Pro
 Module number             210101 / 230101
 Module                    A+W Barcode Manager (EL)
 Brief description         Module for direct, wireless barcode booking
 Available                 Starting with A+W Business v5 / A+W Business Pro v5


3.2. Description
As a fully integrated entry-level solution, the A+W Barcode Manager (EL) can be used in
connection with latest Android scanners for direct, wireless barcode booking.
The actual program runs on a terminal server which connects with the scanner via remote
desktop. The scanner sends all registered data to the currently active data field as keyboard
entries.
The scans are directly written into the database and the user receives direct feedback as to
whether the data input was successful. The following processes are supported:
    •   Receipt of goods
    •   Stock bookings
    •   Rack contents
    •   Breakage reports
    •   Completion reports


3.3. Requirements
    •   A+W Business / A+W Business Pro
    •   Android scanner with current RDP client
    •   Terminal Server




A+W Software GmbH              EN-FUNC-A+W Barcode Manager (EL).docx                            5
3.4. List of functions
After the user has logged in successfully with his personal barcode, he arrives at the main menu.
From here, the following processes can be started:

Booking of goods received

Scan the barcodes of the purchased items for which goods have been received.
This way, the quantities received, boxes, and their content can be corrected if they deviate from
the purchase order.

Stock booking

Additions to and removals from stock can be booked and rebookings can be made in this area.
After the barcode for the stock location has been read, the barcode for the stock item can be read
and the respective quantity entered for the incoming or outgoing booking.
When rebooking stock items, first the stock ID of the item is scanned and the current stock
displayed. Then comes the entry of the quantity to be rebooked and then the new storage
location to which it should be booked.
The A+W Barcode Manager (EL) also has the following five functions for boxes:
    •   Remove sheets: Use this function to reduce the sheet count in a box. For this, first a box
        bar code is scanned, and after that, the quantity displayed is set to the new value.
    •   Decomposing boxes: With this function you can decompose a box. That is, the box is
        deleted and the remaining sheets are booked to stock. For this, first a box is scanned and
        after that, its content can be edited.
    •   Change stock location of boxes: You can use this function to change the stock location of a
        box. For this, first a box is scanned and after that, the bar code of the new storage
        location is entered.
    •   Put box on inventory list: Use this function to place a box on the current inventory list.
        After the box has been scanned, the new storage location can be scanned. After both
        scans have been completed, the current quantity of the sheets in the box can still be
        edited.
    •   Withdrawal of goods: With this function, boxes with ident number can be assigned to an
        order item. First the barcode of an order item is scanned. After that, the number of sheets
        in the box is determined by scanning the box barcode. It can be edited accordingly.




A+W Software GmbH              EN-FUNC-A+W Barcode Manager (EL).docx                                 6
Racks

Rack booking was developed for shipping. The following conditions must be adhered to:
    •   Rack numbers must be unique. You can therefore not create a rack with the same number
        but a different rack type. If the same number is used, a letter should precede the rack
        number (e.g. for the rack type).
    •   When booking racks, the width and the height of the rack is checked and the loading
        weight is checked. These values can be adjusted per rack type.
    •   Since rack booking was developed for shipping, only main items can be added to a rack.
    •   The only racks that can be loaded are those which are not booked for off site, have not
        been reported lost and are not locked.

Completion report

The dialog can be used to change the status of an order item. When an order item has been
scanned, enter the quantity to be reported complete. The program will always preset the full item
quantity. After saving, the data record is processed by the AIS and the status of the order adjusted
if necessary.
Additionally, the bookings are logged and can be evaluated in the booking history.

Breakage report

The dialog can be used to change the status of order items, but only negatively, in contrast to the
completion report.
The reason for breakage and causer can be entered directly in the scanner or scanned if
necessary. After booking a record, the information on the last booking is shown as a summary on
the scanner.
The respective barcodes can be printed out in the programs complaint reason and complaint
creator using the labels form.
Breakage reports may reduce the order status. Additionally, the bookings are logged and can be
evaluated in the booking history.


3.5. Limitations

3.6. Notes
For further processing of the breakage reported (reproduction) in A+W Business Pro, the for-fee
additional module A+W Barcode Manager (EL) - Glass Remake Manager (230105) is required.




A+W Software GmbH              EN-FUNC-A+W Barcode Manager (EL).docx                              7
4. Contact Address
A+W Software GmbH

Siemensstraße 3

35463 Fernwald

Germany

Tel. +49 641 96620-0



E-mail: info@a-w.com

Internet: http://www.a-w.com/




A+W Software GmbH           EN-FUNC-A+W Barcode Manager (EL).docx   8

