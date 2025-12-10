---
description: "EN_AWBusiness_Production_3-1"
---


# Production Data – Booking

**Path:** `Production > Production > Production data > Booking tab`

*Fig. E-98 Production data – Booking*

This tab serves to book the data entered. The data are shown in brief per machine.

Only entries that show an x in the line header will be booked. Booking withdraws the raw material from stock while adding the produced items.

# Logistics

**Path:** `Production > Logistics`

You can plan and control the delivery of produced orders by compiling orders by route, date, rack, etc.

This chapter provides information on the following dialogs in this part of the program:
- "Route List" on page E-205
- "Status Message and Packaging Allocation" on page E-218
- "Consignment" on page E-228
- "List Printing" on page E-233
- "Shipping of Boxes" on page E-236

# Route List

**Path:** `Production > Logistics > Route list`

Route lists can be used to plan the shipping of goods. You can view and print the list based on different selection criteria, e.g. by delivery date, route, status.

This chapter provides information on the following subjects:
- "Menus in Route List Dialog" on page E-203
- "Route List" on page E-205
- "Change Route/Delivery Date" on page E-214
- "Settings (KAPS File)" on page E-215

---
## Menus in Route List Dialog

The menus in the **Route list** dialog serve to define the default setting for the dialog and open other dialogs without closing the route list.

This chapter provides information on the following subjects:
- "Functions Menu" on page E-203
- "Options Menu" on page E-204

### Functions Menu

**Path:** `Production > Logistics > Route list`

This menu can be used to open other dialogs without closing the route list.

**Class**
- **History:**
  Opens a list of processing steps and status changes for the selected document.
  ⇨ Sales, "History" on page C-550
- **Partial delivery**
  Opens the dialog Copy documents in Partial delivery mode, in which you can create a partial delivery.
  ⇨ Sales, "Copy documents" on page C-530
- **Change routes/delivery date:**
  Opens the dialog Change routes/delivery dates, where you can change the route and/or the delivery date.
  ⇨ "Change Route/Delivery Date" on page E-214
- **Copy all or selected to number manager:**
  Opens the dialog NM selection, in which you can move all orders to another number manager.
  ⇨ Sales, "NM Selection" on page C-553

**Navigation group**
- **Previous day/route, next day/route:**
  Changes the view of the list on the Table tab.

**KAPS group**
- **Create KAPS file:**
  Use this function to trigger the creation of the KAPS file. This may take some time if the selected number manager contains a large number of orders.
- **Path for file:**
  Opens a dialog to define the storage place.
  ⇨ "Settings (KAPS File)" on page E-215

**Miscellaneous group**
- **Settings:**
  This entry is only available for certain customers. It serves to define the maximum glass size for the route list.
- **Show document:**
  Opens a preview of the document.

### Options Menu

**Path:** `Production > Logistics > Route list`

This menu can be used to define the standard settings for printing. The options can be enabled or disabled. The settings will not be reset when you close the dialog.

**Table group**
- **Select several lines:**
  This option permits to select several lines from the table by keeping the `<Ctrl>` key pressed.

**Print options group**
- **Supplier name:**
  The supplier's name will be printed on the route list. This option is useful if the shipment includes P.O. items.
- **First item text:**
  Item text 1 from the order is printed on the route list.
- **Product name 1-3:**
  Product names 1-3 are printed on the route list.
- **Leaded designs:**
  Lites with leaded designs will be marked on the route list so that the staff in the shipping area can pack the lites accordingly.
- **Surcharge and service items:**
  Surcharges and services will be omitted from the printed route list.

> **Details not printed on the route list**
> If you have selected many options for printing the route list, you should choose the setting Horizontal in the printer dialog. Otherwise, not all of the selected columns may appear on screen or on the printout.

## Route List Dialog

**Path:** `Production > Logistics > Route list`

Route lists can be used to plan the shipping of goods. Orders of a route can be compiled by various selection criteria, e.g. by delivery date, product, status.

