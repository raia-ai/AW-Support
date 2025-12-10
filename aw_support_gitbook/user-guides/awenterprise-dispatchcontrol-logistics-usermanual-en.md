---
description: "EN-UM-AWEnterprise_20"
---


# Dispatch Explorer

---
## Dispatch Explorer
**Logistics > Dispatch Control > Defining a Period**

*Fig. G-16 Dispatch control – Explorer view*

- **A** Header data: Entry of search criteria
- **B** Explorer - Tree structure
- **C** Detailed information about the selected delivery date
- **D** Detailed information about the selected route
- **E** Selected date level

Dispatch control lists the orders found - based on the search criteria - by delivery date.

- **SA Deliv.**: SA Deliv.: selected dispatch mode.
  - **Technical info**: Toggle field, DB field: `lapool.vmodus`
- **Site**: Site number or client number.
  - **Technical info**: numeric field, DB field: `lapool.hausnr`
- **Deliv. date**: Input field for the delivery date on a certain day.
  - **Technical info**: date field, DB field: `lapool.ltplan`
- **to number**: Input field for the delivery date in a certain period.
  - **Technical info**: date field, DB field: `lapool.ltplan`

## Explorer – Tree structure

For clarity's sake, orders are listed in the Explorer structure. Work with the Dispatch Explorer must be configured appropriately. The dispatch data is displayed on several levels in the Explorer:

- Date level
- Route level
- Document level
- Item Level

Each level is marked by a certain icon. A brief overview of the existing deliveries is displayed in the right half of the dialog.

Select a level from the tree structure. When a level has been selected, the level field is highlighted in blue.

The following four levels provide short bits of information:
- "Overview of the delivery date level" on page G-1903
- "Overview for the tour level" on page G-1905
- "Overview of the order level" on page G-1906
- "Overview of the item level" on page G-1907

## Overview of the delivery date level
**Logistics > Dispatch Control > Enter a period or date in the Explorer**

*Fig. G-17 Date level in the Dispatch Explorer*

After the delivery date selection in the Explorer, the following fields are displayed in the overview:

- **Route**: Route number.
  - **Technical info**: numeric field, DB field: `lapool.routenr`
- **Site**: Site number or client number.
  - **Technical info**: numeric field, DB field: `lapool.hausnr`
- **Type**: Dispatch mode. Due to the limited space, the name of the field (Dispatch mode=type) and the display of the dispatch mode are abbreviated:
  - SA: SA withdrawal
  - E1: PU receipt of goods
  - E2: PU issue of goods
  - **Technical info**: alphanumeric field, DB field: `lapool.vmodus`
- **Name**: Route description from the A+W Enterprise master data.
  - **Technical info**: Display field, DB field: `route.routenname`
- **Tot.**: Total number of items entered for this route.
  - **Technical info**: numeric field, DB field: `lapool.gesstk`
- **Call**: Number of items the customer has ordered for that date.
  - **Technical info**: numeric field, DB field: `lapool.abrufstk`
- **Avail**: Available quantity for this item.
  - **Technical info**: numeric field, DB field: `lapool.sollstk`
- **Pack**: Quantity packed for this item.
  - **Technical info**: numeric field, DB field: `lapool.iststk`
- **Cmp**: Route reported completed. All orders have been packed.
  - All items are ready for shipment.
  - Not all of the items are ready to be shipped.
  - **Technical info**: display field

## Overview for the tour level
**Logistics > Dispatch Control > Enter a period or date in the Explorer**

*Fig. G-18 Tour level in the Dispatch Explorer*

After the route selection in the Explorer, the following fields are displayed in the overview:

- **Order/PO**: Order or PO number for the scheduled delivery depending on dispatch mode. There is always a distinction according to the document type: 5=order, 2=PO.
  - **Technical info**: Numeric field, DB field: `lapool.auftrnr`, `lapool.vorgang`
- **Customer**: Customer name for orders or supplier name for POs for the scheduled delivery.
  - **Technical info**: Alphanumeric field, DB field: `mp.name`

The following fields are adopted from the previous overview:
- Tot. (total)
- Call
- Avail. (available)
- Pack. (packed)
- Cmp (completed)

## Overview of the order level
**Logistics > Dispatch Control > Enter a period or date in the Explorer**

*Fig. G-19 Order level in the Dispatch Explorer*

After the order/PO selection in the Explorer, the following fields are displayed in the overview:

- **Item**: Sequential item number from the order or PO.
  - **Technical info**: Numeric field, DB field: `lapool.posnr`
- **Article**: Name of the article to be delivered.
  - **Technical info**: numeric field, DB field: `artikel.artbez1`

The following fields are adopted from the previous overview:
- Tot. (total)
- Call
- Avail. (available)
- Pack. (packed)
- Cmp (completed)

## Overview of the item level
**Logistics > Dispatch Control > Enter a period or date in the Explorer**

*Fig. G-20 Item level in the Dispatch Explorer*

The overview from the item level lists all order items or items from the purchasing document with the respective fields, as on the order level.

The fields are described in the following section:
- "Overview of the delivery date level" on page G-1903
- "Overview of the order level" on page G-1906

# Dispatch Control – Menus

In the Dispatch Control, there are additional functions available. These are summarized on all available levels under supplementary and info menus. A detailed overview of both menus is provided in the following sections.
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## Supplementary menu
**Dispatch Control – overview levels > <F4>**

*Fig. G-21 Supplementary menu on tour level*

On all levels of the Dispatch Control, you have additional functions that can be accessed via the supplementary menu `<F4>`. Depending on the configuration, context, and data stock, the functions listed here may not be available or only available to a limited extent.

- "Supplementary menu on tour level" on page G-1909
- "Supplementary menu on order level" on page G-1910
- "Supplementary menu on item level" on page G-1910

### Supplementary menu on tour level

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Postpone `<F3>` | "Move” on page G-1950 |
| b | Go to `<F5>` | "Go to” on page G-1948 |
| c | Postpone several items `<Ctrl>` + `<E>` | “Postponement of several items - selection" on page G-1952 |
| d | Order info `<Ctrl>` + `<K>` | "Order info" on page G-1954 |
| e | Print a cargo list `<Ctrl>` + `<F8>` | "Print loading list" on page G-2014 |
| f | Print all cargo lists `<Ctrl>` + `<F12>` | "Print all loading lists" on page G-2015 |
| g | Printing a supplementary cargo list `<Ctrl>` + `<F10>` | "Print supplementary loading lists" on page G-2016 |
| h | List printing | "List printing" on page G-2017 |
| i | Book goods receipt for | "Book goods receipt for" on page G-1957 |
| j | Cancel receipt of goods | "Cancel receipt of goods" on page G-1958 |
| k | Missing quantity check `<Shift>` + `<F9>` | "Missing quantity check for" on page G-1959 |
| l | Preliminary delivery note printing `<Ctrl>` + `<F11>` | "Print loading list" on page G-2014 |
| m | Book to transport | "Book to transport" on page G-1963 |
| n | Cancel transport booking | "Cancel transport booking" on page G-1964 |
| o | Deliv./Receipt of goods. Release + print `<Ctrl>` + `<F9>` | "Deliv./Receipt of goods Release + print" on page G-2020 |

### Supplementary menu on order level

In addition to some functions that are also available on the tour level, the following menu entries are available on the order level:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| i | Rack View for Order | "Rack view for order" on page G-1965 |
| j | Results of the rack scheduling `<Shift>` + `<F12>` | "Results of the rack scheduling" on page G-1966 |
| k | Rack planning | "Rack planning" on page G-1967 |
| o a | Find delivery address | "Find delivery address" on page G-1968 |
| o b | New delivery address | "New delivery address" on page G-1969 |
| t | Rack information | "Rack information" on page G-1970 |

### Supplementary menu on item level

In addition to some functions that are also available on the route and order level, the following menu entries are available on the item level:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| j | Correct Packed Quantity `<Shift>` + `<F10>` | You can use `<F4>` > Correct packed quantity to change the entry in the displayed field. |
| m | Overview | "Dispatch control – overview" on page G-2000 |
| n | Change Delivery Date | "Delivery date changes" on page G-2003 |

## Info menu
**Dispatch Control – Overview Levels > `<Shift>` + `<F4>`**

*Fig. G-22 Info menu on order level*

The info menu `<Shift>` + `<F4>` is the same for all levels. You can use this menu to open other dialogs and start functions. The following entries are displayed:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Lock/Unlock Tour `<Shift>` + `<F10>` | "Set/remove tour lock" on page G-1971 |
| b | Lock all Tours `<Shift>` + `<F12>` | "Lock all tours" on page G-1972 |
| c | Transport data | "Transport data" on page G-1973 |
| d | Stock Reference | "Stock reference" on page G-1974 |
| e | Cancel | Open the submenu "Cancel" on page G-1975 |
| e a | Cancel delivery note | "Cancel delivery note" on page G-1975 |
| e b | Order cancellation | "Order cancellation" on page G-1976 |
| e c | Cancel receipt of goods | "Cancel receipt of goods" on page G-1977 |
| e d | Cancel shipping status | "Cancel shipping status" on page G-1978 |
| f | Racks | Open the submenu "Racks" on page G-1979 |
| f a | Rack Allocation `<Ctrl>` + `<G>` | "Rack allocation - selection" on page G-1980 |
| f b | Resolve Rack `<Ctrl>`+ `<F>` | "Resolve rack - selection" on page G-1982 |
| f c | Free Racks (Overview) `<Ctrl>` + `<L>` | "Free racks (overview)" on page G-1985 |
| f d | Booked Racks (Overview) `<Alt>` + `<E>` | "Booked racks (overview)" on page G-1987 |
| f e | All Racks (Overview) `<Alt>` + `<G>` | "All racks (overview)" on page G-1988 |
| f f | Individual Racks `<Alt>` + `<B>` | "Individual racks" on page G-1990 |
| f g | Racks for Order `<Alt>` + `<A>` | "Resolve rack - selection" on page G-1982 |
| f h | Lite Allocation `<Alt>` + `<F>` | "Lite allocation" on page G-1993 |
| g | SA/PU Information `<Ctrl>` + `<O>` | "SA/PU information" on page G-1996 |
| h | SA/PU info (global) | "SA/PU info (global)" on page G-1998 |
| i | Overview | "Dispatch control - overview" on page G-2000 |
| j | Delivery date changes | "Delivery date changes" on page G-2003 |
| k | Dispatch Information `<Alt>` + `<l>` | "Shipment information" on page G-2004 |
| l | Via Details | "Via details" on page G-2005 |
| m | Finished goods stock | "Finished goods stock" on page G-2006 |
| m a | Finished goods stock | "Finished goods stock" on page G-2007 |
| m b | Finished goods stock - inventory | "Finished goods stock - inventory" on page G-2009 |
| m c | Finalize inventory | "Finalize inventory" on page G-2009 |
| d | Log | "Log" on page G-2010 |

## Buttons
On the data levels of the Dispatch Control, you can use the following buttons:

*Tab. G-1 Overview of the buttons in the Dispatch Control*

| Button | Entry | Description |
| :--- | :--- | :--- |
| [Search] | Starts the document search | "Search" on page G-1947 |
| [Overview] | Graphic overview of the deliveries | "Graphical tour overview" on page G-2012 |
| [Go to] | Go to a particular document | "Go to" on page G-1948 |
| [Sort] | Starts the Postpone dialog | "Move” on page G-1950 |
| [Trigger] | Triggers the selected action | With this button, or alternatively with the `<F3>` button, you can start the selected action. |
| [Details] | Starts the route overview | "RouteInfo tab" on page G-1915 |
| [Routes] | Changes from the lower levels to the tour level | "RouteInfo tab" on page G-1915 |
| [Orders] | Changes from the lower or higher levels to the order level | "Order Info tab" on page G-1925 |
| [Items] | Changes from the higher levels to the item level | "Item Info I tab" on page G-1941 |
| [Explorer] | Changes from the data levels in the Explorer | "Dispatch Explorer" on page G-1901 |
| [Close] | Ends the overview display | It is possible to enter another date. The next [End] closes the Dispatch Control. |

