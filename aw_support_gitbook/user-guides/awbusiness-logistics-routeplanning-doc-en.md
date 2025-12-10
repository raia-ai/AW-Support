---
description: "EN_AWBusiness_LogisticsOptimizer_2_2"
---


---
## Administration

### Additional information
⇨ Software Reference, "Reports" on page J-154

### Packaging Types
In this area, you can administer data for your packaging types. The dialog contains all packing types defined. A packaging might be a rack but also a box.

*(Image: Fig. J-16 Packaging shows a dialog box titled "Packmittel-Typen" (Packaging Types). The top list shows existing types like A-Bock, L-Bock, and Box. The bottom "Detail" section shows properties for a selected type, including ID, Type, Description, Department, Width, Height, Length, Empty Weight, and Costs.)*

The table above shows which packaging types have already been created. You can create new packaging types and also make changes to existing types.
The software reference provides a detailed description of the individual fields.

> **Loading Space Optimization**
> The current version does not support a loading space optimization for trucks. Use the defined packaging types for booking purposes like unloading or collecting (tracking of packaging types).

### Additional information
⇨ Software Reference, "Packaging" on page J-155

### Managing Packaging Types
Here you will learn how to create, edit or delete new packaging types.
The following instructions exist for this training module:
* "How you create one new packaging type" on page J-52
* "How to delete an existing packaging type" on page J-52
* "How to make changes to a certain packaging type" on page J-53

#### How you create one new packaging type
1. Go to the menu bar to **Administration**.
2. Press the icon button **[Packaging Types]**. The **Packaging Types** dialog opens.
3. Press the icon button **[New]**. The lower part of the dialog is now available for editing.
4. Enter the packaging ID in field `Packaging ID`, e.g. 1000100.
5. Enter the type in field `Packaging Type`, e.g. A rack, L rack, box.
6. Field `Department` allows to assign a department to the packaging type. This serves for statistical evaluations. The icon button opens the dialog **Select Department**, containing all defined departments.
7. Enter the specific values in the fields `Width`, `Height`, `Length`, and `Empty Weight`.
8. In field `Costs`, you have the opportunity to set up purchase costs for the packaging type.
9. Enable the checkbox `Do no collect` if the customer shall keep the packaging.
10. The `Description` field allows you to enter information about the packaging type.

#### How to delete an existing packaging type
1. Go to the menu bar to **Administration**.
2. Press the icon button **[Packaging Type]**. The **Packaging Types** dialog opens.
3. Select the packaging type that is to be deleted from the table.
4. Press the icon button **[Delete]**. The entry is deleted.

#### How to make changes to a certain packaging type
1. Go to the menu bar to **Administration**.
2. Press the icon button **[Packaging Type]**. The **Packaging Types** dialog opens.
3. Select the packaging type in the table that is to be changed.
4. Press the **[Edit]** button.
5. Carry out the required changes.
6. Press the **[Save]** button. The data is saved.

### Additional information
⇨ Software Reference, "Packaging" on page J-155

### Data Import
Use this dialog to import data in CSV format (MS Excel).

*(Image: Fig. J-17 Data import shows a dialog for importing CSV data. Options include selecting the 'Data to be Imported' (e.g., Customers), specifying an 'Import Path', and setting options like 'Ignore First Line' and 'Field Separator'.)*

Please select the data to be imported from the combo box. The following options are available:
* Customers
* Departments
* Driver
* Vehicles

The software reference provides a detailed description of the individual fields.

### Additional information
⇨ Software Reference, "Data Import" on page J-157

## Planning Routes
This section shows you how to plan routes and create new destinations.
This includes the following training modules:
* "General" on page J-57
* "Import" on page J-58
* "Routes" on page J-59
* "Destinations" on page J-69
* "The Detailed View" on page J-73

### Routes and Destinations

**Objectives**
* Getting to know both working methods
* Getting to know and understanding the import
* Getting to know and understanding the planning phase
* Getting to know and understanding routes
* Getting to know and understanding destinations

**Benefits**
* Route planning determines the most efficient route from A to D via B and C. This saves time and money.

**Definition**
*   **Route**: The route describes the exact way between several waypoints.
*   **Route**: The route is adopted from A+W Business customer data.

**Please note**
*   **Delivery Date**: Delivery date that was transferred from A+W Business.
*   **Original Route**: This number is a route number from A+W Business.
*   **Route ID**: The route ID assigned by OTR.
*   **Sequence**: The sequence of the waypoints within the route.
*   **Dynamic mode**: Groups and routes are created automatically.

### General
OTR can work in two different modes. Which one to use depends on your work process. The settings are made in the parameters.