This dialog offers the following tabs:
- "Route List - Selection" on page E-206
- "Route List - Table" on page E-210

### Route List – Selection

**Path:** `Production > Logistics > Route list > Selection tab`

*Fig. E-99 Route list - Selection*

Use this tab to define the criteria by which the route shall be compiled.

**Criteria**
Select the option to define the criteria by which the routes are to be shown in the overview:
- **Dispatch:** The date specified is the dispatch day.
- **Delivery:** The date specified is the day of delivery to the customer.

**(Date) from ... to**
These fields are only available if you have not selected a number manager. You can compile routes within a desired space of time. If you have selected a number manager, these fields are inaccessible, and the present date is displayed.

**Route master data**
By selecting this option, you specify which routes should be displayed in the **Available Routes** field.
- **Master data:** All routes from A+W Business are displayed.
- **Route optimization:** All optimized routes from OTR are displayed.

**Available routes**
The list shows all routes defined in the master data. Routes that were adopted in the field **Routes to be displ./Sequence** no longer appear on the list.

**Routes to be displ. / sequence**
This list shows all routes for which route lists have been compiled. The sequence of the routes can be changed by means of the cursor keys below the field.

**From status, to status**
You can set a start and end status to select only the orders that match these criteria. These fields are inaccessible if you have selected a number manager.

**Number Manager**
You can compile the orders for route planning in a number manager in advance.
- Orders will not be loaded from a number manager.
- The route lists shall be compiled from orders from a number manager. The field for selecting the number manager is activated.

**Production preparations**
You can select one or more production preparations as an additional criterion. Keep pressing `<Ctrl>` to select several criteria.

**Breakdown level**
This option defines the way in which the list shall appear on screen and as a printout:
- **Order:** Only order numbers will be displayed and printed.
- **Item:** Order and item numbers will be displayed and printed.
If you have chosen and confirmed a delivery date, you can check the settings on the Table tab.

**Including processing**
Irrespective of the breakdown level, you can define whether processing steps should be shown.
- Processing steps do not appear.
- Processing steps appear on the route list marked by an X in the column Processing.

**Sorting within routes**
This option defines the sequence of the deliveries within the route.
- **Production preparation /Route priority/Cust.no.:** Deliveries are first sorted by production preparation. Within the production preparation, the route is sorted by the priority number defined in the customer master data.
- **Customer no./Status:** Deliveries are initially sorted by customer number, then by status. This option is useful if no priority numbers have been defined in the master data.
- **Route priority/Customer no.:** Deliveries are first sorted by sequence number, then by customer.
- **Customer no./Delivery address (Postcode, city, street):** Deliveries are initially sorted by customer number, then by delivery address.
- **Route optimization:** The deliveries are sorted by route optimization. This option is only activated if the **Route optimization** option is selected in the **Route master data** field.

**Page feed at printout**
This option defines how the list should be printed. Your choice also depends on the criteria by which the route list was compiled.
- **Route/date:** A new page will be started for every route and/or date.
- **Route/date/customer:** For every route, a new page will be started per date and customer.
- **No change:** The route list will be printed without a paging.
- **Route/date/delivery address:** For every route, a new page will be printed per date and customer and delivery address.

**Status excluded from printout**
You can exclude orders with a certain status from printing. You do not need to press any key for multiple selection. This setting makes sense if you compile routes by delivery date.
When you have made a selection, the corresponding orders are shown on the Table tab in blue letters.

**Options**

- **Print selected route/date:** You can restrict the printout to the currently displayed route.
  - All routes on the selected date or from the selected number manager will be printed.
  - Only the route selected on the Table tab will be printed.

- **Without direct delivery:** Orders which are delivered by the supplier directly can be omitted on the printout.
  - All order items of the selected route will be printed.
  - Order items with direct delivery will be excluded from printing.

