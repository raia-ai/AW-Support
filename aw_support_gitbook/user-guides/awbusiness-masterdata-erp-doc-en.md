---
description: "EN_AWBusiness_Master_Data_9_1-2"
---


---
## Overview

### Tutorial 1

### Products
Menu Products consists of three sub-menus:
- **General:** This section is used to enter general data for product definition, e.g. product types, product groups, pattern sides, variants.
- **Products:** This is where product master data are entered, e. g. products, size surcharges, and variants.
- **Glass door systems:** The supplementary module for glass door systems is released only for certain customers.

> ⇨ "Product data" on page B-133

### Prices
This is where you enter the price master data, e. g. rates, prices, price units, price groups, and surcharges.
> ⇨ "Price Master Data" on page B-211

### Stock
This is where you enter the master data for stock management. This section is described in the documentation on Stock Management.

### Partners
Menu Partners consists of three sub-menus:
- **General:** This is where you enter general data related to the partners, e. g. groups, lines of business, projects, classifiers.
- **Customer:** This section serves to enter customer-related data, e. g. address, subsidiaries, shipping addresses, routes, payment terms, and partner-related rounding.
- **Supplier:** This section is used to enter supplier-related data such as the address, partner-related rounding, and sources of supply.

> ⇨ "Customer Data" on page B-35

### Dispatch
This is where you enter the master data for dispatch. This section is described in the documentation Production.

### Production
This section is used to set up the master data for production. This section is described in the documentation Production.

---

### Order
This section is used to set up the master data for documents such as status allocations, rounding, number areas, quantity limits.
> ⇨ Tutorial 2, "Documents" on page B-407

### Finances
This is where you enter the master data for payments and invoices, e.g. tax rates and proceeds accounts.

### Company
This section is used for entering your company's master data, e. g. employees and order areas. Details on document entry, data transfer, and pricing are also defined in company data.

### Text
This section is used to enter standard text for the documents as well as text codes. This includes fixed and variable text for announcements and notifications, e. g. regarding holidays.
> ⇨ Tutorial 2, "Printing of Text and Documents" on page B-459

### Forms
This section serves to enter the details for the printing of documents (forms), e. g. headers and footers, print jobs, and options for printing invoices and sketches.
> ⇨ Tutorial 2, "Forms" on page B-471

### CEKAL
This section is used to enter master data for managing CEKAL text. These details are required only in France and the Benelux countries.

### CE code
This section serves to enter details for the CE codes.

### B2B
This is where the details for data exchange are entered.

---

## Basic ideas

The organisation and maintenance of master data is the basis of A+W Business and its modules. The defined data are adopted for all parts of the system. All business units access the same basic master data, e.g. customers, products, prices, status, currencies.

**(Image: Fig. B-2 Master data - examples)**
*A flowchart illustrating the relationships between different business modules and master data components. Modules like "Sales", "Purchasing", "Statistics", and "Capacity planning" are at the top. These modules interact with "Order", "P.O." (Purchase Order), and "Stock". These, in turn, are connected to core master data sections: "Customer", "Product", "Price", and "Suppliers". Arrows indicate the flow of data and dependencies between the sections.*

Master data are linked with all modules of A+W Business. Master data are the basis for handling your business transactions, e.g. customer orders. Interfaces are used to transfer master data to other programs.

The functions of A+W Business are organised by means of a number of links between the master data. This includes the data used to handle your company's business processes and the company-related default settings. Like all defaults, they can be changed in the actual order.

> **Change master data**
> Some of the master data amendments deeply influence the functioning of A+W Business. You will be informed of which data should not be processed without consulting specialists.

---

## From master data to order

**(Image: Fig. B-3 General settings)**
*A simplified flowchart showing how various master data elements contribute to creating an "Order". Data from "Products", "Prices", "Customer", and "Discounts Surcharges" all feed into the central "Order" document.*

This simplified view shows the interrelations of master data. Company-wide settings form the basis for defining prices, products, customers, etc., and mainly influence the processing of orders, price calculation, invoicing, analyses, etc.

