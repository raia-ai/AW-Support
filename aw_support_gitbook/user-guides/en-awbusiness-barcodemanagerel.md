---
description: "EN AWBusiness BarcodeManagerEL"
---



# EN AWBusiness BarcodeManagerEL

Barcode Manager (EL)       A




                           Deutsch




                  A+W Business
                                                                                                             Introduction




                                       Introduction
                                       This part of the documentation contains editorial notes.


                                       Revision Overview
                                       Version/Date     Description

                                       1.00/03-2023     Original version, transfer fromdocx document



                                       Editorial
                                       The editorial provides information on the following topics:
                                       •   Notes on this Document
                                       •   Copyrights
                                       •   Trademarks
                                       •   Contacts

                                       Notes on this Document
                                       This document is intended for end users of A+W Business.
                                       The documentation and software described are licenses that must be used or
                                       copied only in accordance with the conditions of our license agreement. The
                                       contents of the documentation are only informative and are subject to changes
                                       without prior notice. The text and illustrations were compiled with the utmost
                                       care. However it is not possible to exclude errors completely. A+W Software
                                       GmbH cannot be held liable for errors or inaccuracies, unless they can be at-
                                       tributed to wilful or grossly negligent action.
                                       This document describes the full scope of A+W Business.

                                       Copyrights
                                       © 2017, A+W Software GmbH, all rights reserved, also those for reprinting, the
                                       making of copies and translation.
                                       The documentation may only be copied whole or in part, stored in an archiving
                                       system or transmitted in any other form in accordance with the license agree-
                                       ment. Transmission of the documentation is not allowed, neither electronically,
                                       nor mechanically, nor by recording or in any other way, without A+W Software
                                       GmbH's prior written approval.

                                       Trademarks
                                       All hardware and software designations mentioned in the documentation can
                                       also be registered trademarks or other industrial property rights of third parties.
1.00 / 03-2023




                                       The property rights of third parties must be observed.




                 A+W Business Barcode Manager (EL)                                                                   A-3
                 Introduction




                                Contacts
                                A+W Software GmbH

                                Am Pfahlgraben 4-10

                                D-35415 Pohlheim

                                   +49 6404 2051-0

                                   +49 6404 2051-877

                                zentrale@a-w.com

                                http://www.a-w.com
1.00 / 03-2023




                 A-4                                   A+W Business Barcode Manager (EL)
                                                                                                                                                       Contents




                                       Contents
                                       Introduction ............................................................................................................. A-3
                                         Revision Overview ............................................................................................... A-3
                                         Editorial ............................................................................................................... A-3

                                       Introduction                                                                                                          A-7
                                       Introduction ............................................................................................................. A-9
                                       Settings ................................................................................................................. A-10
                                         Scanner ............................................................................................................. A-10
                                         Registration points in A+W Business ................................................................ A-12
                                         Management of Employees in A+W Business .................................................. A-13
                                         Interface Service ............................................................................................... A-13
                                         Capacity planning ............................................................................................. A-14
                                       Functions .............................................................................................................. A-15
                                         Login .................................................................................................................. A-15
                                         Main menu ......................................................................................................... A-16
                                         Receipt of goods ............................................................................................... A-17
                                         Production report ............................................................................................... A-18
                                            Completion report .......................................................................................... A-19
                                            Breakage report ............................................................................................. A-20
                                         Stock Movements .............................................................................................. A-21
                                            Stock Withdrawal ........................................................................................... A-22
                                            Addition to stock ............................................................................................. A-23
                                            Transfer .......................................................................................................... A-24
                                            Boxes ............................................................................................................. A-26
                                         Racks ................................................................................................................ A-32
                                            Overview of rack menu .................................................................................. A-32
                                            Load racks ..................................................................................................... A-33
                                            Empty racks ................................................................................................... A-35
                                            Display racks .................................................................................................. A-36
                                         Miscellaneous .................................................................................................... A-37
                                            Order Information ........................................................................................... A-37
                                            Login information ........................................................................................... A-38
                                            Change employee .......................................................................................... A-38
                                       Barcodes ............................................................................................................... A-39
                                          Printing barcodes ............................................................................................. A-40
                                         Booking history .................................................................................................. A-41

                                       Partindex                                                                                                          A-43
                                       Index ..................................................................................................................... A-45
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                                                              A-5
                 Contents
