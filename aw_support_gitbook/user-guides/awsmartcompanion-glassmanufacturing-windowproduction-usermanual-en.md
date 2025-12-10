---
title: "EN-UM-AW-SmartCompanion-AWB"
source: "EN-UM-AW-SmartCompanion-AWB.pdf"
tags: ["A+W Smart Companion", "Software Manual", "Glass Manufacturing", "Window Production", "Door Manufacturing", "ERP", "Production Management", "Stock Management", "Barcode Scanning", "Inventory"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This is the official user manual for A+W Smart Companion, a mobile application designed for plant data collection in the glass, windows, and doors industry. It details the functionalities of the Production and Stock modules."
long_description: "The A+W Smart Companion Manual provides comprehensive instructions for end-users on how to operate the mobile application for plant data collection. The manual is divided into three main sections: Overview, Production, and Stock. The Overview section introduces the software, its different license modules (Basic, Production, Stock), and general operating principles, including hardware modes (smartphone, Zebra scanner), messages, and filter functions. The Production module section offers a detailed tutorial on logging in, navigating the user interface, scanning barcodes for various operations like tracking machine status, reporting breakages, and retrieving information on racks, orders, and registration points. The Stock module section guides users through managing inventory, including booking goods receipts, handling stock movements and withdrawals (both with and without order reference), performing inventories, and editing box contents. The manual is designed for customers who use the A+W software suite (A+W Business, A+W Enterprise, A+W Produktion) and assumes basic knowledge of smartphone operation. It aims to facilitate a completely digital, paperless workflow for production and stock management tasks."
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
| > | shows the way to open a dialog, e.g. *Display* > *Filler orders* > *Context menu - List* > *Order overview*. |
| [] | square brackets mark the buttons in the dialog, e. g. **[OK]** to save the data. |
| < > | pointed brackets refer to keys or shortcuts on the keyboard, e. g. **<F1>** is used to open the online help. |

### Contact

**A+W Software GmbH**
Siemensstr. 3
D-35463 Fernwald
Germany

- **Tel.:** +49 641 96620 0
- **E-Mail:** info@a-w.com
- **Web:** http://www.a-w.com

## A: Overview

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

The Production module provides all booking functionalities that you need in the A+W Produktion main module. Reasons for breakage or status messages for racks and trucks can be selected directly from a menu. Therefore, no additional bar code tables are required. Furthermore, you can display the content of a rack, the production status or the location of individual items of an order in production directly on the mobile end user device.

##### A+W Smart Companion – Stock

The Stock module supports A+W Software stock management in a mobile application. Simple, completely digital, and paperless delivery of POs (also with direct production parts), stock transactions, and stock removals.

It is currently integrated with the A+W Enterprise A+W Business modules Purchase Order and Stock.

The Inventory module of the A+W Smart Companion is already integrated into the Stock module.

> **License**
> As with other scanners (Denso, WinCE, etc.), each device with the A+W Smart Companion requires a database license!

#### Operation

In principle, the A+W Smart Companion can be operated very intuitively. Nevertheless, the individual operating and display elements will be explained in the following sections. A+W Smart Companion can be operated using the scan function or using manual inputs. The appropriate steps will be explained below.

##### Module selection

After starting and authentication of A+W Smart Companion, select the desired module.

| Icon | Module |
| :--- | :--- |
| (Wrench Icon) | Production |
| (Warehouse Icon) | Stock |

*A+W Smart Companion* saves the last selected application and automatically selects it after a restart.

The module can be changed in App selection at any time. (See Production: Tutorial, "App selection" on page B-58)

Currently, the Production and Stock modules are supported – additional modules are still under construction.

##### Hardware mode

A+W Smart Companion can be used with the following mobile end user devices:
- Smartphone
- Zebra scanner

Depending on the end user device used, the scan area may look as follows:

###### Smartphone

*Fig. A-1: Smartphone: Scan area*

There is a blue line in the middle; use it to scan the appropriate barcodes with the camera. The **Flashlight** icon is at the top left. In case of weak ambient lighting, you can switch on the flashlight by touching the icon.

###### Zebra scanner

If you are using a Zebra scanner, the screen will look as follows:

*Fig. A-2: Zebra scanner: Scan area*

The barcode that you use to scan the appropriate barcodes is in the middle.

#### Messages and notices

The following messages and notices apply for both modules:

- **Green dot**: The green dot indicates that the booking was transferred successfully to the back end.
- **Yellow dot**: The yellow dot indicates a booking in offline mode. This booking has not yet been transferred to the back end.
- **Red dot**: The red dot indicates that the booking to the back end failed.
- **Gray dot**: The gray dot indicates an outstanding booking for the back end.

#### Messages

In A+W Smart Companion, there are two message types:
- Optical message
- Acoustic message

##### Optical message

After each booking, A+W Smart Companion displays a corresponding notice at the upper edge of the screen. There are two types of these:

- **Green message**: A green message indicates that the booking was made successfully and the data transferred to the back end.
- **Red message**: A red message indicates that the booking was not made successfully and the data was not transferred to the back end. In this case, it is advisable for the employee to contact the administration.

##### Acoustic message

A positive tone sounds if scanning is successful and a negative tone sounds if scanning is unsuccessful. A recent update added acoustic notifications.

#### Filter functions

The filter function is always available in A+W Smart Companion. Its purpose is to limit a results list step by step using various criteria. The filter function can be used alphabetically or numerically.

**Example:**

*Fig. A-3: Total hit quantity*
The list shows various filterable variants like dimensions (e.g., 6000.0 x 1600.0) and attributes (e.g., White, Blue, 10 mm).

**Alphabetical search:**

*Fig. A-4: Alphabetical hit quantity*
Searching for "si" filters the list to show "Silver".

**Numeric search:**

*Fig. A-5: Numeric hit quantity*
Searching for "16" filters the list to show items with "1600.0" and "16 mm".

## B: Production

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

In order to reach the module's main page, an employee barcode has to be scanned or entered. This screen appears automatically if you have selected the Production module.

*Fig. B-1: Scan area (smartphone)*
The upper area of the screen is for scanning. There is a blue line in the middle; use it to scan the appropriate barcodes with the camera. The **Flashlight** icon is at the top left. In case of weak ambient lighting, you can switch on the flashlight by touching the icon. Please don't forget to switch the flashlight off again.

*Fig. B-2: Button for scanning*
In the middle of the screen, there is a button for scanning the employee barcode. When you have placed the blue line on the barcode in question, touch **[Scan]**. The barcode is scanned.

*Fig. B-3: Lower area of the screen*
The **Employee** icon and the **Back to app selection** function are on the lower part of the screen. With the **Employee** icon, you have the opportunity to enter the employee barcode manually using the keyboard. If you touch the **Back to app selection** function, you return to the Module selection screen.

**Here's how to scan the employee barcode**
1. Hold the smartphone with the blue line on the barcode to be scanned. If you are in a dark place when scanning, you can switch on the flashlight by touching the icon. Please remember to switch the flashlight off again.
2. Touch **[Scan]**.
3. The barcode is scanned and you will be on the application's main page.
4. The employee logged in is indicated at the top right of the display (e.g., J. Miller).

**Here's how to enter the employee barcode**
1. Touch the **Employee** button.
2. The *Enter Employee Barcode* screen opens.
3. Touch the **Enter employee ID** field. The numeric keypad opens.
4. Enter the employee ID.
5. Touch **[Save]**. The screen closes and you are on the application's main page.
6. The employee logged in is indicated at the top right of the display.

#### Menu bar

The menu bar is at the lower edge of the screen in each module. With it, you can switch between the individual functions of A+W Smart Companion.

- **Scan**: (Scan icon) Use this function to scan the barcodes in question.
- **Status page**: (Rack status icon) Messages are issued here that report a rack or truck as empty or delivered.
- **Breakage page**: (Broken lite icon) The breakage bookings are made here.
- **Info page**: (Magnifying glass icon) You can query information about rack assignments and order status here.
- **Settings page**: (Gear icon) The most important settings for the A+W Smart Companion are made here.

#### Main page of the Production module

After you have logged in, you're on the module's main page. At the top of the screen, you will see the modes for scanning. A+W Smart Companion offers two modes:
- **Single**: This is the scan mode for individual barcodes. In this mode, each label must be scanned individually.
- **Continuous**: In this mode, several barcodes can be scanned at the same time. This mode is only allowed for product barcodes. It is activated with the **[Scan]** button and ended with the **[Stop Scan]** button.

Beneath this, there is an area for scanning the barcodes, the flashlight, and the button for scanning.

Then the elements appear that are used to book the normal rack and lite transactions:

**Registration point**
(Registration point icon)
Typical registration points are:
- Trucks
- Storage locations
- Product areas
- Machines or machine parts
The registration of a registration point is mandatory. You can either scan the registration point or enter the barcode manually.

**How to scan a lite at a registration point**
1. Hold the smartphone with the blue line on the lite barcode to be scanned.
2. Touch **[Scan]**.
3. The registration point scanned appears on the display (e.g., Seaming 400000310).

**Here's how to book a lite to a registration point (manually)**
1. Touch the **[Registration point]** element. A page with the same name opens.
2. From the *Select registration point* combo box, select the appropriate registration point.
3. From the *Status* combo box, select the appropriate status (e.g., Maintenance, Set-up, Pause, Breakage).
4. Touch **[Save]**.
5. The registration point entered appears on the display.

**Racks**
(Rack icon)
The registration of a rack is optional! You can either scan the rack or enter the barcode manually.

**Here's how to scan a rack**
1. Hold the smartphone with the blue line on the rack barcode to be scanned.
2. Touch **[Scan]**.
3. The rack scanned appears on the display (e.g., 300000001). A green dot indicates a successful booking.

**Here's how to enter the rack barcode**
1. Touch the rack icon button.
2. The *Rack* screen opens.
3. Touch the **Enter rack barcode** field. An alphanumeric keyboard opens.
4. Enter the rack barcode.
5. Touch **[Save]**.
6. The scanned rack appears on the display.

**Product**
(Product icon)
Typical products are:
- Single lite
- IG
- Spacer

In continuous scan mode, the number of scanned products and a small list symbol are displayed next to the product symbol. If you touch this symbol, a list of the scanned barcodes is displayed.

**Here's how to scan a product**
1. Hold the smartphone with the blue line on the product barcode to be scanned.
2. Touch **[Scan]**.
3. The product scanned appears on the display (e.g., Product 000000360). A green dot indicates a successful booking.

**Here's how to enter the product barcode**
1. Touch the product icon button.
2. The *Product* screen opens.
3. Touch the **Enter product barcode** field. The numeric keypad opens.
4. Enter the product barcode.
5. Touch **[Save]**.
6. The scanned product appears on the display.

**Here's how to scan a product in continuous scan mode**
1. Hold the smartphone with the blue line on the product barcode to be scanned.
2. Touch **[Scan]**.
3. Move the blue line over all barcodes to be scanned. Each scanned barcode is signaled by haptic feedback.
4. Touch **[End Scan]**.
5. The products scanned appear on the display (e.g., "3 products"). Next to the number of scanned products, you will see a small list symbol. If you touch this symbol, a list of the scanned barcodes is displayed.

#### Machine status

The machine status can be used to determine the current operating state of a machine (registration point). Depending on the master data, these can be: Off, Maintenance, Error, Operation, etc.

*Image: Registration Point screen showing selection for Status (e.g., Break).*

**Here's how to change the machine status**
1. Touch the **Registration point** element on the main page. A page with the same name opens.
2. Open the *Select status* combo box and select the desired status.
3. Touch **[Save]**. The page closes and you are back on the main page.

#### Status page

This page is used to book a rack or registration points empty or off-site. For this, you select the appropriate action and scan the barcode of the registration point, the rack or the product. The barcode can also be entered manually.

*Image: Status page showing **[Start]** and **[Delivered]** buttons and a scanned truck.*

There are two buttons in the *Select status* area:
- **Start**: This button starts an empty report of a registration point or a rack.
- **Delivered**: Use this button to book a product, a rack or a registration point as delivered.

This screen may contain the following elements:
- Empty rack (icon)
- Full, delivered rack (icon)
- Empty truck (registration point) (icon)
- Full (delivered) truck (registration point) (icon)

**Here's how to scan an empty rack**
1. Touch **[Start]**. The button turns blue.
2. Scan the barcode of the rack in question.
3. The scanned rack appears in the area *2 Scan* in the form of an empty rack.
4. The notice *The actual rack weight was reset* appears at the top of the screen.
> This notice only appears if a rack weight was present.

**Here's how to scan a full (delivered) rack**
1. Touch **[Delivered]**. The button turns blue.
2. Scan the barcode of the rack in question.
3. The scanned rack appears in the area *2 Scan* in the form of a full rack.

**Here's how to scan a delivered product**
1. Touch **[Delivered]**. The button turns blue.
2. Scan the barcode of the product in question.
3. The scanned product appears in the area *2 Scan* with an appropriate icon.

**Here's how to book an empty rack (manually)**
1. Touch **[Start]**.
2. In the area *2 Scan*, touch the notice *Or enter the barcode manually*.
3. The *Assign status* screen opens.
4. In the *Enter rack barcode* field, enter the appropriate barcode.
5. Touch **[Save]**.
6. The rack entered appears in the area *2 Scan* in the form of a full rack.
7. The notice *The actual rack weight was reset* appears.
> This notice only appears if a rack weight was present.

**Here's how to book a rack in a full (delivered) status (manually)**
1. Touch **[Delivered]**.
2. In the area *2 Scan*, touch the notice *Or enter the barcode manually*.
3. The *Assign status* screen opens. Touch the full rack.
4. In the *Enter rack barcode* field, enter the appropriate barcode.
5. Touch **[Save]**.
6. The rack entered appears in the area *2 Scan* in the form of a full rack.

**Here's how to scan an empty truck**
1. Touch **[Start]**.
2. Scan the barcode of the truck in question.
3. The scanned truck appears in the area *2 Scan* with an empty cargo area.

**Here's how to scan a full (delivered) truck**
1. Touch **[Delivered]**.
2. Scan the barcode of the truck in question.
3. The scanned truck appears in the area *2 Scan* with a full cargo area.

**Here's how to book an empty truck (manually)**
1. Touch **[Start]**.
2. In the area *2 Scan*, touch the notice *Or enter the barcode manually*.
3. The *Assign status* screen opens.
4. Open the *Select truck* combo box.
5. Select the desired truck.
6. Touch **[Save]**.
7. The selected truck appears in the area *2 Scan* with an empty cargo area.

**Here's how to book a truck in a full (delivered) status (manually)**
1. Touch **[Delivered]**.
2. In the area *2 Scan*, touch the notice *Or enter the barcode manually*.
3. The *Assign status* screen opens.
4. Open the *Select truck* combo box.
5. Select the desired truck.
6. Touch **[Save]**.
7. The selected truck appears in the area *2 Scan* with a full cargo area.

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
4. Touch **[Scan]**.
5. The scanned product appears in the area *2 Scan* with the reason (e.g., Scratch).

**Here's how to enter a break (manually)**
1. Open the *Select breakage reason* combo box.
2. Select the appropriate breakage reason.
3. Touch the manual entry element.
4. In the *Enter product barcode* field, enter the appropriate product number.
5. Touch **[Save]**.
6. The scanned product appears in the area *2 Scan*.

#### Info page

Information about racks or orders can be called up with this page. The page is divided into two areas: *Information* and *Actions*.

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

*Fig. B-4: Rack information screen*
This screen displays detailed information about a specific rack, including its status, weight, and the contents organized by customer order.

**Explanation of the elements**
- **Header**: Shows the rack number (e.g., Rack 15), status (e.g., Dispatch), weight, and total number of lites. A red 'x' indicates at least one item is incomplete.
- **Customer Section**: Shows the customer name (e.g., Glas Constructor Unlimited) and the completion status of their items on the rack (e.g., 10/10). A green checkmark indicates a complete item.
- **Item Details**: Below each customer, it lists the order number, item number, dimensions, and completion status. A red 'x' indicates an incomplete item.

**Here's how to scan rack information**
1. Touch the **Rack Information** element.
2. Scan the rack for which the information should be displayed.
3. Touch **[Scan]**.
4. The rack information is displayed.

**Here's how to call up rack information with an entry**
1. Touch the **Rack Information** element.
2. Touch the manual entry element.
3. In the *Enter rack barcode* field, enter the appropriate rack number.
4. Touch **[Save]**.
5. The rack information is displayed.

##### Order status

Here you can learn everything about the production progress of an order, its items, and their subparts. After you have scanned the product barcode, an appropriate screen appears.

*Fig. B-5: Order status screen*
This screen shows the customer, delivery date, and a list of items. For each item, it details the processing steps, the machine/location, the planned date/shift, and the completion status (e.g., 8/8, 25/12).

**Explanation of the elements**
- **Customer (Cust)**: Displays the customer's name and address.
- **Delivery date**: Displays the scheduled delivery date.
- **Header parts**: Displays the item number, dimensions, product name, and customer consignment.
- **Processing**: Shows the current processing step.
- **Processing machine**: Shows the machine for the current step.
- **Completion Status**:
    - **Green checkmark**: The production step is complete (e.g., 8/8).
    - **Yellow line-through**: Part of the quantity has been processed (e.g., 12 of 25 pieces are finished).
    - **Red X**: Production has not yet been started.
- **BOM View**: Touching an item can expand it to show the Bill of Materials (BOM), displaying the production progress of individual parts. The blue edge on the left represents the depth of the BOM.

**BOM Element Icons**
- **Float**: Represents a float glass.
- **TG**: Represents tempered glass.
- **Spacer**: Represents a spacer.
- **Grill**: Represents a muntin.
- **IG**: Represents an IG with muntins.
- **Laminated glass**: Represents a LAMI.
- **Foil**: Represents a foil.
- **IG with step**: Represents an IG with a step.
- **LAMI with step**: Represents a LAMI with a step.
- **Patterned glass**: Represents patterned glass.
- **Fire protection glass**: Represents fire protection glass.

Touching one of these elements displays the associated processing and registration point.

##### Order location

This screen provides information about where precisely in production the individual parts of an order are located. After you have scanned the product barcode, an appropriate screen appears.

*Fig. B-6: Order location screen*
This screen shows the customer, delivery date, and a list of items. For each item, it shows the registration point (e.g., Table 1), rack number, and the number of parts at that location.

**Explanation of the elements**
- **Top Area**: Shows customer and delivery date.
- **Item Header**: Shows item number, dimensions, product name, and total order quantity.
- **Location Details**: For each item, it lists the registration point, rack number, and quantity of parts on that rack.

##### Registration point status

This element is in the *Actions* area. Here, you can set a registration point to a desired status (e.g., Off).

**Here's how to set the status for registration points**
1. Touch the **Registration Point Status** element.
2. Open the *Select registration point* combo box and select the point.
3. Open the *Select status* combo box and select the status.
4. Touch **[Save]**.
5. A confirmation message appears: *The registration point was saved*.

##### Rack shifting

This element is in the *Actions* area. It allows you to shift all products from one rack to another. It is not possible to shift a partial quantity.

**Here's how to shift the products by scanning**
1. Touch the **Rack Shifting** element. The *Rack shift* page opens.
2. Scan the barcode of the source rack. The rack number, name, and quantity are displayed.
3. Scan the barcode of the target rack. Its details are displayed. A blue checkmark indicates the shift was successful.

**Here's how to shift the products by entering them**
1. Touch the **Rack Shifting** element.
2. Touch the manual entry element for the source rack.
3. In the *Enter source barcode* field, enter the barcode.
4. Touch **[Save]**. The source rack details appear.
5. Touch the manual entry element for the target rack.
6. In the *Enter target barcode* field, enter the barcode. The shift completes successfully.

##### Actual rack weight

This element is in the *Actions* area. You can enter the current weight of a rack.

**Here's how to scan in the actual rack weight**
1. Touch the **Actual rack weight** element.
2. Scan the barcode of the rack.
3. Enter the weight in the *Enter rack weight (kg)* field.
4. Touch **[Save]**.
5. A confirmation message appears: *The actual rack weight was booked successfully*.

**Here's how to scan in the actual rack weight (manually)**
1. Touch the **Actual rack weight** element.
2. Touch the manual entry element.
3. In the *Enter rack barcode* field, enter the barcode.
4. Enter the weight in the *Enter rack weight (kg)* field.
5. Touch **[Save]**.
6. A confirmation message appears.

##### Rack inventory

This element is in the *Actions* area. You can conduct an inventory for a corresponding rack. After scanning a rack, the *Rack Inventory* page appears.

*Fig. B-7: Rack inventory screen*

**Top section**
Shows the rack number and inspection data (Last Check, Next Check). A red triangle with an exclamation point appears if the inspection interval has elapsed.

**Rack Details**
- **Rack Types**: Select the correct rack type.
- **Details**: Displays rack weight, maximum load, and size.
- **Perform Inspection**: Check this box after a visual inspection.
- **Number of Labels**: Specify how many new labels to print if the barcode is no longer legible.
- **Button**: Can be **[Print]** or **[Save and Print]**.

**Here's how to conduct a rack inventory**
1. Touch the **Rack inventory** element.
2. Scan the barcode of the rack. The data is loaded.
3. Check if the rack type is correct and adjust if necessary.
4. If you performed a visual inspection, check the *Inspection performed* checkbox.
5. If you need new labels, enter the quantity in the *Number of Labels* field.
6. Touch **[Save]** or **[Save and Print]**.
7. A confirmation message appears.

#### Settings

The essential settings for A+W Smart Companion are made on this page.

**Explanation of the elements**
- **Log**: Call up the online booking log to see the last bookings and their transfer status.
- **Download master data**: Force the download of PDC master data (people, registration points, breakage reasons) onto the device. (Production module only).
- **Language**: Select the display language (English, French, Italian, Spanish, Romanian, Chinese).
- **Adjust configuration**: Set the device name and the connection to the back end (Service Locator).
- **App selection**: Select the desired application module (Production, Stock).
- **Information (i)**: Get information about the device ID, name, Service Locator, etc.
- **Help (?)**: Get contact information for A+W Software GmbH.
- **Imperial system**: Switch between metric (mm, kg) and imperial (inches, pounds) units. If imperial is active, a slider appears to adjust reject accuracy (1/8, 1/16, 1/32, 1/64).
- **Hardware mode**: Set whether barcodes should be read with the camera or a built-in scanner (available for Zebra TC20 Pro scanner).
> This element is only displayed if correctly configured in *Infrastructure.Web ForeignLicense*.
- **Log out**: Log out the current user and return to the main page.

## C: Stock

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

In order to reach the module's main page, an employee barcode has to be scanned or entered. This screen appears automatically if you have selected the Stock module.

*Fig. C-1: Area for entry of the employee ID*

Entering or scanning the employee ID is identical for the Production and Stock modules. The procedure is described in the Production module section. After successful log-in, the employee's name appears at the top right.

#### Menu bar

The menu bar is at the lower edge of the screen. With it, you can switch between the individual functions of A+W Smart Companion.

- **Goods receipt** (Warehouse icon with arrow in): Use this function to book incoming goods.
- **Stock movement** (Arrows icon): Use this function to book goods from one stock to another.
- **Stock withdrawal** (Warehouse icon with arrow out): Use this function to book a stock withdrawal.
- **Info page** (Magnifying glass icon): In this area, missing prices are displayed and you can book the inventory.
- **Settings page** (Gear icon): The most important settings for the A+W Smart Companion are made here.

#### Booking goods receipt

After you have logged in, you are on the *Goods receipt* page. Goods receipt is completely digitalized, both for A+W Business and for A+W Production.

*Fig. C-2: Goods receipt page*

**Here's how to select the supplier/PO number**
1. Touch the *Supplier/PO number* field. The PO page opens.
2. Touch the desired PO. The PO number is loaded. (You can also enter it via keyboard).
3. In the *External Supplier Number* field, you can enter the supplier's number from the delivery note.
4. Select the appropriate date from the *Date Received* field.
5. To display the individual items of the PO, touch the blue **[Display items]** bar.

*Fig. C-3: Overview of the items of a PO*

**Explanation of the elements**
The top area displays the PO number, supplier name, consignment number, and customer reference number. It also shows the announced delivery date (calendar icon) and actual delivery date (truck icon).

The individual items of the PO are then listed.

**PO Type Elements**
- **Production order** (Icon): A PO for a production order. Informs A+W Production and allows for optional label printing.
- **Stock order** (Icon): A PO for a stock order in A+W Business (e.g., glass stock, hardware stock).
- **Box order** (Icon): A PO for a box.
> **Display supplier data**: The supplier's article number and name can only be displayed if they are maintained appropriately in A+W Business.

**Item Data**
This area shows the item number, dimensions, variant, and storage location.

**Delivered quantity**
This element (e.g., 200 / 125) represents the ordered (gray) and delivered quantities.
- A **blue** number indicates the delivered quantity matches the ordered quantity.
- A **red** number indicates an over- or under-booking.

**Here's how to book a delivered quantity**
1. In the appropriate item, touch the oval.
2. An area opens to change the quantity. You can swipe up/down or use *Manual entry*.
3. Enter the desired quantity.
4. Touch **[Confirm]**.
5. You are back in the overview.

**Tag item**
A colored bar at the beginning of the line can be gray or blue. Swiping the item from left to right reveals a checkbox. Ticking it turns the bar blue, marking the item.
> **Marking by swiping**: The item marks itself if you swipe far enough with your finger from left to right.

**Override stock location**
If you swipe on an item from right to left, the *Storage location* page opens. Here you can select a new storage location from a combo box. You can also check "Apply Location to All" to book all items to this location.

**Override box stock**
For a box item, the Box ID is displayed. If you swipe from right to left, the box editor opens. You can touch a specific box to edit its details like Supplier ID, Stock Locations, Pieces in Box, and Remarks.

**Assign registration point**
This function is only active for production order goods. Swiping right to left opens the *Location* page where you can assign a registration point (and optionally a rack barcode). You can apply this location to all items.

**Finalizing the Booking**
- Click the blue checkmark at the bottom right to save.
- If there are quantity differences, a notice appears:
    - *Missing items are delivered later*
    - *Missing items are not delivered later*
- Select an option and touch **[Send]**.
- A successful booking is indicated by the notice: *Receipt of goods successfully booked*.

#### Booking stock movements

With this function, you can book goods from one stock to another. A storage location in A+W Business can consist of up to four levels:
- Level 1: e.g., warehouses
- Level 2: e.g., aisles
- Level 3: e.g., racks
- Level 4: e.g., slots

> **Scanning stock articles**: If an EAN barcode is stored in A+W Business, you can scan the article.

**Here's how to re-book articles**
1. On the first page, touch the *Storage location* combo box.
2. Select the storage location from which the article should be removed.
3. From the *Stock articles* combo box, select the article to move.
4. From the *Variant* combo box, select the variant.
5. In the *Quantity that should be moved* field, specify the quantity.
6. Select the *Target storage location* from the combo box.
7. Touch the white checkmark to save.
A successful shift is indicated by the notice: *Stock movement successfully booked*.

#### Booking stock withdrawals

With this function, you can remove goods from a stock. There are two kinds:
- With order
- Without order

##### Stock withdrawal with order

If done with reference to an order, all information is available in A+W Smart Companion.
The *Orders* combo box includes all orders from A+W Business. Select an order or scan the order number, then touch **[Display items]**.

An overview appears showing the customer, delivery date, and a list of items with their dimensions, storage location, variant, packaging, and supplier. You can use the swipe function (left to right) to mark individual items.

> **Removing a box article**: For box articles, the content is displayed (e.g., 2 boxes with 20 pieces each). The quantity is initially 0. Swiping left opens a page to scan the specific boxes being removed.

**Here's how to withdraw goods with reference to an order**
1. Select the order from the *Orders* combo box.
2. Touch **[Display items]**.
3. Remove the desired items from the storage location. Correct the quantity if necessary.
4. Touch the blue dot with the white checkmark to save.
A successful removal is indicated by the notice: *Stock withdrawal (order) successfully booked*.

##### Stock withdrawal without order

For a withdrawal without an order reference, you specify the storage location and quantity. This is useful for stock corrections.
- **Storage location**: Select from the combo box.
- **Stock Articles**: Select the article.
- **Variants**: Select the variant.
- **Quantity in stock**: Shows current stock.
- **Quantity to be withdrawn**: Enter the quantity. The field turns red if you try to withdraw more than is in stock.

**Here's how to withdraw goods without reference to an order**
1. Use the *Storage location* combo box to select the location.
2. From the *Stock articles* combo box, select the article.
3. If applicable, select a variant from the *Variants* combo box.
4. In the *Quantity that should be removed* field, specify the quantity.
5. Touch the blue dot with the white checkmark to save.
A successful removal is indicated by a notice.

#### Info page

With this view, you can conduct inventories or edit the contents of a box.

- **Inventory**
- **Edit Box**

##### Inventory

This is where you take inventory.
> **Inventory as independent action**: The *Inventory* action is licensed separately and is not coupled to the Stock module.

Inventory is started in A+W Business, but stock is not blocked during the process. Employees count quantities without seeing the expected stock level. After counting, data from A+W Smart Companion is compared to A+W Business data.

> **Adjustments using the selection**: If the article is selected first, the inventory stock is adjusted to the article. If the inventory stock is selected first, the article is adjusted to the stock.

**Here's how to count inventory**
1. Open the *Inventory stock* combo box and select the desired inventory date.
2. The view jumps to the next page.
3. Select or scan the article in the *Article number* field.
4. If applicable, select the variant. Entries already counted have a green checkmark.
5. In the *Inventory Stock* field, enter the counted stock.
6. Touch the blue dot with the white checkmark to save.
A successful counting is indicated by the notice: *Stock inventory count successfully stored*.

**Add quantity to a quantity already counted**
If you select an article that has already been counted by someone else, an area appears showing who counted it, when, and the quantity. You can use the `+` icon to add your count to the existing one, or the `arrows` icon to replace it.

##### Checklist

The checklist provides an overview of all articles counted and not counted. There are two views available:
- List view
- Chart view
- Scanned boxes

**Chart View**
- **Inventory progress**: A circular chart shows the percentage progress for the selected stock.
- **Inventory Status**: A donut chart shows the overall status:
    - **Finished (green)**: All variants of the article counted.
    - **Partial (yellow)**: Some variants counted.
    - **Not started (gray)**: No variants counted.
- **Slider**: A slider on the right filters the list to show only articles for which no inventory has been taken yet.

**List View Status Symbols**
- **Gray dot with exclamation point**: Not yet counted. The numbers show (variants existing) / (variants counted), e.g., 3/0.
- **Green dot with arrow**: Counted completely, e.g., 4/4.
- **Partial blue circle**: Counting started, e.g., 2/1.
> **From the checklist directly into the inventory counting**: If you touch an entry in the checklist, you jump directly to the inventory counting for that article.

**Scanned boxes View**
In the *Scanned Box* area, you will see all boxes that have already been scanned.

##### Editing a box

Here you can change the contents of a box. You can remove selected lites or break up the entire box. After scanning or manually entering a box label, a details page appears.

The page shows the box number and its contents (article, pieces). You can enter the number of **Pieces to Move**.

You must then specify a reason:
- **Breakage**: Select a reason from a combo box (e.g., *Miscounted*, *Breakage during removal*) and add an optional comment in the *Remarks* field.
- **Storage location**: Select a new storage location for the pieces being moved.

**Here's how to remove an article from the box (e.g., broken)**
1. Select the **Edit box** action.
2. Scan or enter the box barcode.
3. In the *Pieces to move* field, enter the quantity to remove.
4. Enable the **Reason for removal** radio button.
5. From the *Reason* combo box, select the reason (e.g., broken).
6. Optionally, add a note in the *Notes* field.
7. Touch the blue dot to save. A confirmation appears: *Move from box successfully booked*.

**Here's how to book an article out of the box to another storage location**
1. Select the **Edit box** action.
2. Scan or enter the box barcode.
3. In the *Pieces to move* field, enter the quantity to remove.
4. Enable the **Storage location** radio button.
5. Select the target stock and levels.
6. Touch the blue dot to save. A confirmation appears.

#### Settings

The Settings are identical for the Production and Stock modules. This process is described in connection with the Production module.
(See: Production: Tutorial, "Settings" on page B-57)
