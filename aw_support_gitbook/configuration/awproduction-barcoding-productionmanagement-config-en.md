---
title: "EN_AWProduction_Barcoding_2.01"
source: "EN_AWProduction_Barcoding_2.01.pdf"
tags: ["A+W Production", "Barcoding", "Software Manual", "Production Management", "Glass Manufacturing", "Window Manufacturing", "ERP", "PPS", "Scanner Configuration", "Booking"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical manual for the A+W Production Barcoding module. It provides a tutorial and software reference for end-users, covering basic concepts, booking elements, data entry with scanners, and production monitoring. The guide explains how to track products, racks, and staff through the production process using barcodes."
long_description: "This document is the official user guide for the A+W Production Barcoding module, version 2.01. It serves as both a tutorial for new users and a experienced operators in the glass, window, and door manufacturing industries. The manual details the system's purpose: to collect real-time data on production statuses and processes, thereby increasing transparency and efficiency. It begins with an introduction covering the document's revision history and scope. The tutorial section explains fundamental concepts like direct and indirect objects, booking types (movement, processing, status), and key booking elements such as products, racks, staff, and registration points (e.g., machines, trucks). It provides step-by-step instructions for data entry using various scanner types (online, offline, serial) and includes practical booking examples for common scenarios like loading trucks, handling rejects, and correcting errors. The guide also covers the use of Production Terminals for different workstations (e.g., cutting, IG line, furnace). The software reference section provides detailed descriptions of master data dialogs, including settings for barcode options, registration points, racks, employees, and status values. Finally, it touches upon statistics and monitoring tools like A+W Dashboard and A+W Discovery for analyzing production data."
---

# A+W Barcoding: A+W Production

**A+W - Software for Glass, Windows and Doors**

---
## Introduction

This part of the documentation contains editorial notes.

### Revision overview

| Part Version / Date | Description |
| :--- | :--- |
| 1.00 / 03-2007 | Original version |
| 1.01 / 07-2013 | Layout adapted to CI 2013. |
| 2.0 / 06-2014 | Complete revision |
| 2.01 / 1-2017 | Product and company names adjusted. |

### Editorial

The editorial provides information on the following topics:
*   Notes on this document
*   Copyrights
*   Trademarks
*   Contact

### Notes on this document

This publication is written exclusively for end users of A+W Production in mind.

The documentation and software described therein are licensed only and must be used or copied only in accordance with the terms of our license agreement. The contents of the documentation are for information purposes only and are subject to changes without prior notice.

The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to intentional or grossly negligent behavior.

The descriptions in this document are based on the full program level of A+W Production.

### Copyrights

© 2017, A+W Software GmbH, all rights, including the right of reprint, production of copies and translation, are reserved.

The documentation may be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. This documentation may not be transmitted, neither electronically, nor mechanically, nor by recording or in any other way, without the prior written permission from A+W Software GmbH.

### Trademarks

All hardware and software names mentioned in this documentation might also be registered trademarks or other property rights of third parties. Copyrights of third parties must be complied with.

### Contact

**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
*   Tel: +49 6404 2051-0
*   Fax: +49 6404 2051-877
*   Email: Zentrale@a-w.com
*   Web: http://www.a-w.com

## Tutorial

### Overview

The target group of this training session concerning the A+W Production module are employees who are working at different stations (machines and registration points) within production.

The benefit for the customers is that they can directly control their machines. There are no downtimes due to having to digitalize a shape at a processing machine. It is furthermore not necessary to enter any NC codes at the machine which also means continuous machine deployment.

> **The functions depend on the enabled modules**
> Please note that the individual functions are available only if the corresponding modules and interfaces have been installed and enabled.
> If you detect functions in this description that are not available in your version, please contact A+W Software GmbH.

#### Subjects

This tutorial offers the following subjects:
*   Basic Ideas
*   Booking Elements
*   Data Entry
*   Statistics, Reporting and Monitoring

#### Required knowledge

This tutorial addresses participants who work at different stations (areas, machines and registration points) within Production. The participants must be familiar with the concepts of production terminals and scanners.

> **Required knowledge**
> Basic IT knowledge and/or Windows knowledge are prerequisites for using A+W Production.

### Documentation

For your training on the Barcode Manager, the following documents are available:

| Format | Content |
| :--- | :--- |
| **HTML** | Tutorial and Software Reference |
| **Handout** | Printout of training document for participants |
| **PDF** | Complete documentation (Tutorial, Software Reference) |
| **Online help <F1>** | Context-sensitive dialog help in the A+W Production Software Reference. |

#### Tutorial Structure

This tutorial consists of subjects with several training modules each. Each module consists of the following elements:

*   **Overview**: Each training module starts with an overview of the major topics:
    *   Objectives: What shall be conveyed?
    *   Benefit: What can this knowledge be used for?
    *   Maxims: Which correlations are to be remembered?
*   **Concepts**: First, the concepts and terms of the corresponding training module will be explained. This is followed by examples and instructions.
*   **Exercises**: For some of the training modules, exercises with certain tasks and suggested solutions are available. These exercises will help you to understand and learn to apply A+W Production.
*   **Cross reference section**: At the end of each training module there is a section with cross references pointing to corresponding descriptions in the software reference. This will help you to extend your newly acquired knowledge.
*   **Reading tip**: The contents of a training module are based on the knowledge conveyed in the previous module. We therefore recommend not to skip any training modules. If you are already familiar with a subject you should at least read the summary at the start of a training module in order to bring the main details to mind.

In the practice section of each training unit, the software reference and the exercise section are systematically included by means of cross references. This results in a central theme throughout the entire documentation.

### Display Conventions

Certain parts of sentences are specially marked. The meanings are:

| Style | Description |
| :--- | :--- |
| *Italics* | Marks character strings referring to software elements, e.g. the *Global Shape Data* dialog. |
| **Bold** | Marks phrases to be entered via the keyboard, e.g. the number **0**. |
| > | The so-called breadcrumb path shows how to open a dialog, e.g. File > Import > Transfer file. |
| [] | Square brackets mark buttons in a dialog, e.g. [OK] to save the entries. |
| <> | Angle brackets refer to keys or shortcuts on the keyboard, e.g. <F1> is used to open the online help. |

### Basic Ideas

This documentation shall give you an idea of the Barcoding process and module in A+W Production and a basic understanding of this subject. Moreover, we will explain the basics of A+W Production, the tools used, and the general possibilities and limits.

We strongly recommend referring to detailed documentation on control stations (production terminals), internal A+W Production installation and configuration instructions, scanner installation, configuration, etc. These subjects will be mentioned in this documentation, but not handled in detail. A clear restriction of the areas is not always possible, and not required either.

These instructions are not a substitute for basic knowledge about production structures, the production terminals used, scanners or other A+W software.

#### Document structure

This documentation describes general knowledge on A+W Production. What is A+W Production, the most important components, registration points, which scanner types are used, procedures, etc.

#### Barcoding

A+W Production is a general term for collecting current data about statuses and processes in companies.

It gathers the flow of production at the most important places within production, the so-called registration points, and thus maps the process flow of your production. This is achieved by means of, e.g. barcodes, scanners, Production Terminals (control stations), etc. Directly or indirectly, the gathered data is transferred to an appropriate collection point (AWPort) and saved in the database (A+W Production DB).

#### Purpose of A+W Production

First of all, A+W Production is used to display the current situation. Starting from determining the production status of an order, and tracking the product through production to displaying the performance.

In the case of rejects, apart from the registration point, the reject reason is entered. Corresponding subsequent parts can be created automatically, depending on the configuration. Machine control is also executed automatically based on barcode readings.

Another important aspect of A+W Production are the statistical analyses. You can analyze the productivity and machine times, monitor production mistakes (e.g. reject) and are provided with quality assurance thanks to the batch data collection.

A+W Discovery enables you to create long-term analyses that are available for future planning.

### Booking Elements

This subject shows you how to handle the different objects of A+W Production.

This includes the following training modules:
*   "Products"
*   "Booking Places"
*   "Racks"
*   "Staff"
*   "Status"

#### Products

**Objectives**
*   Getting familiar with objects of A+W Production.
*   What can and what cannot be tracked.

**Definitions**

| Term | Definition |
| :--- | :--- |
| **Direct objects** | Have a barcode and are booked directly. |
| **Indirect objects** | Do not have a barcode because they are automatically included when booked. |

**Note**

| Term | Definition |
| :--- | :--- |
| **Traceable products** | All parts of a bill of materials onto which a barcode can be applied. |
| **Single lite A+W Production** | Every BOM element is identified by its own barcode. |
| **Quantity A+W Production** | All parts of a BOM element have the same barcode. |

#### Basics

A+W Production differentiates between two object types:
*   Direct objects
*   Indirect objects

**Direct objects**

Direct objects are those that have a barcode and can be booked directly. They include:
*   Registration points (places, trucks and machines)
*   Racks and boxes
*   Lites and units
*   Status values / statuses
*   Employees

**Indirect objects**

Indirect objects are those that are automatically included when booked. They include:
*   Processing
*   Batch information

**Lites or Units**

Lites and units are traceable products. These are always all the parts of a bill of materials onto which a barcode can be affixed. Example: Single lite, IG, LAMI, frame, muntin, etc.

In single lite A+W Production (default), every BOM element is identified by a unique barcode. This enables you to determine the exact location and status of a part.

In quantity A+W Production, all parts of a BOM element have the same barcode. As a result, it is no longer possible to determine the exact location and status of a part. Here, quantity statements are only made in relation to production statuses. Accordingly, the booking effort is a lot less.

In contrast to the aforementioned parts, there are parts that cannot be tracked. These include, e.g. gas, butyl, silicone, foils, etc.

To get an optimum data basis, it is therefore essential to book single lites/units to the corresponding registration point or rack in Production.

#### Booking types

We distinguish between three booking types:
*   **Movement bookings:** Movement bookings record the change of location of a rack, unit or lite. This may be a rack (e.g. unit on rack) or a registration point (rack or unit on registration point).
*   **Processing bookings:** Processing bookings register processing steps (e.g. drilling) for units.
*   **Status bookings (e.g. rejects, maintenance):** Status bookings represent the change of status of an object.

Processing and status bookings can also be triggered implicitly, through movement bookings.

Naturally, reject registration is important in this connection. Apart from the registration point and other information, the reject reason is entered. Subsequent parts can be generated automatically, depending on the configuration.

The gathered data can be used for analysis, statistics, and inventory purposes, among other things (e.g. barcode reports, MS-Excel, etc.). It is used for production control, lite/unit and rack tracking and many other purposes.

**Additional Information**
*   See "Reject Management"
*   See "Barcode Reporting"
*   See "Scanning Units"

#### Booking Places

**Objectives**
*   Acquire knowledge about the *Registration Points* dialog.
*   Getting familiar with and understanding the *Error Rack* registration point.
*   Getting familiar with and understanding the *Dispatch* registration point.

**Benefits**
In order to avoid booking mistakes, it is necessary to observe the correct booking order.

**Definitions**

| Term | Definition |
| :--- | :--- |
| **RP** | Short for registration point |
| **Registration points** | Stations within production or dispatch. |
| **Error rack** | An internal registration point with the registration point number 12 and is filled automatically. This registration point will include all units which - because of errors - have lost their allocation to a physical rack or a physical registration point. |
| **Trigger time** | The time defined in the system which determines the point in time from which the truck load is considered to be shipped. It is enabled by the status booking `<Start> <Truck>`. The time can be configured in the system. |

**Note**
Registration points have a unique number and a name.

##### Registration Points

All stations within production (production areas, trucks, machines) that are equipped with scanners and/or Production Terminals are called registration points (RP). They have a unique number and a name.

A machine does not necessarily have to be one registration point. It can also be subdivided into several registration points.

**Example: IG line**
*   1611 > machine entry,
*   1610 > the machine itself and
*   1612 > machine exit.

Splitting machines into several registration points allows detailed production tracking and analysis.

You can book racks, products and statuses to these registration points. The more registration points you have, the more detailed your analyses will be.

*[Image: Screenshot of the Registration Points dialog, showing a table with columns for ID, Name, Description, Type, and Machine No. The bottom half shows detailed fields for a selected registration point like "Registration Point No.", "Barcode", "Name", and checkboxes for "Feedback of Bookings".]*

The table above shows which registration points have already been created. You can create new registration points or change already created registration points.

The checkboxes in the *Feedback of Bookings* section are for production feedback that are used to update the current order status in the upper-level order processing system.

> **Column headers can be configured as desired**
> The headers of the individual columns can be configured as desired. It is therefore possible that the headers shown here do not correspond to the headers in your installation.

##### Error rack

The error rack is an internal registration point. This registration point will include all units which - because of errors - have lost their allocation to a physical rack or a physical registration point.

The internal registration point *Error Rack* has registration point number 12.

Registration point 12 follows the same rules as any other registration point (reports, bookings, corrections, etc.).

Basically, there are two rules for the *Error Rack* registration point:
*   **Rule 1:** The error rack should always be empty!
*   **Rule 2:** If the error rack is not empty, there must be an operation or scanner error.

**How do units get onto the error rack?**

There are several reasons. Apart from a defective scanner/label, this is usually due to operating errors by the staff.

The error rack is used whenever a registration point or rack is scanned with the status `<Start>` while according to A+W Production, this object still holds units. These units are automatically assigned to the Error Rack registration point.

**Possible causes:**

*   **Example 1:**
    Several racks are being used at a registration point. A physical rack has been registered with the scanner; units are booked to this rack `<Rack 1> <Unit 1> <Unit 2>`. When changing to the second rack, the user forgets to scan/register this rack. The units are actually placed onto rack 2 but booked to the wrong rack, namely rack 1.
    If rack 1, which has been correctly loaded, is processed as usual during the production process, this rack will be empty and ready for other tasks.
    According to the scanning rules, rack 1 will be scanned with `<Start> <Rack1>` next time. This resets the rack in barcoding to empty.
    Internally (according to bookings), rack 1 still held the erroneously scanned (allocated) units from rack 2 (see above). These units are automatically booked to the *Error Rack* registration point.

*   **Example 2:**
    A truck is loaded correctly. When all units, racks, and boxes have been loaded, the truck should get the status Shipped `<Shipped><Truck1>`. This is omitted. The truck delivers the goods and is available (empty) for the next transport on the next day.
    According to the scanning rules, it is registered for loading by `<Start><Truck1>`, and reset (empty).
    As the truck is still considered loaded (according to bookings) because of the missing `<Shipped>` booking of the previous day, its entire load is booked to registration point 12 (Error Rack) by the `<Start>` status booking.

*   **Example 3:**
    A loaded rack is unloaded without being scanned, or scanned by a defective scanner. Physically, the rack is empty, but according to barcoding, it is still loaded. The next time the rack is used, in adherence to the scanning rules `<Start><Rack>`, these units will be booked to registration point 12, Error Rack.

**Removing units from the error rack**

The error rack is an internal registration point. As on any other registration point, units on this rack can be changed by new bookings.

There are two methods of booking units from one registration point (in this case the error rack) to another registration point/rack.

1.  **The manual method** is carried out via the *Production Terminal Edit*. You must execute the changes to the registration point (of the rack) manually by using the *Production Terminal Edit*.
2.  **The automatic method** corrects an error automatically by another correct booking during the production process.

> **Tip**
> Check the internal registration point 12 (Error Rack) regularly, and make corrections right away. Apart from the *Production Terminal Edit*, the Barcode Manager reports are available for checking purposes.
> ⇨ See "Barcode Reporting"
> Please remember: from the barcoding point of view, this is a registration point. You can use the same functions and tools for analyses and corrections as for any other registration point!

> **Many units on the error rack**
> If there are many units on the internal registration point 12 *Error Rack*, please contact the A+W customer service. A+W will analyze the reasons together with you and work out a customized and practical solution.

**Correct booking**

Units moved to the internal registration point 12, *Error Rack*, will be automatically removed from the *Error Rack* with the next correct booking of these units at another registration point. They will be assigned to this registration point/rack and vanish from the *Error Rack* registration point.

**Example:**
A loaded rack is unloaded without being scanned, or scanned by a defective scanner. Physically, the rack is empty, but according to barcoding, it is still loaded. The next time the rack is used complying with the scanning rules `<Start> <Rack>`, these units will be booked to the Error Rack (only applies to units which have not been registered again in the meantime, see below!).

Prerequisite for automatic correction is that the units are still being produced and will be scanned during further processing.

Every scan allocates the unit to the corresponding registration point/rack; the unit automatically vanishes from the internal registration point 12, Error Rack.

**Additional information**
*   ⇨ See "Scanning in Dispatch"
*   ⇨ See "Scanning Registration Points"

#### Managing Registration Points

This module will show you how to create new registration points and edit or delete them.

**How to create a new registration point**

1.  Open the *Registration Points* dialog.
2.  Press the icon button [New].
3.  Enter a unique registration point number in the *Registration Point Number* field.
4.  Enter the barcode number for the registration point in the *Barcode* field.
5.  Enter the registration point name in the *Name* field.
6.  The *Description* field allows you to enter information regarding the registration point.
7.  Enter the text that is to be displayed in the production lists in the *Text for Production Lists* field.
8.  Enter the text that is to be displayed in the customer lists in the *Text for Customer Lists* field.
9.  Enter the text that is to be displayed underneath the barcode in the *Subrow for Barcode Labels* field.
10. Select the type of the registration point from the *Registration Point Type* combo box.
11. Using the *Grouping* field, you can define a different grouping to be used for analyses apart from the registration point type.
12. In the *Grouping for Working Shifts* field you can group individual registration points for working shifts.
13. Select the corresponding status from the combo box in the *Current Status* field.
14. If a restriction check has been defined for the registration point, it will be activated and controlled via the *Restriction* combo box.
15. The *Over Quantities* field is in direct connection with the *Restriction* field. You can define the corresponding value in percentage only if the *Restriction* field has one.
16. Activate the *Show Produced Parts* checkbox if completely produced lites should be shown on the *Production Terminal*.
17. If the registration point deviates from the registration point from order entry, please overwrite the entry.
18. Activate the *Processing Feedback* checkbox if the processing progress should be reported to the order processing system precise to the lite.
19. Activate the *Rack Feedback* checkbox if the rack load should be reported to the order processing system.
20. Activate the *Report Rack Load to Rack Server* checkbox if the rack load should be reported to the rack server.
21. Activate the *Unit Feedback* checkbox.
22. Activate the *Production Feedback* checkbox if feedback on the order items should be sent to the order processing system.
23. Click on the icon button [Save] to save the entries.

**How to delete a registration point**

1.  Open the *Registration Point* dialog.
2.  Select the registration point that is to be deleted from the list.
3.  Press the icon button [Delete].
4.  The system queries whether the record shall actually be deleted.
5.  Click on [Yes]. The record will be deleted.

**How to make changes to registration points**

1.  Open the *Registration Point* dialog.
2.  Select the registration point that is to be changed from the list.
3.  Press the icon button [Change]. The dialog will be released for editing.
4.  Carry out the required changes.
5.  Click on the icon button [Save] to save the entries.

**Additional information**
*   ⇨ See Software Reference, "Registration Points"

#### Truck registration point

Each truck is a registration point which follows the same rules as any other registration point. An exception is the emptying of a truck via barcodes. Objects (racks/boxes, etc.) usually leave a registration point by being registered at another registration point. This does not make sense for trucks, for practical reasons. It would have to be scanned when the units are unloaded, e.g. at the construction site.

The objects must be booked off this registration point and transferred to the internal registration point 11 (Off Site) by means of another barcode mechanism. However, this booking must be made only after the truck has been returned fully unloaded!

To avoid a complex technical structure with scanners at the gates, the booking to registration point 11 (Off Site) is made after a time period defined in the system, when the truck is registered after its return by `<Start><Truck>`.

The time period is triggered by scanning the status `<Shipped> <Truck>` for the corresponding truck and/or its load.

Within this time period, the load is considered as not shipped and is still booked to registration point `<Truck>` with status `<Shipped>`. Only after a START registration, AFTER a defined period, the registration point changes to 11.

The status booking `<Start><Truck>` would reset the truck and/or the racks, and move the units involved to the error rack!

After the defined time period, all units are considered to be shipped, and are booked to the internal registration point 11 with status `<Shipped>`; the racks and/or the truck can be used again in the production process.

**Additional information**
*   ⇨ See Software Reference, "Registration Points"
*   ⇨ See "Truck Registration Point"

#### Racks

**Objectives**
*   Acquire knowledge about the *Racks* dialog.
*   Getting familiar with and understanding the booking process.

**Benefits**
In order to understand barcoding, you must know what can be booked to the racks.

**Definitions**

| Term | Definition |
| :--- | :--- |
| **Rack types** | Rack types in barcoding include A racks, L racks, harp racks, boxes and the specific racks for furnace beds and autoclaves. |

**Note**

| Term | Definition |
| :--- | :--- |
| **Book rack** | When a rack is booked to a registration point, all units on the rack will be automatically booked to this registration point as well. |
| **Create racks** | Racks can be created in the master data manually or automatically. |
| **Book** | You can book products or statuses to racks. |
| **Where is a rack located** | A rack is always located at one location (registration point). |
| **Boxes** | Boxes are not returned to the production cycle. |

##### Racks

Use this section to create racks for A+W Production. The following rack types are available:
*   A racks
*   L racks
*   Harp racks
*   Boxes

At some registration points, special racks are required. These are usually the furnaces and autoclaves.

You can book products or statuses to the racks. A rack is always located at one location in production (registration point).

*[Image: Screenshot of the Racks dialog, showing a list of existing racks and fields to define new racks or view properties of a selected rack.]*

The screenshot above shows which racks have already been created. You can create new racks or change already created racks.

##### Filter racks

If you have a large quantity of racks, you can create filters to restrict the displayed racks. You can see in the upper section of the dialog whether a filter has been set.
If a filter has been set, the following is displayed: `Caution: The rack filter is set!`
If no filter has been set, the following is displayed: `No rack filter set`

In order to activate a filter, click on the button [Filter]. The *Rack filter* dialog opens in which you can define and activate the corresponding filter.

> **Column headers can be configured as desired**
> The headers of the individual columns can be configured as desired. It is therefore possible that the headers shown here do not correspond to the headers in your installation.

##### Boxes

At first, boxes are treated like racks but they are not returned to the production cycle. It is therefore useful to use a separate number area for the barcodes.

This barcode area should always be printed and used up completely. This ensures that a barcode cannot be used several times in Production simultaneously.

You can, of course, also print and use up a succession of several smaller areas, e.g. 9000-9099 followed by 9100-9199, 9200-9299, etc., but you should always use the entire number area up to 9999.

The booking history for the boxes still remains expressive if the area is used to its full extent and barcodes repeat themselves after quite a long time.

> **Creating barcodes**
> Always use the report for barcode creation. Alternatively, barcodes can be supplied by a Microsoft Word document.

**Additional information**
*   ⇨ See Software Reference, "Racks"
*   ⇨ See Software Reference, "Rack Filter"
*   ⇨ See "Barcode Reporting"
*   ⇨ See "Scanning Racks and/or Boxes"

#### Managing Racks

This module will show you how to create new racks and to edit or delete them.

**This is how you create one new rack**

1.  Open the *Racks* dialog.
2.  Press the icon button [New].
3.  Enter a unique name for the rack in the *Name* field.
4.  Enter the barcode for the rack in the *Barcode* field.
5.  Select from the *Rack Base Type* combo box to define whether the rack is a regular rack, a tray rack or a box.
6.  Select *Rack Type* from the combo box to define whether the rack is an A rack, a harp rack or special rack.
7.  If the rack is a tray rack, enter the first and last number to be used in the *Slot Number from to* field.
8.  Assign the base registration point to the rack in the *Base Reg. Point* field.
9.  Activate the *Temporary Rack* checkbox if the rack is a temporary rack.
10. Click on the icon button [Save] to save the entries.

**This is how you create several new racks at once**

1.  Open the *Racks* dialog.
2.  Press the icon button [New].
3.  Activate the *Create several racks* checkbox. Underneath the checkbox, the fields *Prefix*, *Start Value*, *End Value* and *BC Start Value* are displayed.
4.  In the *Prefix* field you can enter a letter or letter combination that precedes the start value.
5.  Enter the first number for the racks in the *Start Value* field.
6.  Enter the last number for the racks in the *End Value* field.
7.  In the *BC Start Value* field, enter the barcode number that should be started with.
8.  Select from the *Rack Base Type* combo box whether the racks are regular racks, tray racks or boxes.
9.  Select from the *Rack Type* combo box whether the racks are A racks, harp racks or special racks.
10. If the racks are tray racks, enter the first and last number to be used in the *Slot Number from to* field.
11. Assign the base registration point to the racks in the *Base Reg. Point* field.
12. Activate the *Temporary rack* checkbox if the racks are temporary racks.
13. Click on the icon button [Save] to save the entries.
14. A query is displayed asking you if you really want to insert the corresponding number of racks.

**How to delete a rack**

1.  Open the *Racks* dialog.
2.  Select the rack that is to be deleted from the list.
3.  Press the icon button [Delete].
4.  The system queries whether the record shall actually be deleted.
5.  Click on [Yes]. The record will be deleted.

**How to make changes to a rack**

1.  Open the *Racks* dialog.
2.  Select the rack that is to be changed from the list.
3.  Press the icon button [Change]. The dialog will be released for editing.
4.  Carry out the required changes.
5.  Click on the icon button [Save] to save the entries.

**How to set a rack filter**

1.  Open the *Racks* dialog.
2.  Click on the button [Filter]. The *Rack Filter* dialog opens.
3.  You can filter by the following criteria:
    *   Registration point types
    *   Registration points
    *   Rack name
    *   Rack base type
    *   Rack type
4.  Carry out the required settings.
5.  Click on the button [Accept] to save the entries.
6.  Click on [X] to close the dialog.

**How to delete a rack filter**

1.  Open the *Racks* dialog.
2.  Click on the button [Filter]. The *Rack Filter* dialog opens.
3.  Click on the button [Reset] to clear set filters.
4.  Click on [X] to close the dialog.
5.  All racks are shown again.

**Additional information**
*   ⇨ See Software Reference, "Racks"
*   ⇨ See Software Reference, "Rack Filter"
*   ⇨ See "Scanning Racks and/or Boxes"

#### Staff

**Objectives**
*   Acquire knowledge about the *Employees* dialog.
*   Getting familiar with and understanding how to manage employees.
*   Create and edit employees

**Benefits**
You can define different cost rates for each employee. This enables you to take a closer look at personnel costs. In addition, you can analyze how many employees were involved in processing.

**Note**

| Term | Definition |
| :--- | :--- |
| **Create employees** | An employee must first be created before he can log on at a station. |
| **Registered person** | Is included with the booking. This is the employee responsible for the booking. The registered person remains registered until another name barcode is scanned. |
| **Registration mandatory** | The scanner and A+W Production data can be set so that user registration is mandatory. |

#### Employees

All employees in your company who work with A+W Production must be registered. After an employee has been registered, he can log on at the individual stations. His name is then automatically included in the individual bookings and he is the employee responsible for this booking.

*[Image: Screenshot of the Employees dialog, showing a list of employees with columns for ID, Name, Key, Description, and Barcode.]*

The table above shows which employees have already been created. You can create new employees or change already created employees.

You can define different cost rates for each employee. This enables you to take a closer look at the respective personnel costs.

In addition, it is possible that several employees are registered for one station. Accordingly, you will know how many employees were involved in processing.

You will find a detailed description of the individual fields in the software reference.

> **Column headers can be configured as desired**
> The headers of the individual columns can be configured as desired. It is therefore possible that the headers shown here do not correspond to the headers in your installation.

**Additional information**
*   ⇨ See Software Reference, "Employees"

#### Managing Employees

This module will show you how to create new employees and edit or delete them.

**How to create a new employee**

1.  Open the *Employees* dialog.
2.  Press the icon button [New].
3.  Enter a unique number for the employee in the *Number* field.
4.  Enter the name of the employee in the *Name* field.
5.  The *Description* field allows you to enter information about the employee.
6.  Enter the employee's personnel number in the *Personnel No.* field. This number can be requested from the Payroll office or Accounting.
7.  Enter the barcode number for the employee in the *Barcode* field. In the case of a 9-digit barcode, this might be the combination of the *Number* and *Personnel No.* fields. Example: the employee has number 60, the personnel number is 51 - this results in the barcode 600000051.
8.  Click on the icon button [Save] to save the entries.

**How to delete an employee**

1.  Open the *Employees* dialog.
2.  Select the employee who is to be deleted from the list.
3.  Press the icon button [Delete].
4.  The system queries whether the record shall actually be deleted.
5.  Click on [Yes]. The record will be deleted.

**How to make changes to employee data**

1.  Open the *Employees* dialog.
2.  Select the employee who is to be changed from the list.
3.  Press the icon button [Change]. The dialog will be released for editing.
4.  Carry out the required changes.
5.  Click on the icon button [Save] to save the entries.

**Additional information**
*   ⇨ See Software Reference, "Employees"

#### Status

**Objectives**
*   Acquire knowledge about the *Status Values* dialog.
*   Getting familiar with and understanding different status values

**Benefits**
In order to obtain meaningful analyses, a certain booking discipline must be adhered to.

**Definitions**

| Term | Description |
| :--- | :--- |
| **Status values** | Describe the status of an object |
| **Machine status** | Ready, off, malfunction, maintenance, break, ... |
| **Product status** | Reject, deficiency, ... |
| **Rack status** | Empty, ready, shipped, ... |
| **Registration point status** | Ready, shipped, empty, ... |
| **Action status** | OK, abort, accept, ... |

**Note**
Work interruptions must always be logged.

#### Status values

Recording the actual object status within production is the basic principle of A+W Production.

In order to obtain meaningful data analyses, the master data must be maintained and it is absolutely necessary to book data (quantities and objects) correctly and promptly.

Status values affect the following A+W Production objects:
*   Unit/group
*   Rack
*   Registration points
*   Staff

**Unit/group**
The purpose of this is to enter the status of a lite and/or unit or a product. The following status values are available for example:
*   Not yet produced
*   Reject
*   Defect
*   Ready for shipment

**Rack**
The purpose of this is to enter the status of a rack. Racks can have the following statuses, for example:
*   Empty
*   Full
*   Off site
*   Ready for shipment

**Registration point**
The purpose of this is to enter the status of a registration point. Registration points can have the following statuses for example:
*   Start
*   To
*   Off

It may be necessary to interrupt work at a registration point during an ongoing production process. These interruptions must always be logged.

Possible reasons for an interruption:
*   Machine maintenance
*   Machine failure
*   Breaks
*   Set-up times

**Action barcode**
Apart from entering the aforementioned status values, it is also possible to scan different actions. They include, e.g.:
*   OK
*   Cancel
*   Rotate
*   Next row

*[Image: Screenshot of the Status Values dialog, showing a list of statuses like Breakage, Defect, Start, ReadyForDelivery, etc.]*

The table above shows which status values have already been created. You can create new status values or change already created status values.

> **Column headers can be configured as desired**
> The headers of the individual columns can be configured as desired. It is therefore possible that the headers shown here do not correspond to the headers in your installation.

**Additional Information**
*   ⇨ See Software Reference, "Status Types"
*   ⇨ See "Scanning the Status"

#### Managing Status Values

This module will show you how to create new status values and edit or delete them.

**How to create a new status value**

1.  Open the *Status Values* dialog.
2.  Press the icon button [New].
3.  Enter a unique number for the status value in the *Status Value Number* field.
4.  Enter the name of the status value in the *Name* field.
5.  Enter information about the status value in the *Description* field, e.g. **tool change**.
6.  Enter the text that is to be displayed in the lists in the *Text for Lists* field.
7.  Enter the 9-digit barcode number for the status in the *Barcode* field.
8.  Select the required type from the *Status Type* combo box.
9.  Activate the *AWRack Info* checkbox if the rack server should be notified in the event of a change of this status.
10. Select the required status from the *AWRack Status* combo box.
11. Click on the icon button [Save] to save the entries.

**How to delete a status**

1.  Open the *Status Values* dialog.
2.  Select the status that is to be deleted from the list.
3.  Press the icon button [Delete].
4.  The system queries whether the record shall actually be deleted.
5.  Click on [Yes]. The record will be deleted.

**How to make changes to status data**

1.  Open the *Status Values* dialog.
2.  Select the status that is to be changed from the list.
3.  Press the icon button [Change]. The dialog will be released for editing.
4.  Carry out the required changes.
5.  Click on the icon button [Save] to save the entries.

**Additional information**
*   ⇨ See Software Reference, "Status Types"
*   ⇨ See "Scanning the Status"

### Data Entry

This subject shows you the methods and locations for entering data in production.
This includes the following training modules:
*   "Scanner"
*   "Barcodes"

#### Scanner

**Objectives**
*   Getting familiar with different scanners
*   Getting to know and understanding their functionality
*   The scanner configurations

**Benefits**
Using scanners will assist you in substantially reducing your workload and it saves time.

**Definitions**

| Term | Definition |
| :--- | :--- |
| **Online scanners** | Do not have any memory and the scanner data must be directly transmitted to the connected system. If the connection is interrupted, scanned data will be lost. |
| **Offline scanners** | Have a memory which can temporarily save the scanned data and transfers it when connected with the system. |
| **Serial scanners** | Are used at the terminals, for example. The scanner will not save information temporarily, i.e. without connection to the network, data will be lost. |

**Note**
Apart from their operating system, scanners need software that performs the required functions.

##### Scanner Types

In barcoding, different scanner types are used. Basically, there are online and offline scanners. Scanner selection is highly individual and depends on a variety of factors, e.g.:
*   How many scanners with different logs shall be used?
*   Where shall the scanners be used?
*   Which operating radius do they have to cover?

There are further factors that need to be discussed with the customer directly on site.

**Online scanners**
Online scanners include the line scanners and serial scanners which normally have no memory so that they have to transfer the scanned data directly to the connected system. If the connection is interrupted, scanned data will be lost.

**Denso scanners (WLAN)**
These scanners are WLAN-enabled and communicate directly with AWPort. They have a display and a buffer system for buffering data. Notifications to users can be sent via the built-in display and the scanner's menu structure. If the data transfer is interrupted (e.g. outside the range of the receiving station), data will be temporarily saved in the scanner and transferred when the connection has been re-established. These scanners are used in the shipping area, for instance.

*[Image: Denso online scanner]*

**Serial scanners**
The serial scanners are used at the *Production Terminals* or in connection with *AWPort-Light* as free online scanners. In connection with the *Production Terminals*, they are normally allocated to a fixed registration point (configurable) and replace the keyboard. Bookings are made by the connected *Production Terminal*.

With *AWPort Light*, these scanners can be used as free online scanners wherever a *Production Terminal* is not required. These scanners are robust and reasonably priced. However, they do not have a display or a temporary memory. Notifications to users can be issued only to a certain extent. As these scanners normally do not have a buffer system, scanned data will be lost if the data transfer is interrupted (e.g. outside the range of the receiving station).

**Offline scanners**
The use of offline scanners in an A+W Production environment is subject to special restrictions. Offline scanners are barcode readers that collect barcode registrations and transfer them together at a later stage. As the transfer usually has to be released manually, data registered via offline scanners will be analyzed (much) later than that collected by online scanners. These scanners require well-organized and disciplined working!

##### The scanner configurations

Scanner configurations are multi-layered. Apart from their operating system, scanners need software that performs the required functions. This software is supplied by A+W and has to be transferred to the scanner and configured there.

Furthermore, scanners have to be registered with the A+W Production system.

The necessary configuration steps are usually performed by A+W but can also be executed by specially trained staff.

> **Scanners in practice**
> Currently, WLAN scanners type BHT800BW are deployed almost exclusively. The advantage of this type is that the collected data is always available online.

> **Documentation of configuration**
> Documentation, including the customized configuration, is part of the project planning phase; it will be saved and kept on the customer's computer.

#### Barcodes

Scanners usually require barcodes. Every person, registration point, rack, etc. gets a unique number which is encoded as a barcode for the scanner. These numbers are defined jointly by A+W Software GmbH and the customer during the project planning phase. These barcodes are provided, for example, by an A+W Production report.

Should you need new barcodes for persons, registration points, or racks/boxes, start the report and print the required barcodes.

**Additional information**
*   ⇨ See Software Reference, "Barcode Options"
*   ⇨ See Software Reference, "Barcode Types"

### Booking Examples

This subject shows you how to book correctly.
This includes the following training modules:
*   "Scanning Sequence"
*   "Scanning Units"
*   "Scanning in Dispatch"
*   "Scanning Registration Points"
*   "Truck Registration Point"
*   "Scanning Racks and/or Boxes"
*   "Scanning the Status"
*   "Correcting Erroneous Entries"

#### Scanning Sequence

The following examples shall describe the scanning sequence to be obeyed. To keep the examples quite clear, we have refrained from showing the entire display chain, i. e. we assume that when units are scanned, the scanner has been registered at a registration point, the user has scanned his personal barcode, etc. The total scanning sequence is the combination of the listed examples, and depends on the registration point.

When scanning, first of all, the scanner is always prepared for scanning by registering the person working with it (optional), registering the registration point at the scanner, followed by the other bookings, normally rack registration.

Registration of the person, registration point, scanning the status, etc. only affects all future bookings such as scanning a unit which is then saved in the system with all this information by ALCIM Booking.

**Scanning sequence:**

1.  The user operating the scanner should scan his personal barcode at the start of his shift/scanning. This information will be saved with every scan and serves for analysis purposes later. If this barcode is not scanned, a configurable default value will be saved in the database. A (new) name barcode can be scanned anytime, even after the scanner has been registered at the registration point, e.g. when the operator at a registration point changes.
2.  The registration point where the scanner is used must always be known to the scanner. Every section, machine, truck registered as a registration point has its own barcode. These can be: cutting, IG line 1, IG line 2, furnace, dispatch, truck 1, truck 2, etc.
3.  The rack (box) where the units are stacked has to be scanned, i.e. registered with the scanner. If there are several racks at the registration point, you always have to scan the rack to be currently loaded. Exception: In Dispatch, units are also booked directly to the registration point (truck) (see also Special case truck).
4.  The units: After items 1-3 have been scanned, the units to be stacked or those whose status has changed (e.g. reject report) are scanned.

**Description**
`<Text>` the text in pointed brackets shows the barcode to be scanned (registration point, rack, status, unit, etc.).
The row `<Begin> <Rack> <Unit1> <Unit2> <Unit3 ...>` means: Scan the status `<Begin>`, then the rack `<Rack>` onto which the units should be placed and then all units `<Unit>` in the order in which they should be placed on this rack.

> **Caution with barcode <Begin>**
> The barcode `<Begin>` always resets the rack, box, truck, etc. to empty on the barcode side (reset)! If there were still units present according to barcoding, e.g. on the rack, they will be assigned to the *Error Rack* registration point (see Error Rack)!
> These remaining units according to barcoding can only occur because of forgotten scans, incorrect labels (incorrect readings), etc.!

#### Scanning Units

This module shows you how to scan units.

**How to scan a unit to an empty rack (rack will be emptied by barcoding)**

1.  Register an empty rack with the scanner: `<Begin> <Rack>`
    *[Image: Barcode for "begin" and a transport rack]*
2.  Scan the label of the unit.
    *[Image: Barcode label on a lite]*
    `<Unit 1>`
    `<Unit 2>`
    `<Unit 3>`
    `<Unit 4>`
    ...

**How to scan a unit to a rack that already contains units**
`<Rack> <Unit 1> <Unit 2> <Unit ...>`

**How to scan reject report units**
`<Breakage> <Unit 1> <Breakage> <Unit 2> <Breakage> <Unit ...>`

**How to scan delivery units**
`<Shipped> <Unit 1> <Shipped> <Unit 2> <Shipped> <Unit ...>`

**How to scan units to an empty registration point: Special case Truck**
`<Begin> <RegPoint> <Unit 1> <Unit 2> <Unit ...>`

**How to scan units to a registration point that already contains units**
`<RegPoint> <Unit 1> <Unit 2> <Unit ...>`

**Additional information**
*   ⇨ See "Lites or Units"

#### Scanning in Dispatch

Dispatch needs special attention with regard to barcoding. There are units, racks, boxes, etc. at this registration point, but also trucks which are registration points as well, and form the last link in the production chain. Usually, Denso online scanners are used here.

**General procedure:**

1.  First scan the name tag (it can be scanned again any time)
    `<Schmidt>`
    *[Image: "HELLO, MY NAME IS: Schmidt" name tag]*

2.  Register the registration point with the scanner. Then scan *Dispatch Area* from the list.
    *   `<Dispatch Area>`
    *[Image: Barcode for "Shipping Area"]*

3.  Scan the rack that the units should be placed on.
    *   `<Rack 1>`
    *[Image: Transport rack]*

4.  Scan the label of the unit.
    `<Unit 1>`
    `<Unit 2>`
    `<Unit 3>`
    `<Unit 4>`
    *[Image: Barcode label on a lite]*

> **Note**
> Please stick to the scanning sequence if you want or have to load units and racks/boxes at random!

**Additional information**
*   ⇨ See "Scanner"
*   ⇨ See "Truck registration point"
*   ⇨ See Software Reference, "Registration Points"

#### Scanning Registration Points

Each registration point has its own barcode. Registration point examples:
*   Cutting,
*   IG line 1,
*   IG line 2,
*   Furnace,
*   Dispatch,
*   Truck1,
*   Truck2
*   etc.

**How to scan units to an empty registration point (registration point will be emptied by barcoding): Special case Truck**

1.  Register a new registration point with the scanner: `<Begin> <RegPoint>`
    *[Image: Barcode for "begin"]*
2.  Scan the label of the lite/unit.
    `<Unit 1>`
    `<Unit 2>`
    ...

**How to scan units to a registration point:**

1.  Register the registration point with the scanner: `<RegPoint>`
2.  Scan the label of the lite/unit: `<Unit 1> <Unit 2> <Unit ...>`

**How to scan units to different registration points:**
`<RegPoint 1> <Unit 1> <Unit 2>`
`<RegPoint 3> <Unit 3> <Unit 4> <Unit 5>`
`<RegPoint 1> <Unit 6>`
`<RegPoint 2> <Unit 7> <Unit 8> <Unit 9>`
...

**How to scan racks to a registration point:**
`<RegPoint> <Rack 1> <Rack 2> <Rack ...>`

**How to scan racks to different registration points:**
`<RegPoint 1> <Rack 1> <Rack 2>`
`<RegPoint 2> <Rack 3>`
`<RegPoint 1> <Rack 4>`
...

**How to scan a registration point ready:**
`<Ready> <RegPoint>`

**How to scan the delivery Truck or Trailer:**
`<Shipped> <RegPoint>`

**Additional information**
*   ⇨ See Software Reference, "Registration Points"

#### Truck Registration Point

This module shows you how to scan the Truck registration point.

**General procedure:**

1.  First scan the name tag (it can be scanned again any time)
    `<Schmidt>`
    *[Image: "HELLO, MY NAME IS: Schmidt" name tag]*

2.  Register the new truck with the scanner.
    `<Begin> <Truck1>`
    *[Image: Barcode for "begin" and a semi-truck]*

3.  or register a partly loaded truck with the scanner.
    `<Truck2>`

4.  Scan the label of the unit.
    `<Unit 1>`
    `<Unit 2>`
    ...
    *[Image: Barcode label on a lite]*

**Exercises: Loading an empty and a partly loaded truck**

Truck 1 (empty) and truck 2 (partly loaded) shall be loaded. The loading sequence is free, i. e. the trucks, racks and units can be loaded at random.

**Loading an empty and a partly loaded truck**
1.  Register truck 1 (RP) at the scanner: `<Begin> <Truck1>`
2.  Book units directly to truck 1: `<Unit 1> <Unit 2> <Unit 3>`
3.  Book racks to truck 1: `<Rack 1> <Rack 2>`
4.  Register truck 1 again. Thus, the previous rack will be logged out and the following units can be booked directly on the truck. If this step does not take place, the following units will be booked to the previous rack (rack 2 on truck 1).
    `<Truck1>`
5.  Book units directly to truck 1: `<Unit 4> <Unit 5>`
6.  Book racks to truck 1: `<Rack 3> <Rack 4> <Rack 5> <Rack 6>`
7.  Register truck 2 (RP) at the scanner. This de-registers truck 1 automatically: `<Truck2>`
8.  Book racks to truck 2: `<Rack 9> <Rack 10> <Rack 11>`
9.  Register truck 2 again. Thus, the previous rack will be logged out and the following units can be booked directly on the truck. If this step does not take place, the following units will be booked to the previous rack (rack 11 on truck 2).
    `<Rack 2>`
10. Book units directly to truck 2: `<Unit 6> <Unit 7> <Unit 8> <Unit 9>`
11. Book racks to truck 2: `<Rack 12><Rack 13>`
12. Register truck 1 (RP) at the scanner. This de-registers truck 2 automatically.
    `<Truck1>`
13. Book racks to truck 1: `<Rack 14> <Rack 15>`
14. Register truck 1 again. Thus, the previous rack will be logged out and the following units can be booked directly on the truck.
    `<Truck1>`
15. Book units directly to truck 1: `<Unit 10> <Unit 11>`
16. Loading of truck 1 is completed. The trigger time for truck 1 starts.
    `<Shipped > <Truck 1>`
17. Register truck 2 at the scanner. This de-registers truck 1 automatically.
    `<Truck2>`
18. Book racks to truck 2: `<Rack 9> <Rack 10> <Rack 11>`
19. Loading of truck 2 is completed. The trigger time for truck 2 starts.
    `<Shipped> <Truck 2>`

> **Note**
> Please stick to the scanning sequence if you want or have to load units and racks/boxes at random!
> When loading a truck, racks, boxes, and units can be allocated to the truck registration point. Please make sure that the units which are directly loaded onto the truck (registration point) are not booked to a previously loaded rack/box. Always finish loading a truck with the status booking `<Shipped> <Truck>`.

#### Scanning Racks and/or Boxes

**Prerequisite:** The employee's name and the current registration point must be scanned.

**How to scan a unit to an empty rack (rack will be emptied by barcoding)**
1.  Scan an empty rack: `<Begin> <Rack>`
    *[Image: Barcode for "begin" and a transport rack]*
2.  Scan the label of the unit.
    `<Unit 1>`
    `<Unit 2>`
    ...

**How to scan a transport rack ready for shipment**
`<Ready> <Rack 1> <Ready> <Rack 2> <Ready> <Rack ...>`

**How to scan the delivery Racks/Transport Racks**
`<Shipped> <Rack 1> <Shipped> <Rack 2> <Shipped> <Rack ...>`

**How to scan racks to the truck**
`<RegPoint> <Rack 1> <Rack 2> <Rack ...>`

**Additional information**
*   ⇨ See Software Reference, "Racks"

#### Scanning the Status

Scanning a status barcode results in various barcoding activities in the background that are important for the entire production controlling. If a truck is assigned the `<Shipped>` status for example, this status will be applied to the entire load (racks, boxes, units, etc.); the load will be booked to the (system-) internal registration point 11 (Shipped).

The status barcode describes the status of an object, e.g. a unit (broken etc.), a rack (empty, complete, shipped/<Begin>, <Shipped>, <Broken>, <Ready>, etc.).

The status must **always** be scanned before the object (rack, unit, etc.). If several objects are to be assigned the same status, the status must be scanned separately for every object (`<Status> <Object> <Status> <Object>`).

**How to scan the status Reject Report Units**
`<Breakage> <Unit 1> <Breakage> <Unit 2> <Breakage> <Unit ...>`

**How to scan the status Delivery Units**
`<Shipped> <Unit 1> <Shipped> <Unit 2> <Shipped> <Unit ...>`

**How to scan the status Delivery Several Racks**
`<Shipped> <Rack 1> <Shipped> <Rack 2> <Shipped> <Rack ...>`

**How to scan the status Delivery Truck/Trailer (complete the loading) and Start the Trigger Time**
`<Shipped> <RegPoint>`

**How to register an empty rack (racks will be emptied by barcoding)**
`<Begin> <Rack>`

**How to register an empty registration point (registration point will be emptied by barcoding): Special case Truck**
`<Begin> <RegPoint>`

> **If the <Status> is scanned several times**
> If the status is scanned several times in a row `<Status1><Status2><Status3><Object>`, the last scanned status will be applied to the object, in this example `<Status3><Object>`. The barcode engine checks the bookings and will reject those that are not plausible, e.g. two status bookings in succession.

> **Caution for setting status to <Begin>:**
> The status `<Begin>` resets the object (rack, truck, etc) with respect to the registration point, i.e. to empty! If there were still units present according to barcoding, (e.g. on the truck or rack), they will be automatically assigned to the *Error Rack* registration point.
> Always finish loading a truck with the status booking `<Shipped> <Truck>`.

**Additional information**
*   ⇨ See Software Reference, "Status Types"

#### Correcting Erroneous Entries

It is possible to correct erroneous entries with a new, correct booking! The additional booking is saved in the booking history but has no further effects apart from this correction.

**Example:**
If units have been booked to a rack instead of the registration point by mistake, this error can be corrected by first scanning the registration point and then the unit (to be repeated for every incorrectly scanned unit).
`<RegPoint> <Unit 1> <Unit 2> <Unit ...>`

### Production Terminals

This subject will provide you with a brief overview concerning the different production terminals. This includes the "Introduction" module.

#### Introduction

**Objectives**
*   Getting familiar with different terminals
*   Getting to know and understanding their functionality

**Benefits**
The Production Terminals support you when it comes to loading the lites of a unit from the rack to production (e.g. the line) in the correct sequence. To work efficiently, you have to understand the functioning of the terminals; you must also be capable of handling daily recurring situations.

**Definitions**

| Terminal | Usage |
| :--- | :--- |
| **Production Terminal IG** | Is used at the IG line. |
| **Production Terminal TG** | Is used at the TG line. |
| **Production Terminal LG** | Is used at the LG line. |
| **Production Terminal Order** | Is used wherever large quantities are booked. |
| **Production Terminal Manual Cutting** | Visualizes the work schedule for the lites to be cut at the manual cutting table. |
| **Production Terminal Processing** | Is used at the processing machines. |
| **Production Terminal Edit** | Is used in the shipping office. |

**Note**
Prerequisite for the use of the production terminals is an installed barcode manager (A+W Production).

Production Terminals are control stations for different work stations. Among other things, they are used to show and schedule the processing of lites according to various criteria, to book work performed, to report reject, to create subsequent parts automatically, or to create production statistics. Production terminals are typically used for:
*   Cutting
*   IG line
*   TG furnace
*   LAMI line
*   Dispatch

Control stations visualize and control individual processing steps and can be configured individually. A+W control stations can be used to print labels and reports online, and enter reject including all necessary information. Operation of the control stations is easy and uniform. These intelligent systems enable you to inform your customers of the current state of products at any time.

*[Image: Diagram showing an overview of a production landscape with various terminals, including Terminal Manual Cutting, Terminal Processing, Terminal TG-In/Out, Terminal LG-In/Out, and Terminals for IG Assembly.]*

As every workstation in production requires different information, there are standard terminals configured for the various processes and work flows.

#### A brief explanation of the individual production terminals:

*   **Terminal Manual Cutting**: Visualizes the work schedule for the lites to be cut at the manual cutting table.
*   **Terminal Order**: Is used wherever large quantities are booked.
*   **Terminal Processing**: Is the control station version used with the processing machines, automatically controlling the machines. This module provides detailed information on the processing steps to be performed including true-to-scale production drawings.
*   **Terminal IG-In**: Is installed at the IG line entrance and visualizes the work schedule for the lites to be produced for a batch or a logical production rack/harp rack, in production sequence.
*   **Terminal IG-Assembly**: Is installed between the visual check of lites after the washing machine, and in front of the spacer applicator, visualizing the technical data including the spacer data for each unit to be produced.
*   **Terminal IG-Out**: Installed at the IG line exit and shows the technical and shipping-related data for each unit produced.
*   **Terminal TG-In**: Is the display system at the furnace entry. It shows the furnace bed load and is controlled by the operator. All lites are registered at the scanner; their geometry is checked for completeness of processing.
*   **Terminal TG-Out**: This is the display system at the furnace exit. All lites registered at the furnace entry are displayed based on the clock rate. If defined, the user will get information as to the further use or on stacking in the shipping area.
*   **Terminal Edit**: Is the control station version that is normally used in the shipping office for rebooking units, lites, or groups and for managing off-site racks.
*   **Terminal LG-In**: Installed at the LAMI line entrance, it visualizes the work schedule for the lites of a batch or a logical production rack/harp rack to be produced, in production sequence.
*   **Terminal LG-Assembly**: Installed in the clean room, it shows the work schedule as soon as a lite or unit has been booked at Terminal LG-In. This leaves ample time for cutting the necessary film layers.

> **Production terminals**
> Please see the Production Terminal manual for detailed information on the individual terminals.

### Reject Management

This subject shows you how to handle broken lites.

#### Overview

**Objectives**
*   Getting familiar with how to handle rejects.

**Benefits**
Manual input is not required and as a result the rejects are remade faster. Additional communication between the employees is also not required and thus are avoided.

**Definitions**
*   **Rejects Pool**: You will find an overview of the rejects in the Rejects Pool.

**Note**
*   **Rejects report**: The rejects report is executed at each *Production Terminal* or via scanner.
*   **Labels**: Labels are printed automatically at a central printer.
*   **Automatic remake**: The automatic remake is executed on the residue plate or by table optimization in the *A+W Realtime Optimizer*.

#### Reject Handling (Internal)

When units are reported broken, various internal actions are triggered. After a reject report, all information on the original unit plus all subsequent parts and remakes of subsequent parts will be saved in the database.

Subsequent parts will always be provided with the original barcode number. The barcode number of the original lite is provided with an index in the case of a reject report.

The table shows the changes resulting from the reject reports with regard to the individual flags and barcode numbers.

**Barcoding Reject Handling**

| Barcode | Registration point | Rack | Reject | Subsequent parts index | Description |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 012345678 | Drilling | 15 | 0 | 0 | E1 |
| 012345678 001 | Drilling | 15 | 1 | 0 | E2 (Reject 1) |
| 012345678 | - | - | 0 | 1 | E3 |
| 012345678 002 | Furnace | 20 | 1 | 1 | E4 (Reject 2) |
| 012345678 | - | - | 0 | 2 | E5 |

**Description of table**
*   **E1**: The lite with barcode 012345678 is at the Drilling registration point, on rack 15. The lite has not been reported broken; the reject flag is zero. This is the original lite as the subsequent parts index is zero.
*   **E2**: The lite with barcode 012345678 is reported broken at the Drilling registration point. The reject flag is set. A three-digit index is added to the barcode number. Index 001 shows that this is the first reject.
*   **E3**: A subsequent part is created and is provided the original barcode number 012345678. In addition, the subsequent part index is increased by one (1). The subsequent part index distinguishes the subsequent part from the original lite. As the unit has not been entered, it is not allocated to a registration point.
*   **E4**: The subsequent part has made its way in the production area up to the furnace where it is reported broken. The reject flag is set. A three-digit index is added to the barcode number. Index 002 shows that this is the second reject.
*   **E5**: The second subsequent part is created and is provided with the original barcode number 012345678. In addition, the subsequent part index is increased by one (2). The subsequent part index distinguishes the subsequent part from the original lite. As the unit has not been entered, it is not allocated to a registration point.

> **Note**
> When you print labels for the subsequent parts or at reporting, the above-mentioned values and flags can be analyzed and taken into account. This is usually defined during the project planning phase and can be adapted to the current needs if required. Please ask A+W Software GmbH for available options.

> **Tip**
> You can use filters for the A+W Production views. Standard filters have been set for the barcode manager views which may not show units with a subsequent part index. To display these units, disable all filters (unfiltered). The name of the standard filter is Active!

> **Views and filters**
> For more information on the views and filters, please refer to the A+W Production manual.

### Statistics, Reporting and Monitoring

This subject will introduce you to the reports and different analyses.
This includes the following training modules:
*   "Barcode Reporting"
*   "Monitoring: A+W Dashboard"
*   "Statistics: A+W Discovery"

#### Overview

**Objectives**
*   Getting familiar with standard barcode reports.

**Benefits**
Using the standard reports, you will have an overview of the current status of your production at any time. This will save you time and effort and you are always able to provide your customers with accurate answers.

**Definition**
*   **Reports**: Are flexible tools to control and analyze the production.

**Note**
*   **Standard reports**: Are part of A+W Production
*   **Individual reports**: Can be created at customers' requests at any time.

#### Barcode Reporting

The described reports are standard barcode reports. It is possible to customize reports and create new reports. The reports are a flexible and powerful production control and analysis tool. Please contact A+W Software GmbH; we are glad to advise you and to perform the necessary changes, extensions and amendments or create new, customized reports.

> **Note**
> General reports analyzing a registration point usually show all units allocated to this registration point! If a partly loaded rack is registered at the IG line exit (registration point 1612) for instance to load IG units, the units already existing on this rack will also be booked to registration point 1612! To run analyses which show only the throughput of the IG line, for example, you will require amended reports.

##### Loading the Reports

Reports can be loaded via the A+W Production menu structure. The individual Production Terminals provide reports depending on their function. Shortcuts to reports can be saved on the PC desktop.

> **Note**
> The A+W Production menu structure is dynamic. Menu entries for the Barcode Manager are visible only if a Barcode Managerview is open.

##### Examples of Standard Barcode Reports

Depending on the report, you can enter or select individual parameters for the report. This can be the display time, the registration point to be analyzed, etc.

> **Note**
> The sectional display of reports will give you an overview of the A+W Production reports.

**Unit list**
*Menu: Lists > Unit list*
The unit list shows all parts that are selected in a A+W Production view exact to units. Depending on the filter in the A+W Production view, spacer bars, etc. are also shown.
*[Image: A+W Unit-List report showing columns for Itm, Label, Width, Height, Description, Registration Point, Rack, etc.]*

**Order overview**
*Menu: Lists > Order List*
The order overview shows you where the individual items (head sections) of the order are located.
*[Image: A+W Order-Overview report showing details for an order, broken down by position, with label, reg-point, rack status, booking time, etc.]*

**Order status**
*Menu: Lists > Order status*
The list provides you with information about the order status.
*[Image: A+W "Status for Order" report showing processing steps for each item, with target and actual quantities and dates.]*

**Loading list**
*Menu: Lists > Loading list*
The loading list shows you the actual load. You can restrict content by using filters.
*[Image: A+W Picking-List report showing items for a customer and route, with order details, description, and status.]*

**Rack load per lite**
*Menu: Lists > Rack load per lite*
The list shows you the load per lite for the entered rack number.
*[Image: A+W Rack Load report for a specific rack, showing all lites on it with order, item, dimension, and booking time.]*

**Rack load per item**
*Menu: Lists > Rack load per item*
The list shows you the load per item for the entered rack number.
*[Image: A+W Rack Load report, similar to the per-lite version but aggregated by item.]*

**Booking history**
*Menu: Lists > Booking history*
This list shows you per order, which bookings have taken place and where.
*[Image: A+W History report showing a detailed log of bookings for a specific label, including registration point, rack, status, and processing details.]*

#### Monitoring: A+W Dashboard

**Objectives**
*   Brief introduction to A+W Dashboard
*   Getting to know the options

**Benefits**
A+W Dashboard shows the important key figures of the crucial production points to ensure a high level of transparency.

**Definitions**
*   **Traffic light**: The traffic light shows the current status of a registration point. You can define the meaning of the colors yourself.

**Note**
*   **Period of time**: Database tables with the A+W Production bookings are used for analyses. Usually a time period of max. 24 hours is taken into account.
*   **Correct display**: You need complete A+W Production bookings for meaningful displays.
*   **Display**: A+W Dashboard can be used both on large monitors in various production departments and mobile terminals such as smartphones.
*   **Malfunctions**: In the event of malfunctions, you can communicate the exact situation and in many cases even suggest your own solutions.

##### Overview

A+W Dashboard shows the important key figures of the crucial production points to ensure a high level of transparency. You get information on specific production areas in real time such as cutting to size, ISO lines, processing and TG production: e.g. you will see the actual degree of utilization, the status of each machine, and the production progress.

This program can be used both on large monitors in various production departments and mobile terminals such as smartphones, tablet computers or PDAs. However, this requires an internet browser and access to this program (address and user account).

A+W Production contains predefined displays, although it can also be adapted to individual machines or departments. This enables you to keep an eye on the critical points of your production and take action wherever necessary.

Database tables with the barcoding bookings are used for analysis. Usually a time period of max. 24 hours is taken into account. This is how A+W Dashboard differs from A+W Discovery which allows statistical analyses over longer periods of time.

The analyses are visualized in different ways. You can zoom in and out of the displays and change pages by swiping.

*[Image: Examples of visualization types in A+W Dashboard: A) Traffic light, B) Pie chart, C) Plot diagram, D) Bar chart, E) Speedometer.]*