1.00 / 03-2023




                 A-6        A+W Business Barcode Manager (EL)
Barcode Manager (EL)           A

                       Introduction




                  A+W Business
                 Introduction                                                                               Introduction




                                       Introduction
                                       Online shop floor data collection via barcode scanner is done by a Windows-
                                       CE based scanner supplied by Datalogic (Scorpio). The actual program runs
                                       on a terminal server which connects with the scanner via remote desktop. The
                                       scanner sends all registered data to the currently active data field as keyboard
                                       entries.
                                       To make sure that the barcoding program starts automatically when the scan-
                                       ner is registered at the terminal server, you need to copy a link to the barcoding
                                       program for the user to an autostart group. The program to be linked is called
                                       abcscanner.exe and is found in the A+W Business program directory (e.g.
                                       C:\Program Files\A+W\ALFAK 2011\Program\German). Before starting the
                                       program, the A+W Business start program must be run once on the computer,
                                       and the correct database connection must be entered in the login dialog. From
                                       that point on, the program will always connect to the database using the actual
                                       information.
                                       The automatic start up of the program can be set by means of a configuration
                                       program (A+W Business 5 Scanner AutoStart Config) in the start menu Con-
                                       figTools from A+W Business 5.5 update 3 in the start menu Config Tools. In
                                       this program the scanner program (language dependent) can be selected for
                                       the currently registered user so that the program is started whenever the user
                                       logs in.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                  A-9
                 Settings                                                                     Introduction




                            Settings
                            Scanner
                            The scanner can be configured on any terminal. First, install the configuration
                            software that comes with the scanner on a PC, then connect the scanner via
                            USB. Now start the configuration software (Datalogic Configuration Utility). In
                            the program, first set Postamble im Menü Hw Configuration > Laser > Param-
                            eters > Reader Parameters > Text Formatting. Just enter a tabulator. There
                            are two ways of entering the tabulator. You can either enter a tabulator in an
                            editor (e.g. Notepad or Word) and copy it to the data field by copy and paste.
                            Alternatively, press the ALT key, and keep pressing it while entering on the
                            number block the digits 0 0 9 before releasing the ALT key.
                            At the end of every scan, a [TAB] will be sent to the barcoding program to sig-
                            nalise that this barcode has been registered.




                            Abb. A-1     Completeness of barcode reading


                            The second and last setting is CheckEvaluation in menu Hw Configuration >
                            Laser > Parameters > Reader Parameters > Code39 > Standard. This must
                            be set to Enabled so that the check digits of the Code39 barcodes will be
                            checked instead of being sent to the program as valid data.
1.00 / 03-2023




                 A-10                                              A+W Business Barcode Manager (EL)
                 Introduction                                                                                       Settings




                                       Abb. A-2      Code 39 setting


                                       The second and last setting is CheckEvaluation in menu Hw Configuration > La-
                                       ser > Parameters > Reader Parameters > Code39 > Standard. This must be set to En-
                                       abled so that the check digits of the Code39 barcodes will be checked instead of being
                                       sent to the program as valid data.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                     A-11
                 Settings                                                                                      Introduction




                                          Registration points in A+W Business
                                          Production > Registration points - production




                 Abb. A-3   Registration points - Production


                                          This dialog serves to enter This is required for the receipt of goods and for
                                          completion reports. If the registration point has been clearly allocated to the
                                          barcode type (in the above illustration e.g. for receipt of goods), the user does
                                          not have to register the registration point at the scanner if the corresponding
                                          program point is selected.