# Tours

On the tour level, all routes are listed that are driven on the selected delivery date. The orders or POs with additional details and tour status are listed for each route.

The search fields in the header are explained in the following section:
- "Dispatch Explorer" on page G-1901

> **Technical info in dispatch**
> Some important data is stored in the database table `lapool`. This data exists per order or PO item, route and delivery date. Various displays on the dialogs are formed dynamically or calculated at program runtime. Therefore, the details about the technical information are generally not possible 1:1. In such cases, the Technical Info entry is omitted in this document. The field contents that are determined program-internally (via SQL statement) are not listed in this document. If necessary, please consult the database documentation.

The tour level consists of the following tabs:
- "RouteInfo tab" on page G-1915
- "RackInfo tab" on page G-1918
- "VehicleInfo tab" on page G-1920
- "Optimization tab" on page G-1922

## RouteInfo tab
**Dispatch Control – delivery date entry**
**Dispatch control – Delivery date level > [Details] > RouteInfo tab**

*Fig. G-23 Dispatch Control – RouteInfo tab*

On the RouteInfo tab, general data about the routes is summarized.

**C Current route status**. For the meaning of the individual icons, please consult the following table.
**Technical info**: display field

| S (Status) | Meaning | Information |
| :--- | :--- | :--- |
| white | Open | Not all of the items for this route have been completely packed. |
| green/yellow | Available | Items with available quantity are present for this route. |
| Yellow | Packed | All of the items for this route have been completely packed. |
| blue/yellow | En route | All items scheduled for this route are on their way. |
| blue | Delivery note created | All items of this route have been completely delivery to the customer. |
| red | Locked | This route has been locked. The route lock is set only if one order of the route is booked by another site or client as being en route. See "Set/remove tour lock" on page G-1971. |

*Tab. G-2 Route status*

- **No.**: Route number.
  - **Technical info**: numeric field, DB field: `lapooltou.routenr`
- **Route**: Route description from the A+W Enterprise master data.
  - **Technical info**: Display field, DB field: `route.routenname`
- **Tot.**: Total number of items entered for this route.
  - **Technical info**: display field, DB field: `lapooltou.gesstk`
- **Call**: Number of items the customer has ordered for that date.
  - **Technical info**: display field, DB field: `lapooltou.abrufstk`
- **Pack**: Quantity packed for this item. Use `<F4>` to check for missing quantities.
  - **Technical info**: display field, DB field: `lapooltou.iststk`
  The packed quantity can be changed on the following dialogs:
  - "Missing quantity check for" on page G-1959
  - "Rack view for order" on page G-1965
- **Back.**: Backlog. Item quantity that is not available for the desired tour. If a tour is moved because of Backlog, this quantity will be adopted.
  - **Technical info**: display field, DB field: `lapooltou.rueckstk`
  - "Functions in Dispatch" on page G-1946
- **kg/N**: Net weight in kilogram for this route. The net weight is the total weight of the item, without rack or packaging. The weight is calculated in the program at runtime and displayed rounded on this tab.
  - **Technical info**: Display field, DB field: `lapooltou.gewicht`
- **sqft**: Item surface in square feet.
  - **Technical info**: display field, DB field: `lapooltou.qm`
- **LL**: Number of the loading list if a loading list has been printed for this route. Use `<F4>` to print the loading lists.
  - **Technical info**: display field, DB field: `lapooltou.llnr`
  - "Print loading list" on page G-2014
  - "Print all loading lists" on page G-2015
- **Cmp**: Complete code:
  - All items are packed for delivery.
  - Not all of the items are packed for delivery.
  - **Technical info**: Display field, DB field: `lapooltou.liefkompl`
- **PL**: The preliminary delivery note shows whether all preliminary delivery notes have been printed for this tour.
  - All preliminary delivery notes have been printed.
  - Not all of the preliminary delivery notes have been printed.
  - Use `<F4>` to print a preliminary delivery note.
  - **Technical info**: Display field, DB field: `lapooltou.vlsdrukz`
  - "Print loading list" on page G-2014
- **DN**: The delivery note code indicates whether all delivery notes for the deliveries on this tour are printed.
  - At least one delivery note has been printed.
  - No delivery notes have been printed.
  - Press `<F4>` to print the delivery note.
  - **Technical info**: display field, DB field: `lapooltou.lsdrukz`
  - "Rack information" on page G-1970
- **I**: Dispatch information code indicates whether there is dispatch information for at least one order on this tour.
  - There is at least one order with dispatch info.
  - No dispatch info is available.
  - The dispatch information can be stored in the documents during entry.
  - **Technical info**: Display field, DB field: `lapooltou.vlsdrukz`
  - Sales, "External information" on page D-1316
- **TL**: The tour lock code indicates whether the current tour is locked or booked:
  - gray - The current tour is still en route
  - yellow - The current tour is booked
  - red - The current tour is locked
  - You can use `<F4>` to lock or book the tour.
  - **Technical info**: display field
  - "Rack information" on page G-1970
  - "Lock all tours" on page G-1972

**Additional information**
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## RackInfo tab
**Dispatch Control – delivery date entry**
**Dispatch control – Delivery date level > [Details] > RackInfo tab**

*Fig. G-24 Dispatch Control – tour level - RackInfo tab*

On the RackInfo tab, general data about the routes is summarized and additional rack information is displayed. The display of this tab is dynamic; that is, it is only shown if the work with racks is configured in Dispatch Control.

Most fields have already been described in the previous section:
- "RouteInfo tab" on page G-1915

In addition, the following fields are displayed on the Rack information tab:

- **on rack**: Rack number on which the lites to be delivered are located. For the configuration of the free racks in the Dispatch Control, you must contact an A+W employee.
  - **Technical info**: Display field, DB field: `lapooltou.freigeststk`
- **kg/N**: Net weight in kilogram for this route. The weight is calculated in the program at runtime and displayed to three decimal places on this tab.
  - **Technical info**: Display field, DB field: `lapooltou.gewicht`
- **kg/Tara**: Empty weight of the rack (tarage weight), in kilograms. The tarage weight is displayed in this field if it is stored appropriately in the master data and the goods delivered are already scheduled on the racks.
  - **Technical info**: Display field, DB field: `lapooltou.gewichttara`
- **kg/G**: Gross weight in kilograms for this route. The weight is calculated in the program at runtime and displayed to three decimal places on this tab. The gross weight is calculated from the net weight and tarage weight together. The gross weight is displayed in this field if the goods delivered are already scheduled on the racks.
  - **Technical info**: Display field, DB field: `lapooltou.gewichtbrutto`

**Additional information**
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## VehicleInfo tab
**Dispatch Control – delivery date entry**
**Dispatch Control – Delivery Date Level > [Details] > VehicleInfo tab**

*Fig. G-25 Dispatch control – VehicleInfo tab*

The VehicleInfo tab shows the drivers and vehicle data in addition to the tours.
Most fields have already been described in the previous section:
- "RouteInfo tab" on page G-1915

In addition, the following fields are displayed on the VehicleInfo tab:

- **Driver**: Personnel number of the driver from the employee master data. The driver for this route can be selected on the TransportData dialog.
  - **Technical info**: Numeric field, DB field: `mitarb.manr`
  - "Transport data" on page G-1973
- **Name**: Driver's name. If the driver for this route is selected on the Transport-Data dialog, the name is taken over here directly from the employee master data.
  - **Technical info**: Display field, `mitarb.maname`
- **Vehicle**: License plate of the truck. The vehicle for this route is selected on the TransportData dialog. The vehicles must first be stored in the master data.
  - **Technical info**: Numeric field, DB field: `lkw.lkw.nr`
  - Master Data, "Vehicles" on page B-265
- **Trailer I/II**: License plate of the trailer used. It is possible to select two trailers on the TransportData dialog. The trailer must first be stored in the master data.
  - **Technical info**: Numeric field, DB field: `lkw.lkw.nr`
  - Master Data, "Vehicles" on page B-265

**Additional information**
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## Optimization tab
**Dispatch Control – delivery date entry**
**Dispatch control – Delivery date level > [Details] > Optimization tab**

*Fig. G-26 Dispatch Control – tour level – Optimization tab*

General data about the routes is summarized and additional information about the route optimization is displayed on the Optimization tab. The display of this tab is dynamic; that is, it is only shown if work with the A+W Logistics Optimizer is configured in Dispatch Control.

Most fields have already been described in the previous sections:
- "RouteInfo tab" on page G-1915
- "RackInfo tab" on page G-1918
- "VehicleInfo tab" on page G-1920

In addition, the following fields are displayed on the Rack Information tab:

- **Opti status**: Current status of the route optimization in plain text.
  - **Technical info**: Display field, DB field: `lapooltou.optistatus`
- **Opt.**: Checkbox for route selection for the upcoming optimization.
  - Current route is selected for the optimization.
  - The current route is not selected for the optimization.
- Start the route optimization with the [StartOTR] button.
  - **Technical info**: Display field, DB field: `lapooltou.optkz`

> **Route optimization in A+W Enterprise**
> Route optimization with the A+W Logistics Optimizer is a separately available and configurable extension for A+W Enterprise. Please contact the responsible A+W employee for more information.
> The documentation for the A+W Logistics Optimizer is not part of this document.

**Additional information**
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

# Order Level

On the order level, Dispatch Control provides detailed information on the entered orders such as delivery address, dispatch information, and additional information.

This level offers the following tabs:
- "Order Info tab" on page G-1925
- "OrderInfo/Rack tab" on page G-1929
- "Delivery Address tab" on page G-1931
- "Dispatch Info I tab" on page G-1933
- "Dispatch Info II tab" on page G-1935
- "Add. Info tab" on page G-1937

## Order Info tab
**Dispatch control – delivery date selection > Route selection > Order info tab**

*Fig. G-27 Dispatch control – Order info tab*

The Order info tab shows information about the orders and the dispatch status for every tour.
The search fields in the header are explained in connection with Dispatch control. Tour number and name are shown as well.
- "Dispatch Explorer" on page G-1901

- **C Current order status**: The meaning of the traffic light display on the order level is the same as on the tour level. Here's an explanation:
  - "Route status" on page G-1915
- **Mode**: Dispatch mode. The field is only displayed if you are using the Dispatch Control for the purchasing documents and have made the appropriate selection.
  - **Technical info**: Display field, DB field: `lapoolauf.vmodus`
- **Order/PO**: Order or PO number. All documents are listed here that are scheduled for the route on the selected date. Whether an order or PO number is displayed in this field depends on the dispatch mode selected.
  - **Technical info**: Numeric field, DB field: `lapoolauf.auftrnr`
- **No.**: Delivery note sub-number. If a complete delivery note or several partial delivery notes were already entered, the appropriate number is displayed here.
  - A complete delivery note always has the sub-number 1 and is also marked as complete (Cmp checkbox).
  - Partial delivery notes always have sub-numbers larger than 1 and are not marked as complete (Cmp checkbox).
- If an order is transferred from another site, this field shows the original order number assigned by the sender.
  - **Technical info**: numeric field, DB field: `lapoolauf.subnr`
- **Customer**: Customer or supplier name from the order or the PO.
  - **Technical info**: Alphanumeric field, DB field: `mp.name`
- **Tot.**: Total number of pieces in the order or in the PO.
  - **Technical info**: Numeric field, DB field: `lapoolauf.gesstk`
- **Call**: Number of items the customer or supplier has requested for that date.
  - **Technical info**: Numeric field, DB field: `lapoolauf.abrufstk`
