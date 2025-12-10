---
title: "EN_AWBusiness_Production_2-1"
source: "EN_AWBusiness_Production_2-1.pdf"
tags: ["Logistics", "Scanning", "Barcode", "Picking", "Shipping", "Vehicle Management", "Driver Management", "Inventory", "A+W Business Production", "Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial for the Logistics module of the A+W Business Production software. It provides step-by-step instructions on creating barcode scanning templates, managing shipping and picking processes, defining vehicles and drivers, and generating material and capacity overview reports."
long_description: "This tutorial provides a comprehensive guide to the Logistics functionalities within the A+W Business Production software. It is designed to walk users through various essential tasks for managing the dispatch and delivery of goods. The document begins with instructions on how to create a template for scanning status updates using barcodes, including prerequisites and a step-by-step process. It then moves into the 'Picking' module, explaining its objectives and benefits for organizing dispatch through a company's vehicle fleet. Key sections cover Shipping Organization, how to define vehicles and enter driver details into the master data. The tutorial provides detailed procedures for compiling a vehicle load, allocating orders to trucks, and handling potential overloads. It also covers printing critical documents for drivers, such as loading lists and acknowledgement of receipt lists. The final part of the document focuses on generating analytical reports, specifically the 'Date Overview' for assessing material requirements over a period and the 'Capacity Overview' for previewing production quantities against delivery dates. Each section includes 'How to' guides, explanations of UI elements, exercises, and references to related software documentation."
---

# Logistics Tutorial

---
## Create a Template for Scanning

A+W Software GmbH usually provides the templates for scanning the status. You can complete these templates or set up new barcodes.

> **Prerequisite**
> A text processing program and a barcode font type must be installed on the computer. Please pay attention to the code type your scanners read, e.g. code 39.

### How to create a scanning template based on barcodes
1. Start the text processing program, e.g. Word.
2. Enter the barcode number and name.
3. In the next line, repeat the number but with the prefix s, e.g. **s48**.
4. Allocate the barcode fonts and a suitable type size to the line.

**Fig. E-43: Create a barcode template**
*(This figure shows a Microsoft Word document with three status labels: "Status 48 - AWBar produziert", "Status 68 - AWBar versandfertig", and "Status 88 - AWBar ausgeliefert". Below each label is a corresponding barcode.)*

5. Print the template and check whether the barcodes can be read correctly.

---

## Exercises
Change the order status by simulating the keyboard scanner.
- Raise the status.
- Can you reduce the status? If not, why?
- Change the settings and try reducing the status again.

**Additional Information**
- ⇨ Master Data, "Statusverwaltung" on page B-895
- ⇨ Master Data, "Statuspunkte" on page B-896
- ⇨ Software Reference, "Status Message and Packaging Allocation" on page E-218
- ⇨ Software Reference, "Status Message Options" on page E-223

---

## Picking

### Objectives
- Loading a vehicle for a trip in the optimal way.
- Drawing up lists by date and route as a basis for loading the delivery vehicles.

### Benefits
- Picking serves to organize dispatch through your own fleet of vehicles. The program shows the total weight of the orders to be transported by one vehicle. Overloads or not fully utilized vehicles can thus be avoided, even at the planning stage.
- The loading lists tell the driver which racks to load for the current trip.
- The driver uses the acknowledgement of receipt lists to have the recipient confirm the correct delivery of the individual orders.

### Please note:

- **Fleet of vehicles**: At least one vehicle must be entered in the master data. Drivers can be allocated after they have been entered in the master data as well.
- **Racks**: The terms Rack and Packaging have the same meaning. They include the different types of racks, but also pallet cages, pallets, etc.
- **Loading of vehicles**: You can only print the rack load list if racks have been allocated to the order items.
- **Means of transportation**: All order items are packaged for transportation. Various means of packaging are available, e.g.:
    - Racks of different sizes and shapes
    - Containers
    - Racks etc.
- **Rack allocation**: Order items must be allocated to racks (means of packaging) so that they can be shown on the loading list.
- **Default settings**: Master data
    - Vehicles

---

## Shipping Organization
You have used route planning to plan the dispatch of goods. You can now plan the delivery of the finished orders via your own fleet of vehicles. Picking serves to compile the orders by delivery date and route, and allocate them to a vehicle.

To allocate vehicles and drivers, they must be entered in the master data first. Enter the tare and the total weight of every truck. When orders are allocated, A+W Business checks whether the total weight has been reached or even exceeded. If the Picking dialog shows that the truck is overloaded, the selected orders have to be allocated to another route, another truck, and/or another delivery date.

You can allocate a driver to each truck who does not have to be adopted for picking purposes.

Orders can be automatically collected in a Number Manager for picking. From there, the corresponding rack loading list or the acknowledgement of receipt list can be printed.

The different lists serve to support the drivers in the loading of vehicles and delivery of goods.

> **Prerequisite**
> To allocate drivers to the vehicles, you have to enter the drivers' names in the master data first.

---

## Define Vehicles
To compile the deliveries for a route, allocate the orders to a vehicle. The system can only check whether the selected vehicle is correctly utilized or overloaded if the vehicle data have been entered correctly. This session shows you how to enter the master data for vehicles.

### How to enter a vehicle
1. Go to the menu **Master data > Dispatch > Truck**.

**Fig. E-44: Truck management - enter vehicle**
*(This figure shows the truck management interface. The left panel lists truck names (e.g., GI-AW-123). The right panel shows details for the selected truck: Name, Driver, Tare, Total weight, and a 'Locked' checkbox.)*

> ⇨ Master Data, "Lkw" on page B-874

2. Go to the menu **Start > New** to switch to the input mode. The fields will be enabled.
3. Enter the name, tare, and total weight. Tare and total weight are displayed at picking to prevent the truck from being overloaded. For a name, you can also enter the forwarder who ships your orders.
4. Select the driver who usually drives this truck. The driver can be changed in dispatch planning.
5. Go to the menu **Start > Save** to save the data. The data is saved.
6. Repeat steps 2 to 5 for further vehicles.

---

## Enter Driver Details
The names of the drivers can be allocated to a certain vehicle or route. Once defined, the names cannot be deleted. If a driver should not be used again, he has to be blocked. This session shows you how to enter the master data for drivers.

### How to enter a driver
1. Go to the menu **Master data > Dispatch > Driver**.

**Fig. E-45: Master data - enter driver**
*(This figure shows the driver master data interface, which is a table with columns for Name, External key, and a 'Locked' checkbox. Example names include Eddi Smith, Josef Müller, and Klaus Maier.)*

> ⇨ Master Data, "Lkw" on page B-874

2. Go to the menu **Start > New** to switch to the input mode.
3. Enter the name.
4. Go to the menu **Start > Save** to save the data. The data is saved.
5. If required, repeat steps 2 to 4 for further drivers.

---

## Compile Vehicle Load
To ship the orders of a route, the racks must be loaded onto vehicles. The load is checked against the total weight of the vehicle; any overload will be reported. This session shows you how to allocate the orders to a vehicle.

> **Tip**
> Create a Number Manager with the first order to be picked. You can then collect all orders in this Number Manager for which you establish loading lists.
> Collecting the routes in separate Number Managers, e.g. by delivery date, makes printing easier to control.

### How to compile the load for a truck
1. Go to the menu **Production > Dispatch > Picking**.

**Fig. E-46: Compile the load**
*(This figure shows the 'Picking' interface with several labeled sections.)*

- **A** Number Manager for loading lists
- **B** Positions of the selected order
- **C** Selected truck
- **D** List of orders on Number Manager
- **E** Quantity of all orders for the truck
- **F** Weight of all orders for the truck
- **G** Maximum payload of the truck
- **H** Total number of all selected orders
- **I** Total weight of all selected orders

> ⇨ Software Reference, "Consignment" on page E-228

The overview (D) shows all orders listed in the Number Manager. The Items section (B) shows the items of the selected order.

If you have ticked an item in the Items section, you can open the Status report and rack allocation dialog by selecting **Function > Rack allocation**. This way you can make up for the rack allocation should you want to print a loading list.

> ⇨ "How to allocate the order items to a rack" on page E-100

2. If necessary, tick the checkbox **Transfer to NM**. The combo box (A) for selecting the Number Manager is released.
3. Select the required Number Manager or enter a new name at random.
    - If you select a Number Manager, the orders included will be listed automatically. If you have chosen this method, proceed with step 6.
    - If you have entered a new name, all orders will be removed from the list. If you have chosen this method, proceed with step 4.
4. Go to field **Number** and enter the number of the order you want to pick.
5. Select **Start > Execute** to import the order data.

**Fig. E-47: Picking**
*(This figure shows the 'Picking' interface after orders have been added.)*

- **A** Allocate truck
- **B** Allocate driver
- **C** Total of all orders for the truck
- **D** Sum of all selected orders

The order appears in the Orders section. Compile more orders in the same way.

6. Select the order you want to pick. The fields in sections **Entry** and **Items** list the order details that are important for shipping. You can now change the order details, e.g. the route or the delivery date. The changes will be saved in the order. The values always apply to the entire order. Individual items can only be picked by creating a partial delivery.
7. Check whether the delivery terms are correct. Orders that are going to be picked up require no further treatment. They cannot be deleted from the view, however.
8. Select the truck (A).
9. To adopt the allocation, go to the menu **Start > Execute**. If the truck has been allocated a standard driver in the master data, he will be shown automatically. You can select another driver. The details on the truck and the driver are saved in the order. The weights and quantities of all orders to be delivered with the selected truck on the delivery date are shown in the section **Totals**. If the maximum load is exceeded, the weight (C) is displayed in red. You then have to allocate the (last) order to another route, another vehicle, and/or another delivery date.

**Fig. E-48: Load list**
*(This figure shows the 'Consignment' or load list view, which lists all orders assigned to a specific truck.)*

- **A** Load list
- **B** Orders for the same truck
- **C** Total of all orders for the truck

When a truck is completely loaded, you can print the delivery notes, as well as the loading list and the acknowledgement of receipt list.
> ⇨ "Printing Lists for the Driver" on page E-111

---

## Printing Lists for the Driver
The result of picking is printed on lists:
- The **loading list** shows all racks to be loaded onto this truck. This list tells the driver which racks have to be loaded.
  > ⇨ Software Reference, "List Printing" on page E-233
- The driver uses the **acknowledgement of receipt list** to get confirmations for the delivery of the orders. The list shows all racks by customer and order, including the loaded quantities.
- The **rack list** gives an overview of the shipped racks. The list shows all racks and their shipping date by driver, route, and customer.

### Print Lists
This session shows you how to print the different lists.

> **Rack allocation**
> You have to allocate the order items to a rack in order to print a loading list.

### How to print the loading list for the driver
1. Go to the menu **Production > Dispatch > Print list**.

**Fig. E-49: List printing**
*(This figure shows the 'List Printing' dialog. The main area (A) lists orders from a Number Manager. The bottom section (B) contains checkboxes for the types of lists to print: "Rack loading list", "Acknowledgement of receipt list", and "Rack list (delivered)".)*

- **A** Number Manager
- **B** Printer settings

2. Select the Number Manager (A) that contains the picked orders. The orders appear on the list.
3. Click on the button **[Rack exit]** to check whether the rack allocation is correct. The dialog of that name opens.

**Fig. E-50: Check shipping of racks**
*(This figure shows the 'Rack shipment' dialog, which verifies that racks only contain orders from a single customer.)*

Checking the rack exit makes sure that a rack only contains orders from the same customer. Racks must not contain orders from different customers. Orders that have not been allocated to a rack will not be displayed.

4. Click on **[OK]** to check out the displayed racks, then press **[End]** to close the dialog. The **Print list** dialog reappears in the foreground.
5. Select the option (B) for the list you want to print, e.g. the loading list.
6. Choose one of the following options in the **Print** menu:
    - **Screen**: The list appears on screen. From there, it can also be sent to the printer.
    - **Printer**: The list is sent to the standard printer.

> **Printing more lists**
> Print the acknowledgement of receipt list and the off-site rack list in the same way. To do this, choose the corresponding option in step 5.

---

## Exercises
- Define different vehicles. The individual payloads should be quite different.
- Allocate the appropriate number of vehicles to the orders and make sure that they are properly utilized.
- What can you do if an order cannot be shipped by any of your vehicles because the total weight of all items is too high? Try your solution.

**Additional information**
- ⇨ Master Data, "Tourrangfolge" on page B-802
- ⇨ Master Data, "Lieferdauer (Kunde, Lieferant)" on page B-831
- ⇨ Master Data, "Touren" on page B-872
- ⇨ Software Reference, “List Printing" on page E-233

---

## Overviews
This session shows you how to draw up overviews of your dates and capacities. It covers the following subjects:
- "Date Overview" on page E-115
- "Capacity Overview" on page E-123

---

## Date Overview

### Objectives
- Drawing up criteria for checking the material required within a certain period.
- Drawing up and comparing the schedule based on different criteria.

### Benefits
- You can get an overview of the quantities required for production within a certain period.
- This enables you to determine whether there is sufficient stock on hand for delivering the entered orders without delay.

### Please note:
- **Selection of criteria**: The criteria for drawing up the evaluation depend on the following settings:
    - Evaluation mode
    - Breakdown level
    - Restrictions
- **Evaluation mode**: This mode defines which products or product groups shall be taken into account. Depending on the settings, certain fields are locked or available in order to restrict the evaluation further.
- **Breakdown level**: The breakdown level defines the way in which the selected products shall be grouped.
- **Restrictions**: The restrictions determine the characteristics for restricting the view.
- **Default settings**: None

### Material Required per Period
You can get an overview of the quantities to be produced or delivered within a certain space of time. The evaluation level can be extended down to order or even item level.

Evaluation will show the following values:
- Quantity unit
- Total for this quantity unit (referring to the main or BOM item)
- Total quantity
- Total square metres
- Total linear metres (always refers to the main item).

Sub-totals will be formed for every selection criterion, which are summed up in a grand total.

For evaluation, you can define whether orders from a certain Number Manager or the orders on hand should be assessed based on the defined criteria, e.g. by status. The following evaluation modes are available: by production area, by product group, or by product.

**Fig. E-51: Overview by product type and Number Manager**
*(This figure shows two versions of the 'Date Overview' dialog and the resulting data table.)*
- **A** Breakdown level
- **B** Product type
- **C** Totals of all orders displayed
- **D** Sub-totals per quantity unit

### Evaluation mode
Evaluation can be based on three different modes:
- **Production area**: Within the production area you can distinguish IG, toughened glass, laminated glass, single annealed glass, cutting, and auxiliary material for IG. If you have chosen the production area Cutting, for instance, evaluation can be restricted to Shape cutting.
- **Product groups**: The following has to be taken into account for evaluation by product group: A product can be allocated to two different product groups. One is valid for pricing, the other for statistics. It is therefore necessary to state which of the two PGR areas shall be used for evaluation. Product group combinations can be evaluated as such.
- **Product**: Evaluation by product permits the distinction of product type and product group. You can restrict evaluation to a single product number if required.

> **Showing the reference period**
> Display of the material consumption in a reference period can also include archived orders. Just enable the entry Options in the Archives menu.

---

## Draw up a Schedule
This session shows you how the Schedule dialog can tell you what needs to be produced within a certain period, and which materials are required for this purpose.

> **Choosing the criteria**
> The Schedule dialog offers a multitude of criteria for displaying the future material consumption. The following instruction will not deal with all of them in detail. You will be made aware of any peculiarities, however, which offer a different kind of view.

### How to draw up an overview of the material required
1. Go to the menu **Production > Schedule > Schedule**.

**Fig. E-52: Overview by material and date**
*(This figure shows the 'Date Overview' dialog with several sections for setting criteria.)*
- **A** Selection for the production area mode
- **B** Evaluation mode, releases the groups A, C, D, and E
- **C** Restrictions
- **D** Selection for product group mode
- **E** Selection for production mode
- **F** Breakdown level, subdivides the evaluation

> ⇨ Software Reference, "Date Overview (Dialog)" on page E-267

2. Choose the Number Manager and - if applicable - the client and the order area. Select the option **Number** and enter the order number to get an overview of a single order.
3. Select the evaluation mode (B). Selecting the mode will release more fields for choosing additional criteria. In this example, the mode by production area is selected. If you choose the evaluation mode by product group, you can select a product group (PGR), super product group (SPG), or main product group (MPG) in the section **Select product group (E)**. The evaluation always shows the main product group (MPG), however.
    > ⇨ Master Data, "WGR" on page B-577
    If you also need main product groups or super product groups for your evaluation, you can go to the Capacity overview dialog.
    > ⇨ "Capacity Overview" on page E-123
4. Choose the period to be evaluated. If you enter the same date in both fields, only this one day will be evaluated.
5. Choose the breakdown level. This setting refers to the display of data in the overview. Breakdown by date makes sense, for example, if you want to evaluate a longish period. In the view, the orders will be grouped by date in this case. The sub-total per quantity unit always refers to the breakdown level.
6. Choose the status area of the orders to be taken into account. If you need a preview for quite a long period of time, you should choose the status **Document entered** first, for example. The second status will be **Released for production** because these orders are not completed yet. If you choose **Transfer to Production** in both fields, the preview will be for a short time instead. To evaluate a period in the past, enter the corresponding date. The fields in the section **Evaluation period** are accessible if you select the option **Number** in the **Source** section. Leave the order number field empty in this case.
7. Choose the production areas (A) and restrictions (C) to be displayed. The settings refer to the main product. To view the in-house cut float, for example, tick the option **Cutting**.
8. Go to the menu **Start > Execute** to create the overview.

**Fig. E-53: Schedule by production area**
*(This figure shows the 'Date Overview' results table, populated with data based on the selected criteria. It displays orders grouped by date, with columns for Document ID, Name, Quantity, Units, etc.)*

The evaluation is shown in the section **Table** according to the selection criteria. If the search with the defined criteria did not produce any results a message appears and the Table tab is empty. The print version shows the overview in the same way.

---

## Exercises
- In the Number Manager you are using for these exercises, check the material you will be needing for production until the end of this quarter.
- Change the evaluation mode, then the breakdown level, and compare the results.

**Additional information**
- ⇨ Software Reference, "Date Overview (Dialog)" on page E-267

---

## Capacity Overview

### Objectives
- Defining different evaluation criteria.
- Analyzing the evaluation.

### Benefits
- You can get an overview of the products by the product groups (MPG, PSG, PGR) to be produced within a defined period.
- You can tell whether there is sufficient production capacity for delivering the entered orders without delay.

### Please note:
- **Capacity overview**: This overview has no connection with capacity planning. You cannot change dates or determine the production sequence.
- **Default settings**: None

### Capacity Preview
This will roughly tell you which products have to be finished for a certain delivery date. The Capacity overview dialog is not linked with production or capacity planning in any way. The evaluation shows the quantities by main or super product group, product group, order status, or delivery date. This simple overview tells you whether there is sufficient raw material in stock and whether the scheduled dates are realistic.

---

## Draw up a Capacity Preview by Delivery Date
This session shows you how to draw up an overview of the quantities which have to be delivered on a certain date.

### How to draw up an overview for a delivery date
1. Go to menu **Production > Schedule > Capacity overview**.

**Fig. E-54: Capacity overview by delivery date**
*(This figure shows the 'Capacity Overview' dialog.)*
- **A** Breakdown level
- **B** Fields for selecting the product groups

This dialog is described in:
> ⇨ Software Reference, "Capacity Overview" on page E-275

2. Choose the breakdown level (A). To see how much IG is to be produced, for example, just choose the product groups you have organized for IG.
3. Disable the checkbox **all** to evaluate only certain product groups on the selected breakdown level.
4. Tick the checkbox **with BOM** to include the bills of material in the evaluation. You can use this to get an overview of the processing steps, for example.
5. Choose the status area of the orders, e.g. from **Document entered** to **Production release**.
6. Check the delivery date. The current date is displayed by default. You can change this if required.
7. Go to the menu **Start > Execute** to create the overview.

**Fig. E-55: Capacity overview by product group per delivery date**
*(This figure shows the results of the capacity overview. The data is grouped first by delivery date, and then by product group within each date.)*
- **A** Total per delivery date
- **B** Total amount per product group

The totals of the individual product groups (B) show what needs to be produced within the defined period.