The following sections will provide information on how to set up business partners, products, and prices. The main document settings will be introduced afterwards. The appropriate company-wide settings will be mentioned in this connection.

---

## Orders in A+W Business

All commercial transactions in A+W Business are based on master data. When you enter an order, the following data have to be entered (at least):

-   **Order header**
    -   Customer's name and address
    -   Delivery terms and date
    -   Payment terms
-   **Order items**
    -   Product and product structure, e.g. glass, IG, grills
    -   Sizes and processing steps, e. g. shapes, cut-outs
    -   Prices and discounts
    -   Surcharges, e.g. for transport

**(Image: Fig. B-4 Sales order)**
*A composite screenshot of the A+W Business sales order entry screen.*
*   **A - Order header: customer, delivery date, etc.** Shows the top portion of the screen with fields for customer number, name, address, delivery dates, and other header-level information.
*   **B - Order items: product (glass), prices, etc.** Shows the bottom portion of the screen, which is a grid displaying the line items of the order, including product details, quantity, dimensions, pricing, and discounts.*

When the essential order data have been entered, the item have to be produced, packed, and shipped. It may be necessary to purchase additional articles for production which are not kept on stock. The order triggers other business transactions which are automated as much as possible:

-   Printing of other documents, e. g. order confirmation, delivery note, invoice
-   Purchase order issued by purchasing
-   Withdrawal of stock articles for production
-   Transfer of order data to production
-   Report from production once the order has been produced and is ready to be shipped
-   Delivery
-   Check of customer's payments
-   Transfer of invoices to financial accounting

These processes are dealt with in the sections Sales, Purchasing, Stock management, and Production.

The tutorial on master data shows you how to define and maintain the data of business partners, products, prices, surcharges, and discounts. The second part of the training conveys how these data can be tested in documents and how the processes can be controlled.

## Master Data Input

When you enter master data from scratch you should stick to the following recommendation. It prevents you from having to access data that have not been entered yet.

In customer management you can enter many basic data directly, based on the current requirements for customer master data.

> **Note**
> Whenever you enter or change basic data or master data you should test them first. This way you can see - before actually using the new data - whether the result meets your expectations.

We recommend the following sequence for entering master data:
1.  **Customer Data**
    Enter at least the customer data such as address and communication. Special prices and discounts can be added later.
2.  **Product groups**
    First create the product group concept. You will need it for entering the products.
    Product groups can also be entered in product management.
3.  **Products**
    You can enter prices, surcharges, and discounts together with the product. Alternatively, you can enter the price per product then allocate it in the product definition.
    After entering new products and prices, you should test - in quotation or order entry - whether the prices are calculated as required. This may help to save additional time and work for correcting the master data.
4.  **Prices**
    After entering prices, surcharges, and discounts, you can allocate them to the products. If Other surcharges have been entered already, these can be allocated to the prices.
5.  **Special discounts/surcharges**
    Enter the discounts and surcharges which shall be valid irrespective of prices and partners.
    When you have entered special discounts and surcharges, you should test - at order entry - whether these are added and calculated as required.

---

## Basic Tables

The different dialogs for entering master data offer combo boxes for easy selection of data. The entries in these lists are usually saved in so-called basic tables and can be edited.

### Extending basic tables
The input of data in these simple tables is described here, using supplier groups as an example.

**How to enter a new supplier group**
1.  Select menu **Master Data > Partners > General > Supplier group**.
2.  Go to the menu **Start > New** to switch to the input mode.

    **(Image: Fig. B-5 Line for the new supplier group is released)**
    *A screenshot of the "Supplier Groups" dialog. It shows a table with existing groups like "Glaslieferant / Glass supplier" and "Sonstiges / Misc.". A new, blank line is highlighted, ready for data entry.*

3.  Enter at least the name of the supplier group.
    Make sure that the name refers to a special feature of the group, e.g. accessory supplier.
4.  Select in the menu **Start > Save** to save the data.
    The supplier group is saved and can be selected from the dialogs for allocating groups.

