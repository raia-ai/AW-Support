---
description: "EN-AWBusiness-BarcodeManagerEL"
---


# A+W Barcode Manager (EL)

---
## Introduction and Editorial

This part of the documentation contains editorial notes.

### Revision Overview

| Version/Date | Description |
| :--- | :--- |
| 1.00/03-2023 | Original version, transfer from docx document |

### Editorial

The editorial provides information on the following topics:
- Notes on this Document
- Copyrights
- Trademarks
- Contacts

#### Notes on this Document
This document is intended for end users of A+W Business.

The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of A+W Business.

#### Copyrights
© 2017, A+W Software GmbH, all rights reserved, also those for reprinting, the making of copies and translation.

The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

#### Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### Contacts

**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim

- **Phone:** +49 6404 2051-0
- **Fax:** +49 6404 2051-877
- **Email:** zentrale@a-w.com
- **Web:** http://www.a-w.com

## System Introduction

Online shop floor data collection via barcode scanner is done by a Windows-CE based scanner supplied by Datalogic (Scorpio). The actual program runs on a terminal server which connects with the scanner via remote desktop. The scanner sends all registered data to the currently active data field as keyboard entries.

To make sure that the barcoding program starts automatically when the scanner is registered at the terminal server, you need to copy a link to the barcoding program for the user to an autostart group. The program to be linked is called `abcscanner.exe` and is found in the A+W Business program directory (e.g. C:\Program Files\A+W\ALFAK 2011\Program\German). Before starting the program, the A+W Business start program must be run once on the computer, and the correct database connection must be entered in the login dialog. From that point on, the program will always connect to the database using the actual information.

The automatic start up of the program can be set by means of a configuration program (A+W Business 5 Scanner AutoStart Config) in the start menu ConfigTools from A+W Business 5.5 update 3 in the start menu Config Tools. In this program the scanner program (language dependent) can be selected for the currently registered user so that the program is started whenever the user logs in.

## Settings

### Scanner

The scanner can be configured on any terminal. First, install the configuration software that comes with the scanner on a PC, then connect the scanner via USB. Now start the configuration software (Datalogic Configuration Utility).

_Abb. A-1: Completeness of barcode reading_

In the program, first set **Postamble** in the menu **Hw Configuration > Laser > Parameters > Reader Parameters > Text Formatting**. Just enter a tabulator. There are two ways of entering the tabulator. You can either enter a tabulator in an editor (e.g. Notepad or Word) and copy it to the data field by copy and paste. Alternatively, press the ALT key, and keep pressing it while entering on the number block the digits 0 0 9 before releasing the ALT key.

At the end of every scan, a [TAB] will be sent to the barcoding program to signalise that this barcode has been registered.

_Abb. A-2: Code 39 setting_

The second and last setting is **CheckEvaluation** in the menu **Hw Configuration > Laser > Parameters > Reader Parameters > Code39 > Standard**. This must be set to **Enabled** so that the check digits of the Code39 barcodes will be checked instead of being sent to the program as valid data.

### Registration points in A+W Business

**Path:** Production > Registration points - production

_Abb. A-3: Registration points - Production_

This dialog serves to enter This is required for the receipt of goods and for completion reports. If the registration point has been clearly allocated to the barcode type (in the above illustration e.g. for receipt of goods), the user does not have to register the registration point at the scanner if the corresponding program point is selected.

### Management of Employees in A+W Business

_Abb. A-4: Management of employees - setting_

In user management, you need to enter the personnel numbers of the users who are going to register with the scanner by means of their personnel barcode.

### Interface Service

To book completion reports via scanner, the registered completion reports are buffered in the database before being processed by AIS. To make sure that AIS can assign these bookings, it is necessary to define the entity name of AIS as „sysadm".

This is default after installation. This setting must be checked if more than one entity of AIS is installed.

### Capacity planning

**Path:** Capacity planning > Master data > Organization > Machines

_Abb. A-5: Allocation of machines for registration points_