You can set up each of these display types to correspond with the demands of your production departments and monitoring.

*   **Traffic light (A)**: The traffic light shows the current status of a registration point. You can define the meaning of the colors yourself. This display makes sense for status displays over very short periods such as showing whether a machine is operating or has broken down.
*   **Pie chart (B)**: The pie chart shows the shares of machine statuses reported over a self-defined period. By default, this represents the past 24 hours. With it, the total of all downtimes of all shifts during the time period can be viewed.
*   **Plot diagram (C)**: This line shows the bookings of a past period of time spread out over a display period such as the bookings of the last hour spread over the display period. One point shows the total per grouping (such as per minute, hour or day).
*   **Bar chart (D)**: The bar chart shows statistical data collected via SQL queries. These statistics have to be available for view configuration.
*   **Speedometer (E)**: The speedometer shows the present capacity utilization. For this purpose, the number of booked pieces during the past hour is analyzed. The red-yellow-green marking indicates how the number of pieces are assessed.

> **Correct display only if barcoding bookings are correct**
> You need complete barcoding bookings for meaningful displays.
> A+W Dashboard links the production software A+W Production and the A+W Production Terminal. The Barcoding data is read out through the PPS Web Service.

> **A+W Dashboard**
> Please see the A+W Dashboard manual for detailed information on this module.

