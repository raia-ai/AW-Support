---
title: "US_AWEnterprise_DispatchControl_HelpCards"
source: "US_AWEnterprise_DispatchControl_HelpCards.pdf"
tags: ["A+W Enterprise", "Dispatch Control", "Software Help Guide", "Logistics Management", "Route Planning", "Dispatch Explorer", "Order Management", "Glass Manufacturing", "Window Manufacturing", "Door Manufacturing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A user guide for the A+W Enterprise Dispatch Control module, providing step-by-step instructions (Help Cards) for tasks like managing routes, editing orders, preparing dispatch, and using the Dispatch Explorer."
long_description: "This document is a collection of 'Help Cards' from A+W, a software provider for the glass, windows, and doors industry. It details procedures for the Dispatch Control module in A+W Enterprise version 6. The guide is designed to assist users in performing key logistical functions, covering topics such as searching for deliveries, working with and without the Dispatch Explorer, and editing routes, orders, and individual items. It also provides workflows for preparing dispatch, which includes managing missing quantities, correcting packed quantities, changing delivery addresses, creating delivery notes, and editing loading sequences. Additional functions like displaying route graphics and viewing detailed order information are also explained. The document serves as a practical, task-oriented reference for dispatch planners and logistics personnel, with each help card outlining the objective, prerequisites, and a clear, step-by-step workflow."
---

# A+W Enterprise: Dispatch Control Help Cards

---
## Dispatch Control Overview

The depictions in the Help Cards are based on delivery version A+W Enterprise 6. Individual steps in the workflows may differ depending on the configuration, e.g. working with or without Dispatch Explorer.

**For the purpose of distinction:**

*   The route can be a fixed driving route that is driven on particular days, e.g., route 300 from Frankfurt to Munich is driven on Mondays and Thursdays.
*   The route can be the route to be driven on a particular delivery date, e.g., the route on route 300 delivers the customer orders on Thursday, April 28, 2016.

## Dispatch Explorer

| Help Card                        | Subjects                                         |
| -------------------------------- | ------------------------------------------------ |
| Work without Dispatch Explorer   | - Search for delivery/deliveries on a date.      |
|                                  | - View item for the order.                       |
| Work with Dispatch Explorer      | - Search for routes on a date.                   |
|                                  | - Search for delivery on a date.                 |
|                                  | - View item for the order.                       |

## Editing a Route

| Help Card                    | Subjects                                                              |
| ---------------------------- | --------------------------------------------------------------------- |
| Shift a route                | - Shift route to another delivery date.                               |
|                              | - Shift route to another route.                                       |
| Shift an order               | - Shift order to another delivery date or another route.              |
|                              | - Shift several orders.                                               |
| Shift an item                | - Shift item to another delivery date.                                |
|                              | - Shift item to another route.                                        |
| Shift several items          | - Shift all items not delivered from the previous day.                |
|                              | - Shift several items of an order to another route or another delivery date. |
|                              | - Shift individual quantities to another delivery date.               |
| Shift with the context menu  | - Shift routes, orders, or items in the Explorer.                     |

## Preparing Dispatch

| Help Card                   | Subjects                                               |
| --------------------------- | ------------------------------------------------------ |
| Check a missing quantity    | - Check quantities produced.                           |
|                             | - Book available quantity as packed.                   |
|                             | - Shift missing quantity as backlog.                   |
| Correct packed quantity     | - Check quantities packed.                             |
|                             | - Change quantity reported packed.                     |
| Change the delivery address | - Select alternative delivery address.                 |
|                             | - Enter new address for delivery of backlogs.          |
| Create a delivery note      | - Print preliminary delivery note.                     |
|                             | - Create final delivery note.                          |
| Edit loading sequence       | - Change loading sequence.                             |
|                             | - Print loading list for a route.                      |
|                             | - Print loading list for all routes.                   |
|                             | - Print supplementary loading list.                    |
| Cancel transaction          | Cancel transaction: Order, Delivery note, Dispatch status |

## Additional Functions

| Help Card             | Subjects                                                       |
| --------------------- | -------------------------------------------------------------- |
| Display route graphic | - Display utilization of the routes for a delivery date.       |
|                       | - Display utilization of a route on subsequent delivery days.  |
| View order info       | - View information about the order.                            |
|                       | - View information about the finished products stock for the order. |
|                       | - View booking protocol for the finished products stock.       |

---

## Dispatch Explorer

### Work without Dispatch Explorer (VS 01-001)

> [UI Screenshot: The "Dispatch control" window is shown with a list of routes. The columns include Route, Total, Call, Pack, B.log, kg, sqm, etc. A single route "300 Region West" is displayed.]

**Objective of this activity**
*   Search for delivery/deliveries on a date.
*   View items for the order.

**Prerequisites**
*   Working without Dispatch Explorer must be configured in the program.
*   Routes are planned.

**Additional information**
*   `SA Deliv`: Standard mode for the search (sales - delivery).
*   `SA-IGin.`, `SA-IGout.`: Mode for purchasing. Must be configured.
*   `[Skip]`: Order search via the order or customer number.
*   See also: Shift a route
*   See also: Shift an order
*   See also: Shift an item

**Workflow**
1.  Select menu `Logistics > Dispatch Control`. The `Dispatch Control` dialog opens.
2.  Enter at least the following search criteria:
    *   **Site**: Site.
    *   **Group**: Dispatch group.
    *   **Delivery date**: Date for which the route is planned.
3.  Start search with `<Enter>`. The `Dispatch Control – Route Info` dialog opens with the hit list. From here, you can start all actions for editing the route data.
4.  Open the **Order** tab: Double-click on route or click `[Orders]` or `<F5>`. All orders for the route are displayed.
5.  Open the **Dispatch Info I** tab: Double-click on order or click `[Items]` or `<F5>`. All items of the order are displayed.
6.  Open the **Dispatch Info II** tab: Click `[Menu Version]` or the **Item Info II** tab. The **Dispatch Info II** tab opens with the dimensions for the items of the order.

---

### Work with Dispatch Explorer (VS 01-002)

> [UI Screenshot: The "Dispatch control" window is shown in Explorer view. A hierarchical tree on the left shows dates, routes, orders, and items. The right pane displays details of the selected item.]

**Objective of this activity**
*   Search for routes in a time period.
*   View delivery on a date.
*   View items for the order.

**Prerequisites**
*   Working with Dispatch Explorer must be configured in the program.
*   Routes are planned.

**Additional information**
*   You can access all important commands for dispatch control with `<F4>`.
*   See also: Shift a route
*   See also: Shift an order
*   See also: Shift an item

**Workflow**
1.  Select menu `Logistics > Dispatch Control`. The `Dispatch Control` dialog opens.
2.  Enter at least the following search criteria:
    *   **Site**: Site.
    *   **Group**: Dispatch group.
    *   **Delivery date**: Enter the start and end date for routes in a period.
3.  Start search with `<Enter>`. All days with planned routes are displayed in the Dispatch Explorer. In the detail view, the routes for the selected days are displayed.
4.  Open up levels: Open nodes (`+`) on the day you are searching for.
5.  Repeat step 4 for route level. Orders in the route are displayed in the detail view.
6.  Select the route in the explorer view and select `[Details]`. The **Route Info** tab opens with the routes for the selected day. From here, you can start all actions for editing the route data.
7.  Use `[Explorer]` to jump back to the Explorer view.
*Steps 4 to 7 apply analogously for the order and item level.*

---

## Editing a Route

### Shift a route (VS 02-001)

> [UI Screenshot: The "Move (dispatch)" dialog is displayed. It shows fields for "Frm rte day", "Route", "Order", "Item", and allows setting a new "To date" and "Route" for the transfer.]

**Objective of this activity**
*   Shift route to another delivery date.
*   Shift route to another route.

**Prerequisites**
*   Routes are displayed in the dispatch control.

**Additional information**
*   If the new delivery date does not fit the selected route, the route is not shifted to the new delivery date. If a deviating route is defined, the route is shifted to this route.
*   See also: Shift an order
*   See also: Shift an item
*   See also: Shift several items

**Workflow**
1.  In the **Route Info** tab: Select a route > `[Shift]`. The `Move (Dispatch)` dialog opens.
2.  Select a reason for the shift with `<Space bar>` and enter a note if necessary.
3.  In the **To date** field: Enter a new delivery date.
    *   If the new date is not a valid route day, the route cannot be shifted.
    *   If a route plan has been created: press `<F9>` in the **To date** field and select the route.
4.  Make the shift with `[Start]`. The route is shifted completely to the new delivery date. It is no longer displayed on the **Route Info** tab.
5.  Check shift: Start a route search with the new delivery date.

**Shift route to another route for the same date:**
6.  In the **To date** field: Check the delivery date.
7.  Enter a new route in the **Route** field. If the delivery date is not a route day, the route cannot be shifted.
8.  Make the shift with `[Start]`. The route is shifted completely to the new route. If the delivery date is retained, the route is displayed with the new route number.

---

### Shift an order (VS 02-002)

> [UI Screenshot: A composite image showing the main "Dispatch control" window with the "Order info" tab active. Overlaid are two different "Move (dispatch)" dialogs, one for a single order shift and one for shifting several records.]

**Objective of this activity**
*   Shift an order to another delivery date or another route.
*   Shift several orders.

**Prerequisites**
*   Routes are displayed in the dispatch control.

**Additional information**
*   If the new delivery date does not fit the selected route, the route is not shifted to the new delivery date. If a deviating route is defined, the shift is made here.
*   **Selection of the reason**: For operating or customer cancellation, the item is deleted from the order.
*   See also: Shift an item
*   See also: Shift several items

**Workflow**
1.  Go to the **Route Info** tab > open the order level.
2.  Select an order > `[Shift]`. The `Move (Dispatch)` dialog opens.
3.  Select a reason for the shift with `<Space bar>` and enter a note if necessary. See also the additional info.
4.  **To date** field: Change the delivery date.
5.  Enter a new route in the **Route** field if necessary. If a route plan has been created, press `<F9>` in the **To date** field and select the route.
6.  Make the shift with `[Start]`. The order is shifted completely to the new delivery date and/or the new route.

**Shift several orders of the route:**
7.  Enter the delivery date and route. If the delivery date is not a route day, the order cannot be shifted.
8.  **Shift several records** field: Select Y (yes).
9.  Make the shift with `[Start]`.
10. If necessary, answer the query with `[Yes]`. The orders are shifted.
11. Check shift: Start a route search with the new delivery date.

---

### Shift an item (VS 02-003)

> [UI Screenshot: The "Move (dispatch)" dialog is shown, configured to move a single item (Item 1 from Order 239611). It allows specifying a reason, a new date, and a new route for the item.]

**Objective of this activity**
*   Shift an individual item to another delivery date.
*   Shift an individual item to another route.

**Prerequisites**
*   Routes are displayed on the **Route Info** tab.
*   Customer allows partial delivery.

**Additional information**
*   If the new delivery date does not fit the selected route, the route is not shifted to the new delivery date. If a deviating route is defined, the shift is made here.
*   **Selection of the reason**: For operating or customer cancellation, the item is deleted from the order.
*   See also: Shift several items

**Workflow**
1.  Go to **Route Info** tab > Order level > Open item level.
2.  Select an item > `[Shift]`. The `Move (Dispatch)` dialog opens.
3.  Select a reason for the shift with `<Space bar>` and enter a note if necessary. See also the additional info.
4.  **To date** field: Change the delivery date.
5.  **Route** field: Check the route.
6.  Shift the entire item to the new route with `[Start]`. The entire item is shifted to the new route.
7.  Check shift: Start a route search with the new delivery date.

**Shift item to another route for the same date:**
8.  **To date** field: Check the delivery date.
9.  **Route** field: Enter a new route. If the delivery date is not a route day, the item cannot be shifted.
10. Make the shift with `[Start]`. The item is shifted completely to the new route. If the delivery date was retained:
    *   The item is displayed with the original order number with the new route number.
    *   The item is shifted with the original order number to an existing route.
*   Check shift: Start a route search with the new delivery date.

---

### Shift several items (VS 02-004)

> [UI Screenshot: A composite image showing the "Dispatch control" window with items listed. A "Move (dispatch)" dialog is open for shifting items, and a final "ATTENTION" confirmation box asks "Do you want to shift all entered quantities?".]

**Objective of this activity**
*   Shift all items not delivered from the previous day.
*   Shift several items of an order to another route or another delivery date.
*   Shift individual quantities to another delivery date.

**Prerequisites**
*   Routes are displayed on the **Route Info** tab.
*   Customer allows partial delivery.

**Additional information**
*   Items are only booked if the box in the **Book** column is checked.
*   **Selection of the reason**: For operating or customer cancellation, the item is deleted from the order.
*   See also: Shift a route
*   See also: Shift an order

**Workflow**
1.  Use the **Route Info** tab to display the delivery date from the previous day.
2.  Open the relocation dialog with `<Ctrl> + <E>`. The `Relocation` dialog opens.
3.  Check the current delivery date and click `[Trigger]`. The `Move (Dispatch)` dialog opens.
4.  If necessary, enter the quantity in the **Shift** column.
5.  Select the check boxes in the **Book** column for the shift. The selected items are shifted completely. If only partial quantities are specified, the appropriate quantities will be shifted.
6.  Open the dialog for shifting with `[Trigger]`. The `Move (Dispatch)` dialog opens.
7.  Enter data for shifting. See Help Card "Shift an item", Steps 3 to 5.
8.  Make the shift with `[Start]`.
9.  Answer the query with `[Yes]`. Selected items are shifted to the new delivery date. Check the items not shifted.
10. Check shift: Start a route search with the new delivery date.

---

### Shift with the context menu (VS 02-005)

> [UI Screenshot: Two views of the Dispatch Explorer are shown. The first shows a right-click context menu with the option "Cut out order" selected. The second shows the context menu on a different date with the "Insert" option available.]

**Objective of this activity**
*   Shift routes, orders, or items in the Explorer.

**Note:**
The shifting of routes, orders, and items via the context menu does not trigger any status bookings in the order. This form of shifting only makes sense if a single employee handles the dispatch planning.

**Prerequisites**
*   The Dispatch Explorer is configured.
*   Routes are displayed in the Dispatch Explorer.

**Additional information**
*   See also: Shift several items

**Workflow**
1.  Open the desired level in the Dispatch Explorer.
2.  Place the cursor on the route, order, or item.
3.  Open the context menu (right mouse button) and select an action, e.g., `Cut out order`.
4.  Open the context menu on the target level, e.g., the same route on the following day.
5.  Select an action, e.g., `Insert`.
6.  Open the source and target levels and check whether the data has been shifted as desired.
    *   If an individual item has been inserted into a new delivery date, the item is displayed with the original order number.

---

## Preparing Dispatch

### Check a missing quantity (VS 03-001)

> [UI Screenshot: A composite image showing the "Dispatch control" window with an item list, where the "Complt" and "Pack" quantities differ. A "Missing-qty control for..." dialog is open, leading to a "Dispatch control" dialog for managing the discrepancy.]

**Objective of this activity**
*   Check quantities produced.
*   Book available quantity as packed.
*   Shift missing quantity as backlog.

**Prerequisites**
*   Routes are displayed on the **Route Info** tab.

**Additional information**
*   Missing quantity of the item can be treated in different ways:
    *   Shift as backlog to another delivery date.
    *   As (customer) cancellation, remove from the order and book item as complete.
*   See also: Shift an item
*   See also: Shift several items

**Workflow**
1.  Go to **Route Info** tab > open order level.
2.  Select an order: `<Shift> + <F9>`. The `Missing-qty control for...` dialog opens.
3.  Check the order data and correct if necessary.
4.  Open missing quantity check with `[Trigger]`. The `Dispatch control` dialog opens for the missing quantity check.
5.  Check the quantities in the **Complt.** column. If the finished quantity is not identical to the planned quantity, shift the missing quantity. See also the additional info. (See also: `Shift several items, Step 4`)
6.  Correct the completed quantity after consultation.
7.  Save corrected quantities with `[Booking]`. The quantity for the backlog is displayed in the **B.log** column. (See also: `Correct packed quantity`)
8.  Shift the missing quantity with `[Booking]`. (See also: `Shift an item, Step 3 to 6`). The **Order Info** tab is displayed. The status of the order is set to **Completely packed**.

---

### Correct packed quantity (VS 03-002)

> [UI Screenshot: The "Dispatch control" window is on the "Item info I" tab. The "Pack" quantity is highlighted. A "Booking protocol" dialog is open, where a booking text can be entered.]

**Objective of this activity**
*   Check quantities packed.
*   Change quantity reported packed.

**Prerequisites**
*   Routes are displayed on the **Route Info** tab.

**Additional information**
*   Lock a completely planned route for additional editing: **Route level** > `<Shift> + <F10>`.

**Workflow**
1.  Go to **Route Info** tab > open item level.
2.  Select the item for the booking of the packed quantity.
3.  Check the quantity packed in the **Pack** column. If the packed quantity is not identical to the finished quantity, ask about the current state of packing.
4.  Correct packed quantity after consultation. Enable correction mode with `<Shift> + <F10>`. The cursor jumps to the **Pack** column.
5.  Correct the packed quantity in the **Pack** column.
6.  Book packed quantity: Select the **Cmp** check box. The packed quantity is booked and the item status is implemented.
7.  Repeat steps 2 to 3 as needed for each item.

**Reduce quantity reported packed:**
8.  Correct the packed quantity in the **Pack** column. The `Booking protocol` dialog opens.
9.  Enter booking data.
10. Confirm the reduction of the packed quantity with `[Book]`. The quantity reported packed is booked. The quantity not packed is displayed in the **B.log** field.
11. Shift the reduced quantity to another delivery date. (See also: `Shift several items, Step 4`).

---

### Change the delivery address (VS 03-003)

> [UI Screenshot: The "Search address" dialog is shown. It allows searching for an existing address or entering details for a new one, including name, street, postal code, and contact information.]

**Objective of this activity**
*   Select an alternative delivery address.
*   Enter a new address for the delivery of backlogs.

**Prerequisites**
*   Routes are displayed on the **Route Info** tab.

**Additional information**
*   A new address can be taken over into the customer's master data with `<F3>`.
*   Lock a completely planned route for additional editing: **Route level** > `<Shift> + <F10>`.

**Workflow**
1.  Go to **Route Info** tab > open order level.
2.  Select an order: `<Shift> + <F8>`. The `Delivery address` dialog opens.
3.  Select an address and take over with `[OK]`. Check the address on the **Shipping address** tab.

**Enter address for direct delivery:**
4.  Select an order: Select `<F4> > Delivery address > New shipping address`. The dialog for entering the address is displayed.
5.  Enter data for the direct delivery.
6.  If necessary, change the route: `[Search route]`.
7.  Take over the address with `[OK]`. Check the address on the **Shipping address** tab.

---

### Create a delivery note (VS 03-004)

> [UI Screenshot: Two dialogs are shown. The first is "Prelim.disp.note for...", used for printing a preliminary note. The second is "Dispatch-note release for...", used for creating the final delivery note.]

**Objective of this activity**
*   Print a preliminary delivery note.
*   Create a final delivery note.

**Prerequisites**
*   Printing of preliminary and final delivery notes is configured.
*   Routes are displayed on the **Route Info** tab.
*   The order is reported as completely packed.

**Additional information**
*   Delivery notes can only be printed if the item is reported as completely packed.
*   Depending on the configuration, the invoice is also printed with the delivery note. By default, the transfer to the invoice printing is not configured.

**Workflow**
1.  Go to **Route Info** tab > open order level.
2.  Select an order: `<Ctrl> + <F11>`. The `Prelim.disp.note for...` dialog opens.
3.  Check data and adjust if necessary.
4.  Start printing with `[Trigger]`. The `Print on` dialog opens.
5.  Specify the printer and number of copies to be printed. Generally, you must print at least 2 copies.
6.  Start printing of the preliminary delivery note with `<Enter>`.
7.  Confirm the print query with `[No]`. The copies of the preliminary delivery note are printed.

**Create final delivery note:**
8.  Select an order: `<F4> > <Ctrl> + <F9>`. The `Disp.note release for...` dialog opens.
9.  Check data and adjust if necessary.
10. Book delivery note release with `[Trigger]`. The `Print on` dialog opens.
11. Specify the printer and number of copies to be printed.
12. Start delivery note printing with `<Enter>`. The delivery note is printed. The order status is set to locked. Depending on the configuration, the invoice printing is initiated.

---

### Edit loading sequence (VS 03-005)

> [UI Screenshot: The "Dispatch control" window is open on the "Order info" tab, showing a list of orders with their loading sequence (LS) numbers. A "NOTE" dialog asks to confirm passing on the changed sequence, and a "Print on" dialog is shown for selecting a printer.]

**Objective of this activity**
*   Change loading sequence.
*   Print loading list for a route.
*   Print loading list for all routes.
*   Print supplementary loading list.

**Prerequisites**
*   Functions for the loading sequence must be configured.
*   Routes are displayed on the **Route Info** tab.

**Additional information**
*   It is only possible to print additional loading lists for printed loading lists.
*   Lock a completely planned route for additional editing: **Route level** > `<Shift> + <F10>`.

**Workflow**

**Change Sequential Number**
1.  Go to **Route Info** tab > open order level.
2.  Change to the **Shipping address** tab.
3.  In the **LS** field: Change the sequential number.
4.  Answer the query about whether the number should be assigned to the customer's other orders. The sequential number is inserted for all orders that belong to the same customer.

**Print new loading list**
1.  **Route Info** tab: `<Ctrl> + <F8>`.
2.  Specify the printer and number of copies to be printed.
3.  Start printing with `<Enter>`. The loading list is printed. The status is set to **Locked**.

**Print loading lists for all routes displayed**
4.  **Route Info** tab: `<Ctrl> + <F12>`.
5.  Check the site and time period and adjust if necessary.
6.  Confirm the entry with `<Enter>`.
7.  Specify the printer and number of copies to be printed.
8.  Start printing with `<Enter>`. The loading list is printed. The status is set to **Locked**.

**Print supplementary loading list**
1.  **Route Info** tab: `<Ctrl> + <F10>`.
2.  Repeat steps 5 to 8. Loading lists with the additions to the original loading list are printed.

---

### Cancel transaction (VS 03-006)

> [UI Screenshot: A series of cascading dialogs for cancellation. It starts with "Disp. note cancellation", leading to "Order cancellation", and finally a "Cancel. info." dialog to enter a reason for the cancellation.]

**Objective of this activity**
*   Cancel transaction:
    *   Order
    *   Delivery note
    *   Dispatch status

**Prerequisites**
*   The cancellation function is configured.
*   Routes are displayed on the **Route Info** tab.

**Additional information**
*   See also: View order info

**Workflow**
1.  Open menu `Logistics > Dispatch control` > desired level.
2.  Select a transaction, e.g., an order.
3.  Open the info menu with `<Shift> + <F4>`. The info menu opens.
4.  Select `Cancel`. The submenu opens.
5.  Select the type of cancellation, e.g., `Order cancellation`. The `Order cancellation` dialog opens.
6.  Check the data and confirm with `[Trigger]`.
7.  If necessary, confirm the query with `[Yes]`. A dialog for the reason opens.
8.  Specify the reason for cancellation and confirm with `<Enter>`. The transaction is canceled. The canceled identifier and the reason for cancellation are taken over into the transaction, e.g., into the delivery note or the order.

---

## Additional Functions

### Display route graphic (VS 04-001)

> [UI Screenshot: A series of dialogs and charts. First, two parameter selection dialogs. Then, two charts: "Quantities overview for route 2300" and "Quantities overview for deliv. date 24.05.2016", showing utilization as bar graphs.]

**Objective of this activity**
*   Display utilization of the routes for a delivery date.
*   Display utilization of a route on subsequent delivery days.

**Prerequisites**
*   Routes are displayed on the **Route Info** tab.

**Additional information**
*(None provided in the document for this section.)*

**Workflow**
1.  In the **Route Info** tab:
2.  Start the parameter selection with `<Shift> + <F11>`. The `1. parameter for the overview` dialog opens.
3.  Select parameter 1: `Quantity`, `QM`, or `weight`.
4.  Confirm with `<Enter>`. The `2. parameter for the overview` dialog opens.
5.  Select parameter: `Show all routes for the current delivery round`.
6.  Confirm with `<Enter>`. Actual and target quantities for the routes are displayed.

**Display utilization of a route:**
7.  Select parameter 1 and confirm with `<Enter>`. The `2. parameter for the overview` dialog opens.
8.  Select parameter: `Show next delivery days for the current route`.
9.  Confirm with `<Enter>`. The utilization of the route on subsequent days is displayed.

---

### View order info (VS 04-002)

> [UI Screenshot: A composite image showing several information windows. The main "Information on order" window lists order items. The "Information on document" dialog allows searching for an order. "Finished products stock booking log" and "Finished products stock overview" show detailed stock information.]

**Objective of this activity**
*   View information about the order.
*   View information about the finished products stock for the order.
*   View booking protocol for the finished products stock.

**Prerequisites**
*   Routes are displayed on the **Route Info** tab.
*   Finished products stock must be configured.

**Additional information**
*(None provided in the document for this section.)*

**Workflow**
1.  Go to **Route Info** tab > open order level.
2.  Select an order: `<Ctrl> + <K>`. The `Information on document` dialog opens.
3.  Enter the order number.
4.  Check mode: `SA Deliv`.
5.  Start the search with `[Trigger]`. The `Information on order` dialog opens.
6.  Exit order info: use `[Skip]` to return to the **Item info** tab.

**View orders in finished products stock:**
7.  Open information about the booking protocol of the finished products stock with `[FG stock]`. The `Finished products stock booking log` dialog opens.

**View bookings in finished products stock:**
8.  Open the overview for finished goods stock with `[Protocol]`. The `Finished products stock overview` dialog opens.
