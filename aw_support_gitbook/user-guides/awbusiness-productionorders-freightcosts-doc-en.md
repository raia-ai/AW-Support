---
title: "EN_AWBusiness_Production_2-2"
source: "EN_AWBusiness_Production_2-2.pdf"
tags: ["A+W Business Production", "Production Orders", "Freight Costs", "Issue of Boxes", "Stock Management", "Capacity Overview", "Tutorial", "ERP", "Manufacturing Software"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A training tutorial for the A+W Business Production software, focusing on additional features. The document provides exercises and detailed instructions on managing production orders, calculating freight costs, and handling the issue of boxes for shipping."
long_description: "This document serves as a detailed training module for the A+W Business Production software, specifically covering advanced functions within the Production module. It begins with an exercise guiding users on how to create an overview of scheduled production, applying filters for time period and product groups. The core of the manual is divided into three main sections under 'Additional Features': 'Production Orders,' 'Freight Costs,' and 'Issue of Boxes.' The 'Production Orders' section explains the process of replenishing stock through manual or automatic orders, detailing how to enter production data, report order completion, and book stock additions. The 'Freight Costs' section covers the calculation, evaluation, and distribution of imputed and forwarding freight costs. This helps users determine the profitability of delivery routes and manage costs associated with third-party forwarders. The 'Issue of Boxes' section details the workflow for allocating and withdrawing boxes from inventory for shipping, including the use of dummy boxes for reservation and the process of updating stock levels upon issuing real, ID-tagged boxes. Each section outlines objectives, benefits, system prerequisites, and provides step-by-step instructions accompanied by UI screenshot descriptions."
---

# Overviews Tutorial

---
## Exercises

Draw up an overview of the scheduled production. Select the following criteria:

- 14 days at the beginning of the next quarter
- Breakdown by main product group
- Select main product group 1 and 2

Change the criteria and check the evaluation results.

**Additional information**
⇨ Software Reference, "Capacity Overview" on page E-275

---

# Additional Features

This session will introduce the additional functions of the Production module.

This includes the following training modules:

- "Production Orders" on page E-128
- "Freight Costs" on page E-137
- "Issue of Boxes" on page E-146

---

## Production Orders

### Objectives

- Introducing manual and automatic reports from production orders
- Entering production data and updating the stock on hand by means of booking

### Benefits

Production orders are used to replenish the stock on hand. Reports must be implemented and the stock on hand must be updated for this purpose.

### Please note:

**Addition to stock**
Stock additions based on production orders can be booked automatically or manually:
- Manual status change in the Production module.
- Automatic status reports from Production.

**Default settings**
Company data:
- Parameters tab
- Stock/PP/EDI tab > Registration point

### Stock Article as Part of the Production Order

Production orders are used to replenish the stock on hand. All articles entered in such an order must have the supply type Production. Unlike common (customer's) orders, the items are not reserved in stock but are marked as ordered.

Production orders can be entered in different ways:
- Manual input of a new document of the type Work order.
- Copying a saved (dummy) article.
- Automatic creation based on a shortage in the stock on hand.

Production reports the order complete, and the stock on hand is updated.

Manual and automatic input of production orders is explained in detail in the Stock Management tutorial. The individual steps are therefore only summed up in brief at this point.
⇨ Inventory Management, "Production Orders" on page G-131

In Production, production orders are transferred to Production. The ensuing report from Production and the manual input of production data will be described in detail.

### Reports on Production Orders

The addition to stock based on a production order will not be booked based on the printing of an invoice or delivery note. The booking can be triggered by the following actions:

- Status reports via A+W Business Interface Service from the shop floor automatically trigger the booking.
- By manual booking in the Production data dialog.
  ⇨ "Report a Production Order completed" on page E-132

#### How to allocate a status point to the registration point for reports

1.  Define a registration point for the report in the master data.
    The session on Production reports by file describes how to allocate registration points.
    ⇨ "How to allocate a registration point for the report per file" on page E-61
2.  Allocate to this registration point a status point from which the goods are considered to be produced, e.g. when the first item has been completed.

    *(Fig. E-56 shows the "Registration points production" dialog. A registration point named "Cutting started" is selected. It has a status point of "0047 - Produktionsbeginn/Production start" and is set to trigger on "first sheet completed". The dialog also lists other registration points like "versandfertig/Ready for dispatch" and "ausgeliefert/delivered" with their corresponding status points and trigger conditions.)*

3.  Go to the menu Start > Save to save the data.
    The data is saved.

4.  Now allocate the registration point to the report in company data on the Stock/PU/EDI tab.
    ⇨ "Define Company Data Settings" on page E-131

### Define Company Data Settings

You have to check the settings for the production report in company data. The URL of the ERP Webservice is valid for the transfer to Production and the production report in OrderXML format. These settings are described in detail in connection with transfer to Production.
⇨ "How to check the settings in company data" on page E-30

#### How to allocate the registration point

1.  Go to the menu Master data > Company > Company data and proceed to the Stock/PP/EDI tab.

    *(Fig. E-57 shows a section of the Company Data dialog on the Stock/PP/EDI tab. Under the "Order produced at" section, a "Registration point" dropdown is shown with "0300 - Production started" selected. There is a checkbox for "Book stock receipt for work orders".)*

2.  Go to the section Order produced at and select the registration point.
    When an item from a production order gets a status report from this registration point, the item will be added to the stock. This status report can be made in the following ways:
    - Automatically by A+W Business Interface Service.
    - Manually in the Status report dialog.

3.  Go to the menu Start > Save to save the data.
    The data is saved.

### Report a Production Order completed

The completion report for a production order can be used to update the stock on hand. First, enter the raw material required and all production-relevant data for a production order.

The following booking withdraws the raw material from stock; the items of the production order are added to stock.

The following instructions exist for this training module:
- "How to enter the production data" on page E-132
- "How to book a production order" on page E-135

#### How to enter the production data

1.  Go to the menu Production > Production > Production data.
    The dialog of that name opens.

2.  Go to the menu Start > New to switch to the input mode.

    *(Fig. E-58 shows the "Production data" dialog in input mode. The dialog is divided into sections: General, Work order data, Finished product, and Raw material. Key fields are labeled: A) Production order number, B) Number and name of the product to be added to the stock on hand, C) Production details (setup time, persons, downtime), and D) Raw material to be withdrawn from stock.)*

    ⇨ Software Reference, “Production Data (Dialog)" on page E-197
    All fields - except the reason for downtimes - must be filled in.