1.00 / 03-2023




                 A-12                                                             A+W Business Barcode Manager (EL)
                 Introduction                                                                                         Settings




                                       Management of Employees in A+W
                                       Business




                                       Abb. A-4      Management of employees - setting


                                       In user management, you need to enter the personnel numbers of the users
                                       who are going to register with the scanner by means of their personnel bar-
                                       code.


                                       Interface Service
                                       To book completion reports via scanner, the registered completion reports are buffered
                                       in the database before being processed by AIS. To make sure that AIS can assign
                                       these bookings, it is necessary to define the entity name of AIS as „sysadm“.
                                       This is default after installation. This setting must be checked if more than one entity
                                       of AIS is installed.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                       A-13
                 Settings                                                                                   Introduction




                                          Capacity planning
                                          Capacity planning > Master data > Organization > Machines




                 Abb. A-5   Allocation of machines for registration points


                                          If completion reports are to be booked in A+W Business capacity planning, a
                                          unique registration point must be entered for the machine in question. This is
                                          done in machine management, in Capacity planning > Master data > Organi-
                                          zation > Machines. The work type to be used is always registered via barcode.
1.00 / 03-2023




                 A-14                                                           A+W Business Barcode Manager (EL)
                 Introduction                                                                                  Functions




                                       Functions
                                       The individual barcoding dialogs and their function are listed below.
                                        “Login” auf Seite A-15
                                        “Main menu” auf Seite A-16
                                        “Receipt of goods” auf Seite A-17
                                        “Production report” auf Seite A-18
                                        “Stock Movements” auf Seite A-21
                                        “Racks” auf Seite A-32
                                        “Miscellaneous” auf Seite A-37



                                       Login
                                       Scanner-Start




                                       Abb. A-6      Barcoding – Registration via employee barcode39 setting


                                       After the user has registered successfully, the program proceeds to the main
                                       menu. From there you can go to the corresponding dialogs to enter receipt of
                                       goods, inventory bookings, rack load, or completion reports.
                                        “Main menu” auf Seite A-16
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                 A-15
                 Functions                                                                  Introduction




                             Main menu
                             Scanner > Main menu




                             Abb. A-7     Barcoding - main menu


                             You can access the following functions from the scanner's main menu:
                              “Receipt of goods” auf Seite A-17
                              “Production report” auf Seite A-18
                              “Stock Movements” auf Seite A-21
                              “Racks” auf Seite A-32
                              “Miscellaneous” auf Seite A-37
                             Use the [Back] option to return to the previous dialog.
1.00 / 03-2023




                 A-16                                               A+W Business Barcode Manager (EL)
                 Introduction                                                                                  Functions




                                       Receipt of goods
                                       Scanner > Main menu > Receipt of goods




                                       Abb. A-8      Barcoding - Receipt of goods


                                       Scan the barcodes of the purchased items for which goods have been re-
                                       ceived.
                                       When the purchased item's barcode has been scanned, enter the quantity re-
                                       ceived (via keyboard). The program shows the full quantity for the purchased
                                       item by default; this has to be changed only if the quantity received is different.
                                       If no change is necessary, scan the barcode of the next purchased item. The
                                       program will collect these scans without actually booking them. This is only
                                       done if you press the ENTER key on the scanner or scan the barcode of an-
                                       other P.O. If you press the BACK key or the ESC key while there are pur-
                                       chased items in the memory which have not been booked so far, the program
                                       wil want to know whether these shall be booked now.
                                       If the just scanned P.O. item is a box, you can scan a box ID barcode right af-
                                       terwards and change the contents of the box if necessary. The program auto-
                                       matically enters a quantity of 1 piece which cannot be changed. For boxes with
                                       an ID you can enter different contents.
                                       After a purchased item has been scanned, the bottom quantity field shows the
                                       number of articles ordered, and the number of articles received.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                  A-17
                 Functions                                                                  Introduction




                             Production report
                             Scanner > Main menu > Production report




                             Abb. A-9     Barcoding - Production report


                             The completion and breakage reports are found in the Production report sub-
                             menu, which replaces the previous completion report in the scanner main
                             menu.
                              “Completion report” auf Seite A-19
                              “Breakage report” auf Seite A-20