If completion reports are to be booked in A+W Business capacity planning, a unique registration point must be entered for the machine in question. This is done in machine management, in Capacity planning > Master data > Organization > Machines. The work type to be used is always registered via barcode.

## Functions

The individual barcoding dialogs and their function are listed below.
- "Login"
- "Main menu"
- "Receipt of goods"
- "Production report"
- "Stock Movements"
- "Racks"
- "Miscellaneous"

### Login

**Scanner-Start**
_Abb. A-6: Barcoding - Registration via employee barcode39 setting_

After the user has registered successfully, the program proceeds to the main menu. From there you can go to the corresponding dialogs to enter receipt of goods, inventory bookings, rack load, or completion reports. See "Main menu".

### Main menu

**Path:** Scanner > Main menu

_Abb. A-7: Barcoding - main menu_

You can access the following functions from the scanner's main menu:
- "Receipt of goods"
- "Production report"
- "Stock Movements"
- "Racks"
- "Miscellaneous"

Use the [Back] option to return to the previous dialog.

### Receipt of goods

**Path:** Scanner > Main menu > Receipt of goods

_Abb. A-8: Barcoding - Receipt of goods_

Scan the barcodes of the purchased items for which goods have been received.

When the purchased item's barcode has been scanned, enter the quantity received (via keyboard). The program shows the full quantity for the purchased item by default; this has to be changed only if the quantity received is different. If no change is necessary, scan the barcode of the next purchased item. The program will collect these scans without actually booking them. This is only done if you press the ENTER key on the scanner or scan the barcode of another P.O. If you press the BACK key or the ESC key while there are purchased items in the memory which have not been booked so far, the program will want to know whether these shall be booked now.

If the just scanned P.O. item is a box, you can scan a box ID barcode right afterwards and change the contents of the box if necessary. The program automatically enters a quantity of 1 piece which cannot be changed. For boxes with an ID you can enter different contents.

After a purchased item has been scanned, the bottom quantity field shows the number of articles ordered, and the number of articles received.

### Production report

**Path:** Scanner > Main menu > Production report

_Abb. A-9: Barcoding - Production report_

The completion and breakage reports are found in the Production report sub-menu, which replaces the previous completion report in the scanner main menu.
- "Completion report"
- "Breakage report"

#### Completion report

**Path:** Scanner > Main menu > Production report > Completion report

_Abb. A-10: Barcoding - Production report_

The completion report dialog can be used to change the status of an order item. All scans which are made here are first saved in the database then processed by AIS as STSD reports. Status changes of orders will be made afterwards. For details on configuring the AIS for STSD reports please refer to the previous chapter.

When an order item has been scanned, enter the quantity to be reported complete. The program will always preset the full item quantity. Press ENTER to save the completion report. The record is then processed by AIS, and the order status is amended if necessary. If only one piece is to be processed per scan, you can select the option "Quantity=1". If this option is enabled, when scanning a barcode 1 piece is immediately booked as complete. No additional quantity has to be entered nor the enter button pressed.

The breakage report dialog can be used to change the status of orders, but only negatively, in contrast to the completion report.

#### Breakage report

**Path:** Scanner > Main menu > Production report > Breakage report

_Abb. A-11: Barcoding - breakage report_

Operating and booking work in the same way as the completion report, but it is possible to include the breakage reason and creator. These can be selected either by pressing the button on the scanner or by using the barcode. The barcodes can be printed out in the programs complaint reason and creator using the labels form.

After booking a record, the information on the last booking is shown as a summary on the scanner.

### Stock Movements

**Path:** Scanner > Main menu > Stock movements

_Abb. A-12: Barcoding - Stock movement menu_

Before starting an inventory booking, please define whether goods shall be added or withdrawn. In addition, the menu for boxes is accessible from here.
- "Stock Withdrawal"
- "Addition to stock"
- "Transfer"
- "Boxes"

#### Stock Withdrawal

