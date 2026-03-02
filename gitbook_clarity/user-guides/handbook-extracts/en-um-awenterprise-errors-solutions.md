---
description: "Error messages and solutions from A+W Enterprise (English) handbook"
---

# A+W Enterprise (English) - Error Messages & Solutions

**Source:** Extracted from en-um-awenterprise.md  
**Product:** A+W Enterprise (English)  
**Language:** English

This document contains error messages, warnings, and their solutions extracted from the complete product handbook.

---

## Issue 1

```
            The documentation and software described are licenses that must be used or
            copied only in accordance with the conditions of our license agreement. The
            content of the documentation serves only as information and can be changed
            without prior notice at any time.
            The text and illustrations were compiled with the utmost care. However it is not
            possible to exclude errors completely. A+W Software GmbH cannot be held
            liable for errors or inaccuracies, unless they can be attributed to wilful or gross-
            ly negligent action.
            The descriptions in this document are based on the full program level of A+W
            Enterprise.

```

---

## Issue 2

```
            copied only in accordance with the conditions of our license agreement. The
            content of the documentation serves only as information and can be changed
            without prior notice at any time.
            The text and illustrations were compiled with the utmost care. However it is not
            possible to exclude errors completely. A+W Software GmbH cannot be held
            liable for errors or inaccuracies, unless they can be attributed to wilful or gross-
            ly negligent action.
            The descriptions in this document are based on the full program level of A+W
            Enterprise.


```

---

## Issue 3

```
  Background checks ....................................... D-1043                 Delivery date change log ................................ D-1230
Resubmission ................................................... D-1044            Shape catalog ................................................ D-1231
Modification Functions in Sales ........................ D-1047                    Shape - dimensions ....................................... D-1232
  Document change .......................................... D-1048                Payment management ................................... D-1234
                                                                                   Payment plan ................................................. D-1236
Software Reference ........................................ D-1051                 Error information system ................................ D-1238
Overview .......................................................... D-1057         Production monitor ......................................... D-1240
 Sales menu .................................................... D-1058           Technical Details ............................................... D-1241
 Supplementary menu ..................................... D-1060                   Declaration of performance ............................ D-1241
 Info menu ....................................................... D-1066          Order entry – technical values ....................... D-1242
Search Functions ............................................. D-1068             Bill of Material (BOM) ....................................... D-1249
```

---

## Issue 4

```
                         dled by means of bills of materials.

                         Import and export interfaces
                         Apart from manual input, A+W Enterprise also offers various interfaces for im-
                         porting orders directly from the customers' system. This reduces input times
                         as well as input errors and improves customer relations.
                         Orders can be accepted automatically via the A+W standard interface or indi-
                         vidual customer interfaces.
                         You can also import supplier data via A+W Enterprise. Provided that the sup-
                         plier also uses A+W Enterprise, prices, enquiries, and orders can be easily
                         transferred online. A transfer of POs to third-party systems is possible with the
```

---

## Issue 5

```
                    Project-oriented limit check.
                 Technical info: toggle field, DB field: mp.objlimitpruef

                 Cred. limit This field is only brought to bear if the Cred. Limit field is set to Y.
                 If an order value including the open items and the open orders exceeds the
                 credit limit stored here, a warning is issued.
                 Technical info: numeric field, DB field: mp.firmlimit

                 VAT Selection of the VAT code. The necessary tax codes are stored on the
                 Tax Types menu (Master Data > Keys > System > Taxes).
                 Technical info: <F9>, DB field: mp.mwst
```

---

## Issue 6

```
          A+W Enterprise will inform you.
          Technical info: numeric fields, DB fields: artmdzu.pmaxsv

          Minimum aspect ratio In this field, you can restrict the aspect ratio of an ar-
          ticle to a minimum value. If this aspect ratio is not met at document entry, A+W
          Enterprise will issue a warning.
          Technical info: numeric fields, DB fields: artmdzu.pminsv



B-470                                                       A+W Enterprise Master Data
```

---

## Issue 7

```

        Fig. B-228   Examples of fitting positions


        If there is no fitting position defined for LAMI foil layers, A+W Enterprise will
        inform you accordingly; this will cause an error at document entry.
        In system settings, you can define that the BOM must not be exited without
        correction.
        This field appears in the BOM editor.
        Technical info: numeric fields, DB fields: strukt.pos

```

---

## Issue 8

