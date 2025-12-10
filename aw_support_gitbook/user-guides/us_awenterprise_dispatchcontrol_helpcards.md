---
title: "US AWEnterprise DispatchControl HelpCards"
category: "user_manuals"
product: "Unknown"
doc_type: "Unknown"
language: "EN"
tags: ["US_AWEnterprise_DispatchControl_HelpCards"]
version: "1.0"
last_updated: "2025-12-10"
description: "Dispatch Control                G                           Help Cards                        A+W Enterprise                  Help Cards                                                                                    Dispatch Control                      Dispatch Control                  The depictions in the Help Cards are based on delivery version A+W Enterprise 6. Individual steps in the                  workflows may differ depending on the configuration, e.g. working with or without Dis"
source_file: "US_AWEnterprise_DispatchControl_HelpCards.pdf"
---


# US AWEnterprise DispatchControl HelpCards

Dispatch Control                G

                         Help Cards




                   A+W Enterprise
                 Help Cards                                                                                    Dispatch Control




                 Dispatch Control
                 The depictions in the Help Cards are based on delivery version A+W Enterprise 6. Individual steps in the
                 workflows may differ depending on the configuration, e.g. working with or without Dispatch Explorer.
                 For the purpose of distinction:
                 •   The route can be a fixed driving route that is driven on particular days, e.g.
                     route 300 from Frankfurt to Munich is driven on Mondays and Thursdays.
                 •   The route can be the route to be driven on a particular delivery date, e.g.
                     the route on route 300 delivers the customer orders on Thursday April 28, 2016.

                 Dispatch Explorer

                 Help Card                                           Subjects

                 • Work without Dispatch Explorer                    • Search for delivery/deliveries on a date.
                                                                     • View item for the order.

                 • Work with Dispatch Explorer                       • Search for routes on a date.
                                                                     • Search for delivery on a date.
                                                                     • View item for the order.


                 Editing a route

                 Help Card                                           Subjects

                 • Shift a route                                     • Shift route to another delivery date.
                                                                     • Shift route to another route.

                 • Shift an order                                    • Shift order to another delivery date or another route.
                                                                     • Shift several orders.

                 • Shift an item                                     • Shift item to another delivery date.
                                                                     • Shift item to another route.

                 • Shift several items                               • Shift all items not delivered from the previous day.
                                                                     • Shift several items of an order to another route or
                                                                       another delivery date.
                                                                     • Shift individual quantities to another delivery date.

                 • Shift with the context menu                       • Shift routes, orders, or items in the Explorer.
1.04 / 01-2017




                 A+W Enterprise                                                                                                 2
                 Help Cards                                                               Dispatch Control




                 Preparing dispatch

                 Help Card                       Subjects

                 • Check a missing quantity      • Check quantities produced.
                                                 • Book available quantity as packed.
                                                 • Shift missing quantity as backlog.

                 • Correct packed quantity       • Check quantities packed.
                                                 • Change quantity reported packed.

                 • Change the delivery address   • Select alternative delivery address.
                                                 • Enter new address for delivery of backlogs.

                 • Create a delivery note        • Print preliminary delivery note.
                                                 • Create final delivery note.

                 • Edit loading sequence         •   Change loading sequence.
                                                 •   Print loading list for a route.
                                                 •   Print loading list for all routes.
                                                 •   Print supplementary loading list.

                 • Cancel transaction            Cancel transaction:
                                                 • Order
                                                 • Delivery note
                                                 • Dispatch status


                 Additional functions

                 Help Card                       Subjects

                 • Display route graphic         • Display utilization of the routes for a delivery date.
                                                 • Display utilization of a route on subsequent delivery
                                                   days.

                 • View order info               • View information about the order.
                                                 • View information about the finished products stock for
                                                   the order.
                                                 • View booking protocol for the finished products stock.
1.04 / 01-2017




                 A+W Enterprise                                                                             3
A+W Enterprise Dispatch control