*   **Mode 1:** The routes are used that are created and transferred by A+W Business. OTR uses these routes for planning and optimization of routes (distance, sequence of stops).
*   **Mode 2:** This is the Dynamic Mode. OTR creates the routes itself. No work is necessary in A+W Business. After the import OTR groups the routes automatically based on the addresses. In this step Geolocation of addresses takes place. Grouping is made by the following criteria:
    *   Addresses
    *   Weight per address (orders are grouped by customers)
The assignment is based on target time, additional stops, e.g. for collecting racks and statistical determination of traffic (Nokia maps).
To print delivery notes in correct sequence, the data can be reported to A+W Business in this mode, too.

### Import
Data import is made via number manager. During the import OTR checks the addresses and either uses the address from the order header, an alternate delivery address or the address from the OTR master data.
In this step Geolocation of addresses and grouping take place. Based on longitude and latitude the system calculates the distance between the individual destinations and combines the orders into areas and routes under consideration of weight and available trucks.

*(Image: Fig. J-18 Sections and table overview shows the main planning interface with a map on the left displaying colored groups of destinations, and tables on the right for 'Routes' and 'Destinations'.)*

The table shows in the `Routes` section the number of route to be travelled.
The graphic below contains on the left side the groups in different colors. So you can see at a glance how many destinations are grouped. Adjacent to the right are the respective routes and destinations.
A selected destination on the map is highlighted in the table. Thus, identification is simple and stops can easily be assigned to a different group.

### Routes
This area shows you all routes that are current routes for delivery.

*(Image: Fig. J-19 Route Information shows a table listing current routes with columns for Route Name, Route ID, Delivery Date, Original Route, License Plate, Brand and Model, Fuel Costs, Fuel Consumption, and Truck Load.)*

The content of the field `Name of the Route` (ROUTE NORD) is obtained from the A+W Business master data. The `Route ID` (8) is assigned by OTR and increased by 1 for each route. The `delivery date` (21.03.2014) is from A+W Business, as is the content of the field `Original Route` (21).
Assign the `Truck Driver`, the `License Plate` as well as the `Brand and Model`. The content of the fields `Fuel Costs` and `Fuel Consumption` are obtained from the OTR master data (parameter: Fuel costs, Average Fuel Consumption).
Double-clicking a route opens the Route dialog.
The software reference provides a detailed description of the individual fields.
In case the number manager contains orders with various delivery dates, the system creates or splits automatically different routes. You can override this manually in Planning step.

#### Additional information
⇨ Software Reference, "Creating a New Route - General" on page J-165

### Load a Saved Route
OTR automatically saves the routes after the last process step (Result).
You can access a route at any time in order to optimize it with new parameters. The ID is not changed during this process. Only routes with the following status can be loaded:
*   Roughly scheduled (planned)
*   Scheduled in detail (optimized)

*(Image: Fig. J-20 Saved route list shows a dialog with a list of saved routes in the top panel and the destinations for the selected route in the bottom panel.)*

The software reference provides a detailed description of the individual fields.

#### Additional information
⇨ Software Reference, "Creating a New Route - General" on page J-165

### Copy a Saved Route
With this function, you can copy a route to perform various simulations so that you can make the best possible decision.
Copying the route changes the ID. For this, the route status is insignificant, i.e. you can copy routes with any route status.

*(Image: Fig. J-21 Copy saved route shows the same 'Saved Routes' dialog as the previous figure, but with the 'Copy' button highlighted.)*

The software reference provides a detailed description of the individual fields.

#### Additional information
⇨ Software Reference, "Copy a Saved Route" on page J-161

### Working with Routes
Here you will learn how to create, edit or delete new routes.
The following instructions exist for this training module:
* "How to create a new route" on page J-62
* "How to load a saved route" on page J-66
* "How to copy a saved route" on page J-67
* "How to delete a current route" on page J-67
* "How to combine routes" on page J-68

