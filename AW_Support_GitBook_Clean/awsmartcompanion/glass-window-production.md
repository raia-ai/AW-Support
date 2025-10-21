title: "A+W Smart Companion User Manual"
source: "EN_UM_AW_SmartCompanion_1_1.pdf"
tags: ["software", "user manual", "A+W Smart Companion", "glass manufacturing", "window production", "door manufacturing", "plant data collection", "inventory management", "production tracking", "mobile application"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This user manual provides comprehensive instructions for using the A+W Smart Companion application, a mobile solution for plant data collection in the glass, window, and door manufacturing industries. It covers the Basic, Production, and Stock modules."
long_description: "This document is a detailed user manual for the A+W Smart Companion application, version 1.20 (dated March 2023). The A+W Smart Companion is a mobile app for iOS and Android designed to replace classic barcode scanners for plant data collection in manufacturing environments. The manual is intended for end-users and covers the full scope of the application's functionalities. It begins with an introduction, including a revision history and editorial notes. The main content is divided into a tutorial and detailed documentation. The tutorial guides users through basic operations, from goods receipt to production bookings and inventory management. The documentation section provides in-depth information on the different modules: Basic License, Production, and Stock. It explains core operations, module selection, hardware modes (smartphone and Zebra scanner), and system messages. The Production Module section details logging in, navigating the menu bar, scanning products and racks, reporting breakages, and accessing information like rack status, order status, and order location. The Stock Module section covers functions such as goods receipt, stock movement, stock withdrawal, and inventory checks. The manual includes step-by-step instructions, screenshots, and explanations of all user interface elements, icons, and display conventions to ensure users can effectively operate the application."
---

# A+W Smart Companion

## Introduction

This part of the documentation contains editorial notes.

### Revision Overview

| Part Version / Date | Description                     |
| :------------------ | :------------------------------ |
| 1.20/03-2023        | Actions Reprint and Edit box added |
| 1.10/03-2022        | Rack inventory added            |
| 1.00/03-2021        | Original version                |

### Editorial

The editorial contains the following themes:
- Notes on this Document
- Copyrights
- Trademarks
- Contact

### Notes on this Document

This document is intended only for end users of A+W Smart Companion.
This documentation and the software it describes is only distributed with a license and may only be used and copied according to this license. The contents of the documentation are for information purposes only and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH assumes no liability for errors or imprecise statements unless these can be traced back to intentional or negligent actions.
This document describes the complete stage of expansion of A+W Smart Companion.

### Copyrights

© 2023, A+W Software GmbH all rights reserved, also those for reprinting, the making of copies and translation.
The documentation may only be copied whole or in part, stored in an archiving system or transmitted in any other form in accordance with the license agreement. Without the prior written permission of A+W Software GmbH, the documentation may not be transmitted electronically, by recording or in any other form.

### Trademarks

All hardware and software names mentioned in this documentation may also be registered trademarks or other industrial property rights held by third parties. Copyrights of third parties must be complied with.

### Contact

**A+W Software GmbH**

Am Pfahlgraben 4-10
D-35415 Pohlheim

- **Phone**: +49 6404 2051 0
- **Fax**: +49 6404 2051 877
- **Email**: aw.zentrale@a-w.com
- **Website**: http://www.a-w.com

## Tutorial

### Documentation

The tutorial for A+W Smart Companion will show you how to make bookings in the production and stock areas. Starting with goods receipt to production bookings, on through to inventory.

#### Required knowledge

The tutorial is directed at customers who book lites into stock and production. Knowledge about how to operate a smartphone is assumed. This specifically includes the following gestures: clicking, swiping, zooming in and zooming out.

#### Display conventions

Certain parts of sentences are specially marked. The meanings are:

- **_Italics_**: are marked sequences of symbols that designate the elements of the software such as the _Status selection_.
- **Bold**: marks character strings to be entered via the keyboard, e.g.: Enter the value **0**.
- **>**: The so-called "bread crumb trail" marks the path that you can use to open a dialog, e.g., _Start page >History_.
- **[ ]**: Square brackets designate buttons in the dialog. For instance, you use [Settings] to define the language.
- **< >**: Angled brackets designate buttons or combinations of buttons on your keyboard, such as updating your browser with `<F5>`.

## Basics

The A+W Smart Companion is the smart companion for plant data collection. It can be used on mobile end user devices with the iOS and Android operating systems and therefore replaces the classic barcode scanner.
Depending on the requirements, the A+W Smart Companion can be equipped with various functionalities.

### A+W Smart Companion – Basic License

The Basic License is the basic module of the A+W Smart Companion. It can be downloaded as an app from the App Store (iOS) or the Play Store (Android). Only through a connection with the back end can the following functionalities be enabled.

### A+W Smart Companion - Production

The Production module provides all booking functionalities that you need in the A+W Production main module. Reasons for breakage or status messages for racks and trucks can be selected directly from a menu. Therefore, no additional bar code tables are required. Furthermore, you can display the content of a rack, the production status or the location of individual items of an order in production directly on the mobile end user device.

### A+W Smart Companion – Stock

The Stock module supports A+W Software stock management in a mobile application. Simple, completely digital, and paperless delivery of POs (also with direct production parts), stock transactions, and stock removals.
It is currently integrated with the A+W Enterprise modules Purchase Order and Stock.
The Inventory module of the A+W Smart Companion is already integrated into the Stock module.

> **License**
> As with other scanners (Denso, WinCE, etc.), each device with the A+W Smart Companion requires a database license!

## Operation

In principle, the A+W Smart Companion can be operated very intuitively. Nevertheless, the individual operating and display elements will be explained in the following sections. A+W Smart Companion can be operated using the scan function or using manual inputs. The appropriate steps will be explained below.

### Module selection

After starting and authentication of A+W Smart Companion, select the desired module.

| Icon | Module |
| :--- | :--- |
| 🔧 | Production |
| 🏠 | Stock |
*Tab. 1: Selection of the module*

A+W Smart Companion saves the last selected application and automatically selects it after a restart.
The module can be changed in Settings at any time.
⇨ App selection
Currently, the Production and Stock modules are supported – additional modules are still under construction.

### Hardware mode

A+W Smart Companion can be used with the following mobile end user devices:
- Smartphone
- Zebra scanner

Depending on the end user device used, the scan area may look as follows:

#### Smartphone

> *Fig. A-1: Smartphone: Scan area*
> A blue line is in the middle; use it to scan the appropriate barcodes with the camera. The Flashlight icon is at the top left. In case of weak ambient lighting, you can switch on the flashlight by touching the icon.

#### Zebra scanner

If you are using a Zebra scanner, the screen will look as follows:
> *Fig. A-2: Zebra scanner: Scan area*
> The barcode that you use to scan the appropriate barcodes is in the middle.

## Messages and notices

The following messages and notices apply for both modules:

**Green dot**
The green dot indicates that the booking was transferred successfully to the back end.

**Yellow dot**
The yellow dot indicates a booking in offline mode. This booking has not yet been transferred to the back end.

**Red dot**
The red dot indicates that the booking to the back end failed.

**Gray dot**
The gray dot indicates an outstanding booking for the back end.

### Messages

After each booking, A+W Smart Companion displays a corresponding notice at the upper edge of the screen.
There are two types of these:

**Green message**
A green message indicates that the booking was made successfully and the data transferred to the back end.

**Red message**
A red message indicates that the booking was not made successfully and the data was not transferred to the back end. In this case, it is advisable for the employee to contact the administration.

## Filter function

The filter function is always available in A+W Smart Companion. Its purpose is to limit a results list step by step using various criteria. The filter function can be used alphabetically or numerically.

**Example:**
> *Fig. A-3: Total hit quantity*
> A list of variants is shown, which can be filtered by searching.

**Alphabetical search:**
> *Fig. A-4: Alphabetical hit quantity*
> Searching for "si" filters the list to show "Silver".

**Numeric search:**
> *Fig. A-5: Numeric hit quantity*
> Searching for "16" filters the list to show dimensions containing "1600.0" and "16 mm".

## Production Module

In order to reach the module's main page, an employee barcode has to be scanned or entered.

### Login

This screen appears automatically if you have selected the Production module.

> *Fig. A-6: Scan area (smartphone)*
> The upper area of the screen is for scanning. There is a blue line in the middle; use it to scan the appropriate barcodes with the camera. The Flashlight icon is at the top left. In case of weak ambient lighting, you can switch on the flashlight by touching the icon. Please don't forget to switch the flashlight off again.

> *Fig. A-7: Button for scanning*
> In the middle of the screen, there is a button for scanning the employee barcode. When you have placed the blue line on the barcode in question, touch [Scan]. The barcode is scanned.

> *Fig. A-8: Lower area of the screen*
> The Employee icon and the Back to app selection function are on the lower part of the screen. With the Employee icon, you have the opportunity to enter the employee barcode manually using the keyboard. If you touch the Back to app selection function, you return to the Module selection screen.

#### Here's how to scan the employee barcode
1. Hold the smartphone with the blue line on the barcode to be scanned. If you are in a dark place when scanning, you can switch on the flashlight by touching the icon. Please remember to switch the flashlight off again.
2. Touch [Scan].
3. The barcode is scanned and you will be on the application's main page.
4. The employee logged in is indicated at the top right of the display.

#### Here's how to enter the employee barcode
1. Touch the employee icon button.
2. The following screen opens.
3. Touch the _Enter employee ID_ field. The numeric keypad opens.
4. Enter the employee ID.
5. Touch [Save]. The screen closes and you are on the application's main page.
6. The employee logged in is indicated at the top right of the display.

### Menu bar

The menu bar is at the lower edge of the screen in each module. You can use it to switch between the individual functions of A+W Smart Companion.

**Scan**
Use this function to scan the barcodes in question.

**Status page**
Messages are issued here that report a rack or truck as empty or delivered.
⇨ _Status page_

**Breakage page**
The breakage bookings are made here.
⇨ _Breakage page_

**Info page**
You can query information about rack assignments and order status here.
⇨ _Info page_

**Settings page**
The most important settings for A+W Smart Companion are made here.
⇨ _Settings_

### Main page of the Production module

After you have logged in, you're on the module's main page. At the top of the screen, you will see the modes for scanning. A+W Smart Companion offers two modes:
- Individual
- Continuous

**Single**
This is the scan mode for individual barcodes. In this mode, each label must be scanned individually.

**Continuous**
In this mode, several barcodes can be scanned at the same time. This mode is only allowed for product barcodes. It is activated with the [Scan] button and ended with the [Stop Scan] button.

Beneath this, there is an area for scanning the barcodes, the flashlight, and the button for scanning. You should already be familiar with these elements from the login process.
Then the elements appear that are used to book the normal rack and lite transactions:

#### Registration point
Typical registration points are:
- Trucks
- Storage locations
- Production areas
- Machines or machine parts

The registration of a registration point is mandatory. You can either scan the registration point or enter the barcode manually.

##### How to scan a lite at a registration point
The registration of a registration point is mandatory.
1. Hold the smartphone with the blue line on the lite barcode to be scanned.
2. Touch [Scan].
3. The registration point scanned appears on the display.

##### Here's how to book a lite to a registration point (manually)
1. Touch the [Registration point] element. A page with the same name opens.
2. From the _Select registration point_ combo box, select the appropriate registration point.
3. From the _Status_ combo box, select the appropriate status. The following values are possible:
    - Maintenance
    - Set-up
    - Pause
    - Breakage
    - Maintenance
    ⇨ Chapter "Machine status" on page 26
4. Touch [Save].
5. The registration point entered appears on the display.

#### Racks
Rack registration is optional! You can either scan the rack or enter the barcode manually.

##### Here's how to scan a rack
1. Hold the smartphone with the blue line on the rack barcode to be scanned.
2. Touch [Scan].
3. The rack scanned appears on the display. The green dot indicates that the booking was transferred successfully to the back end.

##### Here's how to enter the rack barcode
1. Touch the rack icon button.
2. The following screen opens.
3. Touch the _Enter rack barcode_ field. An alphanumeric keyboard opens.
4. Enter the rack barcode.
5. Touch [Save]. The screen closes and you are on the application's main page.
6. The scanned rack appears on the display. The green dot indicates that the booking was transferred successfully to the back end.

#### Product
Typical products are:
- Single lite
- IG
- Spacer

In continuous scan mode, the number of scanned products and a small list symbol are displayed next to the product symbol. If you touch this symbol, a list of the scanned barcodes is displayed.

##### Here's how to scan a product
1. Hold the smartphone with the blue line on the product barcode to be scanned.
2. Touch [Scan].
3. The product scanned appears on the display. The green dot indicates that the booking was transferred successfully to the back end.

##### Here's how to enter the product barcode
1. Touch the product icon button.
2. The following screen opens.
3. Touch the _Enter product barcode_ field. The numeric keypad opens.
4. Enter the product barcode.
5. Touch [Save]. The screen closes and you are on the application's main page.
6. The scanned product appears on the display. The green dot indicates that the booking was transferred successfully to the back end.

##### Here's how to scan a product in continuous scan mode
1. Hold the smartphone with the blue line on the product barcode to be scanned.
2. Touch [Scan].
3. Move the blue line over all barcodes to be scanned. Each scanned barcode is signaled by haptic feedback.
4. Touch [End Scan].
5. The products scanned appear on the display, showing the total count. The green dot indicates that the booking was transferred successfully to the back end. Next to the number of scanned products, you will see a small list symbol. If you touch this symbol, a list of the scanned barcodes is displayed.

> **Products List Example:**
> - Product 000000361
> - Product 000000360
> - Product 000000293
> - Product 000000292

### Machine status

The machine status can be used to determine the current operating state of a machine (registration point). Depending on the master data, these can be:
- Off
- Maintenance
- Error
- Operation, ...

You can change the machine status via the main page.

#### Here's how to change the machine status
1. Touch the Registration point element on the main page. A page with the same name opens.
2. Open the _Select status_ combo box and select the desired status.
3. Touch [Save]. The page closes and you are back on the main page.

### Status page

This page is used to book a rack or registration points empty or off-site. For this, you select the appropriate action (the name on the button depends on the master data stored) and scan the barcode of the registration point, the rack or the product. The barcode can also be entered manually by touching the notice text.

On this screen, two buttons are available in the _Select status_ area:
- **Start**: This button starts an empty report of a registration point or a rack. The name on the button depends on the master data stored.
- **Delivered**: Use this button to book a product, a rack or a registration point as delivered. The name on the button depends on the master data stored.

This screen may contain the following elements:
- Empty rack
- Full, delivered rack
- Empty truck (registration point)
- Full (delivered) truck (registration point)

#### Here's how to scan an empty rack
1. Touch [Start]. The button turns blue.
2. Scan the barcode of the rack in question.
3. The scanned rack appears in the area _2 Scan_ in the form of an empty rack.
4. The notice _The actual rack weight was reset_ appears at the top of the screen.
> **Note:** This notice only appears if a rack weight was present.

#### Here's how to scan a full (delivered) rack
1. Touch [Delivered]. The button turns blue.
2. Scan the barcode of the rack in question.
3. The scanned rack appears in the area _2 Scan_ in the form of a full rack.

#### Here's how to scan a delivered product
1. Touch [Delivered]. The button turns blue.
2. Scan the barcode of the product in question.
3. The scanned product appears in the area _2 Scan_ with an appropriate icon.

#### Here's how to book an empty rack (manually)
1. Touch [Start]. The button turns blue.
2. In the area _2 Scan_, touch the notice _Or enter the barcode manually_.
3. The _Assign status_ screen opens.
4. In the _Enter rack barcode_ field, enter the appropriate barcode.
5. Touch [Save].
6. The rack entered appears in the area _2 Scan_ in the form of a full rack.
7. The notice _The actual rack weight was reset_ appears at the top of the screen.
> **Note:** This notice only appears if a rack weight was present.

#### Here's how to book a rack in a full (delivered) status (manually)
1. Touch [Start]. The button turns blue.
2. In the area _2 Scan_, touch the notice _Or enter the barcode manually_.
3. The _Assign status_ screen opens. Touch the full rack.
4. In the _Enter rack barcode_ field, enter the appropriate barcode.
5. Touch [Save].
6. The rack entered appears in the area _2 Scan_ in the form of a full rack.

#### Here's how to scan an empty truck
1. Touch [Start]. The button turns blue.
2. Scan the barcode of the truck in question.
3. The scanned truck appears in the area _2 Scan_ with an empty cargo area.

#### Here's how to scan a full (delivered) truck
1. Touch [Delivered]. The button turns blue.
2. Scan the barcode of the truck in question.
3. The scanned truck appears in the area _2 Scan_ with a full cargo area.

#### Here's how to book an empty truck (manually)
1. Touch [Start]. The button turns blue.
2. In the area _2 Scan_, touch the notice _Or enter the barcode manually_.
3. The _Assign status_ screen opens. Touch the truck with the empty cargo area.
4. Open the _Select truck_ combo box. The combo box includes all trucks created at your company.
5. Select the desired truck.
6. Touch [Save].
7. The selected truck appears in the area _2 Scan_ with an empty cargo area.

#### Here's how to book a rack in a full (delivered) status (manually)
1. Touch [Delivered]. The button turns blue.
2. In the area _2 Scan_, touch the notice _Or enter the barcode manually_.
3. The _Assign status_ screen opens. Touch the truck with the full cargo area.
4. Open the _Select truck_ combo box. The combo box includes all trucks created at your company.
5. Select the desired truck.
6. Touch [Save].
7. The selected truck appears in the area _2 Scan_ with a full cargo area.

### Breakage page

Products can be reported broken on this page. The breakage reason is selected first and then the product is scanned. Possible reasons for breakage can be:
- Scratches
- Breakage
- Bottle glass type
- Defective coating

The breakage reasons are defined individually in the database.

#### Here's how to scan a break
1. Open the _Select breakage reason_ combo box.
2. Select the appropriate breakage reason.
3. Hold the smartphone with the blue line on the product barcode to be scanned.
4. Touch [Scan].
5. The scanned product appears in the area _2 Scan_.

#### Here's how to enter a break (manually)
1. Open the _Select breakage reason_ combo box.
2. Select the appropriate breakage reason.
3. Touch the element to open the manual entry dialog.
4. In the _Enter product barcode_ field, enter the appropriate product number.
5. Touch [Save].
6. The scanned product appears in the area _2 Scan_.

### Info page

Information about racks or orders can be called up with this page. It is divided into an Information area and an Actions area.

**The Information area contains:**
- Rack information
- Order status
- Order location

**The Actions area contains:**
- Registration point status
- Rack shifting
- Actual rack weight
- Rack inventory
- Material request
- Forms

#### Rack information

This is where there is information about rack assignment. After you have scanned the rack barcode, an appropriate screen appears.

##### Explanation of the elements

- **Header**: Shows the rack number (e.g., Rack 15), status (e.g., Dispatch), weight, and number of lites. A red 'X' indicates at least one item is incomplete.
- **Customer Section**: Shows the customer name and the completion status for that customer's items on the rack (e.g., 10/10 with a green checkmark for complete, 40/18 with a red 'X' for incomplete).
- **Item Details**: Below the customer, a list of items shows the Order number, Item number, and Dimensions. The status shows how many lites are on the rack out of the total ordered for that item (e.g., 10/5 means 5 of 10 are on the rack). A red 'X' indicates an incomplete item; a green checkmark indicates a complete item.

##### Here's how to scan rack information
1. Touch the _Rack Information_ element. The _Rack information_ page opens.
2. Scan the rack for which the information should be displayed.
3. Touch [Scan].
4. The rack information is displayed.

##### Here's how to call up rack information with an entry
1. Touch the _Rack Information_ element.
2. Touch the element to open the manual entry dialog.
3. The _Rack information_ page opens. In the _Enter rack barcode_ field, enter the appropriate rack number.
4. Touch [Save].
5. The rack information is displayed.

#### Order status

Here's the information about order status. You can learn everything about the production progress of an order, its items, and their subparts. Similarly, you can see for which machines on which dates and in which shift the individual steps are planned. After you have scanned the product barcode, an appropriate screen appears.

##### Explanation of the elements
- **Cust**: Next to the element, the customer's name and address are displayed.
- **Deliv. Date**: Next to the element, the delivery date is displayed.
- **Header part**: Displays the item number, dimensions, product name, and customer consignment. If the production item deviates from the commercial item, both values are displayed (production item in brackets).
- **Processing**: This element displays a processing step.
- **Processing machine**: This element depicts the processing machine.
- **Completion Status**:
    - **Green Checkmark (e.g., 8/8)**: Indicates all lites are finished for this production step.
    - **Yellow Line-through (e.g., 25/12)**: Indicates part of the total quantity has been processed. 12 of 25 pieces are finished.
    - **Red X (e.g., 25/0)**: Indicates that production for this step has not yet been started.
- **BOM (Bill of Materials)**: Touching the '+' icon next to the header displays the BOM.
    - The blue edge on the left side represents the depth of the BOM. The dots at the end of the line provide information about the production progress of the individual parts.
    - **Float**: Represents a float glass.
    - **TG**: Represents tempered glass.
    - **Spacer**: Represents a spacer.
    - **Muntin**: Represents a muntin.
    - **IG**: Represents an IG with muntins.
    - **LAMI**: Represents a LAMI.
    - **Foil**: Represents a foil.
    - **IG with step**: Represents an IG with a production step.
    - **LAMI with step**: Represents a LAMI with a production step.
    - **Patterned glass**: Represents a patterned glass.
    - **Fire protection glass**: Represents fire protection glass.
    - Touching one of these elements displays the associated processing and registration point. Touching it again closes the BOM.

#### Order location

This screen provides information about where precisely in production the individual parts of an order are located. After you have scanned the product barcode, an appropriate screen appears.

##### Explanation of the elements
- The top area shows the customer and delivery date.
- The number at the end of the header indicates the total number of products in this order.
- The item header shows item number, product name, and order quantity.
- Below the item header, the registration point (e.g., Table 1), the rack number, and the number of parts on that rack at that location are displayed.

#### Registration point status

This element is in the Actions area. Here, you have the opportunity to set a registration point to a desired status. If a registration point is out of service, for example, you can set its status to _Off_.

##### Here's how to set the status for registration points
1. Touch the element. The _Registration point_ page opens.
2. Open the _Select registration point_ combo box and select the desired registration point.
3. Open the _Select status_ combo box and select the desired status.
4. Touch [Save].
5. At the upper edge of the screen, the message _The registration point was saved_ appears.

#### Rack shifting

This element is in the Actions area. Here, you have the opportunity to shift everything that is on a rack to another rack. In the process, you can always only shift all products that are on the rack. It is not possible to shift just a partial quantity.

##### Here's how to shift the products by scanning
1. Touch the element. The _Rack shift_ page opens.
2. Scan the barcode of the source rack that should be emptied. The rack number, name, and quantity on the rack will be displayed.
3. Scan the barcode of the target rack. The rack number, name, and quantity will be displayed. A checkmark in a blue dot indicates the shift was completed successfully.

##### Here's how to shift the products by entering them
1. Touch the element. The _Rack shift_ page opens.
2. Touch the source rack element to open the entry page.
3. In the _Enter source barcode_ field, enter the barcode of the rack that should be emptied.
4. Touch [Save]. The source rack details will be displayed.
5. Touch the target rack element to open the entry page.
6. In the _Enter target barcode_ field, enter the barcode of the rack to which you would like to shift the products. The target rack details will be displayed. A checkmark in a blue dot indicates the shift was completed successfully.

#### Actual rack weight

This element is in the Actions area. Here you have the opportunity to enter the current weight of a rack.

##### Here's how to scan in the actual rack weight
1. Touch the element. The _Actual rack weight_ page opens.
2. Scan the barcode of the rack in question.
3. Enter the weight in the _Enter rack weight (kg)_ field.
4. Touch [Save].
5. The notice _The actual rack weight was booked successfully_ appears at the top of the screen.

##### Here's how to enter in the actual rack weight (manually)
1. Touch the element. The _Actual rack weight_ page opens.
2. Touch the element to open the manual entry dialog.
3. In the _Enter rack barcode_ field, enter the appropriate barcode.
4. Enter the weight in the _Enter rack weight (kg)_ field.
5. Touch [Save].
6. The notice _The actual rack weight was booked successfully_ appears at the top of the screen.

#### Rack inventory

This element is in the Actions area. Here you have the opportunity to conduct an inventory for a corresponding rack. After you have scanned the rack, the following page appears.

##### Top section
This section shows the rack number on the left. On the right, it shows the `Last Check` date and the `Next Check` date. If the inspection interval has elapsed, a red triangle with an exclamation point will be displayed.

##### Rack Details
- **Rack Types**: Select the correct rack type from the combo box if needed.
- **Weight (kg), Load (kg), Size (mm)**: Displays the rack's physical properties.
- **Perform Inspection**: Check this box if you have conducted a visual inspection.
- **Number of Labels**: If a barcode is no longer legible, you can enter the number of new labels to print here. The labels are output immediately on the defined printer.
- **Save/Save and Print**: If you do not need to print a label, the button is [Save]. If you have entered a number of labels to print, the button becomes [Save and Print].

##### Here's how to conduct a rack inventory
1. Touch the element. The _Rack inventory_ view opens.
2. Scan the barcode of the rack in question. The data is loaded.
3. Check whether the rack type is correct. If not, open the _Rack types_ combo box and select the correct rack type.
4. If you have done a visual inspection, check the _Inspection performed_ checkbox.
5. If you need new labels, set the number in the _Number of labels_ field.
6. Touch [Save] or [Save and print].
7. The notice _The actual rack weight was booked successfully_ appears at the top of the screen.

#### Material request
This element can currently only be used with A+W Cantor.

#### Forms
This element can currently only be used with A+W Cantor.

### Settings

The essential settings for A+W Smart Companion are made on this page.

#### Explanation of the elements

- **Log**: Calls up the online booking log to display the last bookings of the user and their transfer status.
- **Download master data**: Forces the download of PDC master data (people, registration points, breakage reasons) to the device. This function is only in the Production module.
- **Language**: Select the display language. Options include German, English, French, Italian, Spanish, Romanian, Chinese. The active language is shown in blue.
- **Adjust configuration**: Sets the device name and connection to the back end (Service Locator).
- **App selection**: Select the desired application (Production Module or Stock module).
- **Information**: Displays device ID, device name, Service Locator, etc. about A+W Smart Companion.
- **Help**: Displays contact information for A+W Software GmbH.
- **Imperial system**: A slider to switch between metric (mm, kg) and imperial (inches, pounds) units. Blue indicates imperial is active.
- **Hardware mode**: A slider to set whether barcodes are read with the camera or the built-in scanner. This is only available for the Zebra TC20 Pro scanner. Blue indicates the built-in scanner is active.
    > **Note:** This element is only displayed if the correct setting is entered in the Infrastructure.Web ForeignLicense. The device has to be set there to the DeviceType Mixed or Hardware scanner.
- **Log out**: Logs out the current user and returns to the main login page.

## Stock module

In order to reach the module's main page, an employee barcode has to be scanned or entered.

### Enter or scan employee

This screen appears automatically if you have selected the Stock module.
Entering or scanning the employee ID is identical for the Production and Stock modules. To avoid redundant explanations, the procedure is described for the Production module.
⇨ _Enter or scan employee_
After successful log-in, the employee's name appears at the top right.

### Menu bar

The menu bar is at the lower edge of the screen. With it, you can switch between the individual functions of the A+W Smart Companion Stock module.

**Goods receipt**
Use this function to book incoming goods.
⇨ _Booking goods receipt_

**Stock movement**
Use this function to book goods from one stock to another.
⇨ _Booking stock movements_

**Stock withdrawal**
Use this function to book a stock withdrawal.
⇨ _Booking stock withdrawals_

**Info page**
In this area, the missing prices are displayed and you can book the inventory.
⇨ _Info page_

**Settings page**
The most important settings for the A+W Smart Companion are made here.
⇨ _Settings_