#### Statistics: A+W Discovery

**Objectives**
*   Brief introduction to A+W Discovery
*   Getting to know the options

**Benefits**
A+W Discovery is used to collect, edit, and visualize your business data. Management and controlling staff can analyze this information and use it for their business decisions.

**Definitions**
*   **Pivot table**: Is a special type of table with the option to display data in different ways.
*   **Fiscal year**: Business year for which a company compiles the results of its business in an annual financial statement.

**Note**
*   **A+W Discovery**: Allows you to create long-term analyses of production data.
*   **Analyses**: Analyses can easily be created in the form of pivot tables using Microsoft Excel.
*   **Data provision**: A+W Discovery can provide data from the ERP systems (A+W Enterprise, A+W Business) and the PPS system (A+W Production).
*   **Client-wide analyses**: You can create client-wide analyses.

##### Overview

Constantly growing demands on modern ERP and PPS systems require more and more powerful controlling and control mechanisms. This is due to tax and legal conditions, and the necessity of analyzing the product portfolio, productivity, and capacity utilization from different points of view.

A+W Discovery is the state-of-the-art Business Intelligence System of A+W Software GmbH tailored to the special needs of modern glass producers and processors. Its setup and integration with the PPS system A+W Production allows evaluating and offsetting statistical parameters and indices from different points of view and deducing the necessary strategic, commercial, or production-related decisions and steps.