- **Avail**: Number of items available for packing.
  - **Technical info**: numeric field, DB field: `lapoolauf.sollstk`
- **Pack**: Quantity packed for this item. Use `<F4>` to check for missing quantities.
  - **Technical info**: numeric field, DB field: `lapoolauf.iststk`
  - "Missing quantity check for" on page G-1959
- **Back.**: Backlog. Item quantity that is not available for the desired tour. If a tour is moved because of Backlog, this quantity will be adopted.
  - **Technical info**: numeric field, DB field: `lapoolauf.rueckstk`
  - "Functions in Dispatch" on page G-1946
- **Add.**: To be delivered later. Quantity to be shipped later. Those additional shipments may be due to postponements.
  - **Technical info**: display field
  - "Functions in Dispatch" on page G-1946
- **ExcSh**: Excess quantity. Number of items exceeding the ordered quantity. Excess quantities may be due to the movement of items.
  - **Technical info**: display field
  - "Functions in Dispatch" on page G-1946
- **LL**: Loading list number if loading lists have already been printed for this tour. Use `<F4>` to print the loading lists.
  - **Technical info**: numeric field, DB field: `lapoolauf.llnr`
  - "Print loading list" on page G-2014
  - "Print all loading lists" on page G-2015
- **PL**: The preliminary delivery note shows whether all preliminary delivery notes have been printed for this route.
  - All preliminary delivery notes have been printed.
  - Not all of the preliminary delivery notes have been printed.
- Use `<F4>` to print a preliminary delivery note.
  - Software Reference, "Print loading list" on page G-2014
- A+W Enterprise will mark the field as 'not printed' in the following cases:
  - Change of route
  - Change of order
  - Change of order item(s)
- Preliminary delivery notes can be printed even if the shipment has not been reported complete. If only the preliminary note has been printed for an order, the order can still be changed in shipping control. If a delivery note has been printed for an order, the order cannot be changed any more in shipping control. A preliminary delivery note is no separate document in the database. The order status does not change because of a preliminary delivery note. When the goods are shipped, the shipped quantity has to be corrected on the preliminary delivery note. To print the delivery note, the corrected quantities must be transferred.
  - **Technical info**: toggle field, DB field: `lapoolauf.vlsdrukz`
- **DN**: Current status of the delivery note:

| DN | Meaning | Information |
| :--- | :--- | :--- |
| gray | Open | No delivery note created yet. |
| Yellow | Booked to transport | "Book to transport" on page G-1963. |
| blue | Delivery note created. | Document has been fully delivered. |
| red-gray | Delivery stop | A delivery stop has been specified for the customer (this status indicator must be configured explicitly). |
| gray-red | No partial delivery | No partial deliveries are desired for this order (this status indicator must be configured explicitly). |
| red-red | Delivery stop/no partial delivery | There is a delivery stop for this customer and no partial delivery is desired for the current order (this status indicator must be configured explicitly). |

*Tab. G-3 Status of the delivery note*

Use `<F4>` to create and print the delivery note. Printing the delivery note creates the corresponding record for financial accounting.
- **Technical info**: display field
- "Rack information" on page G-1970
Use `<Shift>` + `<F4>` > Cancel to cancel the delivery notes.
- "Cancel delivery note" on page G-1975
- **Cmp.**: Order reported complete. All items have been packed.
  - All items are ready for shipment.
  - Not all of the items are ready to be shipped.
  - **Technical info**: display field, DB field: `lapoolauf.kompl`
- **Call**: Call order. The order is delivered on request from the customer.
  - Call order.
  - No call order.
  - **Technical info**: display field, DB field: `lapoolauf.abruf`
- **I Invoiced**: shows whether the order has been completely invoiced.
  - Order completely invoiced.
  - Invoiced not yet completely invoiced.
  - **Technical info**: display field, DB field: `lapoolauf.fakturakz`
- **I Shipping information**: shows whether shipping information is available for this order. Shipping information is entered in Sales or Purchasing in dialog External information. Use `<Shift>` + `<F4>` > SA/PU information to call up this information.
  - There is dispatch information for this order or receipt of goods.
  - There is no dispatch information for this order.
  - **Technical info**: Display field, DB field: `lapoolauf.info`

### Footer

The footer of the tab shows for all items the total quantities in the following fields:
- Tot. (total)
- Call (request)
- Avail. (available)
- Pack. (packed)
- Back. (backlog)
- Add. (To be delivered later)
- ExcSh Excess (delivered quantity)

### Additional information
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## OrderInfo/Rack tab
**Dispatch control – delivery date selection > Route selection > OrderInfo/Rack tab**

*Fig. G-28 Dispatch control – OrderInfo/Rack tab*

The Order info/Rack tab is displayed dynamically if you are working with the Rack module in Dispatch Control. Additional rack information are displayed for each order.
The search fields in the header are explained in connection with Dispatch control. Tour number and name are shown as well.
- "Dispatch Explorer" on page G-1901
Most fields have already been described in the previous section:
- "Order Info tab" on page G-1925
In addition, the following fields are displayed on the OrderInfo/Rack tab:
- **On Rack**: Rack number on which the lites to be delivered are located. For the configuration of the free racks in the Dispatch Control, you must contact an A+W employee.
  - **Technical info**: numeric field, DB field: `lapoolauf.freigeststk`

### Footer
The footer of the tab shows for all items the total quantities in the following fields:
- Tot. (total)
- Call (request)
- Avail. (available)
- Pack. (packed)
- On rack (on the rack)

### Additional information
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## Delivery Address tab
**Dispatch control – delivery date selection > Route selection > DeliveryAddress tab**

*Fig. G-29 Dispatch control – Delivery address tab*

The Delivery address tab provides dispatch information on every order such as: address, travel time, and loading sequence on the truck or trailer.
The search fields in the header are explained in connection with Dispatch control. Tour number and name are shown as well.
- "Dispatch Explorer" on page G-1901
Most fields have already been described in the previous section:
- "Order Info tab" on page G-1925
In addition, the following fields are displayed on the OrderInfo/Rack tab:
- **LS**: Loading sequence of orders on the truck. The sequence of customers on a tour or route determines the loading sequence for the orders. When a new entry is made or an existing entry is changed, A+W Enterprise will want to know whether the changed loading sequence shall be applied to other orders.
  - **Technical info**: numeric field, DB field: `lapoolrouteposnr`
- **Deliv. date**: Scheduled delivery date at the customer's.
  - **Technical info**: date field, DB field: `lapool.ankunft`
- **D. time**: The arrival time is taken over from the order if you are working with the via-Plant delivery.
  - **Technical info**: Alphanumeric field, DB field: `lapool.ankunftszeit`
  - "Shipment information" on page G-2004
- **TT**: Travel time to the customer. The planned travel time is determined from the delivery address for the document (order/PO).
  - **Technical info**: Numeric field, DB field: `lapool.fahrtzeit`
- **Shipping address, street, post code, city**: Customer's or supplier's delivery address. These fields are taken over from the delivery address in the document. The delivery address can be changed in Dispatch Control.
  - **Technical info**: Display fields, DB field: `lapool.lname`, `lapool.lstr`, `lapoolauf.lplz`, `lapoolauf.lort`.
  - "Find delivery address" on page G-1968
  - "New delivery address" on page G-1969
- **Spl**: Split. A number entry in the Split field causes the breakdown of the total quantity into the appropriate number of deliveries.
  - **Technical info**: Numeric field, DB field: `lapool.splitt`

### Footer
The footer of the tab shows for all items the total quantities in the following fields:
- Weight (of the order) of (the total weight to be transported)
- Surface (of the order) of (the total surface to be transported)
- Requested del. date

### Additional Information
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## Dispatch Info I tab
**Dispatch control – delivery date selection > Route selection > Dispatch Info I tab**

*Fig. G-30 Dispatch Control – Dispatch Info I tab*

The Dispatch Info I tab provides further shipping information about the order.
The search fields in the header are explained in connection with Dispatch control. Tour number and name are shown as well.
- "Dispatch Explorer" on page G-1901
Most fields have already been described in the previous section:
- "Order Info tab" on page G-1925
In addition, the following fields are displayed on the Dispatch Info I tab:
- **Ref.**: Reference document for orders transferred from another site.
  - **Technical info**: numeric field, DB field: `kauf.parauftrnr`
- **Ex. sender**: External sender. For transferred orders, the client number of the sending site is displayed.
  - **Technical info**: numeric field, DB field: `kauf.parhausnr`
- **In. sender**: Internal sender. For transferred orders, the order number of the receiving site is displayed.
  - **Technical info**: numeric field, DB field: `kauf.parhausnr`
- **Dispatch Info**: Shipping information is displayed only if it has been defined at order entry. You can edit existing dispatch information or enter new dispatch information in this field. You can use `<Ctrl>` + `<B>` to take the dispatch information over into the order.
  - **Technical info**: Numeric field, DB field: `lapool.exbez2`
- **PAT**: ID of the new packing type from the order. The assigned packing type is displayed on the Dispatch Info I tab in plain text. You can assign a new packing type to the order with the `<F9>` key. This change is only taken over with `<Ctrl>` + `<B>`.
  - **Technical info**: Numeric field, DB field: `lapool.verpackart`
- **ST**: ID of the dispatch type from the order. The assigned dispatch type is displayed on the Dispatch Info II tab in plain text. You can assign a new dispatch type to the order with `<F9>`. This change can only be taken over into the order with `<Ctrl>` + `<B>`. Alternatively, the dispatch type can be stored or changed via the info menu `<Shift>` + `<F4>`.
  - "Shipment information" on page G-2004
  - **Technical info**: numeric field, DB field: `lapool.versandart`
- **ST**: Delivery type ID. The assigned delivery type is displayed on the Dispatch Info II tab in plain text. You can assign a new delivery type to the order with the `<F9>` key. This change is only taken over with `<Ctrl>` + `<B>`.
  - **Technical info**: Numeric field, DB field: `lapool.lieferart`
- **E.Cust**: Exit customs. Number of the customs office in the country of origin. You can enter a different customs clearance office.
  - **Technical info**: numeric field, DB field: `lapool.azsnr`
- **D.Cust**: Destination customs. Number of the customs office in the country of destination. You can enter another customs office in the country of destination.
  - **Technical info**: numeric field, DB field: `lapool.bzsnr`
- **via S**: Number of the site that makes the delivery. The field is only assigned with use of the via-plan module.
  - **Technical info**: Numeric field, DB field: `lapool.viahaus`
- **Route**: Number of the route by which the shipment is made. The field is only assigned with use of the via-plan module.
  - **Technical info**: Numeric field, DB field: `lapool.endroute`

### Additional information
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## Dispatch Info II tab
**Dispatch control – delivery date selection > Route selection > Dispatch Info II tab**

*Fig. G-31 Dispatch Control – Dispatch Info II tab*

Dispatch Info II tab shows the information from the Dispatch Info I tab in detail.
The search fields in the header are explained in connection with Dispatch control. Tour number and name are shown as well.
- "Dispatch Explorer" on page G-1901
Most fields have already been described in the previous section:
- "Dispatch Info I tab" on page G-1933
In addition, the following fields are displayed on the Dispatch Info II tab:
- **Dispatch Info**: Abbreviated dispatch information. This is only displayed if it is stored in the order or the PO. You can change the dispatch information or enter new dispatch information in the field.
  - **Technical info**: display field
- **Packing type**: Description of the packing type. The assigned ID is displayed on the Dispatch Info I tab.
  - **Technical info**: display field
- **Disp. Type**: Description of the dispatch type. The assigned ID is displayed on the Dispatch Info I tab.
  - **Technical info**: display field
- **Incoterm**: Description of the delivery type. The assigned ID is displayed on the Dispatch Info I tab.
  - **Technical info**: display field