3.  Go to the General section and enter the date on which the work order was produced, then fill in the other fields in this section.

4.  Enter the number of the production order (A).
    The order data will be imported.

5.  Select the item number for which you want to enter production data.
    The program automatically shows the quantity and the data of the finished product (B) entered for this item. The following entries only refer to the selected item.

6.  Enter the number of units produced on the defined date.

7.  If the item includes a box, the ID can be assigned automatically. Just tick the checkbox Automatically create ID.
    The contents of the box can only be corrected or the box can only be opened if the boxes were entered with individual IDs.

8.  Go to the section Production details (C) and enter the actual production times as well as the number of employees required for production.

9.  Enter zero (0) in the field Downtime (minutes) if there are no downtimes; otherwise, enter the time during which production had to be stopped.
    The combo box Reason of failure can be used to enter the reason why production did not go as planned. If different reasons were entered before, you can select one of them.

10. Go to the section Raw material (D) and enter the data of the product used to produce this item.
    You can also enter the breakage of raw material as well as the corresponding supplier. Breakage of raw material should always be entered so that the stock on hand can be updated accordingly.

    *(Fig. E-59 shows the "Production data" dialog filled with example data. For instance, Order '20308', Item '1', Article 'IG 5/16/6 A+W', with '200' sheets completed. The Raw material section shows 'Float 5 mm A+W' being used.)*

11. Go to the menu Start > Save to save the data.
    The data are listed on the Table tab in short.

    *(Fig. E-60 shows the "Table" tab within the "Production data" dialog. It lists items for which data has been entered but not yet booked. The labels indicate: A) Item data entered but not booked yet, and B) Booked item (no longer appears on the Booking tab).)*

    The Booking tab shows the items for which data have been entered. You can book these items now on the Booking tab or enter more data on the Order tab.