You can, for instance, collect data revealing the gross margin and the sales volume of certain locations or subsidiaries for a defined time frame (e.g. month or year). This enables you to adjust your cost structures accordingly if necessary, and motivate your staff and sales partners to achieve an increase in turnover in the following year. Version 5.4 additionally implements the fiscal year and fiscal quarter.

You will also be able to analyze key production figures like the quantity of reject per work station or machine downtimes within a defined time frame.

*[Image: Screenshots of A+W Discovery in Excel, showing pivot tables and charts for rejects, produced quantities, and machine activity.]*

Apart from that, A+W Discovery comes with predefined A+W standard reports which allow comparing and aggregating meaningful PPS data. This will put you in full control of all commercial and production-relevant data, products, resources, costs, times, and capacities.

> **A+W Discovery**
> Please see the A+W Discovery manual for detailed information on this module.

## Software Reference

### Overview

The software reference provides information on the following subjects:
*   Master Data

> **Dialogs are accessible from different points**
> Please note that there are various ways of opening functions and dialogs. The corresponding dialogs will only be described once in this document.

### Master Data

*Menu: Master Data > Barcoding*

The Barcoding menu offers the following items:
*   **Barcode Options:** This section is maintained by A+W Software GmbH.
*   **Barcode Types:** This section is maintained by A+W Software GmbH.
*   **Registration Point Types:** This section is maintained by A+W Software GmbH.
*   **Registration Points:** Use this section to manage your registration points. (⇨ See "Registration Points")
*   **Racks:** Use this section to manage your racks. (⇨ See "Racks")
*   **Rack Filters:** Use this section to manage rack filters. (⇨ See "Rack Filter")
*   **Status Types:** This section is maintained by A+W Software GmbH.
*   **Status Values:** Use this section to manage status values. (⇨ See "Status Values")
*   **Employees:** Use this section to manage your employees. (⇨ See "Employees")
*   **Column Assignment:** This section is maintained by A+W Software GmbH.
*   **Columns:** This section is maintained by A+W Software GmbH.
*   **Barcoding Post-Processing:** This section includes post-processing for the event that problems have occurred during data processing. (⇨ See "Post-Processing")