- **PL1, PL2**: Private Long 1 and Private Long 2 are meant for customized supplementary information. At Order entry you can save information in the form of numbers. The field names PL1 and PL2 can be configured customer-specifically. Via the info menu `<Shift>` + `<F4>` in the Dispatch Control, you can store or change these fields.
  - "Shipment information" on page G-2004
  - **Technical info**: numeric field, DB field: `lapool.private_long1`, `lapool.private_long2`
- **PC1, PC2**: Private Char 1 and Private Char 2 are meant for customized supplementary information. At Order entry you can save informational texts. The field names PC1 and PC2 can be configured customer-specifically. The maximum input per field is 15 characters. Via the info menu `<Shift>` + `<F4>` in the Dispatch Control, you can store or change these fields.
  - "Shipment information" on page G-2004
  - **Technical info**: alphanumeric field, DB field: `lapool.private_char1`, `lapool.private_char2`

### Footer
No additional information is output in the tab's footer.

### Additional information
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## Add. Info tab
**Dispatch Control – delivery date selection > Route selection > Add. Info tab**

*Fig. G-32 Dispatch control – Add. Info tab*

Additional info tab shows the delivered quantity and further information on the order, item weight, movements, and information on the release for shipment provided by the customer.
The search fields in the header are explained in connection with Dispatch control. Tour number and name are shown as well.
- "Dispatch Explorer" on page G-1901
Most fields have already been described in the previous section:
- "Dispatch Info I tab" on page G-1933
In addition, the following fields are displayed on the Add. Info tab:
- **Customer**: Customer name or supplier name from the order or PO.
  - **Technical info**: Display field, DB field: `mp.name`
- **T/Del**: Total quantity delivered to the customer so far.
  - **Technical info**: numeric field, DB field: `lapoolauf.geslief`
- **kg/N**: Net weight of the order in kilograms. The net weight is the weight of all items, excluding racks or packaging.
  - **Technical info**: toggle field, DB field: `lapoolauf.gewicht`
- **kg/G**: Gross weight of the order in kilograms. The gross weight is the weight of all items including racks and packaging.
  - **Technical info**: toggle field, DB field: `lapoolauf.gewichtbrutto`
- **sqft**: Total square meters of glass from the order.
  - **Technical info**: Display field, DB field: `lapoolauf.qm`
- **DN**: Traffic light display for the delivery note.
  - "Status of the delivery note" on page G-1927
- **Call**: Call code for the order. The order is delivered on request from the customer.
  - **Technical info**: Display field, DB field: `lapoolauf.abrufkz`
- **Postp.**: Code to mark to postpone the order. If you would like to postpone several orders to another dispatch date, then you must click the checkboxes of the orders in question. The selected orders are then marked with a checkmark. You postpone the orders on the Postpone (Dispatch) dialog.
  - The order will be postponed.
  - The order will not be postponed.
  - **Technical info**: display field, DB field
  - "Functions in Dispatch" on page G-1946
- **Call**: Shows whether the customer is informed of the shipment of goods by phone.
  - Customer will be called prior to dispatch.
  - Customer will get no call.
  - If you enable the field, the Call checkbox will automatically be enabled for all other orders for this customer.
  - **Technical info**: Alphanumeric field, DB field: `lapoolauf.anruf`
- **Print**: Defines whether a delivery note has been printed.
  - Delivery note has been printed.
  - Delivery note has not been printed yet.
  - **Technical info**: display field, DB field: `lapoolauf.druckkz`
- **Type**: The selected delivery note type for this order is shown as a code. The following codes are available:
  - I = individual delivery note
  - C = collective delivery note
  - **Technical info**: display field

### Footer
The footer of the tab shows for all items the total quantities in the following fields:
- kg/N (net weight)
- kg/G (gross weight)
- sqm (total surface in square meters)
- **Technical info**: Display field

### Additional information
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

# Item Level

Item level in Dispatch Control provides detailed information on the individual order items or purchase orders.

This level offers the following tabs:
- "Item Info I tab" on page G-1941
- "Item Info II tab" on page G-1944

From the item level, you can change back to the order or tour level. If you are working with the Dispatch Explorer, you can also change to the Dispatch Explorer to select another date.
- "Dispatch Explorer" on page G-1901

## Item Info I tab
**Dispatch control – delivery date selection > Route selection > Item Info I tab**

*Fig. G-33 Dispatch control – Item info I tab*

Item info I tab provides detailed information on the orders.
The search fields in the header are explained in connection with Dispatch control. The route, order number, and customer name are shown as well.
- "Dispatch Explorer" on page G-1901

- **S**: The entries in column S (status) are loaded from TourInfo and OrderInfo tab.
  - **Technical info**: display field
  - "Route status" on page G-1915
- **Item**: Sequential item number from the order or PO.
  - **Technical info**: Display field, DB field: `lapool.posnr`
- **Article**: Name of the article to be delivered.
  - **Technical info**: display field, DB field: `artikel.artbez1`
- **Tot.**: Total quantity of the item to be delivered.
  - **Technical info**: display field, DB field: `lapoolpos.gesstk`
- **Call**: Number of items the customer has ordered for that date.
  - **Technical info**: display field, DB field: `lapoolpos.abrufstk`
- **Sched**: Scheduled. Item quantity scheduled for dispatch.
  - **Technical info**: display field, DB field: `lapoolpos.sollstk`
- **Avail**: Available quantity for this item.
  - **Technical info**: display field, DB field: `lapoolpos.gefstk`
- **Pack**: Quantity packed for this item. Use `<F4>` to check for missing quantities. You can use `<F4>` > Correct packed quantity to change the entry in this field.
  - **Technical info**: numeric field, DB field: `lapoolpos.iststk`
  - "Missing quantity check for" on page G-1959
  - "Rack view for order" on page G-1965
- **Back.**: Item quantity that is not available for the desired tour.
  - **Technical info**: display field, DB field: `lapoolpos.rueckstk`
- **Add.**: Quantity to be shipped later. Those shipments may be due to movement.
  - **Technical info**: display field, DB field: `lapoolpos.nachstk`
  - "Move” on page G-1950
- **ExcSh**: Excess quantity. Number of items exceeding the ordered quantity. Excess quantities may be due to the movement of items.
  - **Technical info**: display field, DB field: `lapoolpos.ueberstk`
- **T/Del**: Total quantity delivered to the customer so far.
  - **Technical info**: display field, DB field: `lapoolpos.gesliefstk`
- **kg**: Item weight in kilogram.
  - **Technical info**: display field, DB field: `lapoolpos.gewicht`
- **sqft**: Item surface in square feet.
  - **Technical info**: display field, DB field: `lapoolpos.qm`
- **Cmp**: Completely packed item.
  - All items are ready for shipment.
  - Not all of the items are ready to be shipped.
  - **Technical info**: display field, DB field: `lapoolpos.kompl`
  - "Missing quantity check for" on page G-1959
- **I (invoiced)**: Completely invoiced item.
  - Order item has been invoiced.
  - Order item has not been invoiced yet.
  - **Technical info**: display field, DB field: `lapoolpos.fakturakz`

### Footer
The footer of the tab shows for all items the total quantities in the following fields:
- Tot. (total)
- Call (request)
- Sched. (scheduled)
- Avail (available)
- Pack (packed)
- Back. (backlog)
- Add. (To be delivered later)
- ExcSh (Excess quantity)
- T/Del. (delivered in total)
- kg
- sqft

### Additional information
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

## Item Info II tab
**Dispatch Control – Delivery date selection > Route selection > Order / PO selection Item Info II tab**

*Fig. G-34 Dispatch control – Item info II tab*

Item info II tab shows the items for the order in question plus additional information on the individual items.
The search fields in the header are explained in connection with Dispatch control. The route, order number, and customer name are shown as well.
- "Dispatch Explorer" on page G-1901
Most fields have already been described in the previous section:
- "Item Info I tab" on page G-1941
In addition, the following fields are displayed on the Add. Info tab:
- **Pack/Pack. type**: Number and description of the packing type.
  - **Technical info**: display field, DB field: `lapoolpos.verpackart`
- **Width, Height**: Item size.
  - **Technical info**: display field, DB field: `lapoolpos.breite`
- **mm**: Thickness of the item lite in millimeters.
  - **Technical info**: Display field, DB field: `lapoolpos.staerke`

### Footer
The footer of the tab shows for all items the total quantities in the following fields:
- Tot. (total)
- Sched. (scheduled)
- Pack (packed)
- kg
- sqft

### Additional information
- "Supplementary menu" on page G-1908
- "Info menu" on page G-1911
- "Buttons" on page G-1913

# Functions in Dispatch

In the Dispatch Control, you have the opportunity to pack the item quantity manually or to postpone it, to manage racks and print the dispatch documents. Depending on the status of the selected data on the item, order or tour level and the available system configuration, the following functions are available:
- "Search" on page G-1947
- "Go to" on page G-1948
- "Move” on page G-1950
- "Postponement of several items - selection" on page G-1952
- "Postponement of several items - action" on page G-1953
- "Order info" on page G-1954
- "Book goods receipt for" on page G-1957
- "Cancel receipt of goods" on page G-1958
- "Missing quantity check for" on page G-1959
- "Missing quantity check - actions" on page G-1961
- "Print loading list" on page G-2014
- "Book to transport" on page G-1963
- "Rack view for order" on page G-1965
- "Rack information" on page G-1970

Furthermore, you have many overview opportunities and information dialogs using the pre-determined criteria:
- "Cancel transport booking" on page G-1964
- "SA/PU info (global)" on page G-1998
- "Booked racks (overview)" on page G-1987
- "Information on the order" on page G-1955
- "Finished goods stock - overview" on page G-2008
- "Shipment information" on page G-2004
- "Set/remove tour lock" on page G-1971

## Search
**Dispatch Control – [Search]**

*Fig. G-35 Go to...*

You can reach the Search dialog on all data levels. This way, you can search for a particular document and jump directly to this document.
With the key combination `<Ctrl>` + `<K>`, you are also taken to the Order info.

- **Order**: Order number. Enter the number in this field or select the number with `<F9>`. With this search, you get detailed information about the selected document.
  - **Technical info**: Numeric field, selection field, `<F9>`
  - "Information on the order" on page G-1955
- **Mode**: Dispatch mode. If you want to change directly to the PO documents, toggle in the Mode field to the value in question. With a purchasing mode, you can then search for a PO instead of an order.
  - **Technical info**: Toggle field

| Button | Description |
| :--- | :--- |
| [Trigger] | Use Trigger to start the search. |
| [Cancel] | Use Cancel to discard the search. |

## Go to
**Dispatch control – [Go to]**

*Fig. G-36 Go to...*

You can reach the Go to dialog on all data levels. This way, you can search for a particular document and jump directly to this document. The Delivery date, Site, and Mode fields are pre-populated with their current values. If needed, you can change the search criteria.

- **Deliv. date**: Delivery date of the orders. This field is pre-populated with the current date. You can change this entry.
  - **Technical info**: Input field, date format.
- **Site**: Number of the site or client whose orders you are searching. The field is pre-populated with the value that is assigned by default to the current employee in the master data.
  - **Technical info**: Selection field, `<F9>`
- **Route**: Route number. If you leave the Route field empty and there are planned routes for the Delivery date, you jump directly to the Tour Info.
  - **Technical info**: Selection field, `<F9>`
  - "RouteInfo tab" on page G-1915
- **Order**: Order number. If you leave the Order field empty and there are orders for the Delivery date and the selected route, you jump directly to the Order Info.
  - **Technical info**: Selection field, `<F9>`
  - "Order Info tab" on page G-1925
- **Item**: Sequential item number from the document. If you select the fields Delivery date, Route, and Order, the Item Info starts directly.
  - **Technical info**: Selection field, `<F9>`
  - "Item Info I tab" on page G-1941