**Path:** Scanner > Main menu > Stock movement > Withdrawal

_Abb. A-13: Barcoding - stock withdrawal_

The next dialog works the same way for incoming and outgoing stock. After the stock location barcode has been read, the stock article bar code can be read and the respective quantity entered for the incoming or outgoing booking. By pressing the ENTER key, the booking is made directly.

#### Addition to stock

**Path:** Scanner > Main menu > Stock movement > Addition

_Abb. A-14: Barcoding - addition to stock_

(This function works similarly to Stock Withdrawal)

#### Transfer

**Path:** Scanner > Main menu > Stock movement > Transfer

_Abb. A-15: Barcoding - Select stock location_

Under the stock movement menu element, there is now also the function transfer. If you select it, you must first scan a stock location bar code.

_Abb. A-16: Barcoding - Transferring stock item_

After that, you land on the dialog for transferring stock items. Here the user must scan a stock item, that is, the stockID of a stock item, whereupon the current inventory is displayed. Now you should first define the quantity that should be transferred.

_Abb. A-17: Barcoding - Successful transfer_

Here the user can specify a new stock location and make the booking. A success report appears on the screen.

#### Boxes

**Path:** Scanner > Main menu > Stock movement > Boxes

_Abb. A-18: Barcoding - Box warehouse menu_

Starting with A+W Business version 12.5, there is also a Boxes submenu available. With this menu, you can call the following three functions:
- "Change box content"
- "Resolve boxes"
- "Change storage location of boxes"
- "Put box to inventory"
- "Shipping of boxes"

##### Change box content

**Path:** Scanner > Main menu > Stock movement > Boxes > Change content

_Abb. A-19: Barcoding - Change box content_

Use this function to reduce the sheet count in a box. For this, first a box barcode is scanned, and after that, the quantity displayed is set to the new value. By pressing the Enter key, the booking is made.

##### Resolve boxes

**Path:** Scanner > Main menu > Stock movement > Boxes > Resolve

_Abb. A-20: Barcoding - Box warehouse menu_

**Decomposing boxes**
With this function you can decompose a box (that is, the box is deleted and the remaining sheets are booked to stock). For this, first a box is scanned and after that, its content can be edited. By pressing the Enter key, the booking is made.

##### Change storage location of boxes

**Path:** Scanner > Main menu > Stock movement > Boxes > Change storage location

_Abb. A-21: Barcoding - Box warehouse menu_

You can use this function to change the stock location of a box. For this, first a box is scanned and after that, the bar code of the new storage location is entered. The booking is then triggered immediately.

##### Put box to inventory

**Path:** Scanner > Main menu > Stock movement > To inventory list

_Abb. A-22: Barcoding - Put box on inventory list_

Use this function to place a box on the current inventory list. After the box has been scanned, the new storage location can be scanned. After both scans have been completed, the current quantity of the sheets in the box can still be edited. By pressing the Enter key, the booking is made.

##### Shipping of boxes

**Path:** Scanner > Main menu > Stock movement > Boxes > Shipping of boxes

_Abb. A-23: Barcoding - Shipping of boxes_

With this function, boxes with ident number can be assigned to an order item. Initially, an order item barcode must be scanned. After that, the number of lites in the box is determined by scanning the box barcode. It can be edited accordingly. By pressing the Enter key, the booking is made.

### Racks

In order for racks to be able to be processed, the following conditions have to be checked beforehand:
- Rack numbers have to be unique. You can therefore not create a rack with the same number but a different rack type. If the same number is used, a letter should precede the rack number (for the rack type).
- When booking racks, the width and the height of the rack is checked and the loading weight is checked. These values can be adjusted per rack type.
- Rack booking was developed for shipping, i.e. only main items can be added to a rack.
- The only racks that can be loaded are those which are not booked for off site, have not been reported lost and are not locked.
- Point 5 ensures that the allocation of the rack is fully backed at rack exit.

#### Overview of rack menu