1.00 / 03-2023




                 A-18                                                A+W Business Barcode Manager (EL)
                 Introduction                                                                              Functions




                                       Completion report
                                       Scanner > Main menu > Production report > Completion report




                                       Abb. A-10     Barcoding - Production report


                                       The completion report dialog can be used to change the status of an order
                                       item. All scans which are made here are first saved in the database then pro-
                                       cessed by AIS as STSD reports. Status changes of orders will be made after-
                                       wards. For details on configuring the AIS for STSD reports please refer to the
                                       previous chapter.
                                       When an order item has been scanned, enter the quantity to be reported com-
                                       plete. The program will always preset the full item quantity. Press ENTER to
                                       save the completion report. The record is then processed by AIS, and the or-
                                       der status is amended if necessary. If only one piece is to be processed per
                                       scan, you can select the option "Quantity=1". If this option is enabled, when
                                       scanning a barcode 1 piece is immediately booked as complete. No additional
                                       quantity has to be entered nor the enter button pressed.
                                       The breakage report dialog can be used to change the status of orders, but
                                       only negatively, in contrast to the completion report.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                             A-19
                 Functions                                                                     Introduction




                             Breakage report
                             Scanner > Main menu > Production report > Breakage report




                             Abb. A-11    Barcoding - breakage report


                             Operating and booking work in the same way as the completion report, but it
                             is possible to include the breakage reason and creator. These can be selected
                             either by pressing the button on the scanner or by using the barcode. The bar-
                             codes can be printed out in the programs complaint reason and creator using
                             the labels form.
                             After booking a record, the information on the last booking is shown as a sum-
                             mary on the scanner.
1.00 / 03-2023




                 A-20                                               A+W Business Barcode Manager (EL)
                 Introduction                                                                            Functions




                                       Stock Movements
                                       Scanner > Main menu > Stock movements




                                       Abb. A-12     Barcoding - Stock movement menu


                                       Before starting an inventory booking, please define whether goods shall be
                                       added or withdrawn. In addition, the menu for boxes is accessible from here.
                                        “Stock Withdrawal” auf Seite A-22
                                        “Addition to stock” auf Seite A-23
                                        “Transfer” auf Seite A-24
                                        “Boxes” auf Seite A-26
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                            A-21
                 Functions                                                                     Introduction




                             Stock Withdrawal
                             Scanner > Main menu > Stock movement > Withdrawal




                             Abb. A-13    Barcoding - stock withdrawal


                             The next dialog works the same way for incoming and outgoing stock. After
                             the stock location barcode has been read, the stock article bar code can be
                             read and the respective quantity entered for the incoming or outgoing booking.
                             By pressing the ENTER key, the booking is made directly.
1.00 / 03-2023




                 A-22                                                A+W Business Barcode Manager (EL)
                 Introduction                                                            Functions




                                       Addition to stock
                                       Scanner > Main menu > Stock movement > Addition




                                       Abb. A-14     Barcoding - addition to stock
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                           A-23
                 Functions                                                                       Introduction




                             Transfer
                             Scanner > Main menu > Stock movement > Transfer




                             Abb. A-15    Barcoding - Select stock location


                             Under the stock movement menu element, there is now also the function
                             transfer. If you select it, you must first scan a stock location bar code.
                             After that, you land on the dialog for transferring stock items. Here the user
                             must scan a stock item, that is, the stockID of a stock item, whereupon the cur-
                             rent inventory is displayed. Now you should first define the quantity that should
                             be transferred.
1.00 / 03-2023




                             Abb. A-16    Barcoding - Transferring stock item




                 A-24                                                 A+W Business Barcode Manager (EL)
                 Introduction                                                                           Functions




                                       Here the user can specify a new stock location and make the booking. A suc-
                                       cess report appears on the screen.




                                       Abb. A-17     Barcoding - Successful transfer
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                          A-25
                 Functions                                                                  Introduction




                             Boxes
                             Scanner > Main menu > Stock movement > Boxes




                             Abb. A-18    Barcoding - Box warehouse menu


                             Starting with A+W Business version 12.5, there is also a Boxes submenu
                             available. With this menu, you can call the following three functions:
                              “Change box content” auf Seite A-27
                              “Resolve boxes” auf Seite A-28
                              “Change storage location of boxes” auf Seite A-29
                              “Put box to inventory” auf Seite A-30
                              “Shipping of boxes” auf Seite A-31