- **Fill NM completely:** You can move the orders on the route list to a defined number manager.
  - No number manager will be filled.
  - The orders on the route lists are moved to a number manager. You can select a number manager or create a new number manager by entering a name. This option is useful for printing lists after picking.
    ⇨ "List Printing" on page E-233

- **Delete NM:** You can delete the orders of a route list from a number manager. This checkbox is only available if you have checked the checkbox **Fill NM completely**.
  - No orders will be deleted from the selected number manager.
  - All orders will be deleted from the selected number manager so that only new orders remain. This option is useful if you always want to use the same number manager.

### Route List – Table

**Path:** `Production > Logistics > Route list > Table tab`

*Fig. E-100 Route list - Table (breakdown level: order)*

This tab shows all orders matching the selection criteria defined on the **Selection** tab. You can display differently sorted route lists for printing.

When you have made a selection on the tab **Selection > Status to be excluded from printing**, the corresponding orders will be shown in blue letters.

On the breakdown level **Item**, the header is shown in red.

**Selection**

- **Route date:** This field allows you to select any route by date. The list only shows routes that match the selection criteria.
- **[<], [>]**: Use these buttons to scroll through the list of routes in the field **Route date**.

**Preview**
This field shows the dates and/or shipments that are part of the selected route. Choose one of the options to change the preview:
- **By delivery date:** The preview shows all routes on the selected date.
- **By route:** The preview shows all dates within the next fourteen days for the selected route. You can use the columns Quantity, surface, and weight to check whether a lorry is being used to capacity. If it is not being used to capacity, for example, you can search for another route on the list. The vehicles must be entered in the master data.
  ⇨ Master Data, "Lkw" on page B-874

**[All], [none]**
These buttons can be used to select or deselect all shipments on the list. You can change the route and/or the delivery date of the listed orders. First, select the orders. You can select individual entries on the list by double-clicking on the line header. You can select any number of entries.
⇨ "Change Route/Delivery Date" on page E-214

> **Select**
> An order has been selected if an x appears in the line header.

**[Resort table by...]**
Use this button to sort the marked deliveries in the overview by the option selected on the **Selection** tab.
⇨ "Route List – Selection" on page E-206

**Legend**
- **Blue:** Documents will not be printed.
- **Red:** All documents will be printed.

**Overview**
The list shows all orders for a route and for a delivery date. The list will be updated automatically when you select another route by means of the cursor keys or in the field **Route date**.
The columns will be filled depending on the breakdown level. The entries in blue letters will not appear on the printed list, e.g. because the corresponding status is excluded from printing.

- **Customer:** Name of the customer stated in the order.
- **Order:** Order number.
- **Quantity:** Total order quantity.
- **Item:** This column only appears if **Item** has been selected as a breakdown level. The following columns will be displayed by item.
- **Surface:** Total glass surface per order or item.
- **Weight:** Total weight per order or item.
- **Status:** Status of the order.
- **Shipping address:** Shows an alternative shipping address as stated in the order. Depending on the breakdown level, the product name is shown as well.
- **Consignment:** Consignment of the first order item.
- **Shp.:** Shape number (for items including shapes).
- **Rank:** Priority of routes as defined in the customer master data.
- **Input date:** Input date of the order.
- **SQM/item:** Total item surface area.
- **Weight/item:** Total item weight.
- **Proc.:** Processing. If you have chosen the breakdown on item level on the **Selection** tab, x marks items that include processing.
- **Production preparation:** Name of the production preparation which the order has been allocated to.
- **Processings:** Numbers of the product groups of the individual processing steps. The numbers are separated by semicolon (;).
- **Partial delivery:** Order number of the partial delivery.
- **Main order:** Number of the order from which the displayed order has been created as a partial delivery.
- **Document type:** The document type is only shown if it is different from an order, e.g. Complaint.
- **Total:** Total amount of the listed deliveries in Quantity, Surface, and Weight.