#### How to create a new route
1.  Press the **[New Route]** button. This opens the **Route** dialog, tab **General**.

    *(Image of the 'Route' dialog's 'General' tab. Fields include Delivery Date, Start Time, Route Status, Route Name, Description, and Starting Point details like Name, Street, Latitude, Longitude.)*

2.  In the `Delivery Date` field, define the day on which the route is to take place. Clicking on the arrow at the end of the field opens the calendar from which you can easily select the respective date.
3.  In the field `Start Time`, enter the time at which the route is to start. You can set the time with the arrows at the end of the field.
4.  Assign a name to the route in the field `Route Name`.
5.  You can enter a detailed description of the route in the `Description` field.
6.  The content of the fields `Name`, `Address`, in the `Starting Point` are values that you have set up in the parameters (fields: `Start-Company Name`, `Start-Address`). If your route hasn't started yet, you can overwrite the entries.
7.  If the address specified under point 6 should also serve as starting point, enable the checkbox `Use Starting Point`. If the address and starting point do not correspond, it may be attributed to the fact that you have a headquarters with several subsidiaries. In this case, the headquarters is not the starting point of the route.
8.  If the longitude and latitude fields are not filled, click **[Geolocate]**. This opens the **Simple Geolocation** dialog.

    *(Image of the 'Simple Geolocation' dialog. It shows an address field, a map view with a red pin, and Latitude/Longitude fields.)*

    The map view shows you the address with a red dot. If the address is correct, the `Latitude` and `Longitude` fields are filled automatically.
9.  You can accept the data by pressing the **[Accept]** button.
10. Then go to the **Vehicles** tab.

    *(Image of the 'Route' dialog's 'Vehicle' tab. It shows fields for the selected vehicle (License Plate, Brand, Load, etc.) and a section for Drivers.)*

11. Click on the **[Select Vehicle]** button. The **Select Vehicle** dialog opens.

    *(Image of the 'Select Vehicle' dialog, showing a list of available vehicles with their properties.)*

12. Select the vehicle that is to be used for the route.
13. Press the **[OK]** button. The vehicle will be adopted.
14. Switch to the tab **Parameter** tab.

    *(Image of the 'Parameters' tab. It includes settings for Multiroute, Toll Mode, Highway Mode, Tunnel Mode, and Route Mode.)*

15. Make the desired selection for `Toll`, `Highway` and `Tunnel Mode`.
16. Select the `Route mode`.
17. If desired, change the route factors in the `Optimization` area.

    *(Image of the 'Route Factors' dialog with sliders for Distance, Weight, On Time, Priority, and Time factors.)*

18. Press the **[OK]** button. The settings will be transferred. You are now back in the Planning area.

#### How to load a saved route
1.  Press the **[Load Saved Route]** button. The dialog **Saved Route List** opens.

    *(Image of the 'Saved Routes' dialog, listing previously planned or optimized routes.)*

2.  Select the required route.
3.  Press the **[OK]** button. You will be asked whether you want to add the saved route to the current route.
4.  Press the **[Yes]** button. The selected route is adopted. You are now back in the Planning area.

#### How to delete a saved route
1.  Press the **[Load Saved Route]** button. The dialog **Saved Route List** opens.
2.  Select the route that you would like to copy.
3.  Press the **[Delete Route]** button. You will be asked whether you really want to delete the route.
4.  Press the **[Yes]** button. The selected route will be deleted.

#### How to copy a saved route
1.  Press the **[Copy Route]** button. The dialog **Saved Routes** opens.

    *(Image of the 'Saved Routes' dialog.)*

2.  Select the required route.
3.  Press the **[Route]** button. You will be asked whether you want to add the saved route to the current route.
4.  Press the **[Yes]** button. The selected route is adopted. You are now back in the Planning area.

#### How to delete a current route
1.  In the `Route` area, select the route that is to be deleted.
2.  Press the **[Delete Route]** button. You will be asked whether you really want to delete the route.
3.  Press the **[Yes]** button. The selected route will be deleted.
4.  Press the **[Delete Route]** button. You will be asked whether you really want to delete the route.
5.  Press the **[Yes]** button. The selected route will be deleted.

#### How to combine routes
Sometimes it might make sense to combine a route. To do so, proceed as follows:
1.  In the **Destinations** area, select the data records that you would like to combine.

    *(Image showing multiple destinations selected in the 'Destinations' table.)*

2.  Open the context menu with the right mouse key. It is important where (on which route) you open the context menu. Additional stops are assigned to this route. The following message appears:
    `Group selected records by route (Id: 70/Tour Ost / Route East - 21.03.2014-24)`

3.  Point your cursor at the message and click it.
4.  Both routes are combined into one.

    *(Image showing the destinations now grouped under a single route.)*

#### Additional information
*   ⇨ Tutorial, "Routes and Destinations" on page J-56
*   ⇨ Tutorial, "Vehicles" on page J-42
*   ⇨ Software Reference, "Load a Saved Route" on page J-163
*   ⇨ Software Reference, "Creating a New Route - General" on page J-165
*   ⇨ Software Reference, "Creating a New Route - Vehicle" on page J-169
*   ⇨ Software Reference, "Creating a New Route - Parameters" on page J-174
*   ⇨ Software Reference, "Vehicles" on page J-148

### Destinations
This area contains information about the individual destinations that are driven to on the route. Either goods are unloaded or racks are collected at certain destinations.

> **Number of waypoints**
> Please note that a route may not have more than 37 waypoints (destinations). This is the maximum number that Nokia can work with in a route.

*(Image: Fig. J-22 Destinations shows a table of destinations with columns like Route Name, Sequence, Order, Customer, Name, Address, Delivery Weight, and Collected Weight.)*

The content of the field `Name of the Route` (ROUTE NORD) is obtained from the master data. The `Route ID` (8) is assigned by and increased by 1 for each route. The sequence of the waypoints comes from, whereby 0 represents the starting point. The order number is shown in the `Order` field, the customer number in the `Customer` field, the customer name in the `Name` field and the customer address in the `Address` field.
The `Delivery Weight` field contains the weight of the delivered goods. The `Collected Weight` field shows you how heavy the collected goods are. This could involve, e.g. racks that you collect on the way.
The checkboxes `Delivery` and `Collection` indicate whether the waypoint is a delivery point, a collection point or both.
Double-clicking a destination opens the **Edit Destination** dialog.
The software reference provides a detailed description of the individual fields.

#### Additional information
⇨ Software Reference, "Edit Destination" on page J-184

#### Display Documents
If you would like to know what a customer has ordered, you can view the individual orders.
Open **Documents** tab.

*(Image: Fig. J-23 Documents shows the 'Edit Destination' dialog with the 'Documents' tab active. It lists orders for a customer and shows their location on a map.)*

The software reference provides a detailed description of the individual fields.

#### Additional information
⇨ Software Reference, "Show Information" on page J-189

#### Deletion of Documents
The context menu permits to delete documents. This might be necessary for documents with content that can not be delivered.

*(Image: Fig. J-24 Documents shows the context menu with a 'Delete Document' option on a selected document.)*

#### Show Items
If you would like to know which customer has ordered what, you can view the individual items of an order by destination.
Open **Items** tab.

*(Image: Fig. J-25 Items shows the 'Edit Destination' dialog with the 'Items' tab active. It lists the individual product items within an order, with details like product code, description, quantity, dimensions, and weight.)*

The software reference provides a detailed description of the individual fields.

#### Additional information
⇨ Software Reference, "Show Items" on page J-188

#### Show Information
If you would like to know which information are defined for a customer, you can view these.
Open **Information** tab.

*(Image: Fig. J-26 Information shows the 'Edit Destination' dialog with the 'Information' tab active. It displays contact information for the customer, such as Contact Person, Telephone, and E-Mail.)*

The software reference provides a detailed description of the individual fields.

#### Additional information
⇨ Software Reference, "Show Information" on page J-189

### The Detailed View
If you have a large vehicle fleet and a large shipping area, the content of the areas **Routes** and **Destinations** may become very cluttered.
The **Detailed View** gives you the opportunity to restrict the displayed data. If the **Detailed View** button is enabled, only the destinations of the route are shown that you have selected in the **Routes** area.

*(Image: Fig. J-27 Detailed view turned off shows the main planning screen with multiple routes and all their destinations visible, leading to a cluttered view.)*

*(Image: Fig. J-28 Detailed view turned on shows the same screen but with 'Detailed View' active. Only the destinations for the single selected route are displayed, simplifying the view.)*

If you select a route in section **Routes Detailed View** you can use the **Group** icon button to split the route into several groups.
The software reference provides a detailed description of the individual fields.

#### Additional information
⇨ Software Reference, "Detailed View" on page J-191

### Edit Customer Address
OTR offers the possibility to save customer data. For this purpose, the respective value has to be enabled in the parameters (parameter: OTR Customer Addresses).
Then, the button as well as the respective dialog is enabled.

*(Image: Fig. J-29 Customers shows a dialog listing all customers with their number, name, address, and geolocation data.)*

Double-clicking an entry opens the **Edit Destination** dialog. Changes that are made in this dialog are saved in the OTR database and are available the next time. The following values are saved:
*   Geolocation
*   Address
*   Delivery times (from / to)
*   Unloading time

The software reference provides a detailed description of the individual fields.

> **Changes to customer addresses**
> Please note that the changes to customer addresses that you make here are not written back to A+W Business. The changes are saved in the OTR database.

#### Additional information
⇨ Software Reference, "Customers" on page J-190

### Working with Destinations
Here you will learn how to add destinations to a route, to change them and to delete them.
The following instructions exist for this training module:
*   "How to add a new destination to a route" on page J-76
*   "How to delete a destination from a route" on page J-77
*   "How to edit a destination" on page J-78

#### How to add a new destination to a route
1.  In the **Routes** area select the route to which you would like to add a new destination.
2.  Press the **[New Destination]** button. The **New Destination** dialog opens.

    *(Image of the 'New Destination' dialog, with fields for Customer No., Customer, Address, Type (start/mid/end point), delivery times, weights, and a map view.)*

3.  This field `Customer No.` is preset with number 9999. Enter the respective name in the `Customer` field and open the dialog of the same name by pressing the [Customer] button. This is where all customers saved in the OTR database are listed.
4.  In the `Type` field, specify whether the destination is a starting point, the end point or an intermediate point.
5.  In the fields `From` and `To`, you can enter the times at which the driver is to be at a destination. This can be used e.g. if a company has fixed delivery times.
6.  You can set up the duration of stay in the field `Time (minutes)`.
7.  The field `Selected Route` contains all of your routes currently in planning. This way you can simply assign the new destination to the desired route.
8.  You can enter the weight of the delivery in the `Delivery Weight` field.
9.  If you collect empty racks at a destination, you can enter this weight in the `Collected Weight` field. These values are required for the concrete determination of costs but are not absolutely necessary.
10. You can enter a detailed description about the driver in the `Description` field.
11. In the field `Address` you can enter the customer address. Please enter the name of the street and the name of the city separated by comma.
12. Then, press the **[Suggestions]** button. A list with suggestions as well as a map view appears beneath the address. You can transfer an entry from the list to the address field by marking it. You can also click the red marking point in the map view and, while keeping the mouse key pressed, pull it to another position on the map.
13. Close the dialog by pressing the **[OK]** button.

#### How to delete a destination from a route
1.  Tag the location you would like to delete in the **Destinations** area.
2.  Press the **[Delete Destination]** button. The message `Delete Destination` appears.
3.  Close the message by pressing the **[Yes]** button. The entry is deleted.

#### How to edit a destination
1.  Tag the location you would like to edit in the **Destinations** area.
2.  Press the **[Edit Destination]** button. The dialog **Edit destination** opens.
3.  Make the required changes.
4.  Close the dialog by pressing the **[OK]** button.

#### Additional information
*   ⇨ Software Reference, "Edit Destination" on page J-184
*   ⇨ Software Reference, "Customers" on page J-190
*   ⇨ "Working with Routes" on page J-62

### Costs

**Objectives**
*   Working with the Costs dialog
*   Learning and understanding how to work with various costs
*   Creating and editing costs

**Benefits**
*   Fleet park data has to be maintained accurately in order to determine route costs. This is the only way to obtain accurate values.

**Definition**
*   **Variable costs**: Costs that also change when changing a variable (total distance, fuel costs).
*   **Fixed costs**: Costs that remain unchanged when changing a variable (total distance, fuel costs).
*   **Route costs**: What the route actually costs.

**Please note**
*   **Real costs**: Costs that are entered when the driver has returned from the route.

### Expenses
This area shows you which expenses you have to reckon with.

*(Image: Fig. J-30 Costs shows the 'Costs' tab of the Route dialog. It is divided into 'Variable Costs', 'Fixed Costs', and 'Route Costs', with fields for both planned and 'Real' costs.)*

The fields are automatically filled after optimization. Based on these values, you can create various kinds of reports which you can present to the customer as cost analyses.
The tab is divided into three sections:
*   Variable costs / Real variable costs
*   Fixed costs / Real fixed costs
*   Route costs / Real route costs

#### Variable Costs
This area contains the costs that are variable and that also change when changing a variable (total distance, fuel costs). This may involve costs such as average fuel price and average consumption. The values are obtained from the respective parameters (Configuration > Parameter > Vehicles).
The values in the area `Real Variable Costs` can only be entered once your driver has returned with the route report. Then you know how high the actual costs were. You can enter these costs in the dialog **Edit Route** in the tab **Route Information**.
The software reference provides a detailed description of the individual fields.

#### Fixed Costs
This area contains the fixed costs, which remain unchanged when changing a variable (total distance, fuel costs). This involves costs such as insurance, tax and repairs.

**Example**
| Cost type | Costs/Year |
| :--- | :--- |
| Insurance per year | 1,200.00 € |
| Tax per year | 800.00 € |
| Maintenance per year | 300.00 € |

In total: 2,300.00 €. Based on an estimated number of routes of approx. 220 per year, the resulting fixed costs is 10.45 € per route. This value should be included in the vehicle master data. If the vehicle is assigned to a route, the fixed costs of the route will be increased by 10.45 €.
The software reference provides a detailed description of the individual fields.

#### Route Costs
This area contains the total costs of the route. The route costs consist of variable and fixed costs. They cannot be changed manually.
The software reference provides a detailed description of the individual fields.

#### Additional information
*   ⇨ Software Reference, "Creating a New Route - Costs" on page J-180
*   ⇨ Software Reference, "Route Information" on page J-198

## Optimizing Routes
This section deals with the optimization of the route.
This includes the following training modules:
*   "Optimizing Routes” on page J-84
*   "Changing Routes" on page J-88

### Overview

**Objectives**
*   Getting to know and understanding route optimization

**Benefits**
*   The more efficient the route is, the lower the costs are. Routes are optimally calculated and drivers are less burdened.

**Please note**
*   **Optimized route**: Sequence of the waypoints after optimization.
*   **Original Route**: Sequence of the waypoints before optimization.

### Optimizing Routes
Once all waypoints have been localized, the next step in optimizing the route is performed. This means, OTR puts the individual waypoints in an optimum sequence based on the defined factors.

*(Image: Fig. J-31 Optimization of the route shows the optimization result screen. On the left is a map with the optimized route drawn. On the right is a list of the waypoints (stops) in the optimized order, along with a summary of total distance, costs, and time.)*

This dialog shows you the result of the optimization in a chart and in a table. The map with the route is located on the left side. The route width and opacity can be set in the parameters (parameter: `Optimized_Route_Opacity`, `Optimized_Route_Width`). At the right, you see the route as a list.
The combo box in the upper right contains all routes that you have optimized. If you have optimized more than one route, you can select the respective route from the combo box.
The two tabs beneath it (Optimized Route/Original Route) show you the order of the individual stations after optimization (Optimized Route tab) and before optimization (Original Route tab).
The list below this provides a summary of the route in the upper area.

In the example above, the route consists of four stations, whereby the starting point of the route is always regarded as a station.
With the help of the symbols next to it, you can show and hide the route in the map view. Possible settings are:

| Icon | Description |
| :--- | :--- |
| (Traffic Symbol) | **Traffic** This symbol indicates that traffic is turned on. |
| (Show Route Symbol) | **Show route** If this symbol is activated, the route is shown in the map view. |
| (Hide Route Symbol) | **Hide route** If this symbol is activated, the route is hidden in the map view. |

The color symbol allows you to temporarily change the route color in the map view. Click the symbol twice to open the Color dialog. Here you can assign a different color to the route. The default value of the color is based on the parameter settings (`Optimized_Route_Color`).
The small white arrows in the route indicate the direction of the route.
The route has a total distance of 152.13 km and the driving time amounts to 2 hours and 2 minutes. The costs of the route are € 15.44. This value calculates the vehicle's fuel consumption, the fuel costs and the total distance.

> **Costs of Route**
> The costs of the route are calculated on the basis of the values that you have defined for the vehicles. The more accurate these values are, the more accurate the route costs will be. This primarily applies to fuel costs, which tend to fluctuate to a great extent.

The neighboring field `Toll` tells you whether the route contains toll roads.
The starting point is indicated by a green dot. You declared this waypoint as such during planning. You can neither move it nor change it. To make such changes, you have to go back to **Planning**.
All of the following waypoints have a red dot. In addition, the following information icons are available:

| Icon | Description |
| :--- | :--- |
| (Delivery Symbol) | **Delivery** This icon shows you that goods are to be unloaded at this address. |
| (Collection Symbol) | **Collection** This icon shows you that goods are to be collected (generally racks) at this address. |
| (On-time Symbol) | **On-time** This icon shows you that the address has a fixed time at which goods can be unloaded or collected. This can be the case if the customer has fixed times for goods acceptance or goods can only be unloaded at a construction site at certain times. |
| (Priority Symbol) | **Priority** This icon shows you that the address has a priority. |

Waypoints in the list can be shifted to another position by drag & drop. After a waypoint was shifted re-optimization is made automatically.
Double-clicking a waypoint in the list opens a field with respective detailed information in the map view. This field also appears if you double-click the waypoint in the map view.
Double-clicking a route section in the map view opens a field with respective route information, e.g. distance from A to B.

### Different Map Modes
Here you can select from various map views.
*   Map view
*   Satellite
*   Terrain
*   Traffic conditions
*   Public transport
*   Show traffic incidents

In the `terrain` view you can see topography and height. The `satellite` view provides 2D images and the `map` view shows you the map.

**Next step:**
Result of the optimization, Page J-93

#### Additional information
⇨ Software Reference, "Optimize Route" on page J-193

### Changing Routes
This section shows you how you can change route criteria.
The following instructions exist for this training module:
*   "How to assign a priority to a waypoint" on page J-88
*   "How to remove a priority from a way point" on page J-88
*   "How to chang the sequence manually" on page J-88
*   "How to stop an optimization" on page J-89
*   "How to edit the route" on page J-89
*   "How to change factors" on page J-90

#### How to assign a priority to a waypoint
1.  Select the waypoint from the list.
2.  Click on the flag.
The flag is shown in green and symbolizes that the address has priority. After new optimization, this waypoint is located at the uppermost position (priority).

#### How to remove a priority from a way point
1.  Select the waypoint with the priority.
2.  Click on the flag.
The flag is shown in gray and symbolizes that the address no longer has priority.
3.  After new optimization, this waypoint is located at any position in the sequence.

#### How to change the sequence manually
1.  Select the waypoint from the list and keep the mouse key pressed.
2.  Drag the waypoint to the desired location within the list.
3.  Release the mouse key once you have reached the position at which you would like to drop the waypoint.
The waypoint is now moved to this position

> **Do not forget to perform a new optimization**
> If you change the sequence of the waypoints manually, you have to perform a new optimization in order to update the values.

#### How to stop an optimization
If for whatever reason you need to stop an optimization, proceed as follows.
1.  Press the **[Stop Optimization]** button. The optimization is stopped. The data from the previous optimization remain unchanged and are shown.

#### How to edit the route
1.  Press the **[Edit Route]** button. The **Route** dialog opens for the selected route. In this tab you can change the delivery date, the starting time and the name of the route.

    *(Image of the 'Route' dialog, 'General' tab.)*

2.  In the **Vehicles** tab, you can change the vehicle and the driver.
3.  In the **Parameter** tab, you can change the Route Mode and the Optimization Factors.
4.  In the **Costs** tab, you can change the Toll Costs and the Extra Costs.

#### How to change factors
1.  Press the **[Optimization Factors]** button. The **Optimization Factor** dialog opens for the selected route.

    *(Image of the 'Route Factors' dialog with sliders for various factors.)*

2.  Now you can move individual factors back and forth. As the total always amounts to 100%, changes made to factors always affect the other factors.
3.  If you want to fix a value, press the **[Lock]** button. This locks the value and it can no longer be changed.
4.  To reset the factors to the default settings, press the **[Default Values]** button. The values are then changed in line with the parameter settings.

#### Additional information
⇨ Software Reference, “Route Factors" on page J-178

## Check Results
This section deals with the result of the optimization.
This includes the following training modules:
*   "The Result of the Optimization" on page J-93
*   "Change Route Status" on page J-95
*   "Real Route Costs" on page J-96

### Overview

**Objectives**
*   Changing the route status
*   Exporting data for a navigation system
*   Printing delivery lists for your drivers
*   Created subsequent real route costs

**Benefits**
*   By entering real route costs, your estimated route costs become more accurate. This gives you a more solid foundation in planning in terms of costs.

**Definition**
*   **Polylines**: Lines are portrayed on the map with the aid of polylines, which represent a sorted sequence of locations.
*   **Locations**: Are objects on a card that are bound to longitude and latitude coordinates.

**Please note**
*   **White fields**: The white fields in the dialogs Route and Destination are used to copy field content. No changes can be made to the content.
*   **Real costs**: The real costs can only be determined once the driver has returned from the route and has submitted the route report.

### The Result of the Optimization
Once optimization has been run, the last step takes place - the presentation of the result.

*(Image: Fig. J-32 Result of the optimization shows the final result screen, which combines the Routes table, the Destination list, and the map view with the optimized route.)*

This dialog shows you the result of the optimization in detail. It consists of three sections:
*   Routes
*   Route Plan
*   Destination

#### Routes
This area contains the current optimization of the routes.

*(Image: Fig. J-33 Result of the optimization, Route area shows a close-up of the 'Routes' table in the result screen.)*

The `Route Status` field show the status of the route. After optimization, the status is `Roughly scheduled`. Then the delivery date is shown.
The `Original Route` field shows you the route number assigned by A+W Business. The `Route ID` shows you the route ID assigned by OTR. The field `Name of the Route` contains the name that you have assigned or selected in the Planning. The `Costs` involve the costs for a liter of fuel and the field `Consumption` contains the fuel consumption of a vehicle for 100 km. The field `Kilometers Driven` shows you the entire route and the field `Route Time` how much time this route takes. The `Route Costs` are calculated on the basis of the route, vehicle fuel consumption as well as the fuel price. In the field `Weight` you see how heavy the load is, where returned racks are portrayed with a minus sign. The field `Vehicles` shows you which vehicles are used on the route and the field `Truck Driver` shows you the name of the driver.
Double-clicking a route opens the **Route** dialog, which has been described in detail in a previous section.

#### Route Plan

*(Image: Fig. J-34 Route plan shows a map view of the planned route with numbered destination markers.)*

This area shows you the route with its destinations.
The **[Zoom In/Zoom Out]** button lets you zoom in and out of the view.

#### Destination
This area shows you the individual destinations.
Double-clicking a destination opens the **View Destination** dialog, which has also been described in detail in a previous section.

#### Additional information
*   ⇨ Tutorial, "Destinations" on page J-69
*   ⇨ Software Reference, "Edit Destination" on page J-184

### Change Route Status
Once the optimization has been run, you can change the status of the route in this area.
The following values are then available:
*   **Roughly scheduled:** This is the status of the route after optimization.
*   **Detailed schedule:** This status is not analyzed at present.
*   **Released:** Once you have changed the status to released, the `Delivery Date`, the `Sequence` and the `Route` are returned to A+W Business. Additionally, the data are loaded in the Cloud. You can only change the status to released once.

Beside the route status, you can change the department and **Edit the route**.

#### How to change the status of a route
1.  Select the route from the list.
2.  Use the mouse to click the **[Edit Route]** button. The **Edit Route** dialog opens.

    *(Image of the 'Edit Route' dialog's 'Status Route Information' tab, showing the 'Route Status' dropdown.)*

3.  Choose the required status from the combo box `Route Status`.
4.  Exit the dialog by pressing **[OK]**.

#### Additional information
⇨ Software Reference, "Route Status" on page J-196

### Real Route Costs
Only once your driver has returned from their route, are you able to ascertain how high the actual costs were. For instance, the planned free route might have been blocked and the driver may have had to revert to a section with a toll road. This could not have been foreseen at the time the route was planned. The real costs therefore differ from the planned costs of the route.
In OTR you have the possibility to enter the real costs retroactively. They are then available for future route plans.

#### How to enter the real costs
1.  Open the **Query** item in the menu bar.
2.  In the **Route** area, select the respective route.
3.  Use the mouse to click the **[Edit Route]** button. The **Edit Route** dialog opens.
4.  Switch to the tab **Route Information**. The `Real Costs` fields initially have the same values as the cost fields on the right side.

    *(Image of the 'Edit Route' dialog showing the 'Route Information' tab with 'Costs' and 'Real Costs' sections.)*

5.  Correct the `Real Costs` fields. You can overwrite the values or set them all to 0 beforehand with the button **[Clear costs]**.
6.  When you are done with your entries, you see how much the route really cost in the field `Real Route Costs`.

#### Additional information
⇨ Software Reference, "Route Information" on page J-198

## Driving and Tracking Routes
This sections deals with the driver tasks on the route and the possibilities of the employee in the company regarding the tracking.
This includes the following training modules:
*   "Preparations" on page J-99
*   "Driving Routes" on page J-101
*   "Tracking Routes" on page J-109

### Overview

**Objectives**
*   Load documents in the Cloud.
*   Getting to know and understanding the GDC app for the drivers.
*   Getting to know and understanding booking via Browser.
*   Getting to know and understanding the tracking function.

**Benefits**
*   The tracking function always provides the employees in the company with information regarding the route. Many situations are promptly dealt with. E.g. a damaged lite can be reproduced while the truck is still on the route.

**Definition**
*   **GDC app**: App for Android, to be downloaded in Google Playstore free of charge.

**Please note**
*   **Android**: The GDC app available for Android in Google Playstore.
*   **and others**: The users of non-Android systems can use the Browser for direct login.
*   **Update**: Don't forget to press the [Update] button in Route Administrator from time to time to synchronize the data.

### Preparations
To make sure that both the App and the GPS tracking work correctly, the following preliminary work is necessary:

#### Respective Route Status
To load the route data in the Cloud, it is necessary to set the route status to `Released`.
Thus, mark the corresponding route in section **Result**, click on the **Edit Route** button and select the status `Released` from the combobox `Route Status`.
For a detailed description on how to edit the route status, please see:
⇨ "How to change the status of a route" on page J-95

> **Route Status Released**
> As soon as you change the route status to `Released`, it is not possible to transfer these orders again from A+W Business to OTR. If this should be necessary, you have to copy the number manager first to get new order numbers. Make sure that the new order status is in the correct status range (generally 01 to 800).

#### Loading Documents in the Cloud
To provide documents for the driver in digital form, they have to be loaded in the Cloud, too.

*(Image of the 'Attach Files' dialog, showing how to link a file path (e.g., a Google Drive link) to a specific destination on a route.)*

To do so, proceed as follows:

#### How to load documents in the Cloud and reference them
1.  Open the **Query** menu.
2.  Click on the **[Attach Files]** button. The dialog with the same name opens.
3.  Field `Route ID` contains the route selected before. Use fields `Customer` and `Order` to enter information for the driver.
4.  The **Destination** area, shows the destinations that are driven to on the route. Choose the destination for which the document shall be entered.
    *   Click on **[Plus]** icon button. The **Attach Files** dialog opens.
    *   Field `File Name` allows to enter a name, e.g. `Delivery Note`.
    *   Field `File Path` allows to enter the corresponding path for the Cloud, e.g. `https://drive.google.com/file/d/....`
    *   Use field `Description` for further information.
    *   Exit the dialog by pressing **[OK]**.
    *   Section `Files` contains all corresponding documents.

### Install App or use Browser
Booking of data can be based on two different types:
*   Via app (for Android devices)
*   Via Browser (for non-Android devices)

#### How to install the App (Android)
1.  Open Google Play Store.
2.  Load the Android app **GDC: Goods Delivery Control**.
3.  Install the app.

#### How to work with a Browser (non-Android device)
1.  Start the Browser (Safari).
2.  Enter the URL. You find the respective address in OTR in `Start > About A+W Logistics Optimizer`, section `GDC Web App`. In our example: **http://gdcapp.onerbox.com**