12. Repeat steps 2 to 11 until you have entered all the data you wanted to book.
    When you have entered all the data, you can start the booking process on the Booking tab.

#### How to book a production order

1.  Go to the Booking tab.
    Production data are summed up by production date and machine. If you have entered data for different machines, each machine will be represented by a line.
    Already booked data will not be listed.

2.  Select the entries to be booked:
    - Double-click on a line to select a single entry.
    - Click on icon [All] to select all entries on the list.

    *(Fig. E-61 shows the "Booking" tab within the "Production data" dialog. It lists entries grouped by Production date and Machine, with a checkbox to select them for booking. The example shows entries for "ISO-Linie" and "Autom.-Zuschnitt" machines.)*

    Only items marked with an X have been selected.

3.  Go to the menu Start > Save to start booking.
    - Data will be checked first. After that, a production order's involved will be locked during booking.
    - Stock articles from the production orders will be added. New sub-items will be created for boxes if required in order to book each box with a separate ID.
    - Next, the raw material is withdrawn from stock. When the production order has been produced in full, the status is raised and an entry is made in the history.
    - Finally, the locked documents will be released.

    Booked records are removed from the view. For items of production orders which include at least one booked stock article, the product structure cannot be edited any more at item entry.

### Exercises

- Enter a production order manually and change the status (again, manually) to produced.
- Book the addition to stock in the Production data dialog.
- Check the new stock on hand for the products and the raw material.

**Additional information**
⇨ Master Data, "Übermengen" on page B-858
⇨ Master Data, "Firmendaten - Lager/EK/EDI" on page B-967
⇨ Master Data, "Firmendaten - Produktion" on page B-997
⇨ Sales, "New Order based on Copying" on page C-244
⇨ Sales, "Document - header data" on page C-415
⇨ Sales, "Stock Info" on page C-739
⇨ Software Reference, "Production Data (Dialog)" on page E-197

---

## Freight Costs

### Objectives

- Calculating and evaluating imputed freight costs
- Splitting forwarding costs amongst customer orders

### Benefits

- The calculation of imputed freight costs serves to determine whether a certain route on a certain delivery date is really worthwhile.
- Forwarding costs for routes that cannot be serviced by your own fleet of vehicles can be split amongst the customer orders of the corresponding route.

### Please note:

- **Imputed freight costs**: Routes for which the freight costs are high compared with the profit can be determined by means of a list of delivery dates.
- **Distance and mileage**: For every route, a mileage is defined which is used to calculate the delivery costs in connection with the distance entered in the customer data.
- **Radial calculation**: Imputed freight costs are calculated radially based on the distance between the works and the individual customers, even if several customers are served on the same route.
- **Forwarding costs**: Forwarding costs are split proportionally amongst the customer orders of a delivery date on the same route, based on the relation between distance and transported glass surface.
- **Default settings**:
  - **Master data:**
    - Routes > Freight costs
  - **Customer data:**
    - Production tab > Distance
  - **Company data:**
    - Delivery tab (critical freight cost limit)

### Calculations

Two functions are available for calculating the freight costs:

- **Imputed freight costs**
  - Calculation and printout as a list
  - Calculation of freight costs based on delivery dates, customers, and routes
  - Checking the critical limit for freight costs
- **Distribution of forwarding costs amongst customer orders**

> **Freight costs for locked orders**
> Orders locked by another user will not be included in the evaluation without issuing an error report. This may lead to incorrect freight costs in the orders. This applies to both the calculation of freight costs and to the distribution of forwarding costs.

### Settings for Calculating Imputed Freight Costs

The following data must be defined in order to calculate the freight costs:

- Freight costs per kilometer and route
- Distance in kilometers per customer
- Critical freight cost limit

#### How to set up the requirements for calculation

1.  Go to Master data > Dispatch > Routes.

    *(Fig. E-62 shows the "Routes" master data screen. It lists various routes like "Regional", "Tour Nord/Route North", etc., with a column for "€/km" where freight costs per kilometer are entered, e.g., 0.4 for Regional and 0.5 for Tour Nord.)*