### Locks

In nearly all of these dialogs, entries can be locked for further use.

**(Image: Fig. B-6 Example of basic data)**
*A screenshot of the "Titles" dialog, showing a table with entries "Mr.", "Mrs.", and "Company". The "External key" column is labeled 'A' and the "Locked" checkbox column is labeled 'B'.*

External keys can be used for transferring data to other programs.

Locked entries are no longer offered for selection. If they had already been allocated before being locked, they will still be displayed.

### Deletion
Data can be deleted only if they are not being used somewhere else, e. g., if they are not used as a reference. Referenced data have to be locked if they are not going to be used any longer.

If test data are entered during these sessions, and these data are actually going to be used, they can be deleted right away.

> **Additional information**
> ⇨ Overview, "Standard Buttons" on page A-53

---

## Customer Data

This set of topics shows you how to enter master data for customers.

This includes the following training sessions:
-   "Partners" on page B-36
-   "Address Data" on page B-41
-   "Order and Sales Invoice" on page B-53
-   "Employees and Subsidiaries" on page B-60
-   "Text" on page B-67
-   "Classifiers" on page B-73
-   "Finances and Balance" on page B-80
-   "Sales Representatives" on page B-110
-   "Production" on page B-114
-   "Additional Data for Partners" on page B-119

The data for customers and suppliers differ only slightly. The explanations and procedures described in this session therefore mostly also apply to suppliers.

---

## Partners

### Objectives
-   Knowing the difference between master data for partners, customers, and suppliers
-   Completing basic tables for partners

### Benefit
-   Partner data are a quick way of entering orders and purchase orders without having to enter the whole set of data.
-   The entries in the basic tables are linked to another in the more complex dialogs in order to fulfil certain functions, e. g. the country code for selecting the language for a form.

### Note

-   **Partners**: A+W Business distinguishes customers, suppliers, and other partners:
    -   Customers place orders with you and are provided with products by you.
    -   Suppliers will provide you with products you cannot produce yourself.
    -   Partners are all those who are neither customer nor supplier, e.g. your beverage supplier or your tax advisor. A+W Business does not allow entering documents for partners.
    -   Partners from this section can be copied to customer or supplier master data if required.
-   **Partner master data**: Partner master data include all information necessary for entering an order or a purchase order (documents). These data are automatically adopted for the document header and can be changed in the actual document. These changes will not be saved in the partner's master data.
-   **Basic tables**: Basic tables are shown as simple dialogs. They are grouped by topic in the sub-menus of the master data module.
-   **Checkbox Lock**: Entries in the basic tables can be locked. Locked entries are no longer offered for selection. If they had already been allocated before the being locked, they will still be displayed.
-   **Data export**: Partner data can be managed for every client separately. The integrated export function allows to export partner data, e.g. to create serial letters.

---

## Introduction of the Subject 'Partners'

Partner management does not only serve to enter addresses of the partners, but also parameters which make quotation and order entry easier such as route allocation, alternative rounding, staff and subsidiaries, payment terms, projects.

**(Image: Fig. B-7 Interaction of master data for partner management)**
*A flowchart showing how various basic data types feed into the central "Customer-/Supplier Administration". Data from "Titles", "Documents", "Classifiers", "Discounts", "Rounding", and "Projects" all point towards the administration module.*

This illustration shows the interaction of basic data for defining and maintaining partner master data. Partner data can only be completely entered and maintained if the appropriate basic data have been entered before, e. g. titles, discounts, rounding.

---

## Partner Management Dialog

Customer and supplier data are entered in A+W Business as partner master data in dialog Partner management. These master data are used in documents and can be changed there if required. Amendments made in the documents will not be saved in master data.

**(Image: Fig. B-8 Dialog Partner Management)**
*A screenshot of the "Customers | 4000-A+W Training" screen, also known as the Partner Management dialog.*
*   **A - Tabs for different customer data**: Points to the row of tabs at the top (1. Address, 2. Order, 3. Empl./Subsid./Transact., etc.).
*   **B - Open the basic table**: Points to a file folder icon next to a dropdown menu, indicating a way to access and edit the list of options for that field.
*   **C - Additional information and display**: Points to the right-hand panel and the bottom data grid, showing fields for last change information and a summary view of partners.