Dispatch Explorer                                                          Work without Dispatch Explorer                                        VS 01-001


Objective of this activity
•   Search for delivery/deliveries on a date.
•   View items for the order.


Prerequisites
•   Working without Dispatch Explorer must be configured in the program.
•   Routes are planned.


Additional information
•   SA Deliv: Standard mode for the search (sales - delivery).
•   SA-IGin., SA-IGout.: Mode for purchasing. Must be configured.
•   [Skip]: Order search via the order or customer number.

 Shift a route
 Shift an order
 Shift an item


Workflow                                                                   View items for the order.
1 Select menu Logistics > Dispatch Control.                                4 Open the Order tab: Double-click on route or [Orders] or <F5>.
    The Dispatch Control dialog opens.                                         All orders for the route are displayed.
2 Enter at least the following search criteria:                            5 Open the Dispatch Info I tab: Double-click on order or [Items] or <F5>.
    •   Site: Site.                                                            All items of the order are displayed.
    •   Group: Dispatch group.                                             6 Open the Dispatch Info II tab: Click [Menu Version] or the Item Info II tab.
    •   Delivery date: Date for which the route is planned.
                                                                               The Dispatch Info II tab opens with the dimensions for the items of the order.
3 Start search with <Enter>.
                                                                           
    The Dispatch Control – Route Info dialog opens with the hit list.
    From here, you can start all actions for editing the route data.




                                                                                                                                                     1.04 / 01-2017
A+W Enterprise Dispatch control


Dispatch Explorer                                                             Work with Dispatch Explorer                                            VS 01-002


Objective of this activity
•   Search for routes in a time period.
•   View delivery on a date.
•   View items for the order.


Prerequisites
•   Working with Dispatch Explorer must be configured in the program.
•   Routes are planned.


Additional information
You can access all important commands for dispatch control with <F4>.
 Shift a route
 Shift an order
 Shift an item




Workflow                                                                      4 Open up levels: Open nodes {+} on the day you are searching for.
1 Select menu Logistics > Dispatch Control.                                   5 Repeat step 4 for route level.
    The Dispatch Control dialog opens.                                            Orders in the route are displayed in the detail view.
2 Enter at least the following search criteria:                               6 Select the route in the explorer view and select [Details].
    •   Site: Site.                                                               The Route Info tab opens with the routes for the selected day.
    •   Group: Dispatch group.                                                    From here, you can start all actions for editing the route data.
    •   Delivery date: Enter the start and end date for routes in a period.
                                                                              7 Use [Explorer] to jump back to the Explorer view.
3 Start search with <Enter>.
                                                                              
    All days with planned routes are displayed in the Dispatch Explorer.
                                                                              Steps 4 to 7 apply analogously for the order and item level.
    In the detail view, the routes for the selected days are displayed.




                                                                                                                                                        1.04 / 01-2017
A+W Enterprise Dispatch control


Editing a route                                                                             Shift a route                                                           VS 02-001


Objective of this activity
•   Shift route to another delivery date.
•   Shift route to another route.


Prerequisites
•   Routes are displayed in the dispatch control.


Additional information
If the new delivery date does not fit the selected route, the route is not shifted to the
new delivery date. If a deviating route is defined, the route is shifted to this route.
 Shift an order
 Shift an item
 Shift several items




Workflow                                                                                    Shift route to another route for the same date:
1 Route Info tab: Select route > [Shift].                                                   6 To date field: Check delivery date.
    The Move (Dispatch) dialog opens.                                                       7 Enter new route in the Route field:
2 Select reason for the shift with <Space bar> and enter a note if necessary.                   If the delivery date is not a route day, the route cannot be shifted.
3 To date field: Enter delivery date.                                                       8 Make the shift with [Start].
    If the new date is not a valid route day, the route cannot be shifted.                      The route is shifted completely to the new route.
    If a route plan has been created: press <F9> in the To date field and select the            If the delivery date is retained, the route is displayed with the new route number.
    route.                                                                                  