2.  Enter the freight cost per kilometer for every route in column €/km.

    > **Route for forwarder**
    > If you are sending goods via forwarder as well, define another route which is called Forwarder, for instance. Do not enter any freight costs for this route.
    > The session on Route planning describes how to define a new route:
    > ⇨ "How to define a new route" on page E-82

3.  Go to the menu Start > Save to save the data.

4.  Go to Master data > Partners > Customer > Customers.

5.  Enter the distance in kilometers for every customer on the Production tab.

    *(Fig. E-63 shows a snippet of the customer master data, specifically the "Shipping" section, with a "Distance" field set to 10.00.)*

6.  Close partner management after checking and completing all data.

7.  Go to Master data > Company > Company data > Dispatch tab.

8.  Enter the critical freight cost limit in per cent in the section Freight costs.

    *(Fig. E-64 shows the "Freight costs" section in company data, where the "Critical freight costs limit" is set to 1.25 %.)*

9.  Go to the menu Start > Save to save the data.
    The requirements for calculating imputed freight costs are now fulfilled.

### Displaying Imputed Freight Costs

The calculation of the imputed freight costs shows whether a route is really worthwhile on a certain date. An overview shows the routes with freight costs which are too high in relation to the turnover.

Menu Documents > Order > Evaluation > Imputed freight costs serves to display the cost distribution.

*(Fig. E-65 shows the "Imputed freight costs" evaluation screen. It's a table displaying orders grouped by delivery date, route, and customer. Columns include Order value (PP), Contribution Margin (CM), freight cost (FC), and freight cost percentage (FC %). Labels point to: A) Subtotal per customer, B) Total amount for this date, C) Total amount of all routes on the selected delivery date, D) Selected route(s), and E) Total amount for this route.)*

The costs are calculated radially. This means that the distance between the works and the individual customer is always used for calculation.

Imputed freight costs are first calculated at order entry. When an order is entered, the imputed freight costs will be calculated for the present order and for all orders of the customer with the same delivery date and the same route.

> **Example**
>
> A customer receives deliveries by the route Regional at 0.68 €/km.
> With a distance of 10 km, this means imputed freight costs of €6.80 per delivery date.
>
> Proportional distribution of freight costs referring to the actual surface per order:
> 2 orders with a total surface of 40 sqm.
> Order 200188 with a total surface of 30 sqm = 75%
> Order 200189 with a total surface of 10 sqm = 25%
>
> Distribution of the imputed freight costs of €6.80:
> Order 200188 = €5.10 = 75%
> Order 200189 = €1.70 = 25%

If you have defined freight costs, you can also enter the critical freight cost limit as a percentage in company data.

In the order, you can display the calculation in the Functions menu. While the calculation is run, the freight costs that reach or exceed this critical limit are shown in red in A+W Business.

*(Fig. E-66 shows two versions of the "Imputed freight costs" dialog for a single order. The left dialog (A) shows "Order freight costs" at 0.02%, which is below the "Critical freight cost limit" of 1.25% (B). The right dialog (C) shows "Order freight costs" at 2.80%, which is highlighted in red because it has exceeded the critical limit.)*

### Distribution of Forwarding Costs

Forwarding costs incurred by a forwarding agency can be distributed amongst several orders using the following method:

- Distribution of forwarding costs amongst orders by delivery date and route
- Distribution of the total forwarding costs in relation to the distance and to the shipped glass surface

Calculation of the share is based on the actual glass surface without size rounding.

#### How to distribute the forwarding costs for a route

1.  Select in the menu Documents > Order > Evaluation > Imputed freight costs.
    Dialog Imputed freight costs opens.

2.  Go to the Forwarding costs tab.

    *(Fig. E-67 shows the "Forwarding costs" tab of the "Imputed freight costs" dialog. It has sections for: A) Delivery date selection, B) A dropdown to select a Route (without freight costs), and C) a field to enter the total forwarding cost Amount (net).)*

3.  Enter delivery date (A):
    This must be a future date or the present date.

4.  Select the tour (B) e.g. forwarder.
    No freight costs must be entered for this route. The result shows all orders matching the delivery date and route.

5.  Enter the net amount (C) of the forwarder's invoice.