```
                       the various glass types, you have to control which PLCD should be used for
                       price calculation.
                       Via the price list control, it is set from which price list a price is drawn if no price
                       was found in the assigned price list.
                       If in the document management no price in the sense of the set PLCD logic is
                       found, an error message is output.
                       In nearly all dialogs that are used for pricing, you can specify a PLCD from
                       which the price applies. The from-PLCD logic applies separately for all dialogs
                       on which a from-PLCD can be specified.
                       In individual cases, the from-PLCD logic can be overridden. The Price List
                       Control dialog is available for this:
```

---

## Issue 9

```
                              Tutorial, “Price matrices for IG lites” on page C-573

                                No from PLCD logic
                                The from PLCD logic is not applied for matrices. Therefore, for each matrix
                                number, a separate matrix has to be defined in all relevant price list codes
                                (PLCDs). If there is no matrix, an error message is displayed in the order.

                             The number for a new matrix is created as a key on the Matrices dialog.
                              “Matrices” on page C-691
                             You can either create a new matrix via the definition of the limit values or read
                             in a matrix from a file. Furthermore, in the Matrix type field, you can copy an
```

---

## Issue 10

```
                        Tutorial, “From-PLCD logic” on page C-552
                       If the environment variable ISOAUST_ABPLKZ is configured appropriately
                       and the exchange prices are used, the following messages can be displayed:
                       • A message with the PLCD is displayed from which the exchange price was
                            taken.
                       • An error message is displayed because no exchange price could be found
                            in the selected PLCDs. The exchange price is not used for calculation and
                            is set to 0.
                       Technical info: numeric field, DB field: isoaust.pkz

                       Field descriptions
```

---

## Issue 11

```
         6 Enter the order to the end.

          Here's how to save the order temporarily
            Especially for larger orders with several items or complicated entries, it is
            advised that you save the order in question temporarily. The advantage is
            that if a problem occurs, you will be able to use the saved state after restart.
         1 Enter an order header up to the point that seems sensible for saving. How-
           ever, at least one item must be entered completely so that the Save button
           is activated automatically.
           A data record is created in the table kauf with kauf.still=999.
         2 You can save the order again at a later time, e.g. after entering additional
```

---

## Issue 12

```
           items.Here the first data record saved in the table kauf is overwritten.
         3 If an order is entered completely and saved, the kauf.still=-3 is set and the
           order will be presented to the background process intauf for further pro-
           cessing. Alternatively, the order entered can also be placed in the release
           pool.
         4 In the case that the entry is interrupted by a technical problem so that A+W
           Enterprise has to be restarted, the program offers the following possibility:
            •   When starting the order entry, you get a notice that there are still docu-
                ments whose entry has not been completed.
            •   If you confirm this notice, the overview dialog with the saved documents
                opens:
```

---

## Issue 13

```

         Benefits

         • The functions on the item level can help with fast and safe order entry. On the item
           level, individual products are entered that the customer orders. Preventing entry
           errors reduces possible mistaken production.


         Note

         Edit BOM                     This function offers the possibility to make changes to
```

---

## Issue 14

```
         The BOM structure of an item is automatically transferred to the following item
         if you enter the same item number. The BOM number can be changed. You
         can also display the BOM and edit it.
          Master Data, “BOM” on page B-478
         All changes to the BOM must be made carefully. Incorrect actions can cause
         other problems, including a program crash.




D-1010                                                                A+W Enterprise Sales
```

---

## Issue 15

```

                          Only exchange identical article types
                          You can replace an article only with an article of the same type.
                          Example: Replacing glass with a processing step would be nonsense. You
                          have to define the corresponding technical restrictions in article master
                          data so that A+W Enterprise issues a warning.
                           Master Data, “Article” on page B-377
                       3 Confirm the new article number with <Enter>.
                          A+W Enterprise updates the name and all other fields.
                       4 Close the dialog with <End> to save the changes you have made. Use
                         <Home> to reject the changes.
```

---

## Issue 16

```
           manual invoice entry, first an internal number is assigned and only when the
           invoice has been entered completely is this invoice saved under its final num-
           ber. This guarantees a seamless numbering.
           In extremely rare cases (program crash directly after the final invoice number
           has been assigned) it can happen that during the assignment of invoice num-
           bers, there are gaps. Since these gaps can cause problems in controlling, a
           possibility has been created to re-use these numbers. This logic requires a
           special system configuration and may only be activated in consultation with
           A+W. If you are interested, contact an A+W Software GmbH employee.
           Apart from that, you can issue deposit or final invoices with a previously creat-
           ed payment plan, and select automatic release or manual invoicing.
```

---

## Issue 17