Apart from addresses and communication data, customer master data include financial data, data on the customer's credit standing, and specific production data. The file icon (B) can be used to switch to the corresponding basic table in order to complete the data.

Other specific features regarding suppliers will be introduced in the appropriate training session.

> **Data protection**
> Personal data are subject to data protection. Please make sure that this kind of data is protected from improper use by means of the appropriate access rights.

---

## Master Data Dialogs for Partners

Menu Partners offers the sub-menus General, Customer, and Supplier in which you can enter general and partner-specific data. All these dialogs are described in detail in the software reference.
> ⇨ Software Reference, "Partners" on page B-742

The following basic data must be entered so that the complete customer and supplier data can be defined.

| Path > Dialog | Meaning |
| :--- | :--- |
| **Partners > General > Titles** | Apart from the usual titles such as Mr, Mrs, and Messrs, you can enter other titles, e.g. for addressing foreign partners appropriately. |
| **Partners > General > Title** | In A+W Business, titles mainly describe the contact's position in the company, e.g. production manager, managing director. |
| **Dispatch > Delivery terms** | Delivery terms refer to the means of transport by which the goods are going to be shipped, e. g. railway, forwarder. |
| **Dispatch > Routes** | In Routes, you enter the usual day for the route as well as the delivery fee to be used for calculating the freight costs. It is essential to define a route for collection as well as one for transport by forwarder - provided you are using forwarders at all. |
| **Finances > Tax** | These are the different tax rates applied to the orders from your customers. You can enter national as well as international tax rates and allocate the suitable tax rate to every single customer. |
| **Finances > Payment terms** | The payment terms are used for determining the credit term and the cash discount amount. |
| **Finances > Banks** | These are bank accounts you are using for transactions with customers or suppliers. After you have entered the complete details, the system can determine the IBAN in partner master data. |
| **Finances > Currency** | You can enter the different currencies plus the corresponding exchange rates if you are using several currencies. No entries are required for the Euro zone. |
| **Finances > Modes of payment** | You can enter the modes of payment your company will accept. These details can also be transferred to financial accounting (FinAcc). |

In addition to the data entered in the dialogs in menu Partners, other data from the following dialogs can be used for defining customers and suppliers:

-   **Prices:** Price list, key, rate, and Price
-   **Surcharges:** Other surcharges, exchange surcharges, shape surcharges
-   **Finances:** Tax, cost type, cost centers

> **Description of dialogs in other sections**
> Some of these dialogs are described in detail in other sections. These dialogs will not be handled in detail in the master data tutorial.

---

## Address Data

### Objectives
-   Going through the Partner management dialog
-   Defining and allocating customer groups
-   Defining and allocating routes and delivery terms

### Benefit
-   Customer master data are centrally entered and maintained. New orders are therefore always based on up-to-date master data.
-   Address data are used for dispatch and invoicing. Alternative addresses can be entered if required.

### Note

-   **Partner management**: Dialog Partner management serves to enter the master data for every customer which apply just for this partner.
-   **Address**: A main address is entered for every partner which is generally used for shipments and invoicing.
-   **Line of business**: The line of business is an additional analysis and sorting criterion for statistics.
-   **Language**: Documents are printed on the forms that fit the customer's language and customs.
-   **Groups**: Customers can be assigned to a customer group, e.g. for collective maintenance of prices or discounts.
-   **Route**: Routes are the basis for dispatch planning and control. The shipping date is determined by means of the delivery time and the delivery date.

---

## Address Settings

Tab Address serves to enter the data for the address, communication, and dispatch.