**Total**
Display of the sums of all orders appearing in the overview.

#### Example: Printed route list

*Fig. E-101 Route list as a soft copy*

| Deliv.date | Route | Customer | Order | Qty. | Area | Weight | Reference | Shape dis | Status |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 11.07.2013 | 2 Tour Nord/Rou | 1 Glasbau Müller- | 990008 20280 | 20 | 29.0 | 723.4 | | 2 | 955 |
| | | **Total** | | **20** | **29.0** | **723.4** | | | |
| 16.08.2013 | 7 Tour West/Rou | 1 Wolf Glasbau | 990009 20281 | 1300 | 2,808.0 | 94,770.0 | | 0 | 955 |
| | | Wolf Glasbau | 990010 20281 | 650 | 1,404.0 | 38,610.0 | | 0 | 400 |
| | | **Total** | | **1950** | **4,212.0** | **133,380.0**| | | |
| 30.08.2013 | 2 Tour Nord/Rou | 1 A+W Training | 990012 20282 | 1 | 2.2 | 43.2 | 1. Stock | 0 | 50 |
| | | **Total** | | **1** | **2.2** | **43.2** | | | |
| 17.10.2013 | 7 Tour West/Rou | 1 Wolf Glasbau | 990011 20281 | 250 | 540.0 | 21,600.0 | | 0 | 400 |
| | | **Total** | | **250** | **540.0** | **21,600.0** | | | |
| **Total** | | | | **2221** | **4,783.2** | **155,746.6**| | | |

## Change Route/Delivery Date

**Path:** `Production > Logistics > Route list > Functions menu > Route group > Change routes/delivery date`

*Fig. E-102 Change Route/Delivery Date*

On this dialog, you can change the route, the delivery date, the delivery conditions of orders, the driver, and/or the truck for the route. All orders are shown on the dialog that you have marked on the **Route List - Table** dialog.

**Selected orders**
The list shows all orders you have selected in the dialog **Route list – Table**.

**Change to**
Changes always apply to all displayed orders. Choose an option to define what shall be changed:

- **Delivery date:** You can enter another date from the list.
- **Route:** You can select a different route from the list.
  - The route is not changed.
  - The selected route will be adopted for the orders.
- **Del. terms:** You can select another delivery term from the list.
  - The delivery term is not changed.
  - The selected delivery term will be adopted for the orders.
- **Driver:** You can select another driver from the list.
  - The driver is not changed.
  - The selected driver will be adopted for the orders.
- **Truck:** You can select another truck from the list.
  - The truck is not changed.
  - The selected truck will be adopted for the orders.

## Settings (KAPS File)

**Path:** `Production > Logistics > Route list > Functions menu > KAPS group > Path for file`

*Fig. E-103 Settings for KAPS file*

This dialog serves to define the path and the file name for the KAPS file. This is a file for the KAPS Turbosoft interface. The output always refers to the current number manager.

**KAPS file**
- **Path:** Enter the path and the directory for saving the KAPS file.
- **File name ... +day+month+ser.no.:** Enter a code for the KAPS file. You can enter 2 characters. The file name is completed by the date and a serial number.
- **Suffix (without dot!):** Enter the file suffix for the KAPS file.

# Status Message

If you do not use reports from shop floor data collection, you can use the dialog **Status report and rack allocation** to scan orders and change the status.

You can use the keyboard scanner to allocate a new status to the order as well as the appropriate rack. You create the necessary barcodes yourself.
⇨ Tutorial, "Create a Template for Scanning" on page E-101

This chapter provides information on the following subjects:
- "Menus in Status Message Dialog" on page E-216
- "Status Message and Packaging Allocation" on page E-218
- "Select Rack" on page E-224

## Menus in Status Message Dialog

**Path:** `Production > Logistics > Status Message`

The menus can be used to define the default setting for the dialog, start functions and open other dialogs without closing the dialog.
- "Functions menu" on page E-216
- "Options menu" on page E-217