- **Mode**: Dispatch mode. If you want to change directly to the PO documents, toggle in the Mode field to the value in question. With a purchasing mode, you can then search for a PO instead of an order.
  - **Technical info**: Toggle field

| Button | Description |
| :--- | :--- |
| [Trigger] | Use Trigger to start the search. |
| Cont. Delete | You can empty the dialog fields with Delete Content. |
| [Cancel] | Use Cancel to discard the search. |

## Move
**Dispatch control – Data level > `<F4>` Postpone**

*Fig. G-37 Postponement (dispatch)*

This dialog is used to postpone tours, orders, or units to another date or another route. You can enter text describing the reason of postponement in field Reason.

If you start Postponement on the tour level, the whole route can be postponed. In this case, the Order and Item fields in the upper part of the dialog are empty. If you start Postponement on the order or item level, these two fields are pre-populated accordingly.

The fields in the upper part of the dialog indicate what will be postponed:

- **Frm Tour D.**: Originally scheduled delivery date.
- **Route**: Number of the originally scheduled route.
- **Units**: Number of units to be postponed.
- **Order**: Number of the order to be postponed. The display is empty if the entire route is postponed.
- **Item**: Sequential order item number that will be postponed. The display is empty if the entire route or the entire order is postponed.

The fields in the middle of the dialog indicate to when and why the postponement:

- **Reasons**: Choose a reason for the postponement. It can be configured in the system which of these reasons appears as default value on the dialog. The following reasons are possible:
  - **Cust. Request**: The customer has asked for the postponement.
  - **Backlog**: The item is still incomplete or not ready for shipment.
  - **Client-Cancel**: The customer has cancelled the order, the item, or part of the quantity. With the postponement as customer cancellation, both the call quantity as well as the planned quantity are reduced by the amount canceled.
  - **Prod.-Cancel**: Delivery is cancelled for internal reasons, e.g. if the product is no longer available. With Prod. Cancel, only the planned quantity is reduced. The postponement can be configured separately with the reason Prod. Cancel.
  - **Tour Planning**: The postponement is due to route planning or scheduling. The postponement is done analogous to the Cust Request only on the tour level. This possibility can be configured separately. Similarly, the Tour Planning reason can be configured as the default reason.
- With additional configuration, customer-specific reasons can be stored as a selection. With this configuration, the Reason field can be left empty or a free text entered. Here, the system sends an e-mail with the postponement reason to the responsible employee.
- **Postponement**: Text field for entering the reason of postponement. This text will appear in the shipping log.
- **Rack**: Rack number. If you are working with racks in the Dispatch Control, under some circumstances, entire racks can be postponed. However, this possibility depends on other criteria, such as packed and available quantity, rack scheduling, item status.
- **Postpone several records**: Toggle field.
- **To tour day**: New delivery date. When you start postponement, the system checks whether the defined date is a valid delivery date. If the new date is not a valid tour date, then the tour or delivery cannot be postponed. If you are working with planned routes, you can search for a particular tour in this field with `<F9>`.
  - Master Data: Software Reference, "Route plan" on page B-263
- **Route**: Number of the new route if the route needs to be amended due to the postponement.
- **Units**: Number of units to be postponed. A+W Enterprise shows the total quantity by default.

The fields in the lower part of the dialog specify who and when is postponing:

- **Executed by**: Employee number of the person who has made the postponement. This information is written to the log.
  - "Shipment information" on page G-2004
- **on**: Date on which the postponement was made. This information is written to the log.
  - "Shipment information" on page G-2004

## Postponement of several items - selection
**Dispatch control – Data level > `<F4>` Postpone several items**

*Fig. G-38 Postpone several items - selection dialog*

This dialog is used to filter your shipments in order to postpone several items of an order or several orders at the same time. On the following dialog, you specify the quantity to be postponed per item.
- "Postponement of several items - action" on page G-1953

- **Site**: Site number. The field is pre-populated with the current site number. You can only change the value if you are working on a multi-client system.
  - **Technical info**: Selection field, `<F9>`, DB field: `lapool.hausnr`
- **Date**: Delivery date. The field is pre-populated with the date that you displayed on the original data level.
  - **Technical info**: Input field, date format, DB field: `lapool.ltplan`
- **Route**: Route number. The field is pre-populated with the route number that you displayed on the original tour level.
  - **Technical info**: Selection field, `<F9>`, DB field: `lapool.ltplan`
- **Order**: Number of order. The field is pre-populated with the order number that you displayed on the original order level.
  - **Technical info**: Selection field, `<F9>`, DB field: `lapool.auftrnr`
- **Loading list**: Number of loading list. You can search for a particular loading list here if it has already been assigned.
  - **Technical info**: Selection field, `<F9>`, DB field: `lapool.llnr`

## Postponement of several items - action
**Dispatch control – Data level > `<F4>` Postpone several items, make selection**

*Fig. G-39 Postponement of several items*

On this dialog, you select the items for postponement. You also adjust the quantity per item that must be postponed. You have already made the pre-selection through details:
- "Postponement of several items - selection" on page G-1952
Most fields have already been described in the following section:
- "Item Info I tab" on page G-1941
You can change the following fields to make the postponement:

- **Move**: The Postpone field is pre-populated with the item quantity. You can change this quantity if only part of the item should be postponed. At most the item quantity may be postponed. The program checks the plausibility of the value entered.
  - **Technical info**: Input field, numeric field.
- **Book. date**: Checkbox for action marking the booking.
  - Item is marked for postponement.
  - Item will not be postponed.
  - **Technical info**: Selection field, checkbox.

Start the postponement with the [Trigger] button. In the following dialog, enter to when the marked items should postponed.
- "Move” on page G-1950

## Order info
**Dispatch control – Data level> `<F4>` > Order info.**

*Fig. G-40 Postpone several items*

On this dialog, you search for an order (in dispatch mode for sales documents) or for a PO (in dispatch mode with purchasing documents). With the [Trigger] button, you can access the information you're looking for.

- **Order/PO**: Document number. With `<F9>` you can search for the desired document number.
  - **Technical info**: `<F9>`, numeric field, DB field: `lapool.auftrnr`
- **Mode**: Dispatch mode. In this field, you select the dispatch mode. This decides whether the selection will be made by order or PO. With `<F9>` you can search for the desired document number.
  - **Technical info**: Selection field, `<F9>`, DB field: `lapool.vmodus`

The search results are described in the next section:
- "Information on the order" on page G-1955

## Information on the order
**Dispatch control – Data level > `<F4>` > Order info > [Trigger]**

*Fig. G-41 Information on the order or the PO*

On this dialog, you see additional information about the selected document. The dialog title is dynamic; the display is adjusted depending on the dispatch mode. In addition, the appropriate document number appears in the title. All fields on this dialog are informative and cannot be changed.

**C Status of current delivery item.**

| S (Status) | Meaning | Information |
| :--- | :--- | :--- |
| white | Open | There is no dispatch planning for this item. |
| green/yellow | Available | Part of this item is reported as Available. |
| yellow/white | Part on rack | Part of this item is already on the rack. |
| Yellow | Packed | This item is completely packed. |
| half blue | En route | Part of this item is already en route. |
| blue | Delivered | This item has been fully delivered. |
| red | Locked | This item is on a locked tour. |

*Tab. G-4 Status of delivery items*

- **Site**: Site number or client number.
  - **Technical info**: Display field, DB field: `lapool.hausnr`
- **HT**: Handling time from the order or PO in order to load and unload the goods. The handling time can be specified in the market partner master data.
  - **Technical info**: Display field, DB field: `lapool.hausnr`
- **Del. date**: Date on which the order will be delivered to the customer.
  - **Technical info**: display field, DB field: `lapool.ltplan`, `kauf.ltplan`
- **Arrival**: Date on which the shipment reaches the customer. The arrival date is calculated starting from the delivery date - taking into account various other criteria - such as travel time, handling time, tour plan, route days, and the calendar.
  - **Technical info**: Display field, `<F9>`, DB field: `lapool.auftrnr`
- **Route**: Route number.
  - **Technical info**: display field, DB field: `lapool.routenr`
- **Order**: Order/purchase order number.
  - **Technical info**: display field, DB field: `lapool.auftrnr`, `lapool.vorgang`
- **Item**: Item number.
  - **Technical info**: display field, DB field: `lapool.posnr`
- **Tot.**: Total item quantity.
  - **Technical info**: Display field, DB field: `lapool.gesstk`, `kpos.menge`
- **Call**: Number of items the customer has ordered for that date.
  - **Technical info**: display field, DB field: `lapool.abrufstk`
- **Sched**: Quantity of the item already scheduled.
  - **Technical info**: display field, DB field: `lapool.sollstk`
- **Pack**: Quantity packed for this item.
  - **Technical info**: display field, DB field: `lapool.iststk`
- **Width**: Width of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.laenge`
- **Height**: Height of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.breite`
- **kg**: Item weight in kilogram.
  - **Technical info**: display field, DB field: `lapool.gewicht`
- **VP**: Display checkbox if the goods are delivered via-plant.
  - **Technical info**: Display field
- **[FP Stock]**: This button opens the Finished Goods dialog.
  - "Finished goods stock - overview" on page G-2008
- **[Go to]**: This button opens the Go to dialog.
  - "Go to" on page G-1948

## Book goods receipt for
**Dispatch control - Data level > `<F4>` > Book goods received for**

*Fig. G-42 Book goods receipt for*

On this dialog, you select an order for which you would like to book the receipt of goods. This function is only available for the via-plant configuration.

> **via-plant configuration**
> The function scope via-plant is not part of this documentation. If necessary, please request a detailed description from the responsible A+W employee.

## Cancel receipt of goods
**Dispatch control - Data level > `<F4>` > Cancel receipt of goods**

*Fig. G-43 Information on the order*

On this dialog, you select an order for which you would like to book the receipt of goods. This function is only available for the via-plant configuration.

> **via-plant configuration**
> The function scope via-plant is not part of this documentation. If necessary, please request a detailed description from the responsible A+W employee.

## Missing quantity check for
**Dispatch Control – data level > `<F4>` > Missing quantity check for**

*Fig. G-44 Missing quantity check for ...*

On this dialog, you select for which order you would like to check the item quantity. You can check all orders for the particular delivery date or the route or you can select only a particular order. A missing quantity check for is conducted if an item cannot be delivered completely on the specified delivery date.

> **Missing quantity check in dispatch**
> A missing quantity check in dispatch is conducted only at the user's own responsibility. When working with A+W Production, the production software takes over all quantity bookings. If, however, you run the check in Dispatch Control, some of the conditions for the missing quantity check and subsequent booking in the system can be configured individually. Contact an A+W about this.

- **Del. date**: Delivery date for which missing quantities shall be checked. The field is pre-populated with the date that you selected on the previous dialog.
  - **Technical info**: entry field, DB field: `lapool.ltplan`
- **Route**: Number of the route to be checked for missing quantities. If you leave the field empty, all orders for the selected delivery date are loaded into the action dialog.
  - **Technical info**: Selection field `<F9>`, numeric field, DB info: `lapool.routenr`
- **Order**: Number of the order to be checked for missing quantities. If you leave the field empty, all orders for the selected delivery date and the selected route are loaded into the action dialog.
  - **Technical info**: Selection field, date format, DB info: `lapool.auftrnr`
- **Loading list**: Number of the loading/cargo list to be checked for missing quantities. By entering the loading list number, you restrict the selection.
  - **Technical info**: Selection field `<F9>`, numeric field, DB info: `lapool.llnr`

- **[Trigger]**: Use this button to open the Check missing quantities dialog.

### Additional information
- "Missing quantity check - actions" on page G-1961