4 Make the shift with [Start].
    The route is shifted completely to the new delivery date. It is no longer displayed
    on the Route Info tab.
5 Check shift: Start route search with new delivery date.



                                                                                                                                                                        1.04 / 01-2017
A+W Enterprise Dispatch control


Editing a route                                                                             Shift an order                                                          VS 02-002


Objective of this activity
•   Shift order to another delivery date or another route.
•   Shift several orders.


Prerequisites
•   Routes are displayed in the dispatch control.


Additional information
If the new delivery date does not fit the selected route, the route is not shifted to the
new delivery date. If a deviating route is defined, the shift is made here.
Selection of the reason: for operating or customer cancellation, the item is deleted
from the order.
 Shift an item
 Shift several items




Workflow                                                                                    Shift several orders of the route:
1 Route Info tab > open order level.                                                        7 Enter delivery date and route.
2 Select order > [Shift].                                                                       If the delivery date is not a route day, the order cannot be shifted.
    The Move (Dispatch) dialog opens.                                                       8 Shift several records field: Select Y (yes).
3 Select reason for the shift with <Space bar> and enter a note if necessary. See also 9 Make the shift with [Start].
  the additional info.                                                                 10 If necessary, answer the query with [Yes].
4 To date field: Change delivery date.                                                          The orders are shifted.
5 Enter new route in the Route field if necessary:                                          11 Check shift: Start route search with new delivery date.
    If a route plan has been created: press <F9> in the To date field and select the        
    route.
6 Make the shift with [Start].
    The order is shifted completely to the new delivery date and/or the new route.



                                                                                                                                                                        1.04 / 01-2017
A+W Enterprise Dispatch control


Editing a route                                                                             Shift an item                                                             VS 02-003


Objective of this activity
•   Shift individual item to another delivery date.
•   Shift individual item to another route.


Prerequisites
•   Routes are displayed on the Route Info tab.
•   Customer allows partial delivery.


Additional information
If the new delivery date does not fit the selected route, the route is not shifted to the
new delivery date. If a deviating route is defined, the shift is made here.
Selection of the reason: for operating or customer cancellation, the item is deleted
from the order.
 Shift several items




Workflow                                                                                    Shift route to another route for the same date:
1 Route Info tab > Order level > Open item level.                                           8 To date field: Check delivery date.
2 Select item > [Shift].                                                                    9 Route field: Enter route.
    The Move (Dispatch) dialog opens.                                                          If the delivery date is not a route day, the item cannot be shifted.
3 Select reason for the shift with <Space bar> and enter a note if necessary. See also 10 Make the shift with [Start].
  the additional info.                                                                    The item is shifted completely to the new route. If the delivery date was retained:
4 To date field: Change delivery date.                                                         •   The item is displayed with the original order number with the new route number.
5 Route field: Check route.                                                                    •   The item is shifted with the original order number to an existing route.
6 Shift entire item to the new route with [Start].                                           Check shift: Start route search with new delivery date.
    Entire item is shifted to the new route.
7 Check shift: Start route search with new delivery date.




                                                                                                                                                                         1.04 / 01-2017
A+W Enterprise Dispatch control


Editing a route                                                                            Shift several items                                          VS 02-004


Objective of this activity
•   Shift all items not delivered from the previous day.
•   Shift several items of an order to another route or another delivery date.
•   Shift individual quantities to another delivery date.


Prerequisites
•   Routes are displayed on the Route Info tab.
•   Customer allows partial delivery.


Additional information
Items are only booked if the box in the Book column is checked.
Selection of the reason: for operating or customer cancellation, the item is deleted
from the order.
 Shift a route
 Shift an order


Workflow                                                                                   7 Enter data for shifting.
1 Route Info tab to display the delivery date from the previous day.                           See Help Card “Shift an item”, Step 3 to 5.
2 Open relocation dialog with <Ctrl> + <E>.                                                8 Make the shift with [Start].
    The Relocation dialog opens.                                                           9 Answer the query with [Yes].