**(Image: Fig. B-9 Dialog Partner management – tab Address)**
*Screenshot of the Partner Management dialog, focused on the 'Address' tab.*
*   **A - Address data for the order header**: Points to the main address block (Company, Name, Street, etc.).
*   **B - Contact data are completed by the settings on tab Order > Document dispatch**: Points to the 'Connections' section (Phone, Fax, Email).
*   **C - Section Specifications: Selection and input of the appropriate details**: Points to the 'Specification' section on the right (Line of business, Language, Group, Route).

We are going to explain the settings on this tab in closer detail in the following paragraphs.

### Lines of Business
Every customer and supplier can be allocated to a line of business, e. g. glass dealer, window manufacturer, joiner. If a new customer belongs to a line of business which has not been defined before, you can use the file icon to go to dialog Lines of business to enter the new line of business.

The line of business is an additional analysis and sorting criterion for statistics.

### Language
Every customer is allocated the language in which documents and forms shall be printed. The appropriate forms will be selected based on this code.

If you define additional languages you should also translate the price units and quantity units.

### Groups
Partners can be united in groups. Every customer can be allocated to a customer group and every supplier, to a supplier group.

When you enter e. g. discounts or prices for a group, these terms will apply to all members of the group. This makes the maintenance of terms easier.

When you enter a document, the settings which are based on the allocated group, can be changed in the individual fields.

**Examples for the use of groups**
-   **Customer group**
    -   Marginal income limits
    -   Prices
    -   Discounts
    -   Rounding
    -   Surcharges
    -   as a sorting criterion in customer turnover statistics
-   **Supplier group**
    -   Prices
    -   Discounts
    -   Rounding
    -   Surcharges
    -   as a sorting criterion in supplier turnover statistics

The groups for partners are entered in **Partners > General > Partner groups, customer groups, supplier groups**. Proceed as described in connection with Basic tables.
> ⇨ "Extending basic tables" on page B-33

When you have defined the groups you can allocate them to the customer or supplier in Partner management > tab Address.

**(Image: Fig. B-10 Partner management - Group allocation)**
*A cropped screenshot showing the 'Specification' section in the Partner Management dialog. The 'Group' field is set to "Händler/Trader" and the 'Route 1' field is set to "Tour Nord/Route North".*

Calculation of orders (or purchase orders) takes the terms into account in the following sequence:

-   Details from the document
-   Definitions from partner master data
-   Group-specific terms

If no agreements/terms are found, the generally applicable prices, surcharges, and rounding are valid.

---

## Different Customer/Supplier Groups

If a customer shall get other terms for certain product groups, he can be allocated to another customer group.

> **Example**
> Among others, you have defined the customer groups Produces and Dealers.
> Customer A belongs to customer group Dealers. If an order is entered for this customer with an item that belongs to product group Heat protection IG, the terms of customer group Producer shall apply.

These exceptions are defined in dialog Different customer groups.

**(Image: Fig. B-11 Allocation to a different customer group)**
*A screenshot of the "Different Customer Group" dialog. It shows a rule being defined.*
*   **A - Allocated customer**: The "Customer" field is set to `1060 Wolf Glasbau`.
*   **B - Product group**: The "Product group" field is set to `4** - ESG/Tempered glass`.
*   **C - Customer group**: The "Customer group" to apply is `Händler/Trader`.

A customer can also be allocated to a different customer group if he is not allocated to any (common) customer group. The terms for the other customer group only refer to the defined product group. All other terms defined for this customer will be kept as they are.

Different allocations for supplier groups can be made in the same way.

If partner groups have been specified in close detail you can even define several differences per partner. If you order e.g. fittings from a supplier he can belong to the group Dealers while also belonging to the Producers group as he also provides you with toughened glass lites.

---

## Routes and Delivery Terms

Together with customer data and order dates, routes are the basis for dispatch planning and control. Delivery time and delivery date are used for determining the shipping date, i.e. the date on which the goods have to be handed over to the driver.

The delivery time is described in a separate session.

**(Image: Fig. B-12 Routes)**
*A screenshot of the "Routes" dialog. It shows a table listing various delivery routes like "Abholung / Pick up", "Tour Nord / Route North", "Tour Süd / Route South", etc. Checkboxes indicate which days of the week each route runs. There are also columns for freight costs per kilometer (€/km).*