## Missing quantity check - actions
**Dispatch Control – data level > `<F4>` > Missing quantity check for > Make selection > [Trigger]**

*Fig. G-45 Dispatch control – Missing quantity check view*

You conduct the missing quantity check on this dialog. When entering the dialog, the Pack column is pre-populated with the order or item quantity. If the total quantity is not available, you can correct this for the affected order. The missing quantity is written automatically to the BLog (backlog) field. You can postpone the missing quantity to a different date or another route subsequently.

The pre-population is done with the Missing quantity check for... search dialog.
- "Missing quantity check for" on page G-1959

The fields in the header serve for orientation. These fields provide information about where you are.
All fields have already been described in the previous sections:
- "Order Info tab" on page G-1925
- "Item Info I tab" on page G-1941

- **Pack**: Packed quantity. Changing the packed quantity will also change the entry in field Backlog. You can postpone the entire item.
  - **Technical info**: Input field, date format, DB info: `lapool.iststk`
  - "Postponement of several items - action" on page G-1953
- **Back.**: The backlog is the result of deducting the packed quantity from the scheduled quantity.
  - **Technical info**: Display field, date format, DB info: `lapool.rueckstk`
- If the planned units are not available on the planned date, then you must postpone the remaining units (backlog) to another date. When you trigger the booking, you can postpone the missing quantity as backlog:
  - Postponement of several items - action
- **Date**: Scheduled shipping date. If you change the date, A+W Enterprise will want to know whether the date shall be passed on downwards. This means that all items shown in this dialogue will be shipped at the amended date.
  - **Technical info**: Selection field, date format, DB info: `lapool.ltplan`
- **Book. date**: Selection field for booking this record.
  - **Technical info**: Checkbox

### Buttons
If there is a backlog, the corresponding order item must be postponed to another date.
Use [Postpone] to open the dialog Postponement.
- "Postponement of several items - action" on page G-1953
Use [Book] to save the changes. The selected item is reported packed. If the item quantity is packed completely, the status of the item is set to cmp. (complete).
- "Item Info I tab" on page G-1941

## Book to transport
**Dispatch control - Data level > `<F4>` > Book to transport**

Completely packed items can be booked to transport using this menu element. The booking is done in the background. Depending on the system configuration, a delivery note can be generated. Furthermore, it can also be configured whether the bookings to transport for the past and/or future are permitted.

A transport booking causes the appropriate status change:
- "Status of delivery items" on page G-1955

For booking results, see, for example:
- "Log" on page G-2010

> **Book to transport**
> This function can be configured separately. Contact an A+W about this.

## Cancel transport booking
**Dispatch control – Data level > `<F4>` > Cancel transport booking**

*Fig. G-46 Cancel transport booking for...*

On this dialog, you select an order for the transport rebooking. This action assumes that there was already a transport booking. After you have rebooked the transport booking, you can create a new preliminary delivery note or a delivery note for the corrected delivery quantity.

- **Del. date**: Delivery date for which the transport booking is reversed.
  - **Technical info**: entry field, DB field: `lapool.ltplan`
- **Site**: Client number of site number for which the transport booking is reversed.
  - **Technical info**: Selection field `<F9>`, numeric field, DB info: `lapool.hausnr`
- **Order**: Order number for which the transport booking is cancelled.
  - **Technical info**: Selection field `<F9>`, numeric field, DB info: `lapool.auftrnr`
- **Via site**: Number of the site used to cancel the transport booking.
  - **Technical info**: Selection field `<F9>`, numeric field, DB info: `lapool.viaflag`

- **[Trigger]**: Use this button to trigger the rebooking.

## Rack view for order
**Dispatch control - Data level > `<F4>` > Rack view for Order**

*Fig. G-47 Rack view for order*

On this dialog, you receive information about the rack barcodes if these already exist. The information is in the database table `bcbock`.

- **Order**: External order number.
  - **Technical info**: numeric field, DB field: `bcbock.auftrnr`
- **Itm**: Item number in the order.
  - **Technical info**: numeric field, DB field: `bcbock.posnr`
- **Rack**: Rack number on which the order item is located. If an order item is split and distributed across several racks, you will see all assignments on this dialog, e.g. order 4002466, item 3.
  - **Technical info**: Numeric field, DB info: `bcbock.gnr`
- **Slot**: Slot number if the current item is in a slot.
  - **Technical info**: Numeric field, DB info: `bcbock.subnr`
- **Piece**: Number of lites on the rack. Since one record per piece is written to the table bcbock, this quantity is totaled up for the rack in question and displayed here.
  - **Technical info**: Numeric field, DB info: `bcbock.anzahl`

> **Table bcbock in dispatch**
> The booking of the database table `bcbock` is only done if the Free rack function is configured appropriately. Contact an A+W about this.

## Results of the rack scheduling
**Dispatch control – Order Level > `<F4>` > Results of the rack scheduling**

*Fig. G-48 Results of the rack scheduling*

On this dialog, you can view information about the rack scheduling.

> **Database tables for rack scheduling**
> The results of the rack scheduling distinguish themselves depending on the system configuration. If you are using the Free racks function, rack-related data is booked to the database tables `gest` and `gestzu` after reporting from A+W Production. If you are using other configurations, the tables `kposgest` and `bcbock` are used. For this reason, the technical info is not always listed in the following fields. For detailed information about rack scheduling, please contact an A+W employee.

The following fields appear on this dialog:
- **Order**: Order number. Display of the rack scheduling is only possible on the order level. You start the display for a particular order.
  - **Technical info**: Display field, DB info: `lapool.auftrnr`
- **Item**: Item number from the selected order.
  - **Technical info**: Display field, DB info: `lapool.posnr`
- **Quantity**: Item quantity that is present on the current rack.
- **Total**: Total item quantity.
  - **Technical info**: Display field, DB info: `lapool.sollstk`
- **Rack**: Rack number.
- **Type**: Rack type. This designation is determined from the master data.
  - **Technical info**: Alphanumeric field, DB info: `gtyp.kurzbez`
- **Del. date**: Delivery date for the current order item.
  - **Technical info**: Display field, DB info: `lapool.ltplan`
- **Route**: Number of the delivery route.
  - **Technical info**: display field, DB field: `lapool.routennr`

## Rack planning
**Dispatch control - Order level > `<F4>` > Packaging planning**

*Fig. G-49 Preliminary delivery note for...*

On this dialog, you can view information about the packaging planning.

> **Packaging planning in A+W Enterprise**
> The results of packaging planning depend on the system configuration. The packaging planning from the order entry is described below:
> - Sales, "Packaging Planning" on page D-1292

> **Customized settings**
> Customized settings are not part of this documentation.

## Find delivery address
**Dispatch control - Order level > `<F4>` Delivery address > Find delivery address**

*Fig. G-50 Find addresses*

On this dialog, you can select a delivery address insofar as it must be changed. By default, the delivery address from the order is taken over into Dispatch Control. The Find address function is also available in the order entry and was also described there. All addresses are displayed that are stored from the customer for the current order. Displayed fields can differ depending on the system configuration. Use the search fields to filter for a saved address.
- Sales, "Find addresses" on page D-1095

## New delivery address
**Dispatch control - Order level > `<F4>` > Delivery address > New delivery address**

*Fig. G-51 Delivery address*

Use this dialog to enter a new delivery address if no address could be found. Clicking [OK] saves the address only for this delivery. With `<F3>` you can write the new address to the master data.

The fields for the dialog are described in the following section:
- Sales, "New delivery address" on page D-1191

## Rack information
**Dispatch control - Order Level > `<F4>` Rack information**

*Fig. G-52 Rack information*

On this dialog, you can set up customer-specifically whether and which rack information can be output.

Access to the dialog is enabled with the environment variable SQL_GEST_INFO. The GruppeID and SQL number are stored in this variable that control the language, fields, and operations output. The figure above serves only to clarify this and will not be described in any more detail in this document.

## Set/remove tour lock
**Dispatch control - Tour level > `<Shift>` + `<F4>` > Set/remove tour lock**

*Fig. G-53 One of the messages for the tour lock*

Use this function to lock the selected tour, or unlock the selected tour. A tour is a route scheduled for a certain delivery date.
A tour is locked when it has been scheduled and no further orders shall be added.
An alternative route must be defined in master data for the tour to be locked. When a new order is booked for this tour at order entry after the tour has been locked, the new order will be automatically assigned to the alternative route.
The route lock is set only if one order of the route is booked by another site or client as being en route.
If a tour lock has been set, field TS (tour status) has the status Tour locked (tool tip: red).
- "Lock all tours" on page G-1972
- "Route status" on page G-1915

## Lock all tours
**Dispatch control - Tour level > `<Shift>` + `<F4>` > Lock all tours**

*Fig. G-54 Result of the tour lock*

This function is used to lock all tours shown on the tab.
A tour is locked when it has been scheduled and no further orders shall be added.
Alternative routes must be defined in master data for the tours to be locked. When a new order is booked for this tour at order entry after the tour has been locked, the new order will be automatically assigned to the alternative routed.
If all tours are locked, all TS (tour status) have the status Tour locked (tool tip: red).
- "Route status" on page G-1915

## Transport data
**Dispatch control - Tour level > `<Shift>` + `<F4>` > Transport data**

*Fig. G-55 Transport data*

On this dialog, you store the transport data for the current tour. You can enter transport data for orders and purchased orders if you have configured the purchasing documents in Dispatch Control.
- "Dispatch Control - Menus" on page G-1908

- **Route**: Number of the route for which the transport data is defined.
  - **Technical info**: display field, DB field: `lapool.routenr`
- **Driver**: Name of the driver for this tour. Employees are defined in master data.
  - **Technical info**: selection field, numeric field, DB field: `mitarb.manr`
- **Vehicle**: Vehicle for the tour. The vehicles are defined in master data.
  - **Technical info**: Selection field, numeric field, DB field: `lkw.lkw.nr`
- **Trailer**: Two fields for the input of trailers for transport. The trailers are stored in the master data.
  - **Technical info**: Selection field, numeric field, DB field: `lkw.lkw.nr`

Use `<End>` to save the settings.
The transport data entered is displayed on the VehicleInfo tab:
- "VehicleInfo tab" on page G-1920

## Stock reference
**Dispatch control - Tour level > `<Shift>` + `<F4>` > Stock reference**

*Fig. G-56 Message on printing stock reference*

This dialog shows the number of the list of picked orders to be printed. For stored goods, this function is used to start the picking or stock withdrawal. This function is configured customer-specifically.

## Cancel
**Dispatch control – Order Level > `<Shift>` + `<F4>` > Cancel**

You can access the following dialogs via the Cancel menu:
- "Cancel delivery note" on page G-1975
- "Order cancellation" on page G-1976
- "Cancel receipt of goods" on page G-1977
- "Cancel shipping status" on page G-1978

A delivery receipt within the via-plant configuration can be canceled on the following dialog:
- "Cancel receipt of goods" on page G-1958

### Cancel delivery note
**Dispatch control – Order Level > `<Shift>` + `<F4>` > Cancel > Cancel delivery note**

*Fig. G-57 Cancel delivery note*

This dialog is used to cancel existing delivery notes. The marking on Order info tab in field DN (delivery note) changes its status to booked to transport (tool tip: yellow). Status S of the order changes to en route (tool tip: half blue).
Before you trigger the cancellation, the order data that you are canceling is displayed on the dialog.

- **Deliv. date**: Date on which the order shall be delivered to the customer.
  - **Technical info**: display field, DB field: `lapool.ltplan`
- **Route**: Route number.
  - **Technical info**: display field, DB field: `lapool.routennr`
- **Order**: Order number for the delivery note to be cancelled.
  - **Technical info**: display field, DB field: `lapool.auftrnr`

### Order cancellation
**Dispatch control – Order Level > `<Shift>` + `<F4>` > Cancel > Cancel order**