```

                       Background checks
                       The Checks menu consists of the Input and Background check submenus.
                       The Input check basically shows the existing orders the the shape of text. Item
                       data relevant for pricing are shown in detail.
                       The Background check includes an error message system that lists where
                       background processes have caused processing errors. The orders in question
                       can be loaded and edited or corrected as required.
                        Software Reference, “Document Research” on page D-1447


```

---

## Issue 18

```
                       Background checks
                       The Checks menu consists of the Input and Background check submenus.
                       The Input check basically shows the existing orders the the shape of text. Item
                       data relevant for pricing are shown in detail.
                       The Background check includes an error message system that lists where
                       background processes have caused processing errors. The orders in question
                       can be loaded and edited or corrected as required.
                        Software Reference, “Document Research” on page D-1447



```

---

## Issue 19

```
           Delivery date change log ............................................................................... D-1230
           Shape catalog ............................................................................................... D-1231
           Shape - dimensions ....................................................................................... D-1232
           Payment management .................................................................................. D-1234
           Payment plan ................................................................................................ D-1236
           Error information system ............................................................................... D-1238
           Production monitor ........................................................................................ D-1240
         Technical Details ............................................................................................... D-1241
           Declaration of performance ........................................................................... D-1241
           Order entry – technical values ....................................................................... D-1242
              Calculated technical values ....................................................................... D-1242
```

---

## Issue 20

```

    k      Print list                              “List printing” on page D-1427

    l      Overview                                “Overview submenu” on page D-1060

    m      Background check                        “Error information system” on page D-1238

    n      Resubmission                            “Resubmission” on page D-1467

    o      Completion report                       “Completion report” on page D-1469

```

---

## Issue 21

```
                      •   “Delivery date change log” on page D-1230
                      •   “Shape catalog” on page D-1231
                      •   “Shape - dimensions” on page D-1232
                      •   “Payment management” on page D-1234
                      •   “Payment plan” on page D-1236
                      •   “Error information system” on page D-1238
                      •   “Production monitor” on page D-1240




```

---

## Issue 22

```
                      Width, height Width and height of the item in millimeters. For variant articles,
                      the system takes over the dimensions from the article master data. If you
                      change the stock dimensions, the variant query appears: Can the variant ref-
                      erence really be removed?
                      • Click on [No] to reset the entered sizes to the stock sizes.
                      • Click [Yes] to change the stock sizes. This can cause problems in the ware-
                         house and with pricing.
                      Technical info: mandatory fields, numeric fields, DB fields: kpos.laenge,
                      kpos.breite

                      (Field without name) For length, time, and piece articles, instead of width,
```

---

## Issue 23

```
Document Management                                                             Software Reference




                      Error information system
                      Sales > Background Check > Enter date > <F3>




```

---

## Issue 24

```
                      Sales > Background Check > Enter date > <F3>




                      Fig. D-80     Error information system


                      This dialog displays particular processing errors due to the background pro-
                      cess INTAUF starting on the selected date. The orders whose processing has
                      failed are listed in a table.
```

---

## Issue 25

```


                      Fig. D-80     Error information system


                      This dialog displays particular processing errors due to the background pro-
                      cess INTAUF starting on the selected date. The orders whose processing has
                      failed are listed in a table.
                      •    Use <F3> to start the search.
                      •    Use the arrow keys and <Page Up>, <Page Down> to navigate in the table.
                      The following errors can be displayed:
```

---

## Issue 26

```
                      This dialog displays particular processing errors due to the background pro-
                      cess INTAUF starting on the selected date. The orders whose processing has
                      failed are listed in a table.
                      •    Use <F3> to start the search.
                      •    Use the arrow keys and <Page Up>, <Page Down> to navigate in the table.
                      The following errors can be displayed:

                      Error number     Error text               Meaning

                      90               INTAUF incorrect call    Processing by INTAUF is incorrect.
                                                                For more information, you can
```

---

## Issue 27

```
                      failed are listed in a table.
                      •    Use <F3> to start the search.
                      •    Use the arrow keys and <Page Up>, <Page Down> to navigate in the table.
                      The following errors can be displayed:

                      Error number     Error text               Meaning

                      90               INTAUF incorrect call    Processing by INTAUF is incorrect.
                                                                For more information, you can
                                                                examine the INTAUF log.

```

---

## Issue 28

```

                      90               INTAUF incorrect call    Processing by INTAUF is incorrect.
                                                                For more information, you can
                                                                examine the INTAUF log.

                      91               INTAUF loading error     INTAUF could not load the
                                                                document.

                      92               INTAUF write error       INTAUF could not save the
                                                                document.

```

---

## Issue 29