#### Barcode Options

*Menu: Master Data > Barcoding > Barcode Options*

*[Image: Screenshot of the Barcode Options dialog with settings for quantity treatment, label mode, and barcode length.]*

This section addresses the barcode options.

> **Data relevant to the system**
> This entire section is created and changed as required by A+W Software GmbH. Please do not change anything. The data in this dialog is relevant to the system.

#### Barcode Types

*Menu: Master Data > Barcoding > Barcode Types*

*[Image: Screenshot of the Barcode Types dialog, defining types like UNIT, GROUP, RACK, etc., with their IDs and length.]*

This section determines the behavior of barcodes.

> **Data relevant to the system**
> This entire section is created and changed as required by A+W Software GmbH. Please do not change anything. The data in this dialog is relevant to the system.

#### Registration Point Types

*Menu: Master Data > Barcoding > Registration Point Types*

*[Image: Screenshot of the Registration Point Types dialog, defining types like Production Area, Shipping Area, Truck, etc. and their behaviors.]*

This section determines the behavior of registration points.

> **Data relevant to the system**
> This entire section is created and changed as required by A+W Software GmbH. Please do not change anything. The data in this dialog is relevant to the system.

#### Registration Points

*Menu: Master Data > Barcoding > Registration Points*

*[Image: Screenshot of the Registration Points dialog.]*