3 Check the current delivery date and click [Trigger].                                         Selected items are shifted to the new delivery date.
    The Move (Dispatch) dialog opens.                                                          Check the items not shifted.
4 If necessary, enter the quantity in the Shift column.                                    10 Check shift: Start route search with new delivery date.
5 Select the check boxes in the Book column for the shift.                                 
    The selected items are shifted completely. If only partial quantities are specified,
    the appropriate quantities will be shifted.
6 Open dialog for shifting with [Trigger].
    The Move (Dispatch) dialog opens.


                                                                                                                                                           1.04 / 01-2017
A+W Enterprise Dispatch control


Editing a route                                                                       Shift with the context menu   VS 02-005


Objective of this activity
•   Shift routes, orders, or items in the Explorer.
Note:
The shifting of routes, orders, and items via the context menu does not trigger any
status bookings in the order. This form of shifting only makes sense if a single
employee handles the dispatch planning.



Prerequisites
•   The Dispatch Explorer is configured.
•   Routes are displayed in the Dispatch Explorer.


Additional information
 Shift several items




Workflow
1 Open the desired level in the Dispatch Explorer.
2 Place the cursor on the route, order, or item.
3 Open the context menu (right mouse button) and select action, e.g. Cut out order.
4 Open context menu on the target level, e.g. the same route on the following day.
5 Select an action, e.g. Insert.
6 Open the source and target levels and check whether the data has been shifted as
  desired.
    If an individual item has been inserted into a new delivery date, the item is
    displayed with the original order number.





                                                                                                                       1.04 / 01-2017
A+W Enterprise Dispatch control


Preparing dispatch                                                                           Check a missing quantity                                         VS 03-001


Objective of this activity
•   Check quantities produced.
•   Book available quantity as packed.
•   Shift missing quantity as backlog.


Prerequisites
•   Routes are displayed on the Route Info tab.


Additional information
Missing quantity of the item can be treated in different ways:
•   Shift as backlog to another delivery date.
•   As (customer) cancellation, remove from the order and book item as complete.

 Shift an item
 Shift several items



Workflow                                                                                     7 Save corrected quantities with [Booking].
1 Route Info tab > open order level.                                                             Quantity for the backlog is displayed in the B.log column.
2 Select order: <Shift> + <F9>.                                                               Correct packed quantity

    The Missing-qty control for... dialog opens.                                             8 Shift the missing quantity with [Booking].

3 Check the order data and correct if necessary.                                              Shift an item, Step 3 to 6

4 Open missing quantity check with [Trigger].                                                    The Order Info tab is displayed.

    The Dispatch control dialog opens for the missing quantity check.                            The status of the order is set to Completely packed.

5 Check the quantities in the Complt. column.                                                

    If finished quantity is not identical to planned quantity, shift missing quantity. See
    also the additional info.
 Shift several items, Step 4
6 Correct completed quantity after consultation.


                                                                                                                                                                 1.04 / 01-2017
A+W Enterprise Dispatch control


Preparing dispatch                                                                            Correct packed quantity                                              VS 03-002


Objective of this activity
•   Check quantities packed.
•   Change quantity reported packed.


Prerequisites
•   Routes are displayed on the Route Info tab.




Additional information
Lock completely planned route for additional editing: Route level > <Shift> + <F10>




Workflow                                                                                      Reduce quantity reported packed:
1 Route Info tab > open item level.                                                           8 Correct packed quantity in the Pack column.
2 Select item for the booking of the packed quantity.                                             The Booking protocol dialog opens.
3 Check quantity packed in the Pack column.                                                   9 Enter booking data.
    If the packed quantity is not identical to the finished quantity, ask about the current   10 Confirm reduction of the packed quantity with [Book].
    state of packing.                                                                             Quantity reported packed is booked. Quantity not packed is displayed in the B.log
