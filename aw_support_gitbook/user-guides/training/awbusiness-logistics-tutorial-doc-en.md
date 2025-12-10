---
title: "A+W Business Logistic Optimizer Tutorial and Software Reference"
source: "EN_AWBusiness_LogisticsOptimizer_2_3.pdf"
tags: ["logistics", "software", "tutorial", "route optimization", "tracking", "A+W", "ERP integration", "user manual", "software reference"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A comprehensive tutorial and software reference guide for the A+W Business Logistic Optimizer. This document covers driving and tracking routes, using the mobile app, managing booking data, and system administration. It is intended for both drivers and administrators."
long_description: "This document serves as a detailed manual for the A+W Business Logistic Optimizer, a software designed for managing and optimizing logistics routes. The first part is a tutorial aimed at drivers, explaining the entire process from logging in to the driver app, operating the app or browser interface, to booking data at each destination. It covers updating delivery statuses (Accepted, Rejected, etc.), capturing signatures, and managing packaging information. This section also details how administrators can perform live tracking of vehicles and view route progress. The second part is a software reference guide for administrators. It provides in-depth information on system queries, reporting, configuration, and administration. Key topics include filtering and exporting route data, creating statistical reports for cost analysis, configuring database connections (OTR and ERP), setting system-wide parameters for route calculation, and managing master data such as users, vehicles, customers, and departments."
---

# Tutorial

---
## Driving and Tracking Routes

This section contains the information for the driver.
- Enter Password
- Operation of App or Browser
- Booking Data

### Enter Password

On the first login with ID (via app or Browser), the driver is asked to enter the following.

> **Screenshot: Login Screen**
> The interface shows fields for Company ID, User, Password, and Repeat Password. A message indicates "This is the first access. Password must be set."

1.  Enter the corresponding ID from the license information (Start > About A+W Logistics Optimizer, button [License Information], field Companyld).
2.  Enter the **Driver ID** (Administration > Driver, field Driver ID) in field **User**.
3.  Enter the password in field **Password**.
4.  In field **Repeat Password** you have to enter the password again.
5.  Click on [Login], to register.

**Forgot password**
In case you forgot the password, it can be reset in the Driver dialog, checkbox Reset Password.

**Additional information**
⇨ Software Reference, "Driver" on page J-151

### Operation of App or Browser

After the driver logged in routes are shown that are assigned to the driver ID. A click on the route opens the overview with three tabs.

- Destinations
- Information
- Map

#### Destinations Tab

Tab Destinations contains all destinations that are driven to on the route.

> **Screenshot: Destinations Tab**
> The screen displays a tour with a list of destinations, including "A+W", "BECKER GLASBAU", etc., each with a "Released" status and a scheduled time. A "Start" button is prominent.

Press the [Start] icon and you will be asked whether your location shall be transferred via GPS. In order to transfer the position coordinates of the booking back and to access these data from the company, please confirm.

After confirmation the first entry (start point, example above: A+W) is set to Accepted.

### Booking Data

Arriving at the first destination (example above Becker Glasbau) the driver clicks it in the list and the following window opens.

> **Screenshot: Booking Data Window**
> A modal window for "BECKER GLASBAU" shows tabs for Status, Information, and Documents. The Status tab has a dropdown for status selection, a comment box, and a list of documents.

Use the combobox **Status** to assign the respective status. The options are:
- Accepted
- Partially accepted
- Rejected
- Rejected (breakage)
- In route

Select the corresponding status.

Use section **Comment** to enter information. You can enter e.g. a broken lite. Since the data are reported to the Cloud, the company can access these data, too. Thus, breakage can be reproduced immediately.

The section **Documents** shows the order numbers. Depending on the status, you can select or deselect them. Example: If you select status **Accepted**, all documents are automatically selected. If you select status **Partially accepted**, single documents can be chosen. Then, you can select just the documents, for which the delivery was accepted.

### Section Company

A click in the section Company opens a new window. The employee who accepted the delivery can sign in the yellow area.

> **Screenshot: Signature Pad**
> A window with a yellow area for signing. A signature "Erich Hardt" is shown. Buttons for "Cancel" and "Accept" are present.

Click on [Accepted], the window is closed and the signature is displayed at the right side of the screen.

> **Image: Displayed Signature**
> The signature of "Erich Hardt" is shown next to the label "Signature" with a "Yes" indicator.

Now, the word **Yes** is shown below the entry Company. This means a signature exists. If the signature is wrong or must be repeated, click on the trash icon, top right. The signature is deleted and can be repeated.

### Section Packaging

In section Packaging click on [Add], the Packaging window opens.

> **Screenshot: Packaging Window**
> The window shows fields for Barcode, Action (e.g., "Collected"), Comments, and a list of Items.

Enter the respective ID below the **Barcode** entry. In field **Action** you can choose whether the packaging is a delivery or a collection. Use section **Comment** for further information regarding the packaging type.

Click on [Add], a new window opens:

> **Screenshot: Add Item Window**
> A small window prompts for Batch, Order No., and Position.

Enter the batch, the order number, and the line item. Click on [Add] to save the data and you are back in window Packaging.

Click on [Save] to close the window.

### Booked Destinations

Depending on the status, the overview shows the destinations in different colors. Accepted deliveries are marked in green. Partially accepted or rejected deliveries are marked in yellow.

> **Screenshot: Color-Coded Destinations**
> The destination list shows "A+W" with an "Accepted" status highlighted in green, and "BECKER GLASBAU" with a "Partially Accepted" status highlighted in yellow.

### Information Tab

This tab contains information regarding the route.

> **Screenshot: Information Tab**
> The tab displays details like Delivery Date, Start Time, Expected Distance, Expected Time, Status, and Configuration settings (Mode, Avoid Highways, Avoid Tolls, etc.).

### Map Tab

This tab shows the map with the routes to be driven.

> **Screenshot: Map Tab**
> A map is displayed with a highlighted route connecting several waypoints.

## Tracking Routes

The Route administrator provides a permanent online tracking of the vehicles and the drivers. Every time the driver books via App or Safari, the data is updated via cloud.

### Example for a partially accepted delivery

**In the App:**
The app shows the destination list with "BECKER GLASBAU" marked as "Partially Accepted". A detail view for this destination shows the status, comments ("Order 700199 line item 3: Damaged!"), and associated documents.

**In OTR (A+W Logistics Optimizer):**
The administrator view shows a map with the route. A popup for "BECKER GLASBAU" displays its details, including "Status: Partially Accepted".

### Destinations Tab

The different colors show the current status. Destinations in green color were completely delivered. Destinations in yellow color were either partly delivered or rejected.

Double clicking the destination to the right of the map, shows this on the map together with a box that contains all relevant information.

### Tab Logbook

Tab Logbook shows an overview of the route in table form.

> **Screenshot: Logbook Table**
> A table with columns for Date, Route, Customer, Name, Status, and Comment. One entry shows a "Partially Accepted" status with the comment "Order 700199 line item 3: Damaged!".

- **Field Date** shows the date of the route and field **Route** the number.
- **Field Customer** shows the customer number and field **Name** the corresponding name.
- **Field Status** shows the status of the respective destination. The field remains on **Initiate** until the driver selects and books the corresponding status via App or Safari. Then, the data is copied via Cloud. Possible values are:
  - Accepted
  - Partially accepted
  - Rejected
  - Rejected (breakage)
  - In route
- **Field Comment** shows the information defined by the driver.
- **Field User** shows the name of the driver.

If you click on a destination, a point appears at the place where the driver made the booking. This way, you are always informed about the real booking place.

### Documents Tab

Tab Documents gives an overview on the orders of the respective customer (destination) in table form.

| Order No. | Customer | Name | Status | Delivery Weight | Collected Weight |
| :--- | :--- | :--- | :--- | :--- | :--- |
| ► 20483 | 1010 | GLASBAU MUELLER | Initiate | 2.070,00 kg | 0,00 kg |
| 20483 | 1010 | GLASBAU MUELLER | Rejected | 2.070,00 kg | 0,00 kg |
| 20483 | 1010 | GLASBAU MUELLER | Initiate | 2.070,00 kg | 0,00 kg |
| 20483 | 1010 | GLASBAU MUELLER | Rejected | 2.070,00 kg | 0,00 kg |

- **Field Order No.** contains the order number.
- **Field Customer** shows the customer number and field **Name** the respective customer name.
- **Field Status** shows the order status. The field remains on **Initiate** until the driver selects and books the corresponding status via App or Safari.
- **Field Delivery Weight** shows the weight of the order in kg.
- **Field Collected Weight** shows the weight of collected racks.

**Update Display**
Don't forget to press the [Update] button from time to time to synchronize the data.

## Queries

This section deals with the query tools. This includes the following training modules:
- "Routes" on page J-114
- "Reports" on page J-120
- "View" on page J-125

### Overview

**Objectives**
- Knowing and understanding the different queries.
- Getting to know and understanding statistics.
- Getting to know and understanding the calendar.

**Benefits**
- The statistic function is a flexible and powerful control and analysis tool.

**Please note**
- **ITN format**: Export format, e.g. for TomTom navigation systems
- **GPX format**: Export format, e.g. for Garmin navigation systems

### Different Queries

Use this section to query all relevant information depending on the route status. The tab is divided into the following groups:
- Routes
- Reports
- View
- Update

### Routes

This area contains information that are connected to routes. You will find the following entries:
- Filter
- Change
- Clear
- Export
- Status
- History

#### Filter

You can filter the routes by date, route ID, route name, etc.

> **Screenshot: Filter Routes Dialog**
> A dialog box allowing filtering by Date range, Route ID, Route Name, Vehicle, Route Status (Created, Planned, Released, etc.), Driver, Department, and Customer.

##### How to Filter

1.  If you want to filter display by a certain period, enable the checkbox **Date** and enter the requested date in the fields **from** to.
2.  If you want to filter display by a certain route, enter the corresponding route ID in field **Route ID**.
3.  If you want to filter display by a certain route name, enter the corresponding name in field **Route Name**.
4aws If you want to filter display by a certain status, select the corresponding status from the combobox **Route Status**.
5.  If you want to filter display by a certain driver, select the corresponding driver from the combo box in field **Driver ID**.
6.  If you want to filter display by a certain department, select the corresponding department from the combo box in field **Department**.
7.  Use field **Customer** to filter by a customer.

#### Change and Status

Depending on the route status, you can change this or modify the real values (real distance and real costs) of the route. The fields of this dialog are identical with the fields of dialog **Route Information**.
⇨ Software Reference, "Route Information" on page J-198
⇨ Tutorial, "Change Route Status" on page J-95

#### Clear

Use this entry to delete selected routes. There will be a security query. The route will be deleted if you confirm this by [Yes].

#### Export

The system contains the following export functions:
- Export to navigation systems
- Load data to mobile devices (via cloud)

##### Export to Navigation Systems

With this function you can export the route to a navigation system. The data can be exported in the following file formats:
- **ITN format** (e.g. TomTom)
- **GPX format** (e.g. Garmin)

Please refer to the instruction manual of your navigation system for further information on the file format your device works with.

##### Locations

When exporting you have the possibility to choose whether individual locations are to be exported or not.

**If locations are not exported**, the folder in the Explorer looks like this:
`Route_45.itn`
The content of the file lists only the coordinates of the individual waypoints (start, destinations, end).

**If locations are exported**, the folder in the Explorer looks like this, with a separate file for each leg of the journey:
- `Route_45_0.itn`
- `Route_45_1.itn`
- `Route_45_2.itn`
- `Route_45_3.itn`

If one of these files is opened, it contains the coordinates for the start and end of that specific leg, plus all the intermediate coordinate markings that make up the detailed turn-by-turn route.

##### How to export data

1.  Click the **[Export]** button. This opens the Export dialog.
2.  Depending on the navigation system you have, enable the radio button **ITN** (e.g. for TomTom) or **GPX** (e.g. for Garmin).
3.  Enable the checkbox **Insert location**, when the individual locations are to be exported.
4.  Enable the checkbox **Create new folder for this route** if a new folder is to be created for each route to be exported.
5.  In the **Export path** field specify where the file is to be saved.

> **Standard Path for Export Files**
> You define the standard path for exporting data in the parameters (Parameter: `Path_Export_ITN_GPS_File`).

**Additional information**
⇨ Software Reference, "Export" on page J-202

#### History

The history provides information on who made changes to the documents and when. In the history, you can filter by the following criteria:
- Route ID
- Order number
- Customer

##### How to create a history for an order number

1.  Open the **Query** item in the menu bar.
2.  Use the mouse to click the **[History]** button. The **History** dialog opens.
3.  Enter the order number in field **Document**.
4.  Use the mouse to click the **[OK]** button. This data is displayed.

**Additional information**
⇨ Software Reference, "Filter Routes" on page J-201
⇨ Software Reference, "Route Information" on page J-198
⇨ Software Reference, "Export" on page J-202
⇨ Software Reference, "History" on page J-204

### Reports

This section contains all queries related to reports and statistics. You will find the following entries:
- Selected Route
- Report Launcher
- Statistics

#### Selected Route

You can open the confirmation and delivery lists with the button either for one or for all optimization routes.

> **Image: Confirmation and Delivery List**
> A printable report showing route details: Total Distance, Weight, Time, Vehicle, Driver, and a list of destinations with expected arrival times and delivery/collect weights.

You can print the list and give it to the driver. The list contains all relevant information for the route.

**Additional Information**
⇨ Software Reference, "Confirmation and Delivery List" on page J-206

#### Print Lists

This session shows you how to print lists.

##### How to print the list for a certain route of the optimization

1.  In the **Route** area, select the route for which the list is to be printed.
2.  Use the mouse to click the **[Selected Route]** button. This opens the list.
3.  Using the tree structure on the left side, you can view and print a list of the individual destinations.

#### Report Launcher

Use the Report Launcher entry to open the dialog of that name. It contains all reports, defined in the systems. Select the desired report format and click on [Print Report]. The respective Crystal Report opens.

#### Statistics

With the Statistics entry you have access to powerful statistics covering the entire OTR field. Click the entry, the Statistics dialog opens. It contains the following tabs:
- General
- General graphic
- Vehicles
- Driver
- Departments
- Customers

##### General Tab

This area contains information on routes. The real costs are compared with the planned costs. In addition, the deviation is shown in currency as well as in percent.

The dialog is divided into two sections. The left side contains the filter functions that are the basis for the results on the right side.

> **Screenshot: Statistics Dialog (General Tab)**
> The left pane shows filter options (Date, Route Status, Department, etc.). The right pane shows a list of routes and a detailed "Cost Analysis" section comparing Estimated vs. Real costs for Driver, Toll, Fuel, etc., and a "By Destinations" summary.

**Filter function:**
- After activating the checkbox **Date**, you can enter the date in the fields below **from** and **to**.
- Choose the required status from the checkbox **Route Status**.
- Use combo boxes for **Department**, **Vehicles**, and **Driver ID** to filter.
- In addition, you can select a customer number in the **Customer** section.
- The fields and combo boxes mentioned above can be combined freely. If nothing is selected or entered, all available data is displayed.

##### Create a Statistic

This session shows you how to create statistics.

**How to create statistics for a customer**
You would like to know the route costs for a customer in a certain period.
1.  Activate the checkbox **Date** and choose the requested date, e.g. 01.07.2015 to 31.08.2015.
2.  Enter the customer number in section **Customer** or select the customer from the list via Customer button.
3.  Choose the required status from the combo box **Route Status**, e.g. Completed.
4.  Enter the customer number in the section **Customer from to**.
5.  Click [OK]. The data on the right side is updated.
6.  Tab **Customer** shows the data in graphic form.

**How to create statistics for a vehicle**
You would like to know the route costs for a vehicle.
1.  Select the required vehicle from the **Vehicles** combo box.
2.  Click [OK]. The data on the right side is updated.
3aws Tab **Vehicles** shows the data in graphic form.

**How to create statistics for a driver and a vehicle**
You would like to know the route costs for a driver and a certain vehicle.
1.  Select the required driver from the **Drivers** combo box.
2.  Select the required vehicle from the **Vehicles** combo box.
3.  Click [OK]. The data on the right side is updated.
4.  Tabs **Vehicles** and **Drivers** shows the data in graphic form.

**Additional information**
⇨ Software Reference, "Statistics" on page J-210

### View

This section contains all views. You will find the following entries:
- Route
- Destination
- Calendar

#### Route

This dialog shows general information, vehicles, parameters, and the costs for the selected route. The fields of this dialog are identical with the fields of dialog **Route**.
⇨ Software Reference, "Creating a New Route - General" on page J-165
⇨ Software Reference, "Creating a New Route - Vehicle" on page J-169
⇨ Software Reference, "Creating a New Route - Parameters" on page J-174
⇨ Software Reference, "Creating a New Route - Costs" on page J-180

#### Destination

This dialog shows general information on the destinations of the selected route. The fields of this dialog are identical with the fields of dialog **Destinations**.
⇨ Software Reference, "Edit Destination" on page J-184

#### Calendar

The calendar provides an overview of the routes to be driven and routes that have been driven.

> **Screenshot: Calendar View (Driver Layout)**
> A monthly calendar view is shown on the left. The main area shows a Gantt-like chart with drivers listed vertically and dates/times horizontally, with colored blocks representing assigned routes.

The calendar is divided into two types:
- Vehicles
- Driver

The entries of the lower section change after changing the calendar type in the upper section. If you selected the calendar type **Vehicles**, the lower sections shows the vehicles. If you selected the type **Drivers**, the drivers are displayed.

Use the icons **Month** and **Day** to switch between the periods to be displayed. Double-clicking a day in the monthly view opens the respective day view. The left side shows a timeline in half hour intervals.

Double-clicking an entry on this level opens the **Query** dialog. It shows an overview in table form of the routes including all destinations.

Red entries always signal an overlapping, either in connection with the driver or the vehicle. Double-clicking an entry opens the **Edit Route** dialog. It serves to assign a different driver or a different vehicle easily and quickly.

Use the combo box **Route Status** to limit the contents. You can display the routes depending on their status.

***

# Software Reference

## Configuration

All data required to work properly is configured and administered in this area. The area contains:

-   **Database settings:**
    Here you can make settings for the database connections (OTR and ERP).
    ⇨ "OTR Connection" on page J-130
-   **Parameters:**
    This area is for general settings such as consideration of traffic, priority factors, time factors, etc.
    ⇨ "Parameters" on page J-132
-   **Language:**
    Use this combobox to change the language during operation. Presently, the program is available in the following languages:
    - Spanish
    - English (US)
    - German
    - Portuguese
    - Catalan

### OTR Connection

**Path:** Configuration > Settings

This tab applies to the settings for the OTR database server.

**Description of fields**
- **Data Source**: Here you enter the path to the OTR database.
- **Initial Catalog**: In this field you enter the standard database. This is OTR.
- **User ID**: Enter the user ID in this field.
- **Password**: Enter the password in this field.
- **Test**: With this symbol you can test the connection to the OTR database.

> **Database Connection**
> Please note that these settings have to be made for each user.

### ERP Connection

**Path:** Configuration > Database Configuration > ERP Connection tab

This tab applies to the settings for the ERP database server.

- **Use SQL ERP Connection**: Use this checkbox to control whether a connection to the A+W Business database exists or not.
  - ☐ OTR is not connected to A+W Business database.
  - ☑ OTR uses the following settings to connect to A+W Business database.
- **Data Source**: Here you enter the path to the A+W Business database.
- **Initial Catalog**: In this field you enter the A+W Business standard database.
- **User ID**: Enter the user ID here.
- **Password**: Enter the password in this field.
- **Test**: With this symbol you can test the connection to the A+W Business database.

### Parameters

**Path:** Configuration > Parameters

Here you find all parameters including their description and their specific setting.

#### Description of the Parameters

- **Delivery\_Date/Route\_Origin**: Defines how routes are formed. (Parameter name: `Mulit-routes`)
  - **Yes**: Multi-routes are created. Original routes from A+W Business remain.
  - **No**: No multi-routes are created. A single route is created based on the delivery date.

- **Delivery Date**: Applies if `Delivery_Date/Route_Origin` is YES. (Parameter name: `Delivery_Date`)
  - **Yes**: Route is created based on the original route date.
  - **No**: Route is created based on the delivery date.

- **Generate one Route for each Origin Route**: Defines if an own route is generated for each route from A+W Business. (Parameter name: `Route_Origin`)
  - **Yes**: A route for each origin route of A+W Business is created.
  - **No**: One route for each delivery date will be created.

- **Dynamic vehicle Assignment**: Defines if vehicles are assigned dynamically. (Parameter name: `Dynamic_Vehicle_Assignment`)
  - **Yes**: The vehicle will be assigned dynamically for each route.
  - **No**: The vehicles will be permanently assigned to the routes.

- **Trucks not Allowed**: Defines if roads not permitted for trucks can be used. (Parameter name: `Allow_Routes_Without_Trucks`)
  - **Yes**: Even roads not permitted for trucks can be used.
  - **No**: Only roads permitted for trucks can be used.

- **Toll Mode**: Defines if toll roads are permitted. (Parameter name: `Nokia_Avoid_Tolls`)
  - **Always avoid toll roads**: Completely excludes toll roads.
  - **Avoid toll roads partially**: Excludes toll roads, but relaxes if no route can be found.
  - **Penalty for toll roads**: Penalizes the use of toll roads.
  - **Normal**: Retains the sequence of route sections with toll roads.
  - **Preferred**: Prefers connections with toll roads.

- **Train Mode**: Defines if trains are permitted. (Parameter name: `Nokia_Avoid_Trains`)
  - *Options are similar to Toll Mode: Always avoid, Avoid partially, Penalty, Normal, Preferred.*

- **Ferry Mode**: Defines if ferries are permitted. (Parameter name: `Nokia_Avoid_Ferrys`)
  - *Options are similar to Toll Mode: Always avoid, Avoid partially, Penalty, Normal, Preferred.*

- **Highway Mode**: Defines if highways are permitted. (Parameter name: `Nokia_Avoid_Motorways`)
  - *Options are similar to Toll Mode: Always avoid, Avoid partially, Penalty, Normal, Preferred.*

- **Tunnel Mode**: Defines if tunnels are permitted. (Parameter name: `Nokia_Avoid_Tunnels`)
  - *Options are similar to Toll Mode: Always avoid, Avoid partially, Penalty, Normal, Preferred.*

- **Vehicle Type**: Set the vehicle type. (Parameter name: `Nokia_Vehicles`)
  - Truck
  - Automobile

- **Route Type**: Defines the desired mode of the route. (Parameter name: `Nokia_Mode`)
  - **Fastest**: Optimizes based on driving time.
  - **Shortest**: Optimizes based on distance.
  - **Economic**: Optimizes based on fuel consumption.

- **Costs**: Average price per liter fuel. Used if no vehicle has been selected. (Parameter name: `Average_Cost_Fuel`)

- **Average Fuel Consumption**: Average fuel consumption in liters per 100 km. Used if no vehicle has been selected. (Parameter name: `Average_Consumption_Fuel`)

- **Distance Factor**: Factor for shortest distance optimization. (Parameter name: `Ga_Distance_Proportion`)

- **Weight Factor**: Assesses the relationship of weight and distance. (Parameter name: `Ga_Weight_Proportion`)

- **On-Time Factor**: Counts the number of destinations reached within the delivery/pickup time. (Parameter name: `Ga_OnTime_Proportion`)

- **Priority Factor**: Evaluates the route based on the number of priority destinations. (Parameter name: `Ga_Priority_Proportion`)

- **Time factor**: Based on the length of the route, searches for the fastest route. (Parameter name: `Ga_Time_Proportion`)

- **General route**: Defines the name of manually created routes. (Parameter name: `Default_Route_Name`)

- **Initial Department**: Defines the default department. (Parameter name: `Initial_Department`)

- **License WebService**: Contains the WebService address. (Parameter name: `Ort_License_Web_Service`)

- **Start Time of Route**: Defines the default start time of routes. (Parameter name: `Default_Route_Init_Time`)

- **Duration of Route**: Defines the maximum duration of routes (e.g., 8 hours). (Parameter name: `Initial_Max_Route_Time`)

- **Use Default Initial Address**: Defines if a default address is used as the starting point. (Parameter name: `Use_Initial_Point`)

- **Start Company Name**: The name of the company where the route starts. (Parameter name: `Initial_Companyname`)

- **Initial Address**: The default initial address for routes. (Parameter name: `Initial_Address`)

- **Time On-Site**: Default time in minutes for loading/unloading. (Parameter name: `Default_Visiting_Time`)

- **Show Original Route**: Defines if the original (un-optimized) route is shown. (Parameter name: `Show_Original_Route`)

- **Show Optimized Route with Straight Lines**: Defines if the route is shown as straight lines between waypoints. (Parameter name: `Straight_Optimized_Routes`)

- **Opacity of Optimized Route (Map)**: Opacity value for the optimized route (e.g., 0.5). (Parameter name: `Optimized_Route_Opacity`)

- **Optimized Route Width**: Width of the optimized route in pixels. (Parameter name: `Optimized_Route_Width`)

- **Opacity of the Original Route (Map)**: Opacity value for the original route. (Parameter name: `Original_Route_Opacity`)

- **Original Route Width**: Width of the original route in pixels. (Parameter name: `Show_Route_Width`)

- **Optimized Route Color in Map**: Color value for the optimized route (e.g., #0000FF). (Parameter name: `Optimized_Route_Color`)

- **Original Route Color in Map**: Color value for the original route (e.g., #585858). (Parameter name: `Original_Route_Color`)

- **More than One Route**: Defines if the WebServer calculates several routes. (Parameter name: `Alternatives`)

- **Unit System for Distances**: (Parameter name: `Units`)
  - **Metric**: Kilometers and meters
  - **Imperial**: Miles and feet

- **Country-Code**: ISO country code for the installation country (de, es, uk, fr, us, etc.). (Parameter name: `Region`)

- **Uppercase Letters**: Defines if field contents are displayed in uppercase. (Parameter name: `Upper_Case`)

- **Vehicle Assignment**: Defines if vehicles are automatically assigned during order import. (Parameter name: `Automatic_Vehicle_Assignment`)

- **Images for Reports**: Defines whether to create map images for route sections in reports. (Parameter name: `Generate_Destinations_Image`)

- **Overall Appearance of the Application**: Defines the UI theme (e.g., Office 2010 Blue, Sparkle Orange). (Parameter name: `Overall_Appearance_Application`)

- **Enable Login**: Defines if login is necessary. (Parameter name: `Enable_Login`)

- **Password not Necessary**: Defines if the app can be used without a password. (Parameter name: `Allow_No_Password`)

- **ERP Master Data**: Defines if master data from the ERP system is used. (Parameter name: `Use_ERP_Masterdata`)

- **Use Delivery Address**: Defines if the delivery address can be changed in the module. (Parameter name: `Use_Delivery_Address`)

- **Currency**: Defines the local currency unit (€, $). (Parameter name: `Currency`)

- **OTR Customer Address**: Defines if customer addresses can be changed in OTR. (Parameter name: `Use_Customers_OTR`)

- **Next Maintenance Date**: Defines if vehicle maintenance dates are considered. (Parameter name: `Use_Vehicle_Maintenance`)

- **Number of Days**: Number of days before a maintenance due date to show a message. (Parameter name: `Days_Before_Vehicles_Maintenance`)

- **Export Path**: Defines where export files for navigation systems are saved. (Parameter name: `Path_Export_ITN_GPX_File`)

- **Export**: Defines if the export function can be used. (Parameter name: `Use_Export_To_GPS_Systems`)

## Administration

All data required to work properly is configured and administered in this area. The area contains:
- **User**: Change, delete or edit users. (⇨ "User" on page J-142)
- **Status**: Change, delete or edit status. (⇨ "Status" on page J-143)
- **Customer**: Change, delete or edit customers. (⇨ "Customers" on page J-145)
- **Departments**: Change, delete or edit departments. (⇨ "Departments" on page J-147)
- **Vehicles**: Change, delete or edit vehicles. (⇨ "Vehicles" on page J-148)
- **Drivers**: Change, delete or edit drivers. (⇨ "Driver" on page J-151)
- **Reports**: Access reports. (⇨ "Reports" on page J-154)
- **Data import**: Import data. (⇨ "Data Import" on page J-157)

### User

**Path:** Administration > User

This dialog is used to control user profiles, that are registered under Windows or in a domain.

**Description of fields in the section Detail**
- **User ID**: This field contains the user ID, e.g. Windows authentification. The data are automatically generated at program start.
- **Name**: This field contains the name of the user. The field can be changed.
- **Copy from**: As administrator you can copy an existing user. Open the combobox and select the user to be copied.

### Status

**Path:** Administration > Status

This dialog shows you all defined status. You can define a new status or change an existing one. The field **Editable** shows the status that can be changed (indicated by a green checkmark).

**Description of fields**
**Status Type**: This field contains the status type. The types are split into the following:
- **1: Created**: Automatically set by A+W Business when the wizard is used but not saved.
- **50: In edition**: The route has this mode after a saved route was loaded.
- **100: Planned**: After saving, the route gets this status.
- **150: Organized**: A free status for company organization.
- **200: Released**: Routes can be transferred to the GDC App.
- **250: Initiate**: In the GDC App, the user can start tracking by clicking on Start Route.
- **860: Completion deleted**: In the GDC App, the user can cancel the route.
- **870: Total completion**: In the GDC App, the user can close the route after finishing all destinations.
- **880: Completion unfinished**: In the GDC App, the user can close the route, but at least one destination was rejected or partially accepted.
- **890: Deleted**: In the GDC App, the user can cancel the route.
- **900: Partially completed**: All documents were rejected from the GDC App.
- **1000: Archived**: The OTR user can set the status manually. The route vanishes from the GDC App and is saved to the OTR database.

- **Status**: This field contains the status code.
- **Name**: This field contains the status name.
- **Editable**: This field shows whether the status can be edited or not (green tick).

### Customers

**Path:** Administration > Customer

Use this dialog to add, change or delete basic customer data. Customers are saved automatically if the value `USE_CUSTOMERS_OTR` has been set to **Yes** in the parameters.

**Description of fields in tab Main**
- **Customer No.**: The customer number.
- **Name**: The customer name.
- **Telephone**: The phone number.
- **Address**: The customer address.
- **Priority**: Checkbox is active for addresses that are priority addresses.
- **Latitude**: Latitude of the company address.
- **Longitude**: Longitude of the company address.
- **Time**: Time in minutes for unloading and loading.
- **Clock (button)**: Opens a dialog to enter a time range for the driver on-site.
- **Contact Person**: A contact person at the customer.
- **E-Mail-Address Contact**: The email address of the contact.

**Description of fields in tab Information**
- **Name2**: A further name.
- **Name3**: A further name.
- **Telephone 2**: A further phone number.
- **Fax**: A fax number.
- **Web**: The customer's website address.
- **Description**: A further description for the customer.

### Departments

**Path:** Administration > Department

Use this dialog to add, change or delete departments. This serves for statistical evaluations.

**Description of fields**
- **Department**: The department ID, e.g. dispatch.
- **Name**: The name of the department, e.g. dispatch north.
- **Description**: A further description.

### Vehicles

**Path:** Administration > Vehicles

This dialog contains all created vehicles that OTR can work with. A vehicle may be a truck, a trailer, or a transporter. The dialog is divided into two sections: an overview list and a detailed information area.

**Description of fields in the section Detail**
- **License Plate**: The license plate number of the vehicle.
- **Brand**: The brand of the vehicle (e.g., Iveco).
- **Model**: The vehicle model (e.g., Daily 50 C 14).
- **Chassis Number**: The vehicle chassis number.
- **Purchase Date**: The date the vehicle was purchased.
- **Next Maintenance**: The next maintenance date for the vehicle.
- **Department**: Assigns a department to the vehicle.
- **Maximum Width/Height/Length**: Vehicle dimensions in meters.
- **Maximum Load**: Maximum load of the vehicle in kg.
- **Empty Weight**: Empty weight of the vehicle in kg.
- **Consumption**: Average fuel consumption in liters per 100 km.
- **Costs**: Average price for a liter of fuel.
- **Vehicle Type**: Truck or automobile.
- **From / to**: Timeframe of vehicle availability.
- **Driver**: The assigned driver ID.
- **Name/Surname**: The name of the assigned driver.
- **Routes**: Route numbers assigned to the truck.
- **Sequence**: Determines the sequence if a route is assigned to multiple trucks.
- **With Trailer**: Checkbox to define if the vehicle can accommodate a trailer.
- **Vehicle Available**: Checkbox to define if the vehicle is generally available.
- **GPS Type**: Select the GPS provider (e.g., GDC, Atlantis, SkyeEye).
- **Code**: The code of the respective GPS system.
- **Description**: A description of the vehicle.