**Path:** Scanner > Main menu > Racks

_Abb. A-24: Barcoding - Racks menu_

In submenu racks, there are the functions:
- "Load racks"
- "Empty racks"
- "Display racks"

#### Load racks

**Path:** Scanner > Main menu > Racks > Loading

_Abb. A-25: Barcoding - loading racks_

For loading racks, the rack to be loaded first has to be selected. When scanning the rack barcode, you can add the order item to the rack in the next dialog.

_Abb. A-26: Barcoding - loading racks - order items_

After the successful selection of a rack, you can add the order item to the rack. Two different modes are supported hereby, those with the buttons "Quantity = 1" and "Input quantity". The currently set mode is highlighted in green.

The T2 bar code must be used to add order items.

In the mode "Input quantity" after the item barcode has been scanned, the quantity that has not yet been loaded onto the racks is shown. This can then be edited if a smaller number is to be loaded. Pressing the enter button on the scanner confirms the booking.

In the mode "Quantity = 1", the booking is executed directly after scanning the order item barcode. Only 1 piece is booked hereby.

The result of the last booking is always shown in the window "Last booking".

To exchange the racks, press the Back button and then select a different rack.

#### Empty racks

**Path:** Scanner > Main menu > Racks > Empty

_Abb. A-27: Barcoding - empty racks_

With this dialog, a rack can be reported empty. In this process, all allocations of the order items placed on the rack before are deleted.

> **No backup query**
> There is no confirmation query when emptying racks.

#### Display racks

**Path:** Scanner > Main menu > Racks > Display

_Abb. A-28: Barcoding - display racks_

With this dialog, the current allocation of order items on a rack can be displayed. If a rack barcode is scanned, the order items with the respective loaded quantity are shown in the allocation window. In addition, the customer number is also output. The list contains six entries. You can browse with the forward and backward button.

### Miscellaneous

**Path:** Scanner > Main menu > Miscellaneous

The menu Miscellaneous includes the dialogs for order item information, registration information, and change of user.
- "Order Information"
- "Login information"
- "Change employee"

#### Order Information

**Path:** Scanner > Main menu > Miscellaneous > Order information

_Abb. A-29: Barcoding - order information_

When an item barcode has been scanned, order item information will show the item name, item size, quantity, quantity delivered, price per price unit, and the delivery date.

#### Login information

**Path:** Scanner > Main menu > Miscellaneous > Login information

_Abb. A-30: Barcoding - miscellaneous_

The registration information dialog shows the currently registered user, the database, the database system (Microsoft SQL Server or Unify SQL Base), the registration point, the machine, and the work type.

#### Change employee

**Path:** Scanner > Main menu > Miscellaneous > Change employee

_Abb. A-31: Barcoding - login_

The dialog to change an employee is described the following section: "Login".
After scanning a valid user code, the present user will be signed out, and the new user registered.

## Barcodes

The individual dialogs and functions require certain barcodes. These are Code39 barcodes with check digit, with an asterisk at the start and at the end.

| Description | Prefix | User data | Example |
| :--- | :--- | :--- | :--- |
| Personnel barcode | PE | The personnel number as per user management | `*PE000000199F*` |
| Registration point barcode without work type for goods received | ES | ID of registration point | `*ES00000000166*` |
| Registration point barcode and work type for completion report | EA | Registration point ID and work type ID separated by a hyphen | `*EA0000000015-101P*` |
| Order bar code for reporting finished and sheet-rack assignment | T2 | Order number + item number (3-digit) + element number (3-digit) | `*T200000243001001%*` |
| Order barcode for order information | D2 or T2 | Order number + item number (3-digit) + element number (3-digit) (only T2) | `*D200000243002Q*` or `*T200000243002001Q*` |
| P.O. barcode for receipt of goods | D5 | P.O. number + item number (3-digit) | `*D50000070650001.*` |
| Box barcode for stock additions and withdrawals | BO | Box ID. Attention: ID must not start by zero! | `*BOBC00002H*` |
| Stock location barcode for inventory booking | LA | Stock location ID | `*LA0000000001W*` or `*L0000000001W*` |
| Stock article barcode for inventory booking | LP | Stock ID of stock article | `*LP0000000164E*` |
| Rack number | GE | Rack number | `*GE9099E*` |
| Reason for complaint | BR | Number of reason of complaint | `*BR1$*` |
| Cause of complaint | BC | Number of cause of complaint | `*BC2P*` |