### Functions menu

**Path:** `Production > Logistics > Status Message`

This menu can be used to open other dialogs without closing document management. The following entries are displayed:

**Packaging group**
The entries are only available on the **Manual rack allocation** tab.
- **Add:** Allocates different packaging to a selected order.
- **Delete:** Deletes the allocation.

**Functions group**
- **Select all:** The entry is only available on the **Manual rack allocation** tab. You can use it to select all orders on the list.
- **Settings:** Opens the **Options** dialog to define the valid status reports.
  ⇨ "Status Message Options" on page E-223

### Options menu

**Path:** `Production > Logistics > Status Message`

This menu allows you to define the default settings for this dialog.

**Rack type group**
- **Enter rack type:** With this setting, the cursor is on the **Rack** field instead of the field for the rack number during rack allocation on the **Manual rack allocation** tab.
- **Show available racks:** The view is restricted to the racks that are available.

**Date group**
- **Set production date:** Releases the field **End of production date** to be able to enter the date manually during the session.
- **Set delivery date:** Releases the field **Delivery date** to be able to enter the date manually during the session.

**Production group**
- **Release order for production if sub-order produced:** Orders will be released for production when the corresponding internal order is reported complete.

## Status Message and Packaging Allocation

**Path:** `Production > Logistics > Status Message`

You can use a keyboard scanner to change the order status manually. The finished orders can be allocated to racks. These allocations can be printed on lists for shipping.
⇨ "List Printing" on page E-233

This dialog offers the following tabs:
- "Status Message – Order" on page E-218
- "Status Message – Item" on page E-220
- "Status Message – Manual Rack Allocation" on page E-222

### Status Message – Order

**Path:** `Production > Logistics > Status Message > Status Message tab – Order`

*Fig. E-104 Status message – Order*

You can change the order status on this tab to make the order ready for shipping.
⇨ Tutorial, "Manual Change of Status" on page E-95

> **Please obey the input sequence**
> First, enter all defaults that should be valid for this session. Start by scanning and proceed to the status before importing the order. Check the corresponding instructions in the Tutorial chapter.

**Allocation**
- **Order/Status:** Move the cursor to this field before scanning the order or the status. You can enter the order or the status manually. Enter an S (status) or an O (order) and add the status number or order number respectively. The status will be raised automatically when the order is scanned.

**Default**
- **End of production:** This field is only available if you have enabled the option **Set production date** in the Settings menu. Before scanning the order you can enter a new date on which production shall be completed. The new date will not be saved in the order.
- **Delivery date:** This field is only available if the option **Set delivery date** is enabled in the Settings menu. You can enter a new delivery date before scanning the order, e.g. because the production date has been postponed. The new date will be saved in the order.

**Target number manager**
- **(Target number manager):** Before scanning, you can select a number manager or enter a name to move the scanned orders to this number manager. This is useful if you want to print the shipping papers afterwards, for example. The field is activated if the checkbox **Copy to NM** is checked.
- **Copy to NM:** If the checkbox **Copy to NM** is checked, the field **Target number manager** is activated so that you can enter a number manager.
To fill the number manager defined in the field **Target Number Manager**, check the checkbox **Copy to NM**.
  - The scanned orders will not be copied to the number manager.
  - The scanned orders will be automatically copied to the selected number manager.

**Overview**
The order status changes upon scanning. All orders scanned during a session appear on the list.
- **Number:** Number of the scanned order.
- **Customer/supplier:** Customer number.
- **Name:** Customer name.
- **Status:** New order status.
- **Input date:** Date on which the order was entered.
- **OC date:** Issue date of order confirmation.
- **Delivery date:** Delivery date stated in the order or amended date acc. to the field Delivery date.
- **No. of items:** Number of order items.

### Status Message – Item

**Path:** `Production > Logistics > Status Message > Status Message tab – Item`

*Fig. E-105 Status message – Item*