```
                                                                examine the INTAUF log.

                      91               INTAUF loading error     INTAUF could not load the
                                                                document.

                      92               INTAUF write error       INTAUF could not save the
                                                                document.

                      93               INTAUF x attempts        Processing of the document was
                                                                cancelled after the xth unsuccessful
                                                                attempt.
```

---

## Issue 30

```
                                                                attempt.

                      100              INTAUF price different   The internal SA price and the PA EDI
                                                                price are different.

                      Tab. D-4      Error display




D-1238                                                                       A+W Enterprise Sales
```

---

## Issue 31

```



                       Header

                       Display from date Start date starting with which errors are searched for.
                       Technical info: date field

                       Hit list
                       The hit list displays the following fields:
                       •   Order:
```

---

## Issue 32

```
                       Technical info: date field

                       Hit list
                       The hit list displays the following fields:
                       •   Order:
                           Number of the order in which the error occurred.
                           Technical info: display field, DB field: kauferr.auftrnr
                       •   Count:
                           Subnumber, e.g. for invoices or delivery notes.
                           Technical info: display field, DB field: kauferr.subnr
                       •   Document:
```

---

## Issue 33

```
                           Technical info: display field, DB field: kauferr.subnr
                       •   Document:
                           Document type.
                           Technical info: display field, DB field: kauferr.vorgang
                       •   Err:
                           Number of the error that occurred.
                           Technical info: display field, DB field: kauferr.errno
                       •   Error text:
                           Information text about the error that occurred.
                           Technical info: display field, DB field: kauferr.txt
                       •   Date:
```

---

## Issue 34

```
                           Document type.
                           Technical info: display field, DB field: kauferr.vorgang
                       •   Err:
                           Number of the error that occurred.
                           Technical info: display field, DB field: kauferr.errno
                       •   Error text:
                           Information text about the error that occurred.
                           Technical info: display field, DB field: kauferr.txt
                       •   Date:
                           Date on which the error occurred.
                           Technical info: display field, DB field: kauferr.datum
```

---

## Issue 35

```
                           Technical info: display field, DB field: kauferr.vorgang
                       •   Err:
                           Number of the error that occurred.
                           Technical info: display field, DB field: kauferr.errno
                       •   Error text:
                           Information text about the error that occurred.
                           Technical info: display field, DB field: kauferr.txt
                       •   Date:
                           Date on which the error occurred.
                           Technical info: display field, DB field: kauferr.datum
                       •   Time:
```

---

## Issue 36

```
                           Technical info: display field, DB field: kauferr.errno
                       •   Error text:
                           Information text about the error that occurred.
                           Technical info: display field, DB field: kauferr.txt
                       •   Date:
                           Date on which the error occurred.
                           Technical info: display field, DB field: kauferr.datum
                       •   Time:
                           Time at which the error occurred.
                           Technical info: display field, DB field: kauferr.zeit
                       If you are marking a row, you can use <F3> to open the corresponding order
```

---

## Issue 37

```
                           Technical info: display field, DB field: kauferr.txt
                       •   Date:
                           Date on which the error occurred.
                           Technical info: display field, DB field: kauferr.datum
                       •   Time:
                           Time at which the error occurred.
                           Technical info: display field, DB field: kauferr.zeit
                       If you are marking a row, you can use <F3> to open the corresponding order
                       in display mode.


```

---

## Issue 38

```
                       If you are working with internal site separation, first a dialog opens where you
                       can specify the site number. The log displays only the documents for the se-
                       lected site.

                          Delivery note log for the current day
                          A delivery note log is generated for the current day. If the error message is
                          displayed that the file is empty or cannot be read, then no delivery note has
                          been generated on this day.



```

---

## Issue 39

```
                       If you are working with internal site separation, first a dialog opens where you
                       can specify the site number. The log displays only the documents for the se-
                       lected site.

                          Invoice log for the current day
                          An invoice log is generated for the current day. If the error message is dis-
                          played that the file is empty or not readable, then no invoices have been
                          generated on this day.



```

---

## Issue 40

```

               [Int.Order] Branches to an internal order with individual order number for
               production if this exists and the system is configured appropriately. The inter-
               nal orders can only be generated if the environment variable VOR-
               GANGSSTATUS_ADHOCSQL is active and you have incorporated an ad hoc
               SQL query. If the variable is not set, an appropriate error message is dis-
               played.




```

---

## Issue 41

```
               of the dialog.
               The buttons are described for the Document tab:
                “Document info – order” on page D-1429
               In addition, the following button is displayed:

               [Info] Displays the error message from production for the selected item. The
               button is only active if there is an error message for the selected item.




```