4 Correct packed quantity after consultation. Enable correction mode with                         field.
  <Shift> + <F10>.                                                                            11 Shift reduced quantity to another delivery date.
    Cursor jumps to the Pack column.                                                           Shift several items, Step 4
5 Correct packed quantity in the Pack column.                                                 
6 Book packed quantity: Select Cmp check box.
    Packed quantity is booked. Item status is implemented.
7 Repeat steps 2 to 3 as needed for each item.

                                                                                                                                                                        1.04 / 01-2017
A+W Enterprise Dispatch control


Preparing dispatch                                                               Change the delivery address                                     VS 03-003


Objective of this activity
•   Select alternative delivery address.
•   Enter new address for delivery of backlogs.


Prerequisites
•   Routes are displayed on the Route Info tab.




Additional information
•   A new address can be taken over into the customer’s master data with <F3>.
•   Lock completely planned route for additional editing: Route level >
    <Shift> + <F10>




Workflow                                                                         Enter address for direct delivery:
1 Route Info tab > open order level.                                             4 Select order: Select <F4> > Delivery address > New shipping address.
2 Select order: <Shift> + <F8>.                                                      The dialog for entering the address is displayed.
    The Delivery address dialog opens.                                           5 Enter data for direct delivery.
3 Select address and take over with [OK].                                        6 If necessary, change the route: [Search route].
    Shipping address tab: Check address.                                         7 Take over address with [OK].
                                                                                     Shipping address tab: Check address.
                                                                                 




                                                                                                                                                     1.04 / 01-2017
A+W Enterprise Dispatch control


Preparing dispatch                                                                        Create a delivery note                                                   VS 03-004


Objective of this activity
•   Print preliminary delivery note.
•   Create final delivery note.


Prerequisites
•   Printing of preliminary and final delivery notes is configured.
•   Routes are displayed on the Route Info tab.
•   Order is reported completely packed.


Additional information
•   Delivery notes can only be printed if the item is reported as completely packed.
•   Depending on the configuration, the invoice is also printed with the delivery note.
    By default, the transfer to the invoice printing is not configured.




Workflow                                                                                  Create final delivery note:
1 Route Info tab > open order level.                                                      8 Select order: <F4> > <Ctrl> + <F9>.
2 Select order: <Ctrl> + <F11>.                                                               The Disp.note release for... dialog opens.
    The Prelim.disp.note for... dialog opens.                                             9 Check data and adjust if necessary.
3 Check data and adjust if necessary.                                                     10 Book delivery note release with [Trigger].
4 Start printing with [Trigger].                                                              The Print on dialog opens.
    The Print on dialog opens.                                                            11 Specify printer and number of copies to be printed.
5 Specify printer and number of copies to be printed.                                     12 Start delivery note printing with <Enter>.
    Generally you must print at least 2 copies.                                               Delivery note is printed. Order status is set to locked.
6 Start printing of the preliminary delivery note with <Enter>.                               Depending on the configuration, the invoice printing is initiated.
7 Confirm print query with [No].                                                          
    The copies of the preliminary delivery note are printed.


                                                                                                                                                                      1.04 / 01-2017
A+W Enterprise Dispatch control


Preparing dispatch                                                                       Edit loading sequence                                                     VS 03-005


Objective of this activity
•   Change loading sequence.
•   Print loading list for a route.
•   Print loading list for all routes.
•   Print supplementary loading list.


Prerequisites
•   Functions for the loading sequence must be configured.
•   Routes are displayed on the Route Info tab.


Additional information
•   It is only possible to print additional loading lists for printed loading lists.
•   Lock completely planned route for additional editing: Route level >
    <Shift> + <F10>




Workflow                                                                                 Print loading lists for all routes displayed:
1 Route Info tab > open order level.                                                     4 Route Info tab: <Ctrl> + <F12>.
2 Change to the Shipping address tab.                                                    5 Check site and time period and adjust if necessary.
3 Field LS: Change sequential number.                                                    6 Confirm entry with <Enter>.
4 Answer query about whether the number should be assigned to the customer’s             7 Specify printer and number of copies to be printed.
  other orders.                                                                          8 Start printing with <Enter>.
    The sequential number is inserted for all orders that belong to the same customer.       Loading list is printed. The status is set to Locked.
