---
title: "EN_AWBusiness_Production_1-4"
source: "EN_AWBusiness_Production_1-4.pdf"
tags: ["A+W Business", "Production Management", "Logistics", "Route Planning", "Status Reporting", "Interface Service", "Surplus Management", "ERP", "Manufacturing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A tutorial excerpt from the A+W Business Production manual, focusing on production reporting, logistics management, route planning, and status updates. It details how to handle surplus, configure the A+W Business Interface Service, plan and manage delivery routes, and report order status changes manually or via scanning."
long_description: "This document is a detailed tutorial section from the A+W Business Production software manual, version 5.20. It provides step-by-step instructions for key functions related to production reporting and logistics. The first part covers \"Reports from Production,\" explaining how to manage surplus from customer orders using file-less reports and how to configure the A+W Business Interface Service for data exchange with other programs. The second, more extensive part focuses on \"Logistics.\" It guides users through organizing deliveries and dispatch, covering modules like \"Route Planning,\" \"Status Report,\" and \"Picking.\" It details how to define, change, and lock delivery routes; plan shipments using the Route List dialog; change delivery dates; and print route lists. The \"Status Report\" section explains how to manage and update order statuses, both for entire orders and individual items, either manually through the user interface or by using a barcode scanner to simulate production floor feedback. The guide is intended for users responsible for production planning, dispatch, and logistics within the A+W Business environment."
---

# Reports from Production

---
## Surplus

File-less reports permit accepting surplus from A+W Production. This means that surplus from the production of a customer order can be adopted for the order, and can be invoiced. This applies to recurrent or standing customer orders, if the customer accepts possible surplus. The valid surplus must be defined in the master data.

⇨ Master Data, "Produktverwaltung - Fertigung" on page B-606
⇨ Master Data, "Übermengen" on page B-858

> **Surplus only in connection with file-less reports**
> Surplus cannot be accepted if you are using report files (STSP, STSL, STSD, STSB, STSG).

## File-less Reports and Capacity Planning

When working with file-less production reports, you have to consider the following:

- File-less reports can also be imported from A+W Production Capacity Planner. This is impossible, however, if you are using A+W Business Capacity Planning.
- Registration points in A+W Business have to be configured in coordination with A+W Production.

### Additional information

⇨ Master Data, "Erfassungsstellen Produktion" on page B-880
⇨ Master Data, "Firmendaten - Lager/EK/EDI" on page B-967
⇨ Master Data, "Firmendaten - Produktion" on page B-997
⇨ Master Data, "Schnittstellen-Dienst" on page B-1042
⇨ Sales, "Status Message Overview" on page C-574

## A+W Business Interface Service

### Objectives

- Introducing A+W Business Interface Service.
- Defining the settings for the service.

### Benefits

- A+W Business Interface Service serves to communicate with other programs.

### Please note:

| Term | Description |
| --- | --- |
| **A+W Business Interface Service** | A+W Business Interface Service is a Windows service. |
| **Default settings** | **Master data:**<br>- Interface service<br>**Company data:**<br>- Production tab |

## Define the Settings for A+W Business Interface Service

This chapter shows you how to define the parameters for the report files.

### How to define the settings for A+W Business Interface Service

1.  Go to menu **Master data > Company > Interface service** and proceed to the **Options** tab to enter the interval for importing reports.

    *(Image shows the 'Interface service - Options' window with fields for setting intervals for report checks and email dispatch settings.)*

    **Fig. E-29: Interface service - Options**
    - **A**: Interval for A+W Business Interface Service

2.  Determine the interval (A) for A+W Business Interface Service.
    If you enter 2, for example, the service will check whether there are new reports from Production every 2 minutes and, if so, imports them.

3.  Go to the menu **Start > Save** to save the data.
    The data is saved.

### Additional information

⇨ Master Data, "Schnittstellen-Dienst" on page B-1042

# Logistics

This set of topics shows you how to organize deliveries and dispatch in A+W Business.

This includes the following training modules:
- "Route Planning" on page E-80
- "Status Report" on page E-92
- "Picking" on page E-103

## Route Planning

### Objectives

- Compiling orders in a route
- Changing the delivery date or the route
- Assigning a route and a rank to a customer within the route

### Benefits

- Orders are combined by delivery date and route to make the shipments more effective.
- Route lists can be compiled by different criteria in order to optimize dispatch.

### Please note:

| Term | Description |
| --- | --- |
| **Route** | Routes are defined in the master data. They define the days on which deliveries shall be made to the individual areas. |
| **Route sequence** | The route hierarchy defines which customer should be the first on a certain route if there is a second customer on the same route. |
| **Route list dialog** | The Route list dialog serves to plan the shipments. Orders of a route can be compiled by various selection criteria, e.g. by delivery date, product, status. |
| **Changes** | In route planning, you can allocate an order to another route and to another date. Both are saved in the order. |
| **Default settings** | **Master data:**<br>- Terms of delivery<br>- Routes<br>- Truck<br>- Driver<br>**Customer, supplier**<br>- Delivery time<br>**Customer data:**<br>- Address > Route 1, 2 tab<br>- Order > Route hierarchy tab<br>**Company data:**<br>- Dispatch tab |

### Defined Routes

The weekdays for every single route are defined in the master data. A route from Manchester to Birmingham, for example, can be done every Monday and Thursday, for example. This route shall serve all customers along the road, within a radius of 30 miles.

Every customer is allocated a suitable route and rank. The rank defines the sequence in which the customers are served on the route.

> **Example**
>
> Customer A and customer B belong to the southern route. Customer A has rank 1 for this route while B's rank is 2.
>
> Customer A is therefore served before customer B.

The settings from the master data are adopted for the order. This setting can be changed by order. The system automatically checks whether the defined delivery date matches the route days defined for the customer. A message will be displayed in the event of differences. Different dates can be saved. They will be adopted for route planning.

### Define a New Route

You can change the defined routes or replace them with new routes. To calculate freight charges, for example, you have to enter the mileage rate per route. Calculation of freight charges will be introduced in a separate training session.

⇨ "Freight Costs" on page E-137

#### How to define a new route

1.  Select menu **Master data > Shipping > Routes**. The dialog of that name opens.
    ⇨ Master Data, "Touren" on page B-872

2.  Go to the menu **Start > New** to switch to the input mode.

    *(Image shows the 'Define dispatch route' dialog, a table of existing routes with columns for name, days of the week, shipping fee, and shift.)*

    **Fig. E-30: Define dispatch route**
    - **A**: Line for new route
    - **B**: Route days
    - **C**: Shipping fee
    - **D**: Shift during which route is driven

3.  Enter number and name (A). Both can be chosen at random.

4.  Tick check boxes for days (B) on which this new route is used regularly. At order entry, these details will be compared with the defined delivery date. The program will issue a message if date and route day do not match.

5.  Check whether a delivery fee (C) is to be charged.
    Tick the check box for pick-ups and carriers so that the delivery fee is not charged. When using A+W Business Capacity Planning you can define the shifts (D) during which the routes shall be executed, e.g. shift 2 on Monday and shift 1 from Tuesday to Friday.

6.  Move the view to the right (scroll) to enter the departure times, for example.

    *(Image shows the same route table, scrolled to the right to show columns for departure times and kilometer flat rate.)*

    **Fig. E-31: Define dispatch routes - departure times, kilometer flat rate**
    - **A**: Departure time per route day
    - **B**: Kilometer flat rate

    You can enter a departure time (A) for every single route day. The departure time is analyzed by A+W Production Capacity Planner after transfer to Production. If transfer to Production is made in OrderXML format, it is exported to Production. This is why, after an order has been imported, the production software will know the exact departure time of the route by which the order is going to be shipped.

7.  Enter the amount of the delivery flat rate (B) to be charged per kilometer.

8.  Go to the menu **Start > Save** to save the data. The data is saved.

9.  If necessary, repeat steps 2 to 8 for further routes.

### Lock Code

Once defined and allocated, a route cannot be deleted. You can, however, lock a route that should not be allocated any more. Locked routes will not be offered for selection. They will appear in the saved orders, however.

*(Image A shows a dropdown list of routes available for selection in a document. Image B shows the same dropdown list, but one of the routes, "Tour Training", is now missing because it has been locked.)*

**Fig. E-32: Selecting a route in the document**
- **A**: Select the route
- **B**: Locked route does not appear on the list

#### How to lock a route

1.  Select menu **Master data > Shipping > Routes**.
2.  Select the route and move the view by means of the scroll bar at the bottom until the column **Locked** is visible.
3.  Tick the required checkbox and save the amendment.
    The route is no longer offered for selection in document management.

> **Locking of master data**
> In the same way, delivery terms, trucks, drivers, customs routes, and packaging can be locked in the section Production/Dispatch.

## Route Planning (Task)

This session shows you how to compile and change route lists.

### How to plan a route

1.  Go to menu **Production > Shipping > Route list**.

    *(Image shows the 'Route list' compilation dialog with various selection criteria.)*

    **Fig. E-33: Route list - compile route**
    - **A**: Time limit (delivery date range)
    - **B**: Route selection list
    - **C**: Status restriction (from/to)
    - **D**: Number Manager selection
    - **E**: Breakdown level (Order, Item)
    - **F**: Status of the documents that shall not be printed
    - **G**: Target Number Manager

    ⇨ Software Reference, "Route List" on page E-205

    You can choose the following options for compilation:
    - Enter delivery date or period (A): In this case, the selection can also be restricted to a status and/or order area.
    - Choose Number Manager (D): In this case, selection can be restricted only to an order area.

    In both cases, you can also define the details for the breakdown level (E) and printing (F). In this case, a period (A) is entered.

2.  Enter the period within which the delivery date shall lie.
3.  From the list of available routes (B), choose the route the orders of which you want to view.
    If you have entered a period, all orders will be displayed per day and selected route. This means that the route list can easily become confusing if the period is too long and the routes too many. Therefore, a short period and only one route are selected in this example. Selecting all routes on a certain delivery date is also an option.
4.  Restrict the order status (C), e.g. from *Document entered* to *Delivery note printed*.
    You can exclude orders from printing that have a certain status (F). You do not need to press any key for multiple selection. This setting makes sense if you are compiling routes by delivery date. When you have made a selection, the corresponding orders are shown on the **Table** tab in blue letters.
    In this example, the orders are first copied to a new Number Manager (G), from where printing shall be started.
5.  Tick the checkbox **Fill NM completely** and enter the name of the Number Manager.
6.  Define the breakdown level (E) and - if required - the sorting within the routes.
7.  Determine (if necessary) where a new page shall begin at printing.
8.  To start the activity, go to the menu **Start > Execute**.
    The view automatically switches to the **Table** tab. If several routes were found based on the selection criteria, you can view every single route.
    In the next sessions you will learn about the detailed use of the route list.
    ⇨ "Change Route and Delivery Date" on page E-87
    ⇨ "Print Route List" on page E-89

## Change Route and Delivery Date

You can change the master data settings and the setting in the order and use these amendments to compile the dispatch data in an optimal way.

### How to change the route or delivery date

1.  Go to menu **Production > Shipping > Route list**.
2.  Display the routes you want to change.
3.  Go to the **Table** tab.
4.  If required, go to the field **Date/route** and select the date and route in order to display the orders that belong to this route.
5.  Double-click on the line header of the order you want to change.

    *(Image shows the 'Route List' table view with a list of orders for a specific route and date. One order line is marked with an 'x'.)*

    **Fig. E-34: Edit route**
    - **A**: Tick to change
    - **B**: Totals of the listed orders

    Only orders marked with an x (A) in the line header will be changed. You can tick several orders to be changed at once. You can select all orders by clicking on **[All]**.

6.  Go to menu **Functions > Route group > Change Shipping Data**.

    *(Image shows the 'Change routes/Delivery dates' dialog box, where a user can input a new route and/or delivery date for the selected orders.)*

    **Fig. E-35: Change shipping data**

7.  Mark at least one of the checkboxes:
    - **Delivery date** to change the date.
    - **Route** to allocate another route.
    - **Del. Terms** to change the delivery terms.
    - **Driver** to allocate another driver.
    - **Truck** to change the truck.

8.  Enter the new delivery data after each tagged checkbox. The changes apply to all orders shown in the dialog **Change delivery data**.

9.  Click on **[OK]** to save the data. The new delivery data will be adopted.

10. Click on **[End]** to close the dialog. The dialog **Route list** appears in the foreground. The amended routes are removed from the view.

## Print Route List

You can print the result of your work on a list to get an overview of the routes in a certain period.

> **Printing delivery notes based on the route list**
> To print the delivery notes in the sequence of the route list, copy the listed orders to another Number Manager.
>
> - Go to the menu **Functions> Copy to Number Manager** and enter the required Number Manager.
> - If you want to copy only the selected orders to a different number manager, go to the menu **Functions> Copy Selected to Number Manager** and enter the required Number Manager.
> - If you tick the checkbox **Delete**, the selected Number Manager will be emptied before it is filled again.

### How to print the route list

1.  Compile the route list as described in the instructions above.
    ⇨ "How to plan a route" on page E-85

2.  Pay attention to the setting in section **Change page in printout**:
    - **Route/date:** If you have selected several routes, every route will be printed on a new page by date.
    - **Route/date/customer:** If you have selected several routes, every route will be printed on a new page by date and customer.
    - **No change:** The routes will be printed consecutively, by date and customer.
    - **Route/Date/Customer/Delivery Address:** If you have selected several routes, every route will be printed on a new page by date and customer and delivery address.

3.  Go to the menu **Options> Group print options** and choose the settings for printing.
    If the entry **Surcharges and service items** is ticked (orange background), for instance, surcharges and services will be printed on the route list too.

4.  Go to the menu **Print > Screen** or **Printer**.
    The dialog **Print route list** opens.

5.  Check the current settings and change to horizontal format if lots of details are to be included in the printout.

6.  Click on **[OK]** to start printing.

---
*(Image shows an example printout of a 'Route List' detailing orders, quantities, weights, and other information for a specific route and date.)*

**Fig. E-36: Example: Route list for dispatch planning**

Depending on the breakdown level, the list shows, for every delivery date and route, at least:
- Customer
- Order number and partial delivery number
- Quantity, surface, and weight per item
- Totals per order

The supplier name only appears if this option has been selected.

> **Printing more lists**
> Loading and acknowledgement of receipt lists for the drivers can be issued via the dialog **Printing lists**. You should at least first allocate the vehicles and drivers when picking the orders.
>
> ⇨ "Print Lists" on page E-111

### Exercises

- Use the **Route list** dialog to compile different route lists and compare the results shown on the **Table** tab:
    - Create a Number Manager and collect different orders.
    - Compile a list based on this Number Manager.
    - Compile another list by collecting documents with a certain status.
    - Restrict the view to a certain delivery date.
- Go to the **Table** tab, change the delivery date for an order and watch the view. Check the selection criteria by which the order is now displayed.
- Check the print screen for every list and compare the results.

### Additional information

⇨ Master Data, "Tourrangfolge" on page B-802
⇨ Master Data, "Lieferdauer (Kunde, Lieferant)" on page B-831
⇨ Master Data, "Touren" on page B-872
⇨ Master Data, "Lkw" on page B-874
⇨ Master Data, "Fahrer” on page B-875
⇨ Master Data, "Firmendaten - Versand" on page B-1004
⇨ Software Reference, "Route List" on page E-205

## Status Report

### Objectives

- Checking the status allocations for transfer to Production and the completion reports.
- Introducing the rules for status changes.
- Changing the order status using a keyboard scanner.
- Changing the order status using the keyboard.

### Benefits

- Orders can only be processed if the order status permits this. The status is usually changed by reports from the production software.
- (Manual) status reports by scanner are used where (automatic) reports from shop floor data collection are not applicable.

### Please note:

| Term | Description |
| --- | --- |
| **Status** | The status can be allocated to an order item and to an order. It shows the point up to which an order has been processed so far, and the next possible actions. |
| **Status increase** | The status of an order is raised (changed) when all order items have the same, higher status, e.g. when all order items were reported complete. |
| **Automatic rise in status** | If you are using reports from production (barcoding), the status of an order item is changed when a new report file is available. |
| **Rise in status (by keyboard or scanner)** | The status change simulates the rise in status by way of reports. The status points that can be changed can be defined by registration point (user). |
| **Default settings** | **Master data:**<br>- Status allocation<br>**Production:**<br>- Status report > Settings |

### Order Status

Orders (documents) are allocated a specific status with every action. By allocating a minimum or lock status, you can define how an order shall be handled. This requires that the status points and status allocations have been properly defined in the master data.

## Check Status Management and Status Allocation

This session shows you how to check in the master data the status settings that are necessary for the transfer to Production and reports.

The following instructions exist for this training module:
- "How to check status management" on page E-93
- "How to check the status allocation" on page E-94

### How to check status management

1.  Select the menu **Master data > Order > Status management**.

    *(Image shows the 'Status Management' window, a list of defined statuses with their number and name.)*
    
    **Fig. E-37: Master data > Status management**

    ⇨ Master Data, "Statusverwaltung" on page B-895

2.  Check whether the user status exists for the following actions, for example, and define them if required:
    - Order released for production
    - Order transferred to Production
    - Order reported complete
    - Order ready for dispatch
    - Produced (AWBar)
    - Ready for dispatch (AWBar)
    - Shipped (AWBar)

3.  Go to the menu **Start > New** to switch to the input mode.
4.  Enter the number and name.
5.  Go to the menu **Start > Save** to save the data. The data is saved.
6.  Now check the status allocations.

### How to check the status allocation

1.  Select the menu **Master data > Order > Status allocation**.

    *(Image shows the 'Status Allocation' window, which links a 'Status point' (like 'AWBar produced') to a specific 'User status' for a given 'Document type'.)*

    **Fig. E-38: Master data > Order > Status allocation**

    ⇨ Master Data, "Statuszuordnung" on page B-897

2.  Check all status allocations for the document type **Order** which you want to report via scanner, e.g.:
    - AWBar produced
    - AWBar ready for dispatch
    - AWBar shipped

3.  Define the following allocations and correct the existing ones if necessary.

4.  Go to the menu **Start > Save** to save the data. The changes are saved.

## Manual Change of Status

If you do not use reports from shop floor data collection (barcoding) on the shop floor, you can scan orders using the dialog **Status report and rack allocation**. This can be used to simulate barcode reports.

Orders or order items are usually entered by means of a keyboard scanner. The status of an order can be changed for the following reasons, for instance:
- For the whole, finished order so that it can be packed and shipped.
- For individual order items so that partial delivery can be triggered if necessary.

After scanning, shipping papers can be printed, for example.

The access rights for changing the status can be set in different ways:
- The user can only allocate the preset status. This is done without further intervention at the time an order or an order item is scanned.
- The user can allocate more than one status. In this case, the status to be allocated must be scanned as well.
- You can also define whether the status can just be raised, or reset as well.

### Settings for Manual Status Reports

The options for status reports can only be set by a user who has administrator's rights. The valid status points can be defined per workstation.

#### How to define status points for status reports

1.  Go to the menu **Production > Dispatch > Status report**. The **Status report and rack allocation** dialog opens.
2.  Select the menu **Functions > Functions group > Settings**.

    *(Image shows the 'Options' dialog for status reports, allowing an administrator to select which status points are available for manual change at a workstation.)*

    **Fig. E-39: Status report options**

3.  Select the required entry in the field **Available status points**.
4.  Click on the arrow pointing to the right to move the status point to the field **Changeable status points**.
5.  Repeat these steps for all status points that can be changed.
6.  Tick the checkbox **Allow status reduction** if a status can also be reset.
7.  You can also define whether job number 9999 shall be entered automatically if there is no individual job number available. Checkbox **If no job no., enter 9999** is released when you select an entry in field **Changeable status points**.
8.  Click on **[OK]** to save the settings.
    Only status points listed in the field **Available status points** can be allocated at this workstation. At other workstations, you have to adapt the options.

## Manual Change of Status (Task)

To prepare an order for dispatch, for instance, you have to raise the status when all items have been produced.

> **Please obey the input sequence**
> First, enter all defaults that should be valid for this session. Start by scanning and proceed to the status before importing the order.

There are the following instructions for this session:
- "How to change the order status by scanning" on page E-97
- "How to change the status of an order item using the scanner" on page E-99
- "How to allocate the order items to a rack" on page E-100

### How to change the order status by scanning

1.  Go to the menu **Production > Dispatch > Status report**.

    *(Image shows the 'Status message - order' tab of the Status Report dialog. It includes an input field for an order/status point and a list to display successfully scanned orders.)*

    **Fig. E-40: Change status via barcode**
    - **A**: Appears if just one status is permitted.
    - **B**: Number Manager for orders reported complete
    - **C**: Release copy function for Number Manager.

    ⇨ Software Reference, "Status Message and Packaging Allocation" on page E-218

2.  The cursor is automatically on the field **Order/status point**. If you can allocate just one status, this is shown in the title line (A).
3.  If you can allocate more than one status, scan the status barcode first.
4.  If required, enter a new date for the end of production and/or the delivery in the section **Settings**.
5.  Tick the checkbox **Copy to NM (C)** if the changed orders should be copied to a Number Manager. The field **Target Number Manager** is now available, from which you can select the required Number Manager.
6.  Move the cursor to the field **Order/status point**.
7.  Scan the order number. The order number appears in the field **Order/status point** and the [Save] button is released.
8.  Select **Start > Save** in the menu to confirm order number. The order appears on the list. The status is changed. If you have entered a target Number Manager, the order has been copied there.
9.  Repeat steps 6 and 7 to scan the next order.
    To allocate the present order to a rack, go to the tab **Manual rack allocation**.
    ⇨ "How to allocate the order items to a rack" on page E-100

> **No scanner connected**
> If your scanner has failed, you can use the keyboard to change the status. Enter **s** and the code for the status, then **o** and the order number, e.g. **s68** and **o1234**.

### How to change the status of an order item using the scanner

1.  Go to the menu **Production > Dispatch > Status report** then proceed to the tab **Status report – item**. The cursor is automatically on the field **Order item/status point**. If you can only allocate one status, this is shown in the info area.
2.  If required, enter a new date for the end of production and/or the delivery in the section **Settings**.
3.  Scan the order item's barcode. The barcode appears in the field **Order item/status point** and the [Save] button is released.
4.  Go to the menu **Start > Save** to save the data.

    *(Image shows the 'Status message-item' tab. An item barcode has been scanned, and the view shows the details of the current order and the updated status of the scanned item.)*

    **Fig. E-41: Change item status via barcode**

    The order items are read. The status of the scanned item has changed.
5.  Repeat steps 3 and 4 to scan the next item. The order status is changed after all order items have reached the same status.

### How to allocate the order items to a rack

1.  Double-click an order number in the tab **Status report - Order** to change to the tab **Manual rack allocation**.

    *(Image shows the 'Manual rack allocation' tab, listing items from a specific order and providing fields to assign a rack number to each item.)*

    **Fig. E-42: Rack allocation**

    The items of the present order appear on the list.
2.  Go to the field **Rack** and choose the rack type.
3.  Select the position located on a rack.
4.  Move the cursor to the input field and scan the rack number. The cursor automatically moves to the next order item.
5.  Click `<Enter>` to adopt the allocation.
    Once all positions on a rack are allocated, the positions of the next order from the tab **Status report - Order** are shown automatically. To load the next rack, first scan the rack barcode. If you do not have a scanner, you can select the rack number using the button behind the input field.
6.  Go to the menu **Start > Save** to save the rack allocation.
    The data is saved. You can now move to the **Printing lists** dialog to print various lists for loading and for the driver.
    ⇨ "Printing Lists for the Driver" on page E-111