---

## Issue 42

```
               The buttons are described for the Document tab:
                “Document info – order” on page D-1429
               In addition, the following button is displayed:

               [Info] Displays the error message from production for the selected item. The
               button is only active if there is an error message for the selected item.




D-1432                                                                    A+W Enterprise Sales
```

---

## Issue 43

```
                       Technical info: numeric field, DB field: kauf.wlast

                            Restriction check after input of wind load
                            If an appropriate entry is created for the wind load in the master data, the
                            specified wind load is subjected to a restriction check. A note will be dis-
                            played should the restriction check reveal problems.



A+W Enterprise Purchasing                                                                       E-1599
Document Management                                                              Software Reference
```

---

## Issue 44

```
                       stored for the article. For variant articles, the system takes the dimensions
                       from the article master data using the selected variant number. If you change
                       these dimensions, the query appears: Can the variant reference really be re-
                       moved?
                          – Click on [No] to reset the entered sizes to the stock sizes.
                          – Click [Yes] to change the stock sizes. This can cause problems in the
                              warehouse and with pricing.
                       Technical info: mandatory fields, numeric fields, DB fields: kpos.laenge,
                       kpos.breite, kpos.szr

                       (Columns without name) For length, time, and piece articles, instead of
```

---

## Issue 45

```
                            Orders/purchase orders – filter dialog ........................................................ F-1792
                            Orders/purchase orders – hit list ................................................................ F-1793
                            Orders/purchase orders – hit list details .................................................... F-1794
                         Booking status .............................................................................................. F-1796
                            Booking status – unbooked ........................................................................ F-1796
                            Booking status – error ................................................................................ F-1798
                            Booking status – inventory ......................................................................... F-1800
                            Booking status – correction ........................................................................ F-1801
                         Stock information – Pick list .......................................................................... F-1803
                         Stock information – Hit list ............................................................................. F-1804
                         SCC status .................................................................................................... F-1805
```

---

## Issue 46

```

    i      Booking status                            Opens the submenu

    ia     Booking status - Unbooked                 “Booking status – unbooked” on page F-1796

    ib     Booking status - Error                    “Booking status – error” on page F-1798

    ic     Booking status - Inventory                “Booking status – inventory” on page F-1800

    j      Order list                                “Stock information – Pick list” on page F-1803

```

---

## Issue 47

```
                     stocks that contain unbooked or flawed booking records or stocks that are in
                     inventory at the moment. On the Booking status – Correction dialog, you can
                     correct the data for the booking status.
                     This dialog displays the following subdialogs:
                     •   Booking status – unbooked
                     •   Booking status – error
                     •   Booking status – inventory
                     •   Booking status – correction


                     Booking status – unbooked
```

---

## Issue 48

```
                           Number of the article color.
                       •   Qty:
                           Number of unbooked articles.
                       •   Status:
                           Number of the status of the current booking, e.g. stock out.
                       •   Error:
                           Number of the error status. The error status is in plain text in the footer ar-
                           ea.
                       With <F2>, you can display additional columns.
                       •   Quantity:
                           Quantity unit of the article.
```

---

## Issue 49

```
                       •   Qty:
                           Number of unbooked articles.
                       •   Status:
                           Number of the status of the current booking, e.g. stock out.
                       •   Error:
                           Number of the error status. The error status is in plain text in the footer ar-
                           ea.
                       With <F2>, you can display additional columns.
                       •   Quantity:
                           Quantity unit of the article.
                       •   Price:
```

---

## Issue 50

```
Information System                                                                Software Reference




                     Booking status – error
                     Info System > Booking Status > Error




```

---

## Issue 51

```




                     Booking status – error
                     Info System > Booking Status > Error




                     Fig. F-56     Booking Status – Error
```

---

## Issue 52

```
                     Info System > Booking Status > Error




                     Fig. F-56     Booking Status – Error


                     On this dialog, you can display booking information about the stocks that con-
                     tain flawed booking records. On the Booking status – Correction dialog, you
                     can correct the data for the booking status.
```

---

## Issue 53

```
                         Number of the article color.
                     •   Qty:
                         Number of unbooked articles.
                     •   Status:
                         Number of the status of the current booking, e.g. stock out.
                     •   Error:
                         Number of the error status. The error status is in plain text in the footer ar-
                         ea.



```

---

## Issue 54

```
                     •   Qty:
                         Number of unbooked articles.
                     •   Status:
                         Number of the status of the current booking, e.g. stock out.
                     •   Error:
                         Number of the error status. The error status is in plain text in the footer ar-
                         ea.




```