Print new loading list:                                                                  Print supplementary loading list:
1 Route Info tab: <Ctrl> + <F8>.                                                         1 Route Info tab: <Ctrl> + <F10>.
2 Specify printer and number of copies to be printed.                                    2 Repeat steps 5 to 8.
3 Start printing with <Enter>.                                                               Loading lists with the additions to the original loading list are printed.
    Loading list is printed. The status is set to Locked.                                


                                                                                                                                                                          1.04 / 01-2017
A+W Enterprise Dispatch control


Preparing dispatch                                          Cancel transaction                                                      VS 03-006


Objective of this activity
Cancel transaction:
•   Order
•   Delivery note
•   Dispatch status


Prerequisites
•   Cancellation function is configured.
•   Routes are displayed on the Route Info tab.



Additional information
 View order info




Workflow                                                    8 Specify reason for cancellation and confirm with <Enter>.
1 Open menu Logistics > Dispatch control > desired level.       The transaction is canceled. The canceled identifier and the reason for
                                                                cancellation are taken over into the transaction, e.g. into the delivery note or the
2 Select a transaction, e.g. order.                             order.
3 Open info menu with <Shift> + <F4>.                       
    Info menu is opened.
4 Select Cancel.
    Submenu opens.
5 Select type of cancellation, e.g. Order cancellation.
    The Order cancellation dialog opens.
6 Check data and confirm with [Trigger].
7 If necessary, confirm the query with [Yes].
    Dialog for reason opens.


                                                                                                                                        1.04 / 01-2017
A+W Enterprise Dispatch control


Additional functions                                                  Display route graphic                                                VS 04-001


Objective of this activity
•   Display utilization of the routes for a delivery date.
•   Display utilization of a route on subsequent delivery days.


Prerequisites
•   Routes are displayed on the Route Info tab.



Additional information




Workflow                                                              Display utilization of a route.
1 Route Info tab:                                                     7 Select parameter 1 and confirm with <Enter>.
2 Parameter selection with <Shift> + <F11>.                               Dialog 2. parameter for the overview opens.
    Dialog 1. parameter for the overview opens.                       8 Select parameter: Show next delivery days for the current route.
3 Select parameter 1: Quantity, QM, weight.                           9 Confirm with <Enter>.
4 Confirm with <Enter>.                                                   Utilization of the route on subsequent days is displayed.
    Dialog 2. parameter for the overview opens.                       
5 Select parameter: Show all routes for the current delivery round.
6 Confirm with <Enter>.
    Actual and target quantities for the routes are displayed.




                                                                                                                                              1.04 / 01-2017
A+W Enterprise Dispatch control


Additional functions                                                    View order info                                                   VS 04-002


Objective of this activity
•   View information about the order.
•   View information about the finished products stock for the order.
•   View booking protocol for the finished products stock.


Prerequisites
•   Routes are displayed on the Route Info tab.
•   Finished products stock must be configured.




Additional information




Workflow                                                                View orders in finished products stock:
1 Route Info tab > open order level.                                    7 Open information about booking protocol of the finished products stock with [FG
                                                                          stock].
2 Select order: <Ctrl> + <K>.
                                                                            The Finished products stock booking log dialog opens.
    Information on document dialog opens.
                                                                        View bookings in finished products stock:
3 Enter order number.
                                                                        8 Open overview for finished goods stock with [Protocol].
4 Check mode: SA Deliv.
                                                                            The Finished products stock overview dialog opens.
5 Start search with [Trigger].
                                                                        
    Information on order dialog opens.
6 Exit order info: use [Skip] to return to the Item info tab.




                                                                                                                                              1.04 / 01-2017