*Fig. G-58 Order cancellation*

This dialog is used for canceling an order. In the rules, orders in the Sales area are canceled since the logistics employees do not have the necessary sales information under some circumstances. For order cancellation in dispatch, there can be data inconsistencies if the order is already in production and has the status Local-correction.

- **Order**: Number of the order to be cancelled.
  - **Technical info**: display field, DB field: `lapool.auftrnr`
- **Canc. Inform.**: Information on the cancelled order. Maximum length of this text is 60 characters.
  - **Technical info**: Alphanumeric field, DB info: `kauf.exbez2`

You trigger this action with `<Trigger>`. Depending on the order status, the program can output a security query with a status indication or decline the action. If you want to cancel the order nevertheless, you must enter the reason for cancellation on the following dialog. This reason is displayed in the foreground for the user when the order is called up.

**Additional Information**
- Sales, "Cancel" on page D-1198

### Cancel receipt of goods
**Dispatch control – Order Level > `<Shift>` + `<F4>` > Cancel > Cancel receipt of goods > [Trigger]**

*Fig. G-59 Canc. Inform.*

This dialog is used for canceling a goods receipt. This menu element can only be called up for purchasing documents in dispatch mode.
Before you trigger the cancellation, the data for the goods receipt that you are canceling is displayed on the dialog.

- **Deliv. date**: Delivery date on which the receipt of goods should occur.
  - **Technical info**: Display field, DB info: `lapool.ltplan`
- **Route**: Route number.
  - **Technical info**: display field, DB field: `lapool.routennr`
- **Order**: Number of the PO for which the goods receipt should be canceled.
  - **Technical info**: Display field, DB info: `lapool.auftrnr`, `lapool.vorgang=2`
- **Canc. Inform.**: Information text for the cancelled goods receipt. Maximum length of this text is 60 characters.
  - **Technical info**: Alphanumeric field, DB info: `kauf.exbez2`

### Cancel shipping status
**Dispatch control – Data level > `<Shift>` + `<F4>` > Cancel > Cancel dispatch status**

*Fig. G-60 Message on the cancelled dispatch status*

This function is used to cancel the dispatch status. Dispatch Control automatically sets an order's dispatch status to `Scheduled` if an order is postponed to another delivery date in Dispatch Control. When the dispatch status has been cancelled, the order can be amended at order entry without restrictions.
The Dispatch Control staff has to check with order entry if an order has not been passed on to production yet. The reasons for this are:
- When an order is entered or changed at order entry, the data will be transferred to production. Production produces the order for the defined delivery date.
- If Dispatch Control postpones a released order, production will not be automatically informed of the postponement.

# Racks

Lites are generally placed on racks in production and transported this way. These racks can also be managed in Dispatch Control.
The use of rack scheduling and rack management is customer-specific, so that not all functions and dialogs are available to the same extent. For additional information about the racks in Dispatch Control, please contact an A+W employee.

Dialogs that can be called up with `<Shift>` + `<F4>` Racks are described below:
- "Rack allocation - selection" on page G-1980
- "Rack allocation - view" on page G-1981
- "Resolve rack - selection" on page G-1982
- "Resolve rack - view" on page G-1983
- "Free racks (overview)" on page G-1985
- "Booked racks (overview)" on page G-1987
- "All racks (overview)" on page G-1988
- "Individual racks" on page G-1990
- "Racks for order" on page G-1991
- "Lite allocation" on page G-1993

## Rack allocation - selection
**Dispatch control - Data level >Shift> + >F4> > Racks > Rack allocation**

*Fig. G-61 Selection dialog rack allocation*

On this dialog, you search for an order for which you want to see the rack scheduling. The order selected here must already be scheduled on one or several racks.

- **Site**: Site number on which you work in dispatch.
  - **Technical info**: Display field, DB info: `lapool.hausnr`
- **Del. date**: Delivery date whose data you want to edit in dispatch.
  - **Technical info**: Selection field, date format, DB info: `lapool.ltplan`
- **Route**: Route number whose data you want to edit in dispatch.
  - **Technical info**: Selection field `<F9>`, DB info: `lapool.routennr`
- **Order**: Order number of the order to be edited. The order selection is possible with `<F9>`. In the field next to this, the appropriate Dispatch mode is displayed.
  - **Technical info**: Numeric field, DB info: `lapool.auftrnr`
- **Loading list**: Loading list number if a loading list has already been printed for the order.
  - **Technical info**: Display field, DB info: `lapool.llnr`

With [Trigger] you load the rack data for the selected order. The results of the displays are described on the following dialog:
- "Rack allocation - view" on page G-1981

## Rack allocation - view
**Dispatch control - Data level >Shift> + >F4> > Racks > Rack allocation, selection made**

*Fig. G-62 Rack allocation*

On this dialog, you see the rack allocation for the selected order. The rack allocation is done in A+W Production in that the order items are packed on racks and reported off-site. In addition, there can be tour allocation. You see the results of the report on this dialog.

The dialog title is constructed dynamically, so that in the title, you can see the delivery date and route on which your order is scheduled.

- **Cmp**: Complete code for the current order item on the rack. The code is set if the total item quantity is already allocated to the rack.
  - **Technical info**: display field
- **Rack**: Rack number on which the current order item is located.
  - **Technical info**: Display field, DB field: `gest.exgnr`
- **RType**: Rack type of the current rack number from the rack master data.
  - **Technical info**: Display field, DB field: `gest.exgnr`
- **Order**: Current order number.
  - **Technical info**: display field, DB field: `lapool.auftrnr`, `gestzu.auftrnr`
- **Itm**: Item number of the selected order.
  - **Technical info**: display field, DB field: `lapool.posnr`
- **Article**: Article description from the master data.
  - **Technical info**: display field, DB field: `artikel.artbez1`
- **Tot.**: Total quantity of the item.
- **Call**: Already called quantity of the item.
- **Width**: Width of the lite from the item.
  - **Technical info**: Numeric field, DB field: `lapool.laenge`
- **Length**: Height of the lite from the item.
  - **Technical info**: Numeric field, DB field: `lapool.breite`
- **On rack**: Quantity that is on the rack.
- **Book. date**: Checkbox for the booking.
  - Item is marked for booking.
  - Item will not be booked.

With [All] you can mark all rack records on the dialog to start other actions.
With [Trigger] you save the rack allocation if you have to make manual changes on the dialog.

## Resolve rack - selection
**Dispatch control - Data level `<Shift>` + `<F4>` > Racks > Resolve rack**

*Fig. G-63 Selection dialog for rack resolution*

On this dialog, you select for which delivery date and route you want to resolve the rack.
The selection fields are identical to those in the rack allocation:
- "Rack allocation - selection" on page G-1980

## Resolve rack - view
**Dispatch control - Data level `<Shift>` + `<F4>` > Racks > Resolve rack**

*Fig. G-64 Rack resolved dialog*

On this dialog, you trigger the rack resolution. If you mark the rack for editing (Free column) and execute the action, the allocation to the route and delivery date is triggered and the packed quantities are unpacked again. Subsequently, there can be a new rack-PDC booking, insofar as all criteria for the new booking are fulfilled.

> **Rack bookings via PDC in Dispatch Control**
> The Rack bookings via PDC function must be configured appropriately in your system. Please contact the responsible A+W employee for more information.

- **Rack**: Rack number on which the current order item is located.
  - **Technical info**: Display field, DB info: `gest.exgnr`
- **RType**: Rack type (name) of the current rack number from the rack master data.
  - **Technical info**: Display field, DB info: `gest.typnr`, `gtyp.kurzbez`
- **Order**: Current order number.
  - **Technical info**: Display field, DB info: `lapool.auftrnr`, `gestzu.auftrnr`
- **Itm**: Item number of the selected order.
  - **Technical info**: display field, DB info: `lapool.posnr`, `gestzu.posnr`
- **Article**: Article description from the master data.
  - **Technical info**: display field, DB field: `artikel.artbez1`
- **Tot.**: Total quantity.
  - **Technical info**: Display field, DB info: `lapool.geststk`
- **Width**: Width of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.laenge`
- **Length**: Height of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.breite`
- **on Rack**: Quantity that is on the rack.
  - **Technical info**: Display field, DB info: `gestzu.menge`
- **Free**: Checkbox for marking.
  - Item is marked for booking.
  - Item will not be booked.

If you [Trigger] the booking, you are first asked whether the existing rack allocation should actually be deleted and the packed quantity unpacked again.
With [All] you mark all rack records on the dialog to start additional actions.
With [Trigger] you resolve the rack allocation.

## Free racks (overview)
**Dispatch control - Data level `<Shift>` + `<F4>` > Racks > Free racks (overview)**

*Fig. G-65 Free racks dialog (tour overview)*

On this dialog, you get information about free racks on the current tour. When entering the dialog, it is checked whether there are complete racks for the desired delivery date and tour. If not, you can display all racks for this tour.

- **Cmp**: Complete code for the current order item on the rack. The question mark indicates that the item is not yet completely available.
  - **Technical info**: display field
- **Rack**: Rack number on which the current order item is located.
  - **Technical info**: Display field, DB info: `gest.exgnr`
- **Order**: Order number on this tour.
  - **Technical info**: Display field, DB info: `lapool.auftrnr`, `gestzu.auftrnr`
- **Itm**: Item number of the selected order.
  - **Technical info**: display field, DB info: `lapool.posnr`, `gestzu.posnr`
- **Article**: Article description from the master data.
  - **Technical info**: display field, DB field: `artikel.artbez1`
- **Tot.**: Total quantity.
  - **Technical info**: Display field, DB info: `lapool.gesstk`
- **Sched**: Scheduled quantity.
  - **Technical info**: Display field, DB info: `lapool.sollstk`
- **Call**: Quantity called.
  - **Technical info**: display field, DB field: `lapool.abrufstk`
- **on Rack**: Quantity that is on the rack.
  - **Technical info**: Display field, DB info: `gestzu.menge`
- **Width**: Width of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.laenge`
- **Length**: Height of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.breite`

With [Rack] you start the Lite allocation dialog for the selected rack:
- "Lite allocation" on page G-1993

## Booked racks (overview)
**Dispatch control - Data level `<Shift>` + `<F4>` > Racks > Booked racks (overview)**

*Fig. G-66 Booked racks dialog (tour overview)*

This dialog displays all booked racks for the current tour. You can postpone the desired (marked) racks on this dialog to another tour.

- **Book. date**: Checkbox for the booking. Mark the desired item in order to postpone it with the [Postpone] button. On the Postpone dialog, the data is pre-populated with the current tour and it can then be changed. If a different tour is entered, all rack quantities are postponed and rebooked to racks. Here, the packed quantity is always postponed, even if the postponement is to an earlier date.

The dialog displays the same field as on the dialog for free racks:
- "Free racks (overview)" on page G-1985

You can use the following buttons on the dialog:
- **[Postpone]/`<F3>`**
  - "Move" on page G-1950
- **[Rack]/`<F5>`**
  - "Lite allocation" on page G-1993
- **[Total]/`<Shift>` + `<F9>`**
  - The total of all lites per rack is formed and displayed on the dialog.
- **[All/Complete]/`<Shift>` + `<F8>`**
  - If on the dialog free and complete racks are displayed, you can restrict the display to all or complete.

## All racks (overview)
**Dispatch control - Data level `<Shift>` + `<F4>` > Racks > All racks (overview)**

*Fig. G-67 All racks dialog (tour overview)*

On this dialog, you can see the total rack overview for the current order. With the [Rack] button, you can rebook rack quantities:
- "Lite allocation" on page G-1993

The following fields appear on this dialog:

- **Cmp**: Complete code for the current order item on the rack.
  - The question mark `?` indicates that the item is not yet completely available.
  - An asterisk `*` indicates that the item is complete.
  - An empty field indicates that this item is not yet packed.