---

## Issue 55

```




                       Booking status – correction
                       Info System > Booking Status > Unbooked, error, inventory > <F5>




                       Fig. F-58    Booking status – correction
```

---

## Issue 56

```


                       On this dialog, you can correct the data of the booking status of the following
                       dialogs:
                       •   Booking status – unbooked
                       •   Booking status – error
                       •   Booking status – inventory

                       Body

                       Article Article number and description.
```

---

## Issue 57

```

                     Article Article description.

                     Stock Stock description.

                     Error Error status in plain text.

                     Status Status of the current booking in plain text, e.g. stock out.



```

---

## Issue 58

```
                          whereby 31 is always the last day of the month and is adjusted automati-
                          cally to the month (28(29), 30 or 31).

                          At the time of the backup, no stock inventories and no flawed bookings may
                          be open; otherwise, the backup cannot be done. If successful or in case of
                          error, the responsible employee can be informed about the result via e-
                          mail. Please contact a A+W employee for the correct system setting for this
                          function.

                       Date Date of the last backup.
                       Technical info: display field, DB field: wlx_m.savedate
```

---

## Issue 59

```
    Workflow
1 Select Booking > In menu.                                      Check booking:
     The Stock In dialog opens.                                 7 Info System > Booking Status > Unbooked menu: non-
                                                                  booked bookings.
2 Select article and stock.
                                                                8 Info System > Booking Status > Errors menu: incorrect
3 Enter article variant, article quantity, and purchase price
                                                                  bookings.
  per piece or per quantity unit.
                                                                9 Info System > History > Enter Filter Criterion menu >
     Total price of the item is displayed.
```

---

## Issue 60

```
    Workflow
1 Select Booking > Out menu.                                    Check booking:
     The Stock Out dialog opens.                               7 Info System > Booking Status > Unbooked menu: non-
                                                                 booked bookings.
2 Select article and stock.
                                                               8 Info System > Booking Status > Errors menu: incorrect
3 Enter article variant and article quantity in pieces or
                                                                 bookings.
  quantity unit.
                                                               9 Info System > History > Enter Filter Criterion menu >
     Total price of the item is displayed.
```

---

## Issue 61

```
    Workflow
1 Select Booking > Slot in menu.                                 Check booking:
     The Slot warehouse In dialog opens.                        7 Info System > Booking Status > Unbooked menu: non-
                                                                  booked bookings.
2 Select article and warehouse.
                                                                8 Info System > Booking Status > Errors menu: incorrect
3 Enter article variant, article quantity, and purchase price
                                                                  bookings.
  per piece or per quantity unit.
                                                                9 Info System > History > Enter Filter Criterion menu >
     Total price of the item is displayed.
```

---

## Issue 62

```
    Workflow
1 Select Booking > Slot Out menu.                               Check booking:
     The Slot warehouse Out dialog opens.                      7 Info System > Booking Status > Unbooked menu: non-
                                                                 booked bookings.
2 Select article and warehouse.
                                                               8 Info System > Booking Status > Errors menu: incorrect
3 Enter article variant and article quantity in pieces or
                                                                 bookings.
  quantity unit.
                                                               9 Info System > History > Enter Filter Criterion menu >
     Total price of the item is displayed.
```

---

## Issue 63

```
    Workflow
1 Select Booking > Box In menu.                                 Check booking:
     The Box Warehouse In dialog opens.                        8 Info System > Booking Status > Unbooked menu: non-
                                                                 booked bookings.
2 Select article and box warehouse.
                                                               9 Info System > Booking Status > Errors menu: incorrect
3 Select article variant.
                                                                 bookings.
4 Enter box designation and packaging type.
                                                               10 Info System > History > Enter Filter Criterion menu >
5 Enter article quantity and supplier's article price.            <F3>.
```

---

## Issue 64

```
1 Select Booking > Box Out menu.                                   Boxes will be removed from stock.
     The Box Warehouse Out dialog opens.                        Check booking:
2 Select article and box warehouse.                            8 Info System > Booking Status > Unbooked menu: non-
                                                                 booked bookings.
3 Select box with the article variant in question and press
  <F4>.                                                        9 Info System > Booking Status > Errors menu: incorrect
                                                                 bookings.
     Supplementary menu opens.
                                                               10 Info System > History > Enter Filter Criterion menu >
4 Select Boxes > Box Out menu.
                                                                  <F3>.
```

---

## Issue 65