This dialog is used to define new registration points, or change existing registration points.
Technical info: database table: `AWBAR_STELLEN`

**List of status values**
*   **ID**: Unique number assigned to the registration point.
*   **Name**: Name assigned to the registration point.
*   **Description**: Description that you have given the registration point.
*   **Type**: Type that you have assigned to the registration point.

**Description of fields**
*   **Registration Point No.**: Enter the registration point number in this field. (DB field: `Esnr`)
*   **Barcode**: Enter the registration point barcode in this field. (DB field: `Esbc`)
*   **Name**: Enter the registration point name in this field. (DB field: `Esname`)
*   **Description**: Enter a detailed description for the registration point in this field. (DB field: `Allgbez`)
*   **Text for Production Lists**: Enter a text in this field that is to be displayed in the production lists. (DB field: `Lst1bez`)
*   **Text for Customer Lists**: Enter a text in this field that is to be displayed in the customer lists. (DB field: `Lst2bez`)
*   **Subrow for Barcode Labels**: Enter a text in this field that is to be displayed underneath the barcodes. (DB field: `Barcbez`)
*   **Reg. Point Type**: The combo box shows all registration point types defined in your company. Select the corresponding type. (DB field: `Typ`)
*   **Grouping**: In this field you can group the registration points for analyses regardless of registration point types, e.g. all furnaces of a group. (DB field: `Gruppe`)
*   **Grouping for Working Shifts**: Use this field to group registration points to create working shifts. (DB field: `Shift_Group`)
*   **Current Status**: Use this field to assign a current status to a registration point. The combo box includes all the statuses defined in your company. (DB field: `Zustandnr`)
*   **Restrictions**: This value enables or disables the restriction check and defines the quantity to which the restriction check refers.
    *   `0`: Restriction check is switched off.
    *   `1`: The restriction check refers to the technical production quantity.
    *   `2`: The restriction check refers to the quantity available. All lites which have completed the previous process, are available.
    *   `3`: The restriction check refers to the quantity available. All lites which have completed all previous processes, are available.
    (DB field: `Restriction`)