The week days for every single route are defined in master data. A route from Manchester to Birmingham for example can be done every Monday and Thursday for example. This route shall serve all customers along the road, within a radius of 30 miles.

You can also enter freight costs which can be used to check whether the shipping of a single order is worthwhile. The type of delivery is set as a delivery term, e. g. Truck or Forwarder.

For your local customers you should also define a route called Collection for which no freight costs must be charged.

Every customer is allocated a suitable route and rank. The rank is defined on tab Order.

The rank defines the sequence in which the customers are served on the route.

> **Example**
> Customer A and customer B belong to the southern route. Customer A has rank 1 for this route while B's rank is 2.
> Customer A is therefore served before customer B.

The settings from master data are adopted for the order. This setting can be changed by order. The system automatically checks whether the defined delivery date matches the route days defined for the customer. A message will be displayed in case of differences. Different dates can be saved. They will be adopted for route planning.

### Customs routes
The routes for cross-border deliveries are entered in **Master data > Dispatch > Customs routes**. You can specify border crossings or the name of the route. Customs routes are required for dispatch planning. They cannot be allocated in partner master data.

Routes and route planning are described in detail in section Production.

---

## Route Definition

You can change the defined routes or replace them by new routes. To calculate freight charges for example you have to enter the mileage rate per route.

**How to define a route**
1.  Go to menu **Master Data > Dispatch > Routes**.
2.  Go to the menu **Start > New** to switch to the input mode.

    **(Image: Fig. B-13 Line for new routes is accessible)**
    *A screenshot of the "Routes" dialog with a new blank line ready for input.*
    *   **A - Number (ID) can be chosen at random**: Points to the "No." column for the new route.
    *   **B - Name of the route**: Points to the "Name" column.
    *   **C - Tick the weekdays on which this route is run**: Points to the row of weekday checkboxes (Mon, Tue, Wed, etc.).

3.  Enter the number (A) and name (B).
    Both can be chosen at random.
4.  Tick the checkboxes (C) for the days on which the route is usually run.
    At order entry, these details will be compared with the defined delivery date. The program will issue a message if date and route day do not match.
5.  Move (scroll) the view to the right to specify further details. You can also use the `<Tab>` key to pass from field to field.

    **(Image: Fig. B-14 Define shipping routes - departure time)**
    *A scrolled-right view of the "Routes" dialog.*
    *   **A - Departure time per weekday**: Points to the columns for departure times (e.g., Depart. Wed).
    *   **B - Mileage (freight costs)**: Points to the "€/km" column.

    You do not have to enter all the data. If you do not work in shifts for example or do not have your own shipping department, you can skip the fields in question.
6.  Move the view further to the right to enter e. g. the freight costs per kilometre (B).

    > **Do not charge shipping fees for collection**
    > For the route Collection for which no shipping fee must be charged, you have to tick the checkbox w/o shipping fee.

7.  Select in the menu **Start > Save** to save the data.
    The data will be saved.
8.  If necessary, repeat the steps 2 to 7 for further routes.

---

## Input of Partner Master Data

The dialogs for entering customer-, supplier-, and partner data are quite similar and are therefore described as one. In the following example, dialog Partner management is opened for customers. The steps are the same for Suppliers and Partners.

> **Potential customers or suppliers**
> You can enter data in the 'general partners' section at first. Using the copy function, you can save these data later in 'customers' or 'suppliers'.

You can view the free numbers in dialog Partner management by clicking on the [Zoom] icon next to the input field for the number.

**(Image: Fig. B-15 Display and selection of free numbers)**
*A screenshot of the "Free numbers/areas" dialog box.*
*   **A - Free numbers**: Points to the list of available number ranges (e.g., 1-999, 1001-1009).
*   **B - Number to be adopted**: Points to the input field at the bottom where a user can enter a specific number.

An appropriate dialog for entering product data is also available.