```
•    Use <F5> to change from a column to the variant-related      Bookings can be corrected on the Booking Correction dia-
     details in the footer.                                       log.
•    Use <Ctrl> + <E> to edit the individual lite information.     Book booking correction

    Workflow
1 Select Booking > Box In menu.                                   10 Info System > Booking Status > Errors menu: incorrect
                                                                     bookings.
     The Box Warehouse In dialog opens.
                                                                  11 Info System > History > Enter Filter Criterion menu >
2 Select article and individual lite box warehouse.
                                                                     <F3>.
```

---

## Issue 66

```
    Workflow
1 Select Booking > Box Out menu.                                        Check booking:
     The Box Warehouse Out dialog opens.                               7 Info System > Booking Status > Unbooked menu: non-
                                                                         booked bookings.
2 Select article and individual lite box stock.
                                                                       8 Info System > Booking Status > Errors menu: incorrect
3 Select variant.
                                                                         bookings.
4 Use <Ctrl> + <E> to change to the individual lite informa-
                                                                       9 Info System > History > Enter Filter Criterion menu >
  tion.
```

---

## Issue 67

```
    Workflow
1 Select Booking > Rack In menu.                             Check booking:
     The Rack Warehouse In dialog opens.                    9 Info System > Booking Status > Unbooked menu: non-
                                                              booked bookings.
2 Select either article and rack stock or the rack.
                                                            10 Info System > Booking Status > Errors menu: incorrect
3 Select article variant.
                                                               bookings.
4 Select rack or create new rack.
                                                            11 Info System > History > Enter Filter Criterion menu >
5 Select slot for the rack.                                    <F3>.
```

---

## Issue 68

```
1 Select Booking > Rack out menu.                                  Article will be removed from rack stock.
     The Rack Out dialog opens.                                 Check booking:
2 Select either article and rack stock or the rack.            10 Info System > Booking Status > Unbooked menu: non-
                                                                  booked bookings.
3 Select Order-related tab.
                                                               11 Info System > Booking Status > Errors menu: incorrect
4 Select variant on the rack.
                                                                  bookings.
5 Enter booking quantity of the variant in quantity unit.
                                                               12 Info System > History > Enter Filter Criterion menu >
6 Enter order number.                                             <F3>.
```

---

## Issue 69

```
1 Select Booking > Rack out menu.                                  Article will be removed from rack stock.
     The Rack Warehouse Out dialog opens.                       Check booking:
2 Select either article and rack stock or the rack.            10 Info System > Booking Status > Unbooked menu: non-
                                                                  booked bookings.
3 Select Rebooking tab.
                                                               11 Info System > Booking Status > Errors menu: incorrect
4 Select variant on the rack.
                                                                  bookings.
5 Enter booking quantity of the variant in quantity unit.
                                                               12 Info System > History > Enter Filter Criterion menu >
6 Enter new rack.                                                 <F3>.
```

---

## Issue 70

```
    Workflow
1 Select Booking > Out (order-related) menu.                      Check booking:
     The Stock Out (order-related) dialog opens.                 7 Info System > Booking Status > Unbooked menu: non-
                                                                   booked bookings.
2 Select order.
                                                                 8 Info System > Booking Status > Errors menu: incorrect
     Items of the order are displayed.
                                                                   bookings.
3 Select item of the order for removal.
                                                                 9 Info System > History > Enter Filter Criterion menu >
4 Enter quantity of the article.                                   <F3>.
```

---

## Issue 71

```
    Workflow
1 Select Booking > Stack in menu.                                Check booking:
     The Stack Warehouse In dialog opens.                       7 Info System > Booking Status > Unbooked menu: non-
                                                                  booked bookings.
2 Select stack warehouse and supplier.
                                                                8 Info System > Booking Status > Errors menu: incorrect
3 Use <Shift> + <F8> to create a new stack number.
                                                                  bookings.
4 Enter article variant, article quantity, and purchase price
                                                                9 Info System > History > Enter Filter Criterion menu >
  per piece or per quantity unit.
```

---

## Issue 72

```
     Existing stacks will be displayed.
                                                              11 Info System > Booking Status > Unbooked menu: non-
3 Select stack and enter new total quantity in the Quantity
                                                                 booked bookings.
  field.
                                                              12 Info System > Booking Status > Errors menu: incorrect
4 Confirm booking with <End>.
                                                                 bookings.
     Stack is set to the quantity entered.
                                                              13 Info System > History > Enter Filter Criterion menu >
 Book article from the stack warehouse:                         <F3>.
```

---

## Issue 73