- **Rack**: Rack number on which the current order item is located.
  - **Technical info**: Display field, DB info: `gest.exgnr`
- **Order**: Order number on this tour.
  - **Technical info**: Display field, DB info: `lapool.auftrnr`, `gestzu.auftrnr`
- **Itm**: Item number of the selected order.
  - **Technical info**: display field, DB info: `lapool.posnr`, `gestzu.posnr`
- **Article**: Article description from the master data.
  - **Technical info**: display field, DB field: `artikel.artbez1`
- **Tot.**: Total quantity.
  - **Technical info**: Display field, DB info: `lapool.gesstk`
- **Sched**: Scheduled quantity.
  - **Technical info**: Display field, DB info: `lapool.sollstk`
- **Pack**: Quantity called.
  - **Technical info**: display field, DB field: `lapool.iststk`
- **on Rack**: Quantity that is on the rack.
  - **Technical info**: Display field, DB info: `gestzu.menge`
- **Width**: Width of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.laenge`.
- **Length**: Height of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.breite`.
- **Del. date**: Delivery date on which the rack is already allocated.
  - **Technical info**: Display field, DB info: `gest.mdat`
- **Route**: Route number to which the rack is already allocated.
  - **Technical info**: Display field, DB info: `gest.routnrZ`

> **Lite-rack allocation via PDC report**
> For the allocation of lites to racks via PDC report, no fixed allocation is possible if the quantities reported do not match the data in dispatch. Then these racks remain in the system as free racks. If a fixed allocation to a tour is not possible because the quantities in dispatch are on different tours, then you can total up the dispatch quantity from the individual racks on this view in order to make the allocation subsequently.
> Prerequisite: The tours from which the quantities are postponed to the desired tour are not locked by another user.

## Individual racks
**Dispatch control - Data level `<Shift>` + `<F4>` > Racks > Individual racks**

*Fig. G-68 Individual racks*

Use this menu element to call up complete information about a rack. On the selection dialog, you select the desired rack number with `<F9>` or you enter it manually. With [Trigger] you start the lite-rack allocation. The fields for the Lite-Rack allocation dialog are described in the following section:
- "Lite allocation" on page G-1993

- **Racks**: Name of the rack for which the information should be determined.
  - **Technical info**: selection field, `<F9>` alphanumeric, DB field: `gest.exgnr`

## Racks for order
**Dispatch control - Data level `<Shift>` + `<F4>` > Racks > Racks for order**

*Fig. G-69 Rack view for order*

Use this menu element to call up complete rack information for an order. In the selection dialog, you select the desired order number with `<F9>` or you enter it manually.
With the [Trigger] button, you will see the rack overview for the selected order. With the [Rack] button, you start the lite-rack assignment.
The fields for the Lite-Rack allocation dialog are described in the following section:
- "Lite allocation" on page G-1993

- **Racks**: Number of the rack for which the information should be determined. This number is then taken over on the Rack view for the order dialog and displayed in the Rack field.
  - **Technical info**: selection field, `<F9>` alphanumeric, DB field: `gest.exgnr`
- **Order**: Number of the order for which documents are listed.
  - **Technical info**: display field, DB field: `lapool.auftrnr`, `gestzu.auftrnr`
- **Itm**: Item number of the selected order.
  - **Technical info**: display field, DB field: `lapool.posnr`, `gestzu.posnr`
- **Article**: Article description from the master data.
  - **Technical info**: display field, DB field: `artikel.artbez1`
- **Total**: Total quantity.
  - **Technical info**: display field, DB field: `lapool.gesstk`
- **Del. date**: Delivery date on which the rack is already allocated.
  - **Technical info**: Display field, DB info: `gest.mdat`
- **Route**: Route number to which the rack is already allocated.
  - **Technical info**: Display field, DB info: `gest.routnrZ`
- **Pcs.**: Quantity that is on the rack.
  - **Technical info**: Display field, DB info: `gestzu.menge`
- **Width**: Width of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.laenge`.
- **Length**: Height of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.breite`.
- **DN**: Delivery note code.
  - "Status of the delivery note" on page G-1927

## Lite allocation
**Dispatch control - Data level `<Shift>` + `<F4>` > Racks > Lite rack allocation**

*Fig. G-70 Lite rack allocation dialog*

On this dialog, you allocate lites to a rack, route, and delivery date or you get information about existing allocations. You can delete the allocation and therefore empty the rack.

> **Lite rack allocation**
> The functional principle of rack allocation is described separately and can be requested from a responsible A+W employee.

- **Rack**: Rack number for which the rack allocation is executed, displayed or should be changed.
  - **Technical info**: Alphanumeric field, DB field: `gest.exgnr`
- **Type**: Rack type number. The rack types are stored under Logistics - Rack Management - Rack Master Data - Rack Types.
  - **Technical info**: Numeric field, DB field: `gtyp.gtypnr`
- **Remark**: Information field with 60 characters for the rack-lite allocation.
  - **Technical info**: Alphanumeric field, DB field: `gest.bemerk`
- **Weight**: Empty weight of the selected rack. The rack weight is stored per Rack type under Logistics - Rack Management - Rack Master Data - Rack Types. With `<Shift>`+`<F8>` you can change the Weight field. This change applies only for the current rack and is not taken over into the master data for all racks of the rack type.
  - **Technical info**: Numeric field, DB field: `gtyp.eiggew`
- **Modified**: Name of the employee who made the last change to the rack allocation data. The name is determined from the employee master data using the employee number.
  - **Technical info**: Display field, DB field: `gtyp.aendermanr`
- **Fixed tour allocat.**: If the lite-rack allocation has already been made, the route-delivery date allocation will be displayed as information on this line.
- **Booked**: Name of the employee who made the last change to the rack allocation data. The name is determined from the employee master data using the employee number.
  - **Technical info**: Display field, DB field: `gtyp.aendermanr`
- **Lite allocation**: Under the lite allocation, the name of the employee and date of the last change or booking are output. The name is determined from the employee master data using the employee number.
  - **Technical info**: Display field, DB field: `gtyp.aendermanr`
- **Order**: Number of the order that is allocated to the current rack.
  - **Technical info**: Numeric field, DB field: `gestzu.auftrnr`
- **Itm**: Internal item number from the order.
  - **Technical info**: Numeric field, DB field: `gestzu.posnr`
- **Tnr**: Tupel number. The field is only relevant for purchasing documents with extended workbench.
  - **Technical info**: Numeric field, DB field: `aufstrukt.tnr`
- **Quantity**: Item quantity that is on the rack.
  - **Technical info**: Numeric field, DB field: `gestzu.menge`
- **Total**: Total item quantity from the order.
  - **Technical info**: Display field, DB field: `lapool.gesstk`, `kpos.menge`
- **Available**: Available item quantity.
  - **Technical info**: display field
- **D.Route**: Dispatch route. As soon as a fixed lite-rack allocation is made, the appropriate route number is displayed in this field and in the next field, the Delivery date.
  - **Technical info**: display field
- **Deliv. date**: Specified delivery date. As soon as a fixed lite-rack allocation is made, the appropriate delivery date is displayed in this field, and in the field before this one, the Dispatch route.
  - **Technical info**: display field
- **Width**: Width of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.laenge`
- **Height**: Height of the lite from the item.
  - **Technical info**: Display field, DB field: `lapool.breite`
- **Article**: Product name of the item article from the master data.

You have additional possibilities on this dialog:
- With `<Shift>`+`<F8>` you can change the Weight field.
- With `<F5>` you can show the Dispatch info dialog. The dialog is only displayed if there is dispatch information.
- With [Empty] or `<Ctrl>`+`<F8>` you can empty the rack. That is, the content of the rack is removed.

## SA/PU information
**Dispatch control - Order level > `<Shift>` + `<F4>` > SA/PU information**

*Fig. G-71 SA/PU information dialog*

This dialog provides information about the selected order. Insofar as you are working with POs in Dispatch Control, the order information is combined with the associated PO information.

- **Order**: Current order number.
  - **Technical info**: display field
- **Itm**: Internal item number from the order.
  - **Technical info**: display field
- **Tot.**: Total item quantity from the order.
  - **Technical info**: display field
- **Call**: Quantity already called.
  - **Technical info**: display field
- **Pack**: Quantity already packed.
  - **Technical info**: display field
- **Width**: Width of the lite from the item.
  - **Technical info**: Display field
- **Height**: Height of the lite from the item.
  - **Technical info**: Display field
- **Purchase order**: Current PO number if a PO was created for the order item.
  - **Technical info**: display field
- **Itm**: Internal item number from the PO.
  - **Technical info**: display field
- **Date**: PO date.
  - **Technical info**: display field
- **Mode**: Dispatch mode
  - **Technical info**: display field

## SA/PU info (global)
**Dispatch control – Order level > `<Shift>` + `<F4>` > SA/PU info (global)**

*Fig. G-72 SA/PU info (global) dialog*

With the SA/PU Info (global) menu item, you can call up the combined sales and purchasing information for a selected order. On the selection dialog (small figure) you enter the number or select the desired document with `<F9>`. Depending on the dispatch mode selected, you can search for an order or a PO.

The search fields in the header and dispatch mode are described in the following section:
- "Dispatch Explorer" on page G-1901

- **Order**: Number of order.
  - **Technical info**: Display field, DB info: `lapool.auftrnr`
  - If you have selected a PO on the selection dialog, then a PO number is in the Order field and the order number in the Reference field.
- **Itm**: Number of the item.
  - **Technical info**: display field, DB field: `lapool.lfdpos`
- **Article**: Article name of the order.
  - **Technical info**: display field, DB field: `artikel.artbez1`
- **Tot.**: Total item quantity.
  - **Technical info**: Display field, DB info: `lapool.gesstk`
- **Call**: Number of items the customer has ordered for that date.
  - **Technical info**: display field, DB field: `lapool.abrufstk`
- **Date**: Delivery date from the order or PO (1st column on the dialog).
  - **Technical info**: Display field, DB info: `lapool.ltplan`
- **Route**: Route number.
  - **Technical info**: Display field, DB info: `lapool.routenr`
- **Site**: Site number or client number.
  - **Technical info**: display field, DB field: `lapool.hnr`
- **Ref.**: Number of the reference document. If you have selected a PO on the selection dialog, then a PO number is in the Order field and the order number in the Reference field.
  - **Technical info**: Display field, DB info: `lapool.auftrnr` (lapool.vorgang=2 (PO) or 5 (order))
- **Itm**: Item number from the reference document.
  - **Technical info**: Display field, DB info: `lapool.posnr`
- **Date**: Delivery date from the reference document.
  - **Technical info**: Display field, DB info: `lapool.ltplan`
- **Route**: Number of the route from the reference document.
  - **Technical info**: Display field, DB info: `lapool.routenr`
- **Sched**: Scheduled quantity.
  - **Technical info**: Display field, DB info: `lapool.sollstk`
- **Kind**: Dispatch mode for reference document. The following values are displayed:
  - SA Deliv. (SA withdrawal)
  - P1. (PU outgoing goods)
  - P2. (PU incoming goods)
  - **Technical info**: display field, DB field: `lapool.vmodus`

## Dispatch control – overview
**Dispatch control - Data level > `<Shift>` + `<F4>` > Overview**

*Fig. G-73 Shipping control – overview*

With the Overview menu, you start the search dialog with which you can combine various criteria to create an overview.

The following selection criteria are available:
- Site
- Del. Dat (planned delivery date)
- Route (delivery route)
- Order (order number)
- External (customer order no.)
- L/L (number of the loading list)
- Proj. (project number)
- Customer (customer number)
- Weight (item weight in kg)
- Surface (area per item in sq m)
- Width (lite height in mm)
- Height (lite length in mm)