1.00 / 03-2023




                 A-26                                                A+W Business Barcode Manager (EL)
                 Introduction                                                                                Functions




                                       Change box content
                                       Scanner > Main menu > Stock movement > Boxes > Change content




                                       Abb. A-19     Barcoding - Change box content


                                       Use this function to reduce the sheet count in a box. For this, first a box bar
                                       code is scanned, and after that, the quantity displayed is set to the new value.
                                       By pressing the Enter key, the booking is made.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                               A-27
                 Functions                                                                       Introduction




                             Resolve boxes
                             Scanner > Main menu > Stock movement > Boxes > Resolve




                             Abb. A-20    Barcoding - Box warehouse menu


                             Decomposing boxes
                             With this function you can decompose a box (that is, the box is deleted and the
                             remaining sheets are booked to stock). For this, first a box is scanned and after
                             that, its content can be edited. By pressing the Enter key, the booking is made.
1.00 / 03-2023




                 A-28                                                A+W Business Barcode Manager (EL)
                 Introduction                                                                                Functions




                                       Change storage location of boxes
                                       Scanner > Main menu > Stock movement > Boxes > Change storage location




                                       Abb. A-21     Barcoding - Box warehouse menu


                                       You can use this function to change the stock location of a box. For this, first
                                       a box is scanned and after that, the bar code of the new storage location is
                                       entered. The booking is then triggered immediately.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                A-29
                 Functions                                                                        Introduction




                             Put box to inventory
                             Scanner > Main menu > Stock movement > To inventory list




                             Abb. A-22    Barcoding - Put box on inventory list


                             Use this function to place a box on the current inventory list. After the box has
                             been scanned, the new storage location can be scanned. After both scans
                             have been completed, the current quantity of the sheets in the box can still be
                             edited. By pressing the Enter key, the booking is made.
1.00 / 03-2023




                 A-30                                                 A+W Business Barcode Manager (EL)
                 Introduction                                                                                Functions




                                       Shipping of boxes
                                       Scanner > Main menu > Stock movement > Boxes > Shipping of boxes




                                       Abb. A-23     Barcoding - Shipping of boxes


                                       With this function, boxes with ident number can be assigned to an order item.
                                       Initially, an order item barcode must be scanned. After that, the number of lites
                                       in the box is determined by scanning the box barcode. It can be edited accord-
                                       ingly. By pressing the Enter key, the booking is made.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                A-31
                 Functions                                                                       Introduction




                             Racks
                             In order for racks to be able to be processed, the following conditions have to
                             be checked beforehand:
                             •   Rack numbers have to be unique. You can therefore not create a rack with
                                 the same number but a different rack type. If the same number is used, a
                                 letter should precede the rack number (for the rack type).
                             •   When booking racks, the width and the height of the rack is checked and
                                 the loading weight is checked. These values can be adjusted per rack type.
                             •   Rack booking was developed for shipping, i.e. only main items can be add-
                                 ed to a rack.
                             •   The only racks that can be loaded are those which are not booked for off
                                 site, have not been reported lost and are not locked.
                             •   Point 5 ensures that the allocation of the rack is fully backed at rack exit.


                             Overview of rack menu
                             Scanner > Main menu > Racks




                             Abb. A-24     Barcoding - Racks menu


                             In submenu racks, there are the functions:
                              “Load racks” auf Seite A-33
                              “Empty racks” auf Seite A-35
                              “Display racks” auf Seite A-36