```
    Workflow
1 Select Booking > Correction menu.                           Check bookings:
     The Booking Correction dialog opens.                    6 Info System > Booking Status > Unbooked menu: non-
                                                               booked bookings.
2 Enter filter criteria.
                                                             7 Info System > Booking Status > Errors menu: incorrect
     The hit list for the search is displayed.
                                                               bookings.
3 Correct quantities/number and/or price in the columns.
                                                             8 Info System > History > Enter Filter Criterion menu >
4 Open the detail view of the selected data record with        <F3>.
```

---

## Issue 74

```
                                     history.

• View orders/purchase orders      • View information about order and rack-related
                                     bookings.

• View booking status              • View and correct bookings not booked or with errors.
                                   • Call up overview for all stocks in the inventory.

• View available stock inventory   • View ordered, planned, and available stock inventory.

• View stock forecast              • View inventory forecast for planned stock inventories
```

---

## Issue 75

```




    Goal of the action
•    View and correct bookings not booked or with errors.      •   Call up overview for all stocks in the inventory.

    Requirements



```

---

## Issue 76

```
    Requirements



    Additional information
Information about the booking status for incorrect data re-    following dialogs: Info System > Booking Status > Error, In-
cords and for the inventory is listed in the same way on the   ventory.

    Workflow
1 Info System > Booking Status > Unbooked menu: non-           3 Correct data.
  booked bookings.
```

---

## Issue 77

```
cords and for the inventory is listed in the same way on the   ventory.

    Workflow
1 Info System > Booking Status > Unbooked menu: non-           3 Correct data.
  booked bookings.
                                                               4 Use <Ctrl> + <F8> after correction of the error cause to
     The Booking Status dialog for unbooked data records         reset the error status.
     opens.
                                                               5 Active the stock booker with <Shift> + <F8>.
2 Open the detail view of the selected data record with
                                                               6 Save correction with <End>.
```

---

## Issue 78

```

    Workflow
1 Info System > Booking Status > Unbooked menu: non-           3 Correct data.
  booked bookings.
                                                               4 Use <Ctrl> + <F8> after correction of the error cause to
     The Booking Status dialog for unbooked data records         reset the error status.
     opens.
                                                               5 Active the stock booker with <Shift> + <F8>.
2 Open the detail view of the selected data record with
                                                               6 Save correction with <End>.
  <F5>.
```

---

## Issue 79

```


                   Start functional test (F test)
                   <Ctrl> + <F4> > <Shift> + <F12> > <9> > [No]
                   This combination of keys will start the functional test. The service engineers
                   need this recording of program flow to be able to find the causes of errors.
                   Please obey the following things in connection with the functional test:
                   •   Only switch it on if asked to do so by a service engineer.
                   •   Once started, every action of the software will be recorded.
                   •   Requires additional computing capacity and memory.
                   •   Can be executed together with database recording.
```

---

## Issue 80

```
– Discount method B-223                     Enter value
– Discounts B-227                           – search for original number D-1124
Document entry A-25                         – search for reference D-1123
Document Field Configuration B-499          Entry w/o prices D-1132
Document type                               ERP System A-22, A-23
– Allocation E-1628                         Error F-1798
Document types                              Evaluation
– Enter or change B-245                     – Market Partner B-132
– Market Partner B-168                      – Menu overview F-1695
– output type D-1222                        Exchange
Documents                                   – assign exchange list C-614, C-616
```

---

## Issue 81

```
IG                                        – Booking status, correction F-1801
– base prices C-584                       Info system
– calculation type single price C-584     – Available stock F-1807
– create exchange list C-610              – Booking status, booking records not
– Spec exchange prices C-930                booked F-1796
– Spec. basic prices C-942                – Booking status, error F-1798
– Spec. exchange prices C-949             – Booking status, inventory F-1800
– Spec. product group factors C-895       – Menu overview F-1696
IG exchange prices                        – Orders/purchase orders F-1792, F-1793,
– spec. minimum price C-933                 F-1794
– Spec. prices C-930                      – Stock forecast F-1809
```

---

## Issue 82

```
IG exchange prices                        – Orders/purchase orders F-1792, F-1793,
– spec. minimum price C-933                 F-1794
– Spec. prices C-930                      – Stock forecast F-1809
– spec. surcharges C-933                  – Stock range F-1806
IG prices                                 Information
– AIR surcharges C-736                    – error D-1238
– basic prices C-704                      – market partner D-1195
– convert matrices C-724                  – note text D-1300
– Exchange TG/LAMI/Special C-730          – order display D-1465
– master data C-703                       Information system A-35
– Matrix editor C-715                     Input without prices D-1032
```

---