### Printing barcodes

In the following programs in A+W Business, a barcode printing functionality was implemented for the online plant data recording (via barcode scanner):

- Employee management (Master data > Company > Employees)
- Registration point in production (e.g. Master data > Production > Other > Registration points production)
- Default time (Capacity planning > Master data > Default times > Default times)
- Print program (e.g. Documents > Order > Print order)
- Stock definition (Master data > Stock > Stock definition)
- Stock management (Stock management > Inventory management)
- Racks (Production > Rack management > Racks)
- Reason of complaint (Master data > Products > General > Complaint reason)
- Cause of complaint (Master data > Products > General > Complaint cause)

If the useful data does not exceed the possible data length, the barcodes are filled up with zeros (0) (except rack barcodes). Furthermore, all barcodes received a final test digit. A general print functionality was also installed in the employee management (1). The barcodes contain the personnel number (here 199) of the employee (example: PE000000199F). The registration point barcode (2) is formed from the ID of the registration point (example: ES00000000166). In the default times program (3), the user now has the opportunity to print a registration point barcode with work type for the completion report in the online PDC. This is composed of the ID of the registration point and the ID of the work type separated by a hyphen (example: EA0000000015-101P). The print program for the form printing (4) can print an order barcode (order info in online PDC) or a purchase order barcode (incoming goods in online PDC), effective immediately. This barcode includes the document number, the 3-digit item number, and a 3-digit part number (always 000 since only main items are output here) (example order T200000243002000Q – example purchase order: D50000070650001.). For the stock booking in the PDC, the stock location must be scanned accordingly. For this, on the one hand the barcode printing on the stock definition dialog (5) was reworked and on the other hand, the online PDC was expanded. Effective immediately, the online PDC can process such storage location barcodes with an L-prefix. The barcode includes the ID of the storage location (example: *L0000000001W*). Then, barcodes of the stock items (5) are necessary for the stock booking. In the stock management, the appropriate barcodes, which include the ID of the stock item, can now be printed (example: LP0000000164E). For racks, a list of racks can be selected in rack management (7) and then printed for this barcode (Functions > Print Rack Barcode). As the racks are alphanumeric, they are not filled with leading zeros.

**Note:** All bar codes are written to the report variable F_IDENT_C39 of the respective form/report.

### Booking history

It is now possible to protocol the implemented completion and breakage reports. The switch "fill history table for completion reports" must be activated in the company master data on register 15. Capacity planning to activate the function.

If the switch has been activated, the edited reports are recorded in the table `FS_BOOK_HISTORY`. If the booking is active in the A+W Business capacity planning, the reports will also be recorded when booked in the same way. This also applies for reports performed via the dialog in A+W Business. Otherwise the bookings are recorded in `PD_AWBAR`.

The following data is hereby saved:
- Order number
- Item number
- BOM element
- Time of scanning
- Employee
- Registration point
- Work type (only for booking in capacity planning, otherwise 0)
- Breakage reason (only for breakage reports)
- Cause of breakage (only for breakage reports)
- Booked quantity
- Origin (BDE, manual, implicit)

Furthermore, there is a dialog on analysis of the booking history (Statistics > Booking history). Now the records to be displayed can be filtered via the QBE mode so that precise statistics, e.g. per employee, can be created.

_Abb. A-32: Barcoding - login_

By pressing, the displayed records can also be grouped according to two dynamic criteria, which can also be set in the dialog.