1.00 / 03-2023




                 A-32                                                     A+W Business Barcode Manager (EL)
                 Introduction                                                                                 Functions




                                       Load racks
                                       Scanner > Main menu > Racks > Loading




                                       Abb. A-25     Barcoding - loading racks


                                       For leading racks, the rack to be loaded first has to be selected. When scan-
                                       ning the rack barcode, you can add the order item to the rack in the next dialog.




                                       Abb. A-26     Barcoding - loading racks - order items


                                       After the successful selection of a rack, you can add the order item to the rack.
                                       Two different modes are supported hereby, those with the buttons "Quantity =
                                       1" and "Input quantity". The currently set mode is highlighted in green.
1.00 / 03-2023




                                       The T2 bar code must be used to add order items.




                 A+W Business Barcode Manager (EL)                                                                A-33
                 Functions                                                                      Introduction




                             In the mode "Input quantity" after the item barcode has been scanned, the
                             quantity that has not yet ben loaded onto the racks is shown. This can then be
                             edited if a smaller number is to be loaded. Pressing the enter button on the
                             scanner confirms the booking.



                             In the mode "Quantity = 1", the booking is executed directly after scanning the
                             order item barcode. Only 1 piece is booked hereby.



                             The result of the last booking is always shown in the window "Last booking".



                             To exchange the racks, press the Back button and then select a different rack.
1.00 / 03-2023




                 A-34                                               A+W Business Barcode Manager (EL)
                 Introduction                                                                                Functions




                                       Empty racks
                                       Scanner > Main menu > Racks > Empty




                                       Abb. A-27     Barcoding - empty racks


                                       With this dialog, a rack can be reported empty. In this process, all allocations
                                       of the order items placed on the rack before are deleted.

                                          No backup query
                                          There is no confirmation query when emptying racks.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                               A-35
                 Functions                                                                     Introduction




                             Display racks
                             Scanner > Main menu > Racks > Display




                             Abb. A-28    Barcoding - display racks


                             With this dialog, the current allocation of order items on a rack can be dis-
                             played. If a rack barcode is scanned, the order items with the respective load-
                             ed quantity are shown in the allocation window. In addition, the customer
                             number is also output. The list contains six entries. You can browse with the
                             forward and backward button.
1.00 / 03-2023




                 A-36                                                 A+W Business Barcode Manager (EL)
                 Introduction                                                                                 Functions




                                       Miscellaneous
                                       Scanner > Main menu > Miscellaneous
                                       The menu Miscellaneous includes the dialogs for order item information, reg-
                                       istration information, and change of user.
                                        “Order Information” auf Seite A-37
                                        “Login information” auf Seite A-38
                                        “Change employee” auf Seite A-38


                                       Order Information
                                       Scanner > Main menu > Miscellaneous > Order information




                                       Abb. A-29     Barcoding - order information


                                       When an item barcode has been scanned, order item information will show the
                                       item name, item size, quantity, quantity delivered, price per price unit, and the
                                       delivery date.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                A-37
                 Functions                                                                      Introduction




                             Login information
                             Scanner > Main menu > Miscellaneous > Login information




                             Abb. A-30    Barcoding - miscellaneous


                             The registration information dialog shows the currently registered user, the da-
                             tabase, the database system (Microsoft SQL Server or Unify SQL Base), the
                             registration point, the machine, and the work type.


                             Change employee
                             Scanner > Main menu > Miscellaneous > Change employee




                             Abb. A-31    Barcoding - login


                             The dialog to change an employee is described the following section:
                              “Login” auf Seite A-15
