---
title: "EN_AWBusiness_LogisticsOptimizer_2_1"
source: "EN_AWBusiness_LogisticsOptimizer_2_1.pdf"
tags: ["A+W", "Logistic Optimizer", "OTR", "Route Planning", "ERP", "Software Manual", "Glass Industry", "Windows and Doors", "Tutorial", "Fleet Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A user manual and tutorial for the A+W Logistic Optimizer (OTR) software, version 2.01. It covers the basic principles, administration, route planning, optimization, and tracking features of the software designed for the glass, windows, and doors industry."
long_description: "This document is a comprehensive guide for the A+W Logistic Optimizer (OTR - Optimizer of Transport Routes), version 2.01, dated January 2017. It serves as both a tutorial for new users and a software reference for experienced operators. The guide is structured into two main parts: a tutorial and a software reference. The tutorial section provides a step-by-step introduction to the system, covering basic principles, database connections, the user interface, and the core workflow of planning, optimizing, and tracking delivery routes. It details administration tasks such as managing master data for users, customers, vehicles, and drivers. The software reference section offers a detailed description of every function, dialog, and parameter within the OTR module. The primary goal of the software is to optimize transportation routes to reduce time, fuel consumption, and costs, while increasing productivity for businesses in the glass, windows, and doors sector. The manual explains how to use the system's features, including dynamic route grouping, map-based planning, and integration with a mobile app for drivers."
---

# A+W Logistic Optimizer
**A+W Business**
**A+W - Software for Glass, Windows and Doors**

## Introduction
This part of the documentation contains editorial notes.

### Revision Overview

| Part Version/Date | Description |
| :--- | :--- |
| 1.00/05-2014 | Original Version. |
| 2.00/05-2016 | Complete Revision. |
| 2.01/01-2017 | Product and company names adjusted. |

### Editorial
The editorial provides information on the following topics:
- Notes on this document
- Copyrights
- Trademarks
- Contacts

### Notes on this document
This document is intended for end users of A+W Business.

The documentation and software described are licenses that must only be used or copied in accordance with the conditions of our license agreement. The contents of the documentation are only informative and are subject to changes without prior notice. The text and illustrations were compiled with the utmost care. Still, errors cannot be totally excluded. A+W Software GmbH cannot be held liable for errors or inaccuracies, unless they can be attributed to wilful or grossly negligent action.

This document describes the full scope of OTR.

### Copyrights
© 2017, A+W Software GmbH, all rights reserved, including the right of reprint, the production of copies and of the translation.

The documentation may be copied, completely or in part, saved in an archiving system or transferred in any other form only in accordance with our license agreement. Transmission of the documentation is not allowed, neither electronically, nor mechanically, nor by recording or in any other way, without A+W Software GmbH's prior written approval.

### Trademarks
All hardware and software names mentioned in this documentation can also be registered trademarks or other property rights of third parties. Third-party copyrights must therefore be observed.

### Contacts
**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
📞 +49 6404 2051 0
📠 +49 6404 2051 877
📧 Zentrale@a-w.com
🌐 http://www.a-w.com

## Contents
*This is a summary of the document's table of contents.*

- **Revision Overview**
- **Editorial**
- **Tutorial**
    - Overview
    - Documentation
    - Basic Principles of the OTR
    - User Interface
    - Administration
    - Planning Routes
    - Optimizing Routes
    - Driving and Tracking Routes
    - Queries
- **Software Reference**
    - Configuration
    - Administration
    - Planning
    - Optimization
    - Result
    - Query
    - Statistics
- **Partindex**
- **Index**

# Tutorial
**A+W Business**
**A+W - Software for Glass, Windows and Doors**

## Overview
The A+W Logistic Optimizer (also called OTR - Optimizer of Transport Routes) deals with the basics of route planning. This tutorial is based on the understanding of the master data and the number manager.

> **The functions depend on the enabled modules**
> Please note that the various functions are only available if the associated modules and interfaces are installed and enabled.
> If you detect functions in this description that are not available in your version, please contact A+W Software GmbH.

### Subjects
This tutorial offers the following subjects:
- Basic Principles of the OTR
- Administration
- Planning Routes
- Optimizing Routes
- Check Results
- Driving and Tracking Routes
- Queries

### Required knowledge
This tutorial is meant for those who prepare orders for delivery and monitor delivery using different trucks in OTR. Participants must be familiar with the master data and number manager concept.

### Documentation
The following documents are available for the OTR module:

- **Handout**: Printout of tutorial for training session
- **PDF**: Complete documentation
    - Tutorial
    - Software Reference
    - Index
- **Online help `<F1>`**: Context-sensitive dialog help for the OTR software references and tutorials on the basic version

### Tutorial Structure
This tutorial consists of subjects with several training modules each. Each module consists of the following elements:

- **Overview**: Each training module starts with an overview of the major topics:
    - Objectives: What shall be conveyed?
    - Benefit: What can this knowledge be used for?
    - Maxims: Which correlations are to be remembered?
- **Concepts**: First, the concepts and terms of the corresponding training module will be explained. This is followed by examples and instructions.
- **Exercises**: For some of the training modules, exercises with certain tasks and suggested solutions are available.
- **Cross-references**: At the end of each training module there is a section with cross references pointing to additional information in the software reference and in other sections. This will help you to extend your newly acquired knowledge.

> **Reading tip**
> The contents of a training module are based on the knowledge conveyed in the previous module. We therefore recommend you do not skip any modules.
> If you are already familiar with a subject you should at least read the summary at the start of a training module in order to bring the main details to mind.

### Display conventions
Certain parts of sentences are specially marked. These have the following meanings:

| Style | Description |
| :--- | :--- |
| *Italics* | marks character strings describing the software elements, e.g. the *Number Manager* dialog. |
| **Bold** | Marks character strings to be entered via the keyboard, e.g.: Enter the value **0**. |
| > | The so-called breadcrumb trail shows how to open a dialog, e. g. *Production > Production > Transfer to production*. |
| `[]` | Square brackets mark buttons in a dialog, e.g. `[OK]` to save the data. |
| `< >` | Angle brackets refer to keys or shortcuts on the keyboard, e.g. `<F1>` is used to open the online help. |

## Basic Principles of the OTR
The objective of meaningful route optimization and routing planning in the transport field is to reduce transportation times and routes and thus reduce fuel consumption significantly. As a result, the environmental impact is reduced, vehicles are subject to less wear and drivers are not burdened with unnecessary mileage.

Routing planning as well as route optimization therefore save costs and increase productivity.

The Optimizer for Transport Routes (OTR) organizes your destinations, customer addresses or stopping points into a useful and efficient order.

In addition to your individual fleet of vehicles, this order also takes the defined route requirements, e. g. tunnels or toll roads, into consideration. The technology is based on Nokia Maps in combination with a mathematical algorithm.

The driver can book and report deliveries directly via mobile App. In addition, all necessary information regarding the total route and individual loading stations are provided.

The office can monitor the deliveries via GPS.

The procedure is as follows:
Planning -> Optimization -> Result
*Fig. J-1 Standard process for the delivery sequence*

The process is divided into four phases:
- In this phase you create the route(s). You can create new routes, edit existing ones or also delete them. Within the routes, you can add destination locations (stopping points), and also edit or delete individual locations. During this phase, you also have access to the individual items in order to obtain an overview.
- **Optimization**: Optimization of the route takes place in this phase. On the overview map, you will see the routing and, on the right side, a list of the individual stations (waypoints). You can exchange individual stations and you have access to the optimization factors. The optimizations considers settings and modifications of the planning phase - for example certain unloading times or priorities of customers (loading stations).
- **Result**: This phase provides the total result of the route, divided into the individual routes, the graphical route plan and the list of the destination locations.

### Database Connections
To work with the module, the following two database connections have to be in place:
- OTR
- ERP

#### Connection to the OTR database
The connection to the OTR is necessary to plan the routes.

*Fig. J-2 Database settings OTR*

A dialog appears when you call the database for the first time. In the field *Data Source* enter the path to the OTR database server. You can obtain this information from your contact at our A+W Support or Qualified Service.

Enter the standard database in the field *Start Catalog*. This is OTR. You can also obtain the *User ID* and *Password* from your contact at A+W Support or Qualified Service.

After you have made the settings, you can establish a test connection to the database with the `[Test]` button.

> **Database connection**
> Please note that these settings have to be made for each user.

**Additional information**
⇨ Software Reference, "OTR Connection" on page J-130

#### Connection to the ERP database
The connection to the ERP database server is necessary for the module to access the data from A+W Business.

*Fig. J-3 Database Settings ERP*

A dialog with the tab *OTR* appears when you call the database for the first time. Switch to the tab *ERP Connection*.

Enter the standard database in the field *Start Catalog*. You can also obtain the *User ID* and *Password* from your contact at A+W Support or Qualified Service.

After you have made the settings, you can establish a test connection to the database with the `[Test]` button.

> **Database connection**
> Please note that these settings have to be made for each user.

**Additional information**
⇨ Software Reference, "OTR Connection" on page J-130

### Dynamic Mode
When working with the dynamic mode, the following dialog opens after clicking the OTR icon button in number manager:

*Fig. J-4 Dynamic mode, delivery areas*

This is where OTR groups destinations based on coordinates and under consideration of weight and the geolocation takes place.

Field *Number of delivery areas* shows in how many groups OTR combined the individual destinations.

You can either accept or change the value. In case you change it, a recalculation based on the new value takes place in background.

> **Geolocation in Dynamic Mode**
> If geolocation was successful for all addresses, the Geolocation phase will be skipped in OTR.

After pressing the `[OK]` button, dialog *Select Vehicle* appears.

*Fig. J-5 Dynamic mode, select vehicle*

The dialog gives an overview of the individual vehicles defined in the system. You can either choose certain vehicles (own trucks or transport companies) or all vehicles. By selecting all vehicles, the system has the freedom to distribute the orders optimally on the trucks.

If you enable the checkbox *Maximum vehicle weight and visiting time*, the maximum load defined in the master data as well as the time defined for the customer are taken into consideration.

Click on `[OK]`, the following display opens:

*Fig. J-6 User interface after start*

OTR uses the above mentioned entries for calculation. On the left-hand side you see the map containing the individual groups that are visited. The top right shows the routes and the destinations below.

The number in field *Groups* is identical with the number on the map (s.a.).

The `[Groups]` button contains the menu entries:
- Hierarchical
- EM

These are two types of calculation leading to different results. The appropriate mode depends on how many groups and how many destinations are visited.

To make this clear, we split 94 destinations into different numbers of groups and show the result of both modes.

*Images showing map layouts for 3, 4, 6, and 9 groups in both Hierarchical and EM modes.*

According to our experience, the EM mode has a more efficient splitting of destinations for just a few groups. If you have a large amount of groups, the hierarchical mode has a more efficient splitting.

Use the menu entries *Hierarchical* and *EM* to simulate the splitting and to choose the best result.

> **Calculation of Groups**
> The splitting always takes place under consideration of the vehicle values defined in the master data.

Tab *Route Information* provides an overview of the truck load, weight, and the route time.

The progress bar in column *Status* shows the percentage of the truck load.

**Next step:**
⇨ Optimization, Page J-84

**Additional information**
⇨ Software Reference, "Groups" on page J-182

### User Interface
Open the module OTR by pressing the `[OTR]` button in the number manager. Once you have started OTR, the module appears as follows:

*Fig. J-7 User interface after start*
- **A** Menu bar
- **B** Tool bar
- **C** Process presentation
- **D** Map
- **E** Map tools
- **F** Overview of the routes
- **G** Overview of the destinations
- **H** Button

The upper area contains, from left to right, the menu bar (A), the tool bar (B) and presentation of the whole process (C) from planning up to data transfer. With the wizard, you can complete the entire process (planning, geolocation, etc,) in just a few steps.

The `[Next]` button takes you one step further in the process. Please note that you can only continue if no errors have occurred in the respective process. For instance: in the Geolocation area you can only continue to the next step if all destinations could be located.

The `[Back]` button takes you one step back in the process.

The optimization results are displayed at the end of this process and you can decide whether you are going to accept (save) the route and the optimization results or repeat the optimization with other settings to achieve a better result.

The map (D) shows the destinations combined to groups. The area below shows the tools to edit routes on the map (E). The *Routes* (F) section contains all upcoming routes and the *Destinations* (G) section shows you the individual stations of the route. The (H) button takes you to the next step in the process.

Below the map you will find the following tools:

#### Description of the individual icons

| Icon | Description |
| :--- | :--- |
| Menu | If you enable this icon button you can use the `<Ctrl>` key to select one or more destinations. These are displayed in red. A popup menu opens with actions that can be made at this point. |
| Destinations | If you enable this icon button the map shows the last two digits of the route ID. If the icon button is disabled the numbers of the destinations are displayed. |
| Groups | With this icon button the outward destinations are connected by lines. |
| Groups | With this icon button the delivery areas are displayed circular. |
| Information | With this icon button you turn the route information (Nokia Maps) on or off. |
| Optimized route | After the optimization you can use this icon button to show or hide the route. |
| Destinations | With this button you can show or hide destinations. |

| Zoom | This icon button lets you zoom in and out (map). The sections *Routes* and *Destinations* are hidden. Click the icon button again to show the sections *Routes* and *Destinations* and to reduce the map. |

Enable the *Menu* button, keep the `<Ctrl>` key pressed and click on a destination. The following menu opens:
```
(1-1034) Customer: 1010 GLASBAU MUELLER
JOIN GROUPS - ROUTES
  (0-1033) ROUTE 04.05.2016 GI-AW1
  (1-1034) ROUTE 04.05.2016 GI-AW6
  (2-1035) ROUTE 04.05.2016 GI-AW2
  (3-1036) ROUTE 04.05.2016 GI-AW3
DELETE DESTINATION
  (1-1034) 1010 GLASBAU MUELLER
DESTINATION
  Priority
  Starting Point
  Intermediate Point
```

Use this menu to combine groups. Thus, keep the `<Ctrl>` key pressed and click on the destination you want to move. The menu opens and you click in the menu on the group, the destination shall be moved to. The menu closes and the destination is now in the requested group.

It is very easy to delete a destination, keep the `<Ctrl>` key pressed and select the destination. The menu opens and section *Delete Destination* contains the selected one. Click it and it will be deleted.

> **Delete Destination**
> Presently, after deleting a destination the status for the order (orders) is not changed in the ERP. Only for the other orders (planned, optimized, released, etc.)

In section *Destination* you can mark a destination as priority or assign a different point. The following points are possible:
- Starting point
- Intermediate point
- End point

**Additional information**
- ⇨ "The Menu and Tool Bars" on page J-24
- ⇨ "Field help" on page J-30

### The Menu and Tool Bars
The menu bar contains the most important functions for the user. The individual menus can be opened with the click of a mouse. Some menu items can be directly opened with the aid of key combinations (e.g. Ctrl+S = Start).

The *Start* area contains the following buttons:

#### Description of the individual icons

| Icon | Description |
| :--- | :--- |
| Close | This is used to close the module. |
| Check Service | This button is used to check connection to the service. |
| Logbook | This button is used to open the logbook, in which daily events are recorded. |
| Help | This button opens the A+W Business Help. |
| About OTR | This button opens a dialog containing information about the version and the license key. |

The *View* area contains the following entries which are used to adjust the appearance of OTR:
- 2010 Blue
- 2010 Silver
- 2007 Blue
- 2007 Silver
- 2010 Black
- 2007 Black
- Sparkle Blue
- Sparkle Orange
- Sparkle Purple
- 2003 Professional Style

The *Configuration* area contains the following buttons:

#### Description of the individual icons

| Icon | Description |
| :--- | :--- |
| Settings (Configuration) | This button lets you access the database settings. It opens the *Settings* dialog. |
| Parameters | This button takes you to the parameters. It opens the *Parameters* dialog. |
| Import/Export | Use this icon button to backup the parameter in XML format. |
| Language (English) | You can select the program language for OTR with this button. |

The *Settings* area contains the following buttons:

#### Description of the individual icons

| Icon | Description |
| :--- | :--- |
| User (Users) | This button takes you to the users. The *User* dialog opens. |
| Status | This button lets you access the status. The *Status* dialog opens. |
| Customers | This button takes you to the customers. The *Customer* dialog opens. |
| Departments (Department) | This button takes you to the departments. The *Department* dialog opens. |
| Vehicles | You can access the fleet park by pressing this button. It opens the *Vehicles* dialog. |
| Drivers | With this button, you have access to your drivers. The *Drivers* dialog opens. |
| Reports | This button takes you to the reports. The *Report* dialog opens |
| Packaging types (Packaging) | This icon button allows you to access the packaging types. The *Packaging Types* dialog opens. |
| Data import | With this button you can import data in CSV format. The *Data import* dialog opens |

The *Query* area contains the following buttons:

#### Description of the individual icons

| Icon | Description |
| :--- | :--- |
| Filter | This button is used to filter individual routes. It opens the dialog *Filter routes*. |
| Edit route | This button is used to change the route status and the real costs. The *Edit Route* dialog opens. |
| Delete route | This button is used to delete a previously selected route. |
| Export route | With this button, you can export data to a navigation system. This opens the *Export* dialog. |
| Edit status (Change of Status) | This button is used to change the route status. The *Change status* dialog opens. |
| History | This button is used to view the document history. It opens the *History* dialog. |
| Selected route | This button opens the Crystal Report *Confirmation and Delivery List* for the selected route. |
| Report launcher | This button opens the *Report launcher* dialog for the selected route. |
| Statistics | This button opens the *Statistics* dialog for the selected route. |
| View route (Route) | This button opens the *Route* dialog. |
| View destination (Destination) | This button opens the *Destination* dialog. |
| Calendar | This button opens the *Calendar* dialog. The calendars shows the routes traveled by vehicles and drivers. |
| Route administrator | This button serves for online tracking of the currently traveling routes. |
| Attach files | This button is used to add a document to a destination. |

#### The tool bar in the planning phase
The tool bar in the planning phase enables access to all functions and dialogs that are relevant to this phase.

##### Description of the individual icons

| Icon | Description |
| :--- | :--- |
| Copy saved route (Copy) | With this button, you can add a saved route. The dialog *Saved Routes* opens. |
| Load saved route (Saved Route) | With this button, you can add a new route to a saved route. The dialog *Saved Route List* opens. |
| Import destinations | With this button, you can import destinations. The *Data Import* dialog opens. |
| New route (Add) | This button is used to create a new route. The *Route* dialog opens. |
| Edit route | This button is used to edit a previously selected route. |
| Delete route (Delete) | This button is used to delete a previously selected route. |
| Groups | With this button, you can split routes in groups. |
| Vehicles | Use this button to assign a different vehicle to the route. The *Vehicles* dialog opens. |
| New destination (Add) | This button is used to add a new destination to a route. The *Destination* dialog opens. |
| Edit destination (Edit) | By pressing this button, you can edit a previously selected destination. The dialog *Edit destination* opens. |
| Delete destination (Delete) | By pressing this button, you can delete a previously selected destination. |
| Packaging | This button opens the *Packaging* tab. |
| Detailed view | This button gives you a detailed view of the destinations of a route. |
| Initialize | This button takes you back to the starting situation. If, e.g. you have grouped records, which you wish to undo, click this button. |

#### The tool bar in the optimization phase
The tool bar in the realization phase enables access to all functions and dialogs that are relevant to this phase.

##### Description of the individual icons

| Icon | Description |
| :--- | :--- |
| Optimize route | This button optimizes the route again. |
| Stop optimization | This button is used to stop the optimization. |
| Traffic | This button is used to determine the traffic based on statistical values (Nokia Maps). |
| Stop traffic | Use this button to abort traffic determination. |
| Edit route | This button is used to edit a route. The *Route* dialog opens. |

#### The tool bar in the result phase
The tool bar in the result phase enables access to all functions and dialogs that are relevant to this phase.

##### Description of the individual icons

| Icon | Description |
| :--- | :--- |
| View route (Route) | This button opens the *Route* dialog. |
| View destination (Destination) | This button opens the *Destination* dialog. |
| Edit route | This button is used to change the route status and the real costs. The *Edit Route* dialog opens. |

### Field help
If the [Help] icon is located next to a field, hover your mouse on it and it shows you information about the field.

*Fig. J-8 Field help*

**Additional information**
⇨ "User Interface" on page J-21

## Administration
This section introduces the master data in OTR.
This includes the following training modules:
- "Parameters" on page J-32
- "User" on page J-34
- "Status" on page J-35
- "Customers" on page J-37
- "Departments" on page J-40
- "Vehicles" on page J-42
- "Driver" on page J-46
- "Reports" on page J-49
- "Packaging Types" on page J-51
- "Data Import" on page J-54

### Parameters
In this area you define standard settings to work with OTR.
The parameters are first divided into two groups:
- **Parameters for the configuration of the application**: These parameters are used for general configuration, such as text format, unit systems, currency, etc.
- **Parameters for routes**: Routes are created and optimized on this basis of these values. Via the *Edit Route* dialog you can always access these values and make temporary changes.

The software reference provides a detailed description on this.

**Additional information**
⇨ Software Reference, "Parameters" on page J-132

### Master Data

#### Objectives
- Getting to know the parameters
- Learning and understanding how to work with the vehicles fleet
- Learning and understanding how to work with users and departments
- Learning and understanding how to work with drivers

#### Benefits
- Fleet park data has to be maintained accurately in order to determine route costs. This is the only way to obtain accurate values. As it may be necessary to contact your driver by phone, we recommend keeping their data up to date.

#### Definition
| Term | Definition |
| :--- | :--- |
| Fixed costs | Costs that remain unchanged when changing a variable (total distance, fuel costs). |

#### Please note
| Topic | Note |
| :--- | :--- |
| Creating a new vehicle | When creating a new vehicle, we recommend having the vehicle registration at hand. |
| Maintenance date | You have the opportunity to enter the next maintenance date for your vehicle. The module reminds you of this date in due time. |
| Assigning a driver | You can assign the vehicle to a fixed driver. |
| Costs | Costs can be set up per driver based on time or distance. |
| Personnel | OTR differentiates between own personnel (employees) and external personnel (hired drivers). |

### User
This section is used to control user profiles, that are registered under Windows or in a domain. The data is automatically generated at program (OTR) start.

*Fig. J-9 User*

The table above shows which profiles have already been created. As administrator you can define e.g. users with default profile (language, presentation of user interface, etc.) that can be copied later on.
The software reference provides a detailed description of the individual fields.

> **Rights**
> To edit, the user must be a member of the administrator group. The users are registered, after starting OTR from A+W Business. Otherwise, the users are registered by the operating system.

**Additional information**
⇨ Software Reference, "User" on page J-142

### Status
Depending on the route condition, it has a certain status.

*Fig. J-10 Status*

The table above shows which status types have already been created. You can define a new status or change an existing one. The field *Editable* shows the status that can be changed. A green checkmark indicates that the status can be changed. All status types without green checkmarks cannot be changed.

To load data into the cloud, a manual change of status may be necessary for those routes, manually released for the driver.

The individual status are grouped. The group (650) for example deals with various behaviors concerning destinations. It contains the following status:
- Destination problem: The truck could not reach the destination.
- Destination not found: The destination was simply not found.

The software reference provides a detailed description of the individual fields.

#### Managing Status Types
Here you will learn how to create, edit or delete new status types.

##### How to create a new status
1. Go to the menu bar to *Administration*.
2. Press the `[Status]` button. The *Status* dialog opens.
3. Press the icon button `[New]`. The lower part of the dialog is now available for editing.
4. Click on the icon button. The *Status Type* dialog opens. From the list select the type the status belongs to. Click `[OK]`. The dialog closes. The information will be adopted.
5. Field *Status* is prepopulated with the next free number.
6. In the *Status name* field, enter the name.
7. Whether the checkboxes *Routes* and *Destinations* are enabled or not depends on the groups, they are allocated to.
8. You can enter a detailed description of the status in the *Description* field.

##### How to delete an existing status
1. Go to the menu bar to *Administration*.
2. Press the `[Status]` button. The *Status* dialog opens.
3. Select the status from the table that is to be deleted.
4. Press the icon button `[Delete]`. The entry is deleted.

##### How to make changes to a certain status
1. Go to the menu bar to *Administration*.
2. Press the `[Status]` button. The *Status* dialog opens.
3. Select the status from the table that is to be changed. The checkmark in field *Editable* indicates that the status can be changed.
4. Press the `[Edit]` button.
5. Carry out the required changes.
6. Press the `[Save]` button. The data is saved.

**Additional information**
⇨ Software Reference, "Status" on page J-143

### Customers
In OTR you can manage individual, additional customer data (addresses). This may be helpful to manage loading and unloading addresses without creating them in the ERP system (A+W Business Customer Master Data). To activate this property, set the value `USE_CUSTOMERS_OTR` to `Yes` in the parameters.

*Fig. J-11 Customers*

If the parameter is enabled, OTR checks during import whether the customer is already saved. If not it is saved and can be used immediately.
The software reference provides a detailed description of the individual fields.

#### Managing Customers
Here you will learn how to create, edit or delete new customers manually.

##### How to create a new customer manually
1. Go to the menu bar to *Administration*.
2. Press the `[Customer]` button. The *Customer* dialog opens.
3. Press the icon button `[New]`. The lower part of the dialog is now available for editing.
4. Enter the required number in field *Customer*. Note: Each number can only be assigned once.
5. Enter the name of the customer in the *Name* field.
6. Enter the telephone number in the *Telephone Number* field.
7. In the field *Address* you can enter the customer address. Please enter the name of the street and the name of the city separated by comma.
8. If the longitude and latitude fields are not filled, click `[Geolocate]`.
9. In field *Time (Minutes)* you can enter the time that the driver has on site.
10. In field *Time Range* you can enter the unloading time on-site for the driver.
11. In field *Contact Person* you can enter a contact person for the customer.
12. In field *E-Mail Address Contact* you can enter the email address of the contact.

##### How to delete an existing customer
1. Go to the menu bar to *Administration*.
2. Press the `[Customer]` button. The *Customer* dialog opens.
3. Select the customer from the table that is to be deleted.
4. Press the icon button `[Delete]`. The entry is deleted.

##### How to make changes to a certain customer
1. Go to the menu bar to *Administration*.
2. Press the `[Customer]` button. The *Customer* dialog opens.
3. Select the customer from the table that is to be changed.
4. Press the `[Edit]` button.
5. Carry out the required changes.
6. Press the `[Save]` button. The data is saved.

**Additional information**
⇨ Software Reference, "Customers" on page J-145

### Departments
Use this dialog to add, change or delete individual departments. This serves for statistical evaluations. On this basis individual evaluations can be implemented. Thus, external companies (transport companies) can be defined as *Department*.

*Fig. J-12 Departments*

The table above shows which departments have already been created.
The software reference provides a detailed description of the individual fields.

#### Managing Departments
Here you will learn how to create, edit or delete departments.

##### How to define a new department
1. Go to the menu bar to *Administration*.
2. Press the `[Department]` button. The *Department* dialog opens.
3. Enter the number of the department in the *Department* field.
4. Enter the name of the department in the *Name* field.
5. You can enter a description of the department in the *Description* field.

##### How to delete an existing department
1. Go to the menu bar to *Administration*.
2. Press the `[Department]` button. The *Department* dialog opens.
3. Select the department from the table that is to be deleted.
4. Press the icon button `[Delete]`. The entry is deleted.

##### How to make changes to a certain department
1. Go to the menu bar to *Administration*.
2. Press the `[Department]` button. The *Department* dialog opens.
3. Select the department from the table that is to be changed.
4. Press the `[Edit]` button.
5. Carry out the required changes.
6. Press the `[Save]` button. The data is saved.

**Additional information**
⇨ Software Reference, "Departments" on page J-147

### Vehicles
In this area you find all vehicles that are available for the delivery of goods. This includes:
- Truck
- Automobile
- Trailer

*Fig. J-13 Vehicles*

The table above shows you which vehicles have already been created. You can create new vehicles and also make changes to existing vehicles.
The software reference provides a detailed description of the individual fields.

> **Vehicle data**
> When creating a new vehicle, we recommend having the vehicle registration at hand. Data will be requested by the system that you can find here, such as empty weight.

**Additional information**
⇨ Software Reference, "Vehicles" on page J-148

#### Managing Vehicles
Here you will learn how to create, edit or delete new vehicles.

##### How to create a new vehicle
1. Go to the menu bar to *Administration*.
2. Press the `[Vehicles]` button. It opens the *Vehicles* dialog.
3. Press the icon button `[New]`. The lower part of the dialog is now available for editing. For the entries that follow, we recommend having the vehicle registration at hand.
4. Fill the fields *License Plate*, *Brand*, *Model* and *Chassis Number* on the basis of the vehicle registration documents.
5. Fill the field *Purchase Date*.
6. In the field *Next Maintenance*, you can enter the date for the next maintenance. If the entry *New maintenance date for vehicles* is enabled in the parameters, the field here is evaluated accordingly.
7. Field *Department* allows to assign a department to the vehicle. This serves for statistical evaluations. The button opens the dialog *Select Department*, containing all defined departments.
8. Fill the fields *Maximum Width*, *Maximum Height*, *Maximum Length*, *Maximum Load* and *Empty Weight* on the basis of the information in the vehicle documentation.
9. Enter the average fuel consumption of the vehicle in the *Consumption* field in liters, e.g. 18.5.
10. Enter the average price for a liter of fuel in the *Fuel Costs* field, e.g. 1.43. You can set up the currency unit in the parameters.
11. Enter the average price for a liter of fuel in the *Fixed Costs* field, e.g. 1.43. You can set up the currency unit in the parameters.
12. Select the vehicle type from the combo box *Vehicle Type*.
13. The fields *Driver ID*, *First Name* and *Surname* are linked to the `[Add driver]` button. If you press the button, the *Driver* dialog opens. You can select a driver here. This is recommended if employees have a fixed assignment to a vehicle.
14. The route numbers shown here are transferred from AWBusiness and serves to assign trucks to certain route numbers.
15. The *Sequence* field is in direct connection with the *Routes* field. If the same route number is allowed for two or more trucks, this field allows to determine the sequence. The field will be evaluated if the value `ROUTE_ORIGIN` has been set to `Yes` in the parameters.
16. The checkbox *Vehicle Available* is used to define whether the vehicle is generally available for all routes.
17. If your vehicle is equipped with a trailer hitch, enable the checkbox *Truck with trailer*.

##### How to delete an existing vehicle
1. Go to the menu bar to *Administration*.
2. Press the `[Vehicles]` button. It opens the *Vehicles* dialog.
3. Select the vehicle that is to be deleted from the table.
4. Press the icon button `[Delete]`. The entry is deleted.

##### How to make changes to a certain vehicle
1. Go to the menu bar to *Administration*.
2. Press the `[Vehicles]` button. It opens the *Vehicles* dialog.
3. Select the vehicle in the table that is to be changed.
4. Press the `[Edit]` button.
5. Carry out the required changes.
6. Press the `[Save]` button. The data is saved.

##### How to assign a vehicle to a fixed driver
1. Go to the menu bar to *Administration*.
2. Press the `[Vehicles]` button. It opens the *Vehicles* dialog.
3. Select the vehicle in the table that is to be assigned to a driver.
4. Press the `[Edit]` button.
5. Press the `[Add Driver]` button. The *Drivers* dialog opens.
6. Select the desired driver.
7. Press the `[OK]` button. The dialog is closed and you are now back in the *Vehicles* dialog.
8. Press the `[Save]` button. The data is saved.

##### How to remove a fixed driver
1. Go to the menu bar to *Administration*.
2. Press the `[Vehicles]` button. It opens the *Vehicles* dialog.
3. Select the vehicle in the table, from which the driver is to be removed.
4. Press the `[Edit]` button.
5. Press the `[Delete Driver]` button. The driver is deleted.
6. Press the `[Save]` button. The data is saved.

**Additional information**
- ⇨ Software Reference, "Vehicles" on page J-148
- ⇨ Software Reference, "Driver" on page J-151

### Driver
In this area, you can administer data for your drivers. In this area you find all drivers that are available for the delivery of goods. This includes:
- Company drivers
- Drivers from other companies (hired drivers)

*Fig. J-14 Driver*

The table above shows you which drivers have already been created. You can create new drivers and also make changes to existing drivers.
The software reference provides a detailed description of the individual fields.

**Additional information**
⇨ Software Reference, "Driver" on page J-151

#### Managing Drivers
Here you will learn how to create, edit or delete new drivers.

##### How to create a new driver
1. Go to the menu bar to *Administration*.
2. Press the `[Driver]` button. The *Drivers* dialog opens.
3. Press the icon button `[New]`. The lower part of the dialog is now available for editing.
4. Enter a short description of the driver in the *Driver ID* field.
5. Fill the fields *Name*, *Surname* and *Surname 2*.
6. Enter the tax number of the employee in the field *Tax ID*.
7. Enter the e-mail address of the employee in the *E-Mail* field.
8. In the *Costs* field you can enter an amount attributed to the route that is caused by the employee. Costs are differentiated by time and by distance. Please enable the underlying radio buttons (*By time* / *By distance*). The value entered here is included in the evaluation in the *Costs* tab.
9. In the *Address* field, enter the address of the employee and enter the respective telephone numbers in the fields *Telephone* and *Telephone 2*.
10. In the *Contact* field, you can enter the name of a contact person if the driver is not employed with your company. Example: You book a driver from a transport company for a route.
11. In the field *Contact Address* you can enter the address of your contact.
12. Enter the respective telephone number in the *Telephone-Contact* field.
13. You can enter a description of the driver or the contact in the *Description* field and the e-mail in the respective *E-mail Address Contact* field.
14. Field *Department* allows to assign a department to the driver. This serves for statistical evaluations. The button opens the dialog *Select Department*, containing all defined departments.
15. Via the checkbox *Company Driver* you can indicate whether the driver is employed with your company and via the checkbox *Available*, whether the driver is always available.
16. The checkbox *Reset Password* is used to reset the password necessary at start of the GDC App (mobil App for drivers).

##### How to delete an existing driver
1. Go to the menu bar to *Administration*.
2. Press the `[Driver]` button. The *Drivers* dialog opens.
3. Select the driver from the table that is to be deleted.
4. Press the icon button `[Delete]`. The entry is deleted.

##### How to make changes to a certain driver
1. Go to the menu bar to *Administration*.
2. Press the `[Driver]` button. The *Drivers* dialog opens.
3. Select the driver from the table that is to be changed.
4. Press the `[Edit]` button.
5. Carry out the required changes.
6. Press the `[Save]` button. The data is saved.

**Additional information**
⇨ Software Reference, "Driver" on page J-151

### Reports
In this area, you can administer data for your reports. The dialog contains all reports defined. OTR works with reports on basis of SAP Crystal Reports.

*Fig. J-15 Reports*

The table above shows which reports have already been created. You can create new reports and also make changes to existing reports.
The software reference provides a detailed description of the individual fields.

**Additional information**
⇨ Software Reference, "Reports" on page J-154

#### Managing Reports
Here you will learn how to create, edit or delete new reports.

##### How to create a new report
1. Go to the menu bar to *Administration*.
2. Press the `[Report]` button. The *Report* dialog opens.
3. Press the icon button `[New]`. The lower part of the dialog is now available for editing.
4. Enter the name of the report in the *Name* field, e.g. **Short**.
5. Field *Report Path* allows to enter where the report is to be saved.
6. The *Description* field allows you to enter information about the report.
7. Use the checkboxes in section *Parameter* to select the information to be printed on the report.

##### How to delete an existing report
1. Go to the menu bar to *Administration*.
2. Press the `[Report]` button. The *Report* dialog opens.
3. Select the report from the table that is to be deleted.
4. Press the icon button `[Delete]`. The entry is deleted.

##### How to make changes to a certain report
1. Go to the menu bar to *Administration*.
2. Press the `[Report]` button. The *Report* dialog opens.
3. Select the reports from the table that is to be changed.
4. Press the `[Edit]` button.
5. Carry out the required changes.
6. Press the `[Save]` button. The data is saved.