You can use this tab to change the status of individual order items. The order status is only changed if all order items have the same status. Individual items cannot be allocated to racks.

The fields in sections **Allocation**, **Default** and **Target number manager** are described in detail in connection with the tab **Status message – Order** tab.
⇨ "Status Message - Order" on page E-218

**Item overview**
- **Current order:** This field shows the order number for which the items are listed.
The list shows all items of the current order:
  - **Item:** Order item number.
  - **Status:** Status of the order item. It can differ from the status of the items.
  - **Qty:** Item quantity.
  - **Width, Height:** Dimensions of the item.
  - **Description:** Name of the glass.

### Status Message – Manual Rack Allocation

**Path:** `Production > Logistics > Status Message > Manual Rack Allocation tab`

*Fig. E-106 Status message - Manual rack allocation*

This tab can be used to allocate racks (and their rack numbers) to the order items. Racks can be allocated by scanner or manually.

**Allocation**
- **Packaging:** This combo box offers all packaging types defined in the system. This can be rack types, boxes, containers, etc.
- **[Directory]:** Use this button to open the **Select rack** dialog to search for a free rack number of the selected rack type.
  ⇨ "Select Rack" on page E-224

## Status Message Options

**Path:** `Production > Logistics > Status Message > Functions menu > Functions group > Settings`

*Fig. E-107 Status report options*

This dialog serves to define the status points that can be changed. The settings can be defined so that they only apply to the currently logged-in user.

> **Administrator rights required**
> The options in the Status report dialog can only be changed by the system administrator.

- **Available status points:** The list shows all status points defined in the master data.
- **Changeable status points:** The list shows all status points that can be selected as a new status.
- **Permit status reduction:** By default, the status is incremented with the status report. In some cases, however, it may be necessary to reset the status, e.g. if an order was accidentally booked as finished.
  - The status of an order or of an item cannot be reduced. If you need to correct an error, the status of the individual order can be reduced in document management.
    ⇨ Sales, "Functions menu" on page C-398
  - The status can be reset. The **Notification when lock status is achieved** checkbox is activated.
- **Notification when locked status is achieved:** You can specify whether a message is output in case of a status reduction. This checkbox is only released if the **Status reduction permitted** checkbox is activated.
  - No message is output.
  - If in case of a status reduction, the lock status is higher than the order status, a message is output. You can then decide whether you want to change the status.
- **No seq. no., then enter 9999:** By default, a sequential number is assigned by the system when a production batch is created. With this option, you specify whether batches without batch number are assigned a batch number. This checkbox is only activated if an entry in the **Changeable status points** field is marked.
  - No batch number is assigned to the batch.
  - The sequential number 9999 is assigned if there is no individual batch number.

## Select Rack

**Path:** `Production > Logistics > Status Message > Manual Rack Allocation tab > [Directory]`

*Fig. E-108 Manual rack allocation - Select rack*

If you do not use a keyboard scanner, you can select a free rack from this dialog and allocate it to the present order.

**Filter**
- **Rack type:** The combo box offers all the rack types defined in the master data for selection.
- **Rack no. from, to:** You can restrict the display of racks to a sequence of rack numbers.
The rack numbers are defined in the **Racks management** dialog.
⇨ "Racks" on page E-239
- **Unavailable racks:** If racks are reported off site, they cannot be allocated again. You can omit these rack numbers from the view.
  - Only racks that can be used for the present order will be displayed.
  - All racks will be displayed.

**Overview**
The list shows all racks matching the search criteria.
- **Rack number:** The rack number entered in the master data.
- **Description:** The name entered in the master data.
- **Rack type:** If the search has not been limited to a certain rack type, the display of the rack type serves for further distinction of the racks.
- **Off site:** Shows whether the rack is being used at present.
- **Shipping date:** The shipping date is only displayed if the rack number is allocated to an order. If the rack has been booked as free again, this field will be empty.