1.00 / 03-2023




                             After scanning a valid user code, the present user will be signed out, and the
                             new user registered.



                 A-38                                                 A+W Business Barcode Manager (EL)
                 Introduction                                                                                         Barcodes




                                             Barcodes
                                             The individual dialogs and functions require certain barcodes. These are
                                             Code39 barcodes with check digit, with an asterisk at the start and at the end.


                 Description                                    Prefix   User data                        Example

                 Personnel barcode                              PE       The personnel number as per      *PE000000199F*
                                                                         user management

                 Registration point barcode without work type   ES       ID of registration point         *ES00000000166*
                 for goods received

                 Registration point barcode and work type for   EA       Registration point ID and work   *EA0000000015-101P*
                 completion report                                       type ID separated by a hyphen

                 Order bar code for reporting finished and      T2       Order number +                   *T200000243001001%*
                 sheet-rack assignment                                   item number (3-digit) +
                                                                         element number (3-digit)

                 Order barcode for order information            D2 or    Order number +                   *D200000243002Q* or
                                                                T2       item number (3-digit) +          *T200000243002001Q*
                                                                         element number (3-digit) (only
                                                                         T2)

                 P.O. barcode for receipt of goods              D5       P.O. number + item number (3- *D50000070650001.*
                                                                         digit)

                 Box barcode for stock additions and            BO       Box ID. Attention: ID must not   *BOBC00002H*
                 withdrawals                                             start by zero!

                 Stock location barcode for inventory booking   LA       Stock location ID                *LA0000000001W* or
                                                                                                          *L0000000001W*

                 Stock article barcode for inventory booking    LP       Stock ID of stock article        *LP0000000164E*

                 Rack number                                    GE       Rack number                      *GE9099E*

                 Reason for complaint                           BR       Number of reason of complaint    *BR1$*

                 Cause of complaint                             BC       Number of cause of complaint     *BC2P*
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                         A-39
                 Barcodes                                                                        Introduction




                                Printing barcodes
                            In the following programs in A+W Business, a barcode printing functionality
                            was implemented for the online plant data recording (via barcode scanner):
                            •    Employee management (Master data > Company > Employees)
                            •    Registration point in production (e.g. Master data > Production > Other >
                                 Registration points production)
                            •    Default time (Capacity planning > Master data > Default times > Default
                                 times)
                            •    Print program (e.g. Documents > Order > Print order)
                            •    Stock definition (Master data > Stock > Stock definition)
                            •    Stock management (Stock management > Inventory management)
                            •    Racks (Production > Rack management > Racks)
                            •    Reason of complaint (Master data > Products > General > Complaint rea-
                                 son)
                            •    Cause of complaint (Master data > Products > General > Complaint cause)
                            If the useful data does not exceed the possible data length, the barcodes are
                            filled up with zeros (0) (except rack barcodes). Furthermore, all barcodes re-
                            ceived a final test digit. A general print functionality was also installed in the
                            employee management (1). The barcodes contain the personnel number
                            (here 199) of the employee (example: PE000000199F). The registration point
                            barcode (2) is formed from the ID of the registration point (example:
                            ES00000000166). In the default times program (3), the user now has the op-
                            portunity to print a registration point barcode with work type for the completion
                            report in the online PDC. This is composed of the ID of the registration point
                            and the ID of the work type separated by a hyphen (example: EA0000000015-
                            101P). The print program for the form printing (4) can print an order barcode
                            (order info in online PDC) or a purchase order barcode (incoming goods in on-
                            line PDC), effective immediately. This barcode includes the document number,
                            the 3-digit item number, and a 3-digit part number (always 000 since only main
                            items are output here) (example order T200000243002000Q – example pur-
                            chase order: D50000070650001.). For the stock booking in the PDC, the stock
                            location must be scanned accordingly. For this, on the one hand the barcode
                            printing on the stock definition dialog (5) was reworked and on the other hand,
                            the online PDC was expanded. Effective immediately, the online PDC can pro-
                            cess such storage location barcodes with an L-prefix. The barcode includes
                            the ID of the storage location (example: *L0000000001W*). Then, barcodes of
                            the stock items (5) are necessary for the stock booking. In the stock manage-
                            ment, the appropriate barcodes, which include the ID of the stock item, can
                            now be printed (example: LP0000000164E). For racks, a list of racks can be
                            selected in rack management (7) and then printed for this barcode (Functions
                            > Print Rack Barcode). As the racks are alphanumeric, they are not filled with
                            leading zeros.
                            Note: All bar codes are written to the report variable F_IDENT_C39 of the re-
                            spective form/report.