*   **Over Exceeding**: Enter the quantities exceeded as a percentage in this field. This value is analyzed only if the restriction check is enabled. (DB field: `Overbook`)
*   **Show Produced Parts**: This checkbox controls whether produced parts are shown or not. (DB field: `Show_produced_parts`)
*   **Machine of the Order Entry**: This field shows the machine of the order entry. If you change the entry, the changed machine is reported back. (DB field: `Maschinennr`)

**Description of the fields in section Feedback of Bookings**
*   **Processing Feedback**: Controls whether there will be feedback regarding the processing. If a lite is booked to a registration point, the processing progress is written precisely to the lite into file ST-SD*.ASC.
*   **Rack Feedback**: Controls whether there will be feedback regarding the rack load. If a rack is booked to a registration point, the rack occupation is written precisely to the lite into file ST-SG*.ASC.
*   **Register Rack Load to Rack Server**: Controls whether the rack load should be reported to the rack server.
*   **Unit Feedback (STSU*.asc)**: Use this checkbox to assign the A+W Production labels to A+W Business order items.
*   **Production Feedback**: Use this checkbox to update the current order status in A+W Business.

#### Racks

*Menu: Master Data > Barcoding > Racks*

*[Image: Screenshot of the Racks dialog.]*

This dialog is used to define new racks, or change existing ones.
Technical info: database table: `AWBAR_GESTELLE`

