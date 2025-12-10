---
title: "EN-UM-AW-SmartCompanion-AWE"
source: "EN-UM-AW-SmartCompanion-AWE.pdf"
tags: ["A+W", "Smart Companion", "Software Manual", "Production", "Stock Management", "Glass", "Windows", "Doors", "ERP", "Barcode Scanning"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A user manual for the A+W Smart Companion mobile application, a tool for plant data collection in the glass, windows, and doors industry. It details the functionalities of the Production and Stock modules."
long_description: "This document is the complete user manual for the A+W Smart Companion, a mobile application designed for plant data collection and management within the glass, windows, and doors manufacturing sector. It serves as a smart replacement for traditional barcode scanners, running on iOS and Android devices. The manual is divided into three main parts: Overview, Production, and Stock. The Overview section introduces the basic and licensed features, operational modes for different hardware (smartphones, Zebra scanners), and universal functionalities like messages and filter functions. The Production module guide details user login, the main interface for scanning and booking items, managing machine statuses, handling breakage reports, and accessing detailed information on racks, orders, and inventory. The Stock module guide provides comprehensive instructions on managing warehouse operations, including booking goods receipts, tracking stock movements, processing stock withdrawals (with or without order reference), performing inventory counts for box stocks and warehouses, and editing box contents. The manual is intended for end-users who perform bookings in production and stock areas."
---

# A+W Smart Companion Manual

---
## Editorial

### Revision overview of the documentation

| Version | Description |
| :--- | :--- |
| 2024-06 | Revision of part Overview |
| 2021-03 | Original version |

### Notes
This document is intended only for end users of A+W Smart Companion.
The documentation and software described are licenses that must be used or copied only in accordance with the conditions of our license agreement. The content of the documentation serves only as information and can be changed without prior notice at any time. The text and illustrations were compiled with the utmost care. However it is not possible to exclude errors completely. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.
This document describes the full scope of A+W Smart Companion.

### Copyrights
© 2024, A+W Software GmbH all rights reserved, also those for reprinting, the making of copies and translation.
The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

### Trademarks
All hardware and software designations mentioned in the documentation can also be registered trademarks or other industrial property rights of third parties. The property rights of third parties must be observed.

### Display conventions
Individual elements of the sentences are displayed in a special form. The meanings are:

| Convention | Description |
| :--- | :--- |
| *Italics* | marks character strings describing the software elements, e.g. the *Buckets dialog*. |
| **Bold** | marks character strings to be entered via keyboard, e.g.: **Enter 0**. |
| > | shows the way to open a dialog, e.g. Display > Filler orders > Context menu - List > Order overview. |
| [] | square brackets mark the buttons in the dialog, e. g. [OK] to save the data. |
| < > | pointed brackets refer to keys or shortcuts on the keyboard, e. g. <F1> is used to open the online help. |

### Contact
A+W Software GmbH
Siemensstr. 3
D-35463 Fernwald
Germany

Tel.: +49 641 96620 0
E-Mail: info@a-w.com
Web: http://www.a-w.com

## Table of Contents

### Overview
- Tutorial
- Documentation
- Basics
  - A+W Smart Companion - Basic License
  - A+W Smart Companion - Production
  - A+W Smart Companion - Stock
- Operation
  - Module selection
  - Hardware mode
    - Smartphone
    - Zebra scanner
  - Messages and notices
    - Messages
    - Optical message
    - Acoustic message
  - Filter functions

### Production
- Tutorial
- Login
- Menu bar
- Main page of the Production module
  - Machine status
- Status page
- Breakage page
- Info page
  - Rack information
  - Order status
  - Order location
  - Registration point status
  - Rack shifting
  - Actual rack weight
  - Rack inventory
- Settings

### Stock
- Tutorial
- Login
- Menu bar
- Booking goods receipt
  - Override stock location
  - Assign registration point
- Booking stock movements
- Booking stock withdrawals
  - Stock withdrawal with order
  - Stock withdrawal without order
- Info page
  - Missing prices
  - Inventory
    - Inventory of a box stock
    - Inventory of a warehouse
  - Checklist
- Editing a box
- Print again
- Settings

### Index

---

## Overview

### Revision overview of the module
- **06-2024:** Acoustic notification added
- **2021-03:** Original version

This module provides information on the following subjects:
- Tutorial

### Tutorial
This section provides information on the following subjects:
- Documentation
- Basics
- Operation

#### Documentation
The tutorial for *A+W Smart Companion* will show you how to make bookings in the *production* and *stock* areas. Starting with goods receipt to production bookings, on through to inventory.

**Required knowledge**
The tutorial is directed at customers who book lites into stock and production. Knowledge about how to operate a smartphone is assumed. This specifically includes the following gestures: clicking, swiping, zooming in and zooming out.

#### Basics
The A+W Smart Companion is the smart companion for plant data collection. It can be used on mobile end user devices with the iOS and Android operating systems and therefore replaces the classic barcode scanner.

Depending on the requirements, the A+W Smart Companion can be equipped with various functionalities.

##### A+W Smart Companion - Basic License
The Basic License is the basic module of the A+W Smart Companion. It can be downloaded as an app from the App Store (iOS) or the Play Store (Android). Only through a connection with the back end can the following functionalities be enabled.

##### A+W Smart Companion - Production
The *Production* module provides all booking functionalities that you need in the *A+W Produktion* main module. Reasons for breakage or status messages for racks and trucks can be selected directly from a menu. Therefore, no additional bar code tables are required. Furthermore, you can display the content of a rack, the production status or the location of individual items of an order in production directly on the mobile end user device.

##### A+W Smart Companion – Stock
The *Stock* module supports A+W Software stock management in a mobile application. Simple, completely digital, and paperless delivery of POs (also with direct production parts), stock transactions, and stock removals.

It is currently integrated with the A+W Enterprise A+W Business modules Purchase Order and Stock.

The *Inventory* module of the A+W Smart Companion is already integrated into the Stock module.

> **License**
> As with other scanners (Denso, WinCE, etc.), each device with the A+W Smart Companion requires a database license!

#### Operation
In principle, the A+W Smart Companion can be operated very intuitively. Nevertheless, the individual operating and display elements will be explained in the following sections. A+W Smart Companion can be operated using the scan function or using manual inputs. The appropriate steps will be explained below.

##### Module selection
After starting and authentication of A+W Smart Companion, select the desired module.

| Icon | Module |
| :--- | :--- |
| [Wrench Icon] | Production |
| [Warehouse Icon] | Stock |
*Tab. 1 Selection of the module*

A+W Smart Companion saves the last selected application and automatically selects it after a restart. The module can be changed in App selection at any time.
(See Production: Tutorial, "App selection" on page B-58)

Currently, the Production and Stock modules are supported – additional modules are still under construction.

##### Hardware mode
A+W Smart Companion can be used with the following mobile end user devices:
- Smartphone
- Zebra scanner

Depending on the end user device used, the scan area may look as follows:

**Smartphone**
**(Fig. A-1: Smartphone: Scan area)**
There is a blue line in the middle; use it to scan the appropriate barcodes with the camera. The *Flashlight* icon is at the top left. In case of weak ambient lighting, you can switch on the flashlight by touching the icon.

**Zebra scanner**
If you are using a Zebra scanner, the screen will look as follows:
**(Fig. A-2: Zebra scanner: Scan area)**
The barcode that you use to scan the appropriate barcodes is in the middle.

##### Messages and notices
The following messages and notices apply for both modules:

**Green dot**
A green dot indicates that the booking was transferred successfully to the back end.

**Yellow dot**
A yellow dot indicates a booking in offline mode. This booking has not yet been transferred to the back end.

**Red dot**
A red dot indicates that the booking to the back end failed.

**Gray dot**
A gray dot indicates an outstanding booking for the back end.

##### Messages
In A+W Smart Companion, there are two message types:
- Optical message
- Acoustic message

**Optical message**
After each booking, A+W Smart Companion displays a corresponding notice at the upper edge of the screen. There are two types of these:

- **Green message:** A green message indicates that the booking was made successfully and the data transferred to the back end.
- **Red message:** A red message indicates that the booking was not made successfully and the data was not transferred to the back end. In this case, it is advisable for the employee to contact the administration.

**Acoustic message**
A positive tone sounds if scanning is successful and a negative tone sounds if scanning is unsuccessful.

##### Filter functions
The filter function is always available in A+W Smart Companion. Its purpose is to limit a results list step by step using various criteria. The filter function can be used alphabetically or numerically.

- **Example:** A list of variants can be filtered by searching for text (e.g., "si" filters to "Silver") or numbers (e.g., "16" filters to dimensions like "6000.0 x 1600.0" and "16 mm").

---

## Production

### Revision overview of the module
- **2021-03:** Original version

This module provides information on the following subjects:
- Tutorial

### Tutorial
This section provides information on the following subjects:
- Login
- Menu bar
- Main page of the Production module
- Machine status
- Status page
- Breakage page
- Info page
- Settings

#### Login
In order to reach the module's main page, an employee barcode has to be scanned or entered. This screen appears automatically if you have selected the *Production* module.

**(Fig. B-1: Scan area (smartphone))**
The upper area of the screen is for scanning. There is a blue line in the middle; use it to scan the appropriate barcodes with the camera. The *Flashlight* icon is at the top left. In case of weak ambient lighting, you can switch on the flashlight by touching the icon. Please don't forget to switch the flashlight off again.

**(Fig. B-2: Button for scanning)**
In the middle of the screen, there is a button for scanning the employee barcode. When you have placed the blue line on the barcode in question, touch [Scan]. The barcode is scanned.

**(Fig. B-3: Lower area of the screen)**
The *Employee* icon and the *Back to app selection* function are on the lower part of the screen. With the *Employee* icon, you have the opportunity to enter the employee barcode manually using the keyboard. If you touch the *Back to app selection* function, you return to the *Module selection* screen.

**Here's how to scan the employee barcode**
1. Hold the smartphone with the blue line on the barcode to be scanned. If you are in a dark place when scanning, you can switch on the flashlight by touching the icon. Please remember to switch the flashlight off again.
2. Touch [Scan].
3. The barcode is scanned and you will be on the application's main page.
4. The employee logged in is indicated at the top right of the display (e.g., J. Miller).

**Here's how to enter the employee barcode**
1. Touch the employee button.
2. The *Enter Employee Barcode* screen opens.
3. Touch the *Enter employee ID* field. The numeric keypad opens.
4. Enter the employee ID.
5. Touch [Save]. The screen closes and you are on the application's main page.
6. The employee logged in is indicated at the top right of the display.

#### Menu bar
The menu bar is at the lower edge of the screen in each module. With it, you can switch between the individual functions of A+W Smart Companion.

- **Scan:** Use this function to scan the barcodes in question.
- **Status page:** Messages are issued here that report a rack or truck as empty or delivered.
- **Breakage page:** The breakage bookings are made here.
- **Info page:** You can query information about rack assignments and order status here.
- **Settings page:** The most important settings for the A+W Smart Companion are made here.

#### Main page of the Production module
After you have logged in, you're on the module's main page. At the top of the screen, you will see the modes for scanning. A+W Smart Companion offers two modes:
- **Single:** This is the scan mode for individual barcodes. In this mode, each label must be scanned individually.
- **Continuous:** In this mode, several barcodes can be scanned at the same time. This mode is only allowed for product barcodes. It is activated with the [Scan] button and ended with the [Stop Scan] button.

Beneath this, there is an area for scanning the barcodes, the flashlight, and the button for scanning. You should already be familiar with these elements from the login process.

Then the elements appear that are used to book the normal rack and lite transactions:

**Registration point**
Typical registration points are:
- Trucks
- Storage locations
- Product areas
- Machines or machine parts
The registration of a registration point is mandatory. You can either scan the registration point or enter the barcode manually.

- **How to scan a lite at a registration point:** The registration of a registration point is mandatory.
  1. Hold the smartphone with the blue line on the lite barcode to be scanned.
  2. Touch [Scan].
  3. The registration point scanned appears on the display.

- **Here's how to book a lite to a registration point (manually):**
  1. Touch the [Registration point] element. A page with the same name opens.
  2. From the *Select registration point* combo box, select the appropriate registration point.
  3. From the *Status* combo box, select the appropriate status. Possible values: Maintenance, Set-up, Pause, Breakage. (See Chapter "Machine status" on page B-34)
  4. Touch [Save].
  5. The registration point entered appears on the display.

**Racks**
The registration of a rack is optional! You can either scan the rack or enter the barcode manually.

- **Here's how to scan a rack:**
  1. Hold the smartphone with the blue line on the rack barcode to be scanned.
  2. Touch [Scan].
  3. The rack scanned appears on the display. A green dot indicates the booking was transferred successfully.

- **Here's how to enter the rack barcode:**
  1. Touch the rack button.
  2. A screen opens to enter the rack barcode.
  3. Touch the *Enter rack barcode* field. An alphanumeric keyboard opens.
  4. Enter the rack barcode.
  5. Touch [Save].
  6. The scanned rack appears on the display with a green dot.

**Product**
Typical products are:
- Single lite
- IG
- Spacer
In continuous scan mode, the number of scanned products and a small list symbol are displayed next to the product symbol. If you touch this symbol, a list of the scanned barcodes is displayed.

- **Here's how to scan a product:**
  1. Hold the smartphone with the blue line on the product barcode to be scanned.
  2. Touch [Scan].
  3. The product scanned appears on the display with a green dot.

- **Here's how to enter the product barcode:**
  1. Touch the product button.
  2. The *Product* screen opens.
  3. Touch the *Enter product barcode* field. The numeric keypad opens.
  4. Enter the product barcode.
  5. Touch [Save].
  6. The scanned product appears on the display with a green dot.

- **Here's how to scan a product in continuous scan mode:**
  1. Hold the smartphone with the blue line on the product barcode to be scanned.
  2. Touch [Scan].
  3. Move the blue line over all barcodes to be scanned. Each scanned barcode is signaled by haptic feedback.
  4. Touch [End Scan].
  5. The products scanned appear on the display (e.g., "4 products"). Next to the number, a list symbol appears. Touching this symbol displays a list of the scanned barcodes.

#### Machine status
The machine status can be used to determine the current operating state of a machine (registration point). Depending on the master data, these can be:
- Off
- Maintenance
- Error
- Operation, ...

**Here's how to change the machine status**
1. Touch the *Registration point* element on the main page. A page with the same name opens.
2. Open the *Select status* combo box and select the desired status.
3. Touch [Save]. The page closes and you are back on the main page.

#### Status page
This page is used to book a rack or registration points empty or off-site. For this, you select the appropriate action (the name on the button depends on the master data stored) and scan the barcode of the registration point, the rack or the product. The barcode can also be entered manually by touching the notice text.

There are two buttons in the *Select status* area:
- **Start:** This button starts an empty report of a registration point or a rack.
- **Delivered:** Use this button to book a product, a rack or a registration point as delivered.

This screen may contain the following elements:
- Empty rack
- Full, delivered rack
- Empty truck (registration point)
- Full (delivered) truck (registration point)

> **The actual rack weight was reset**
> This notice appears if a rack weight was present and an empty rack/truck is booked.

**Instructions for use:**
- **Scan an empty rack/truck:** Touch [Start], then scan the barcode.
- **Scan a full (delivered) rack/truck/product:** Touch [Delivered], then scan the barcode.
- **Book an empty rack/truck (manually):** Touch [Start], then touch the "Or enter the barcode manually" notice. Select or enter the item.
- **Book a full (delivered) rack/truck (manually):** Touch [Delivered], then touch the "Or enter the barcode manually" notice. Select or enter the item.

#### Breakage page
Products can be reported broken on this page. The breakage reason is selected first and then the product is scanned. Possible reasons for breakage can be:
- Scratches
- Breakage
- Bottle glass type
- Defective coating
The breakage reasons are defined individually in the database.

**Here's how to scan a break**
1. Open the *Select breakage reason* combo box.
2. Select the appropriate breakage reason.
3. Hold the smartphone with the blue line on the product barcode to be scanned.
4. Touch [Scan].
5. The scanned product appears in the *Scan Product* area.

**Here's how to enter a break (manually)**
1. Open the *Select breakage reason* combo box.
2. Select the appropriate breakage reason.
3. Touch the product element.
4. In the *Enter product barcode* field, enter the appropriate product number.
5. Touch [Save].
6. The scanned product appears in the *Scan* area.

#### Info page
Information about racks or orders can be called up with this page.
The **Information** area contains:
- Rack information
- Order status
- Order location

The **Actions** area contains:
- Registration point status
- Rack shifting
- Actual rack weight
- Rack inventory

##### Rack information
This is where there is information about rack assignment. After you have scanned the rack barcode, an appropriate screen appears.

**(Fig. B-4 Rack information)**
- **Header:** Displays rack number (e.g., Rack 15), status (e.g., Dispatch), weight (e.g., Weighted 237.06 kg), and total lite count (e.g., 47). A red 'x' indicates at least one item is incomplete.
- **Customer Section:** Shows the customer name (e.g., Glas Constructor Unlimited) and the completion status of their items on the rack (e.g., 10/10). A green checkmark indicates all items for that customer are complete.
- **Item Details:** For each customer, it lists the order number, item number, product details, dimensions, and the number of lites on the rack vs. ordered (e.g., 10/5). A red 'x' indicates an incomplete item.

**Here's how to scan rack information**
1. Touch the *Rack information* element.
2. Scan the rack.
3. Touch [Scan].
4. The rack information is displayed.

**Here's how to call up rack information with an entry**
1. Touch the *Rack information* element.
2. Touch the manual entry element.
3. In the *Enter rack barcode* field, enter the rack number.
4. Touch [Save].
5. The rack information is displayed.

##### Order status
Here, you can learn everything about the production progress of an order, its items, and their subparts (BOM). After you have scanned the product barcode, an appropriate screen appears.

**(Fig. B-5 Order status)**
- **Customer:** The customer's name and address are displayed.
- **Delivery date:** The delivery date is displayed.
- **Header parts:** Shows the item number, dimensions, product name, and reference/consignment number.
- **Processing:** This section lists each processing step (e.g., IG-Assembly, Packing, Delivery).
- **Processing machine:** For each step, it shows the machine/location (e.g., IG-Line 1), the completion status (e.g., 8/8 finished), the planned date, and shift.
  - A green checkmark means the step is complete.
  - A red 'X' means production has not started.
  - A yellow dot with a line through it means partial completion.
- **BOM (Bill of Materials):** Touching a processing element can expand it to show the BOM. A blue edge on the left indicates the BOM depth. Each component (Float, Spacer, Laminated glass, etc.) has its own production status.

##### Order location
This screen provides information about where precisely in production the individual parts of an order are located. After scanning the product barcode, a screen appears.

**(Fig. B-6 Order location)**
- The top area shows customer, delivery date, and total number of products in the order.
- The main area lists each item of the order, its quantity, and the location of its parts.
- For each item, it breaks down where the pieces are located (e.g., 10 parts on rack 4711 at Table 1, 5 parts at Seaming, 5 parts at Dispatch).

##### Registration point status
This element is in the *Actions* area. Here, you have the opportunity to set a registration point to a desired status (e.g., Off).

**Here's how to set the status for registration points**
1. Touch the *Registration point status* element.
2. Open the *Select registration point* combo box and select the point.
3. Open the *Select status* combo box and select the desired status.
4. Touch [Save].
5. A confirmation message appears.

##### Rack shifting
This element is in the *Actions* area. Here, you have the opportunity to shift everything that is on a rack to another rack. It is not possible to shift just a partial quantity.

**Here's how to shift the products by scanning**
1. Touch the *Rack shift* element.
2. Scan the barcode of the source rack (the one to be emptied).
3. Scan the barcode of the target rack. A checkmark in a blue dot indicates a successful shift.

**Here's how to shift the products by entering them**
1. Touch the *Rack shift* element.
2. Touch the manual entry element.
3. In the *Enter source barcode* field, enter the source rack barcode and touch [Save].
4. Touch the target element.
5. In the *Enter target barcode* field, enter the target rack barcode. The shift is completed.

##### Actual rack weight
This element is in the *Actions* area. Here you have the opportunity to enter the current weight of a rack.

**Here's how to enter the actual rack weight (scan or manual)**
1. Touch the *Actual rack weight* element.
2. Scan or manually enter the barcode of the rack in question.
3. Enter the weight in the *Enter rack weight (kg)* field.
4. Touch [Save].
5. A confirmation message appears.

##### Rack inventory
This element is in the *Actions* area. You can conduct an inventory for a rack. After scanning the rack, the *Rack inventory* page appears.

**(Fig. B-7 Rack inventory)**
- **Top section:** Shows the rack number, last check date, and next check date. A red triangle with an exclamation point appears if the inspection interval has elapsed.
- **Rack Details:** Displays rack type, weight, max load, and size. You can correct the rack type if needed.
- **Perform Inspection:** Check this box if you have conducted a visual inspection.
- **Number of Labels:** If a barcode is no longer legible, you can enter a number here to print new labels on a defined printer.
- **Save/Print:** Touch [Save] or [Save and Print] to complete the action.

**Here's how to conduct a rack inventory**
1. Touch the *Rack inventory* element.
2. Scan the barcode of the rack. The data is loaded.
3. Check if the rack type is correct. If not, select the correct type.
4. If you have done a visual inspection, check the *Inspection performed* checkbox.
5. If you need new labels, set the desired number in the *Number* field.
6. Touch [Save] or [Save and Print].
7. A confirmation message appears.

#### Settings
The essential settings for A+W Smart Companion are made on this page.

- **Log:** Calls up the online booking log to display the last bookings and their transfer status.
- **Download master data:** Forces the download of PDC master data (people, registration points, breakage reasons) to the device. (Production module only).
- **Language:** Select the display language (English, French, Italian, Spanish, Romanian, Chinese).
- **Adjust configuration:** Sets the device name and the connection to the back end (Service Locator).
- **App selection:** Select the desired application (Production, Stock (A+W Enterprise), Stock (A+W Business)).
- **Information:** Get information (device ID, device name, Service Locator, etc.) about A+W Smart Companion.
- **Help:** Get contact information about A+W Software GmbH.
- **Imperial system:** Switch between metric (mm, kg) and imperial (inches, pounds) units. If imperial is active, a slider appears to adjust reject accuracy (1/8, 1/16, 1/32, 1/64).
- **Hardware mode:** Set whether barcodes should be read with the camera or with a built-in scanner (available for Zebra TC20 Pro scanner).
> **The element is not displayed:** This element is only displayed if the correct setting is entered in the Infrastructure.Web ForeignLicense. The device has to be set there to the DeviceType Mixed or Hardware scanner.
- **Log out:** Logs out the current user and returns to the main page.

---

## Stock

### Revision overview of the module
- **2024-03:** Box warehouse added
- **2023-03:** Actions Reprint and Edit box added
- **2022-03:** Rack inventory added
- **2021-03:** Original version

This module provides information on the following subjects:
- Tutorial

### Tutorial
This section provides information on the following subjects:
- Login
- Menu bar
- Booking goods receipt
- Booking stock movements
- Booking stock withdrawals
- Info page
- Settings

#### Login
In order to reach the module's main page, an employee barcode has to be scanned or entered. This screen appears automatically if you have selected the *Stock* module.

**(Fig. C-1 Area for entry of the employee ID)**
Entering or scanning the employee ID is identical for the Production and Stock modules. The procedure is described in the Production module. (See Production: Login)
After successful log-in, the employee's name appears at the top right.

#### Menu bar
The menu bar is at the lower edge of the screen. With it, you can switch between the individual functions of A+W Smart Companion.
- **Goods receipt:** Use this function to book incoming goods.
- **Stock movement:** Use this function to book goods from one stock to another.
- **Stock withdrawal:** Use this function to book a stock withdrawal.
- **Info page:** In this area, the missing prices are displayed and you can book the inventory.
- **Settings page:** The most important settings are made here.

#### Booking goods receipt
After you have logged in, you are on the *Goods receipt* page. Goods receipt is completely digitalized, both for A+W Enterprise and for A+W Produktion.

**(Fig. C-2 Goods receipt page)**

**Here's how to select the supplier/PO number**
1. Touch the *Supplier/PO number* field. The PO page opens.
2. Touch the desired PO. The PO number is loaded.
3. In the *External Supplier Number* field, you can enter the supplier's number on the delivery note.
4. Select the appropriate date from the *Date Received* field.
5. To display the individual items of the PO, touch the blue [Display items] bar.

**(Fig. C-3 Overview of the items of a PO)**

**Explanation of the elements**
The top area displays supplier, PO number, consignment, and delivery dates. Then the individual items of the PO are listed.

- **PO Type:** Icons indicate the type of Purchase Order:
  - **Production order:** Goods are for production. Informs A+W Produktion.
  - **Stock order:** Goods for general stock (glass, hardware, etc.).
  - **Stock order (with missing price):** A warning that the price is not yet stored in A+W Enterprise.
  - **Box stock order:** A PO for a box stock.
> **Book boxes only completely**
> Goods receipts for boxes can only be booked completely. The box quantity delivered must match the box quantity ordered.

- **Item Data:** Includes dimensions, variant, and storage location.
- **Delivered quantity:** A gray number is the ordered quantity. A blue number means delivered quantity matches ordered. A red number indicates an over- or underbooking.
- **Tag item:** A colored bar at the start of the line can be toggled from gray to blue by swiping or tapping a checkbox to mark items.

**Here's how to book a delivered quantity**
1. In the appropriate item, touch the oval displaying the quantity.
2. An area opens to change the quantity. Enter the desired quantity.
3. Touch [Confirm].
4. The area is closed and you are back in the overview.

##### Override stock location
If you swipe on an item from right to left, the *Storage location* page opens. You can select a new storage location from a combo box. Activate the *Apply Location to All* checkbox to book all items to this location.

##### Assign registration point
This function is only active if the goods are for a production order. If you swipe in this area from right to left, the *Location* page opens, where you can select a registration point and/or enter a rack barcode.

**Saving:** To save your inputs, click the checkmark at the right bottom edge of the display.
If there are quantity differences, a notice appears:
- Missing items are delivered later
- Missing items are not delivered later
Select the desired option and then touch [Send]. A successful booking is indicated with the notice: "Receipt of goods successfully booked".

#### Booking stock movements
With this function, you can book goods from one stock to another one.

> **Scanning stock articles**
> If an EAN barcode has been stored in A+W Enterprise for the article, you can also scan the article in question.

**Here's how to re-book articles**
1. On the first page, touch the *Storage location* combo box and select the source location.
2. From the *Stock articles* combo box, select the article to move.
3. From the *Variant* combo box, select the variant.
4. In the *Quantity that should be moved* field, specify the quantity.
5. Select the *Target storage location* from the combo box.
6. Touch the checkmark to save. A successful shift is indicated with the notice: "Stock movement successfully booked".

#### Booking stock withdrawals
With this function, you can remove goods from a stock. There are two kinds of stock withdrawals:
- With order
- Without order

##### Stock withdrawal with order
If the stock withdrawal is done with reference to an order, all information about this order is available.
- The *Orders* combo box includes all orders created in A+W Enterprise. Select an order or scan the order number.
- Touch [Display items] to see a detailed overview of the order.
- The overview lists each item with its dimensions, storage location, variant, packaging, and supplier.
- The quantity area shows ordered vs. removed quantity (e.g., 360/360 Pcs).
> **Removing a box article**
> For box articles, the content of the boxes is also displayed. To remove, you must swipe left or touch the quantity to open a new page where you scan the specific boxes being removed.

**Here's how to withdraw goods with reference to an order**
1. Select the order from the *Orders* combo box.
2. Touch [Display items].
3. Remove the desired items from the storage location. Correct the quantity if necessary.
4. Touch the blue dot with the white checkmark to save.
5. A successful removal is indicated with the notice: "Stock withdrawal (order) successfully booked".

##### Stock withdrawal without order
For a stock withdrawal without reference to an order, you have to specify the storage location, article, and quantity.
- If you try to remove a quantity larger than what is on hand, the field is outlined in red and the Save element is deactivated.

**Here's how to withdraw goods without reference to an order**
1. Use the *Storage location* combo box to indicate the source location.
2. From the *Stock articles* combo box, select the article to remove.
3. If applicable, select the variant from the *Variants* combo box.
4. In the *Quantity that should be removed* field, specify the quantity.
5. Touch the blue dot with the white checkmark to save.
6. A successful removal is indicated.

#### Info page
This view includes the following areas:
- **Information:** Missing prices
- **Actions:** Inventory, Editing a box, Print again

##### Missing prices
Here the articles are listed for which the price still has to be maintained in A+W Enterprise. The employees in the warehouse have no access to the prices here. In case of missing prices, the employees in the warehouse should make contact with the appropriate employee in administration.

##### Inventory
This is where you take inventory.
> **Inventory as independent action**
> The Inventory action is licensed separately and is not coupled to the Stock module. Stock is not blocked during inventory.

The inventory is done on the stock location level and is started in A+W Enterprise. After counting, the data from A+W Smart Companion is compared to the data in A+W Enterprise.

In the Inventory area, a distinction is made between two locations:
- Box stock
- Warehouse

###### Inventory of a box stock
If you are working at a company with one or several box stocks, you can simply scan the box(es) in question for the inventory.
1. Select the appropriate box stock from the *Inventory stock* combo box.
2. Touch [Start].
3. You can now scan the box barcode or enter it via the keyboard.
4. Scanned boxes will be displayed in a list with a status symbol:
    - **Checkmark:** The box was scanned successfully.
    - **!:** An error occurred during scanning.
    - **Yellow warning:** This box was scanned twice.

> **Scanning boxes**
> When you scan the boxes during an inventory, as many boxes as you wish can be scanned. The scanned boxes are added to the inventory after scanning.

###### Inventory of a warehouse
The inventory of a warehouse requires more inputs (article name, variant, etc.).

**Here's how to count inventory**
1. Open the *Inventory stock* combo box and select a stock.
2. Select the article to count in the *Article name* field.
3. Select the variant from the *Variants* field. Entries that have a green checkmark have already been counted.
4. Touch the *Quantity* field and enter the quantity counted.
5. Touch the blue dot with the white checkmark to save. A notice "Stock inventory count successfully stored" appears.

**Add quantity to a quantity already counted**
If you select an article/variant that has already been counted, a new area appears.
- It shows who last counted it and when.
- In the *Quantity that should be added* field, enter the new quantity.
- Use the `+` icon to add to the existing count or the `arrows` icon to replace the existing count.

###### Checklist
The checklist provides an overview of all articles counted and not counted. There are two views available: List view and Chart view.
- **Slider:** A slider at the top allows you to filter for "Articles without inventory".
- **List View Symbols:**
  - **Gray exclamation point:** Article not yet counted. The numbers on the right show variants counted vs. total variants (e.g., 3/0).
  - **Green arrow:** Article counted completely (e.g., 4/4).
  - **Partial blue circle:** Counting has started but is not complete (e.g., 2/1).
- **Chart View:** Displays the inventory progress as a percentage and a donut chart showing the overall status (Completed, Not started, Partial).
> **From the checklist directly into the inventory counting**
> If you touch an entry in the checklist, you jump directly to the inventory counting for the article in question.

##### Editing a box
Here you have the opportunity to change the contents of a box. You can remove selected lites or break up the entire box.
1. After touching the *Edit Box* element, scan or manually enter the box label.
2. A page appears showing the box contents (article, pieces in box).
3. Enter the number of *Pieces to Move*.
4. Specify the reason: *Breakage* or *Storage location*.
    - If **Breakage**, select a reason from the *Reason* combo box (e.g., Miscounted, Cut size) and add optional remarks.
    - If **Storage location**, select a new *Stock Location* from the combo box.
5. Touch the blue circle with the white checkmark to confirm.

**Here's how to remove an article from the box (e.g., in case it is broken)**
1. Select the *Edit box* action.
2. Scan or enter the box barcode.
3. In the *Pieces to move* field, enter the quantity to remove.
4. Enable the *Reason for removal* radio button and select the appropriate reason.
5. Touch the checkmark to save.

**Here's how to book an article out of the box to another storage location**
1. Select the *Edit box* action.
2. Scan or enter the box barcode.
3. In the *Pieces to move* field, enter the quantity to move.
4. Enable the *Storage location* radio button and select the target location.
5. Touch the checkmark to save.

##### Print again
Here you have the opportunity to reprint labels for boxes. If a box label is no longer legible, you can reprint it here on the defined printer.
1. Touch the *Reprint* element.
2. In the *Supplier/PO number* area, select the box PO in question.
3. Touch [Display items] to show all items for the selected PO.
4. The view shows each box and its contents. Touch the checkbox for the box(es) whose labels should be reprinted.
5. The Print icon is enabled, showing the number of labels to be printed.
6. Touch the Print icon to start printing.

> **Reprinting label for complete box**
> In the view, the box symbol is on the right side. To reprint labels for complete boxes, touch this symbol and then enter or scan the box number.

**Here's how to print the new label**
1. Touch the *Supplier/PO number* field.
2. Select the appropriate PO.
3. Touch [Display items].
4. Select the appropriate item(s).
5. Touch [Print].

#### Settings
The Settings are identical for the Production and Stock modules. To avoid redundant explanations, this process is described in connection with the Production module.
(See Produktion: Tutorial, "Settings" on page B-57)
