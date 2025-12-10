---
title: "EN-FUNC-AW_Dashboard"
source: "EN-FUNC-AW_Dashboard.pdf"
tags: ["A+W Dashboard", "Functional Description", "Software for Glass", "KPI Visualization", "Production Monitoring", "Barcoding Service", "Capa View", "Report View"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A functional description of the A+W Dashboard, a web-based service for visualizing production Key Performance Indicators (KPIs). This document outlines the software's features, requirements, and various functional modules, including the core Dashboard, Barcoding Service Views, Capa View, and Report View."
long_description: "This document provides a detailed functional description for the A+W Dashboard, a software solution by A+W designed for the glass industry. The A+W Dashboard is a browser-based application that offers real-time visualization of production data, helping to monitor output, machine capacity, and employee performance through graphical representations. The document covers the core idea behind the program, its key features like real-time monitoring and mobile accessibility, and the technical requirements for its implementation. It breaks down the main components and their functions: the core Dashboard (module 220040) with its Monitor, View, Page, and Control editors; the Barcoding Service Views (module 220041) for displaying booking, processing, and status-based data; the Capa View (module 220042) for capacity and utilization displays; and the Report View (module 220043) for generating PDF reports. Legal information, including trademarks, copyrights, and a disclaimer of liability, is also included."
---

# A+W Dashboard: Functional Description
*A+W - Software for Glass*

***

---
## 1. Content

1.  **Content**
2.  **Notes on this document**
    - 2.1. Trademarks
    - 2.2. Copyrights
    - 2.3. Disclaimer of Liability
3.  **Performance Description**
    - 3.1. Data
    - 3.2. Description
        - 3.2.1. The idea behind the program
        - 3.2.2. Features
        - 3.2.3. Display time period
    - 3.3. Requirements
    - 3.4. List of functions - Dashboard (220040)
        - 3.4.1. Monitor
        - 3.4.2. View editor
        - 3.4.3. Page editor
        - 3.4.4. Control editor
    - 3.5. List of functions – Barcoding Service Views (220041)
        - 3.5.1. Booking-based displays
        - 3.5.2. Processing-based displays
        - 3.5.3. Status-based displays
    - 3.6. List of functions – Capa View (220042)
        - 3.6.1. Capacity display
        - 3.6.2. Detailed view
    - 3.7. List of functions – Report View (220043)
4.  **Contact Address**

## 2. Notes on this Document

This documentation and the software described in it are only licensed and may only be used and copied pursuant to this license. The contents of the documentation are for information purposes only and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. In spite of this, we cannot rule out all mistakes. A+W Software GmbH cannot be held liable for errors or inaccuracies unless they can be attributed to wilful or grossly negligent action.

### 2.1. Trademarks

All hardware and software names mentioned in this documentation may also be registered trademarks or other industrial property rights held by third parties. Copyrights of third parties must be complied with.

### 2.2. Copyrights

© 2015, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation. The documentation can be copied, completely or in part, saved in an archiving system, or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without the written prior approval of A+W Software GmbH.

### 2.3. Disclaimer of liability

A+W Software GmbH does not assume any liability for data errors resulting from the basics of the standard functions provided by Microsoft, Unix or other software and hardware suppliers.

A+W Software GmbH reserves the right to change software data, structure, and interfaces as part of program expansions without prior announcement. All amendments, extensions, database queries, reports, analyses, and interface extensions which have been individually created for our customers and/or machine and software partners as well as all related costs and expenses are to be borne by the customer (customers, machine and software partners). This includes also any necessary long-term costs and efforts for the expansion and adjustment of subsequent program versions. This is necessary to make sure that the commissioned amendments/extensions which have been made or developed for a version will work flawlessly and can be used in the successor version.

## 3. Performance Description

### 3.1. Data

| | |
| :--- | :--- |
| **Product** | A+W Production |
| **Module number** | 220040: Dashboard 220041, 220042, 220043 : data services |
| **Module** | A+W Dashboard |
| **Brief description** | Visualization module for display of various KPIs |
| **Available** | |

### 3.2. Description

The A+W Dashboard is a service with a Web-based interface. A+W Dashboard can be started in the newest version of any browser. The address to the requested server can be saved as a favorite or link on the desktop – like all Internet addresses.

*[Figure - Overview of views]*

#### 3.2.1. The idea behind the program

A+W Dashboard is a tool for visualizing production. It displays the current output and capacity of the machines and employees in graphic form. The A+W Dashboard can, if desired, display reports in PDF format.

For evaluation, the database tables are used with PDC bookings and processings.

#### 3.2.2. Features

A+W Dashboard displays important key figures at decisive points in production, thus ensuring great transparency. You get information on specific production areas in real time such as cutting to size, ISO lines, processing and TG production: e.g. you will see the actual degree of utilization, the status of each machine, and the production progress. This program can be used both on large monitors in various production departments and mobile terminals such as smartphones, tablet computers or PDAs. However, this requires an internet browser and access to this program (address and user account).

This means that the display can be used as an online monitoring tool and decision-making tool if machine states change in the course of a shift or scheduled quantities cannot be met.

In case of faults, the employees can communicate the situation exactly and in many cases suggest their own solution approaches.

A+W Dashboard includes pre-defined displays, however with the use of a pre-defined quantity of display possibilities, it can also be adapted to the respective machine or department. This enables you to keep an eye on the critical points of your production and take action wherever necessary.

#### 3.2.3. Display time period

The time period across which the data can be displayed ranges - depending on the display – from 1 to 14 days.

### 3.3. Requirements

- PDC must be set up and used for the machine performance displays
- The PPS Webservice must be reachable and the report set up for the report display
- In order to be able to use the CapaView, A+W Production Capacity Planning must be set up and used
- The server that hosts the corporate service must have an IIS Version 7 and be reachable via a Web browser for the end devices handling the display
- The end device handling the display must have a current Web browser
- The system relies on the booking content of the tables awbar_booking, pool_teile, pool_bearbeit auf. Deleted and/or archived data cannot be displayed.

### 3.4. List of functions – Dashboard (220040)

The A+W Dashboard is a browser-based environment/application in which data can be displayed. This data must be provided by various services. The dashboard itself - without the associated services - displays no data.

The A+W Dashboard environment offers the following scope of services for the creation and display of prepared content:

#### 3.4.1. Monitor

The monitor is the entry point into the A+W Dashboard. Here, all views set up are displayed. From here, all editors and set-up views can be selected.

You reach the monitor with a current Web browser under the address `//SERVERNAME/Corporate.Web`

#### 3.4.2. View editor

The View Editor allows the creation, changing, and deletion, as well as the exporting and importing of views.

After opening the View Editor, all previously-created views are displayed. From here, you can reach the editing functions with [Edit data record]. There, you can use DragAndDrop to drag already-created pages from a pool into the active view and sort them.

The View Editor can be reached with the Web browser under the address `//SERVERNAME/Corporate.Web/ViewEditor` or it can be selected on the monitor.

#### 3.4.3. Page editor

The page editor allows the creation, changing, and deletion, as well as the exporting and importing of pages.

After opening the page editor, all previously-created pages are displayed. From here, you can reach the editing functions with [Edit data record]. There, you can use DragAndDrop page dividers on the page, shift it, and thus set up a cascaded division of the page. You can drag the controls created into the subdivisions that arise. This way, you can create a customized page.

The page editor can be reached with the Web browser under the address `//SERVERNAME/Corporate.Web/PageEditor` or it can be selected on the monitor.

#### 3.4.4. Control editor

The control editor allows the creation, changing, and deletion, as well as the exporting and importing of controls.

After opening the control editor, all previously-created controls are displayed. From here, you can reach the editing functions with [Edit data record]. There, you can specify the data source and the type of control. Depending on the control selected, additional settings may be displayed.

The control editor can be reached with the Web browser under the address `//SERVERNAME/Corporate.Web/ControlEditor` or it can be selected on the monitor.

### 3.5. List of functions – Barcoding Service Views (220041)

#### 3.5.1. Booking-based displays

The booking-based data can be displayed as tacho or line diagram. Displayed is the number of registered bookings on a registration point. Reproductions and status bookings also count as registered bookings. Each reading/booking is displayed, for example in the case of breakage also the remake (processing 2x).

The time period considered can be set.

**Speedometer**
The tacho displays the number of registered bookings for the set period. In the booking-based displays, the tacho can only display the measurement units (number of bookings, number of status changes).

**Line chart**
The line diagram displays the number of bookings within the set time period on a curve. You can display the average value and the target value using two continuous lines. This way, a deviation upward or downward is easy to spot.

#### 3.5.2. Processing-based displays

The processing-based data can be displayed as tacho or line diagram. It can be set in which unit the display is made: unit or area, linear meters, weight, or efficiency of a registration point. The display of linear meters is only possible for machines that perform edge processings. The data displayed is based on the database tables "pool_teile" and "pool_bearbeit". Imperial measurement/quantity units (inches, sqft, lbs) cannot be displayed. Only data in the metric system (dimension/quantity unit) can be displayed. The time period considered can be set.

**Speedometer**
The tacho displays units or area processed, weight, or the efficiency of the set registration point within the set time period.

**Line chart**
The line diagram displays units or area processed, weight, or the efficiency of the set registration point within the set time period on a curve. You can display the average value and the target value using two continuous lines. This way, a deviation upward or downward is easy to spot.

#### 3.5.3. Status-based displays

The status-based data can be displayed as traffic light or pie chart. Displayed are the booked stati of a registration point (for example, on, off, ready, maintenance, fault). The time period considered can be set.

**Traffic light**
The traffic light displays the currently-booked actual state of a registration point. The traffic light can have the state red, yellow or green. Which status which traffic light color indicates can be set in the control editor.

**Pie chart**
The pie chart displays the booked status of the registration point in question for the set time period. Stati are grouped in the three colors red, yellow, and green (analogous to the traffic light). The pie chart displays the booking stati within the stored time period. The percentages of the pie specify the respective share of a status of the total time period in %.

Which traffic light color indicates which status can be set in the ControlEditor.

### 3.6. List of functions – Capa View (220042)

#### 3.6.1. Capacity display

The capacity display can be displayed separately in the browser as well incorporated using a special URL in A+W Dashboard or A+W Business.

In order to display the utilization of a machine, the machine and a time period must be selected. The displayed units can be switched between planned time, pieces, and planned quantity, which depend on the machine type. The display can be switched between day-by-day and shift-by-shift view.

The bars displayed display the completely produced quantities in green, the planned quantities in blue, and the reserved quantities in gray.

The detail view for a bar opens if you click the appropriate bar.

#### 3.6.2. Detailed view

In the detail view, you can display order-precise data.

### 3.7. List of functions – Report View (220043)

The PDF view is a control on the A+W Dashboard. Here you can call up reports that you have set up. The required parameters are determined dynamically and can be specified during the configuration. In contrast to the other controls on the A+W Dashboard, the report is not updated cyclically; instead, it must be reloaded manually.

For the report display, the PPS Webservice is required.

## 4. Contact Address

**A+W Software GmbH**
Siemensstraße 3
35463 Fernwald
Germany

Tel. +49 641 96620-0

E-mail: info@a-w.com
Internet: http://www.a-w.com/