1.00 / 03-2023




                 A-40                                               A+W Business Barcode Manager (EL)
                 Introduction                                                                                  Barcodes




                                       Booking history
                                       It is now possible to protocol the implemented completion and breakage re-
                                       ports. The switch "fill history table for completion reports" must be activated in
                                       the company master data on register 15. Capacity planning to activate the
                                       function.
                                       If the switch has been activated, the edited reports are recorded in the table
                                       FS_BOOK_HISTORY. If the booking is active in the A+W Business capacity
                                       planning, the reports will also be recorded when booked in the same way. This
                                       also applies for reports performed via the dialog in A+W Business. Otherwise
                                       the bookings are recorded in PD_AWBAR.
                                       The following data is hereby saved
                                       •   Order number
                                       •   Item number
                                       •   BOM element
                                       •   Time of scanning
                                       •   Employee
                                       •   Registration point
                                       •   Work type (only for booking in capacity planning, otherwise 0)
                                       •   Breakage reason (only for breakage reports)
                                       •   Cause of breakage (only for breakage reports)
                                       •   Booked quantity
                                       •   Origin (BDE, manual, implicit)


                                       Furthermore, there is an dialog on analysis of the booking history (Statistics >
                                       Booking history). Now the records to be displayed can be filtered via the QBE
                                       mode so that precise statistics, e.g. per employee, can be created.
1.00 / 03-2023




                 A+W Business Barcode Manager (EL)                                                                 A-41
                 Barcodes                                                                  Introduction




                            Abb. A-32   Barcoding - login


                            By pressing, the displayed records can also be grouped according to two dy-
                            namic criteria, which can also be set in the dialog.
1.00 / 03-2023




                 A-42                                            A+W Business Barcode Manager (EL)
Barcode Manager (EL)         A

                       Partindex




                  A+W Business
                 Partindex                                                                Index




                 Index
                 A                                   M
                 Addition to stock     A-23          Machines
                                                     – Capacity planning A-14
                 B                                   Menu A-16
                 Barcoding
                 – Barcodes A-39                     O
                 – Change employee A-38              Others   A-37
                 – Functions A-15
                 – Login A-15                        P
                 – Login information A-38            Production report A-18
                 – Main Menu A-16                    – Breakage report A-20
                 – Order information A-37            – Completion report A-19
                 – Other functions A-37
                 – Printing barcodes A-39, A-40
                 – Production report A-18            R
                 – Rack functions A-33, A-35, A-36   Racks A-32
                 – Rack menu A-32                    – Display A-36
                 – Racks A-32                        – Empty A-35
                 – Stock movements A-21              – Loading A-33
                 Booking history A-41                – Menu overview A-32
                 Booking of boxes                    Receipt of goods A-17
                 – Change content of boxes A-27      Registration points
                 – Change storage location A-29      – A+W Business master data    A-12
                 – Inventory list A-30               re-login A-38
                 – Resolve box A-28
                 – Shipping of boxes A-31            S
                 Box manangement A-26                Scanner
                 Breakage report A-20                – Main Menu A-16
                                                     – Receipt of goods A-17
                 C                                   Settings
                 Change employee A-15                – Tables A-10
                 Change stock A-24                   Stock movements A-21
                 Completion report A-19              – Addition to stock A-23
                                                     – Book box to inventory list A-30
                                                     – Booking of boxes A-26
                 E                                   – Change box location A-29
                 Employee                            – Change content of boxes A-27
                 – A+W Business        A-12, A-13    – Change stock A-24
                                                     – Resolve box A-28
                 F                                   – Shipping of boxes A-31
                 Functions                           – Stock withdrawal A-22
                 – Overview     A-15                 Stock withdrawal A-22

                 I                                   T
                 Interface Service     A-13          Tables
1.00 / 03-2023




                                                     – Settings   A-10
                 L
                 Login   A-15


                 A+W Business Barcode Manager (EL)                                        A-45
                 Index                            Partindex
1.00 / 03-2023




                 A-46    A+W Business Barcode Manager (EL)