6.  Select in the menu Start > Execute to calculate forwarder's costs.

    *(Fig. E-68 shows the "Forwarding costs" tab after execution. A) A route without freight costs is selected ("Spedition/Forwarding Agency"). D) The total forwarding cost for this route is entered (250.00). The list shows two orders with their glass surface per order (B) and the calculated share of forwarding costs (C) for each.)*

    The defined forwarding costs have been distributed amongst the orders by distance and glass surface.
    If orders are missing from the list, they are either locked by other users or have a different delivery date or route.

### Exercises

- Go to the master data and enter the freight costs of two routes for which you have entered orders.
- Enter the distance in the customer data.
- If required, enter new orders with customers and routes for which you have defined the costs and the distance.
- Check the imputed freight costs at order entry.
- Distribute the forwarding costs to the shipment you have compiled in picking.

**Additional information**
⇨ Master Data, "Touren" on page B-872
⇨ Master Data, "Partnerverwaltung - Produktion" on page B-795
⇨ Master Data, "Firmendaten - Versand" on page B-1004
⇨ Sales, "Imputed Freight Costs" on page C-712

---

## Issue of Boxes

### Objectives

- Understanding the different 'issued' booking versions for boxes.
- Issue of boxes.

### Benefits

- The boxes on stock are allocated to an order in the issuing area, and are thus marked as reserved.
- Depending on the settings, the reserved boxes are withdrawn from stock either before or after the delivery note is issued.

### Please note:

- **Booking of issued goods**: Boxes can be withdrawn before or after the delivery note is issued.
- **Allocating boxes to an order**: Boxes can be allocated before or after the delivery note is printed, and are thus reserved.
- **Stock on hand**: Boxes can only be allocated if they are entered in the stock with a box ID.
- **Default settings**:
  - **Company data:**
    - Stock/PP/EDI tab > stock management mode
    - Parameters tab (virtual item numbers)

### Withdrawal of Boxes

Boxes are usually withdrawn from stock when the delivery note is printed. Printing of the invoice can also be used as a trigger for the withdrawal.

As the person who enters the order will not know which box is actually going to be shipped, he first enters a dummy box with the required sizes. The stock on hand can only be updated after the ID of the real box is entered and withdrawn from stock.

**Example**
A dummy box (without ID) with the required sizes is entered in the order. 3 is specified as the quantity. This reserves three of the dummy boxes.

| Withdrawal |
| :--- | :--- |
| **Before printing the delivery note** | **After printing the delivery note** |
| - The real box IDs are scanned in the issuing area.<br>- Reservation of the dummy box is canceled.<br>- The three boxes with IDs are marked as reserved.<br>- The delivery note is printed. Three boxes are booked upon issue of goods. | - The delivery note is printed.<br>- The reserved dummy boxes will be withdrawn.<br>- When the boxes are issued, the three real box IDs are scanned.<br>- Reservation of the dummy boxes is canceled.<br>- The three boxes are withdrawn. |

*Tab. E-2: Withdrawal of boxes before or after printing the delivery note*

### Box Withdrawal

This session shows you how to withdraw boxes for shipping. The following steps have usually been taken already:

- Product 1005 (for example) was entered in the customer order:

  *(Fig. E-69 shows an order item line for Product 105, "Float 5 mm Kiste/Box", with a quantity entered.)*

- [F1] in the Stock info dialog was used to select the dummy box 104, 400x500:

  *(Fig. E-70 shows the stock search dialog. A "dummy" box item (A), which has no specific ID, is listed. Its reserved quantity is shown, indicating a reservation (B) has been made against this general item.)*

- The box was added to the order and saved, e.g with an item quantity of 3:

  *(Fig. E-71 shows the order item line again, this time with a quantity of 3.)*

- 3 additional reservations were booked for the dummy box on stock:

  *(Fig. E-72 shows the stock info screen again. The "Res." (reserved) quantity for the dummy box (A) has increased by 3.)*

- The booking journal (stock management) shows the item quantity as reserved:

  *(Fig. E-73 shows the "Booking Journal" dialog. It lists a reservation entry for Order 20318, Item 1, with a quantity of 3.00 for the product "Float 5 mm A+W".)*

Next, boxes with IDs shall be allocated and withdrawn after printing the delivery note.