**List of racks**
*   **Name**: Name assigned to the rack.
*   **Rack**: Barcode assigned to the rack.
*   **Type**: Rack type assigned to the rack.

**Description of fields**
*   **Define Multiple Racks**: Activate this checkbox if you want to create several racks at once. The fields *Prefix*, *Start Value*, *End Value* and *BC Start Value* are displayed.
*   **Prefix**: Enter a prefix for the rack names.
*   **Start Value / End Value**: Define the numerical range for the new racks.
*   **BC Start Value**: Enter the starting barcode number.

**Properties section**
*   **Rack Base Type**: Select the rack type (Normal, Tray rack, Crate). (DB field: `Typ_KZ`)
*   **Rack Type**: Select the specific rack type (Furnace bed, A-Rack, Harp rack, AutoClav rack). (DB field: `Typ_KZ`)
*   **Slot Number from... to**: Used for tray racks to show the first and last occupied tray number. (DB fields: `Erstfachnr / Lbelfach`)
*   **Base Reg. Point**: Select the base registration point for the rack. (DB field: `Basisesnr`)
*   **Temporary Rack**: Check to mark the rack as temporary. (DB field: `Tempkz`)

**Batch Data section**
*   **Current RP**: Shows the registration point where the rack is currently located. (DB field: `Esnr`)
*   **Last RP**: Shows the registration point where the rack was previously located. (DB table: `Esnralt`)
*   **Current Status**: Shows the current status of the rack (e.g. delivered, empty, etc.). (DB table: `Zustandnr`)
*   **Last Status**: Shows the previous status. (DB table: `Zustandnralt`)

**Customer Data section**
*   **Customer Number**: Enter the customer number for "off site" racks. (DB table: `Kundennr`)
*   **Customer Name**: Enter the customer name for "off site" racks. (DB table: `Kundenname`)
*   **Delivery Location**: Enter the delivery location for "off site" racks. (DB field: `Lieferort`)
*   **Route Number**: Enter the route number for "off site" racks. (DB field: `Tournr`)

#### Rack Filter

*Menu: Master Data > Barcoding > Rack Filter*

*[Image: Screenshot of the Rack Filter dialog.]*

In this dialog you can create filters yourself to limit the number of displayed racks.

**Description of fields**
*   **Registration Point Type**: Filter by a specific type of registration point.
*   **Registration Point**: Filter by a specific registration point.
*   **Rack Name from to**: Filter by a range of rack names.
*   **Rack Base Type**: Filter by the base type of the rack.
*   **Rack Type**: Filter by the specific type of rack.
*   **Company-Owned Racks**: Enable to filter by company-owned racks only.

#### Status Types

*Menu: Master Data > Barcoding > Status Types*

*[Image: Screenshot of the Status Types dialog.]*

This section determines the behavior of a status.

> **Data relevant to the system**
> This entire section is created and changed as required by A+W Software GmbH. Please do not change anything. The data in this dialog is relevant to the system.

#### Status Values

*Menu: Master Data > Barcoding > Status Values*

*[Image: Screenshot of the Status Values dialog.]*

This dialog is used to define new status values, or change existing ones.
Technical info: database table: `AWBAR_ZUSTAND`

**List of status values**
*   **ID**: Unique number assigned to the status.
*   **Name**: Name assigned to the status.
*   **Description**: Description that you have given the status.
*   **Type**: Type that you have assigned to the status.

**Description of fields**
*   **Status Number**: A unique number assigned to the status. You can overwrite the system's suggestion. (DB table: `Zustandnr`)
*   **Name**: Assign a name for the status in this field. (DB table: `Zustandname`)
*   **Description**: Save a detailed description for the status in this field. (DB table: `Beschreibung`)
*   **Text for Lists**: Enter a text in this field that is to be displayed in the lists. (DB table: `Listenname`)
*   **Barcode**: Enter the barcode for the status in this field. (DB table: `Zustandbc`)
*   **Status Type**: This combo box includes all created status types. Select the corresponding type. (DB field: `Typ`)
*   **AWRack Info**: Use this checkbox to control whether or not the rack server should be notified in the event of a change of this status. (DB field: `Notify`)
*   **AWRack Status**: This combo box includes all AWRack statuses. Select the corresponding status. (DB field: `Awrackstate`)

#### Employees

*Menu: Master Data > Barcoding > Employees*

*[Image: Screenshot of the Employees dialog.]*

This dialog is used to enter new employees, or change existing employee data.
Technical info: database table: `AWBAR_PERSON`

**List of employees**
*   **Number**: Unique ID assigned to the employee.
*   **Name**: Name assigned to the employee.
*   **Personnel No.**: The employee key. It is identical with the ID.
*   **Description**: Description that you have given the employee.
*   **Barcode**: Barcode assigned to the employee.

**Description of fields**
*   **Number**: Enter a unique number for the employee in this field. (DB field: `PersonNr`)
*   **Name**: Enter the name of the employee in this field. (DB field: `PersonName`)
*   **Description**: In this field you can enter additional information relating to the employee. (DB table: `Beschreibung`)
*   **Employee No.**: Enter the employee number in this field. This number will be provided to you by the payroll office or accounting. (DB table: `PersonKey`)
*   **Barcode**: Enter the barcode for the employee in this field. It is compiled from the number and the employee number. (DB field: `Personbc`)

#### Column Assignment

*Menu: Master Data > Barcoding > Column Assignment*

*[Image: Screenshot of the Column Assignment dialog.]*

This section addresses the assignment of columns.

> **Data relevant to the system**
> This entire section is created and changed as required by A+W Software GmbH. Please do not change anything. The data in this dialog is relevant to the system.

#### Columns

*Menu: Master Data > Barcoding > Columns*

*[Image: Screenshot of the Columns dialog.]*

This section addresses the columns.

> **Data relevant to the system**
> This entire section is created and changed as required by A+W Software GmbH. Please do not change anything. The data in this dialog is relevant to the system.

#### Post-Processing

*Menu: Master Data > Barcoding > Post-Processing*

*[Image: Screenshot of the Barcoding Post-Processing dialog.]*

Any problems that may occur during the processing of the barcoding data can be found here. The errors must be corrected!

**Description of fields**
*   **Initialization Only**: If you activate this radio button, only errors that have occurred during the barcoding initialization are shown.
*   **Bookings Only**: If you activate this radio button, only errors that have occurred during booking are shown.
*   **All**: Use this radio button to display all parts that are pending post-processing.
*   **Not Processed**: Use this radio button to limit the displayed data to parts that have not yet been processed.

**Description of buttons**
*   **Repeat**: Use this button to reevaluate the booking record.
*   **Set Processed**: Press this button to clear the display.
*   **Update**: Press this button to update the display.

## Index Barcoding

*   **B**
    *   Barcoding bookings
        *   Continuous booking
    *   Boxes
*   **C**
    *   correct data
*   **D**
    *   Data relevant to the system
        *   Barcode options
        *   Barcode types
        *   Column assignment
        *   Columns
        *   Registration point types
        *   Status types
    *   Denso scanners
    *   Direct objects
    *   Dispatch
*   **E**
    *   Error rack
    *   Expert mode
        *   Overview
*   **I**
    *   Indirect objects
*   **M**
    *   Module
        *   function
*   **O**
    *   Offline scanners
    *   Online scanners
    *   Overview
        *   Expert mode
*   **R**
    *   Rack filter
        *   Company-owned racks
        *   Rack base type
        *   Rack name from ... to
        *   Rack type
        *   Reg. point type
        *   Registration point
    *   Racks
        *   Base reg. point
        *   BC start value
        *   Create multiple racks
        *   Current reg. point
        *   Current status
        *   Customer name
        *   Customer number
        *   Delivery location
        *   End value
        *   Filter
        *   Last reg. point
        *   Last status
        *   Prefix
        *   Rack base type
        *   Rack type
        *   Route number
        *   Slot number from ... to
        *   Start value
        *   Temporary rack
    *   Registration Point
        *   Grouping
        *   Grouping for shifts
        *   Restrictions
        *   Barcode
        *   Current status
        *   Description
        *   Machine for order entry
        *   Name
        *   Number
        *   Processing feedback
        *   Produced parts
        *   Production feedback
        *   Quantities exceeding
        *   Rack feedback
        *   Registration point type
        *   Report rack load
        *   Subrow for labels
        *   Text for customer lists
        *   Text for production lists
        *   Truck
    *   Registration points
        *   Manage
    *   Required knowledge
*   **S**
    *   Scan
        *   Units
    *   Scan units
    *   Scanner
        *   Configuration
        *   Serial scanners
    *   Staff
    *   Standard report
        *   Booking history
        *   Loading list
        *   Order overview
        *   Order status
        *   Rack load per item
        *   Rack load per lite
        *   Unit list
    *   Status
        *   Action barcode
        *   Rack
        *   Registration point
        *   Unit/group
    *   Status barcode
        *   Scan
    *   Status values
        *   AWRack info
        *   AWRack status
        *   Barcode
        *   Description
        *   Status name
        *   Status number
        *   Text for lists
