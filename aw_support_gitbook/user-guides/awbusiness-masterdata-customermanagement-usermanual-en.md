---
title: "EN-UM-AWBusiness_10"
source: "EN-UM-AWBusiness_10.pdf"
tags: ["A+W Business", "Master Data", "Software Reference", "Customer Management", "Supplier Management", "Production", "Order Management", "Financial Data", "ERP", "Invoicing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for A+W Business Master Data, detailing the configuration and management of core business entities. It covers customer and supplier data, project management, shipping logistics, production settings, order processing, and financial data setup."
long_description: "This comprehensive software reference manual provides detailed instructions and descriptions for managing master data within the A+W Business system. It is designed for system administrators and advanced users responsible for configuring and maintaining the foundational data that drives the software's operations. The document is divided into several key sections: Customer, Supplier, Shipping, Production, Order, and Financial Data. Each section explains the various dialogs, fields, and parameters available. Key topics include setting up customer-specific order parameters, managing individual and customized products, defining delivery times and routes, and handling complex project invoicing. The guide also covers production-related settings such as optimization keys, cutting table configurations, and registration points for tracking. Additionally, it details the setup for order management, including number ranges, status management, and document types, as well as the configuration of financial data like taxes, payment conditions, and proceeds accounts. With screenshots, field-level explanations, and cross-references, this manual serves as an essential tool for ensuring the A+W Business system is correctly configured to meet specific business requirements."
---

# Software Reference

---
## Customer

### Customer - order parameters

*Abb. B-510 Customer - order parameters*

This dialog is used to define settings that override the settings from product master data or item entry. The settings only apply to the selected combination of partner and product group or product.

> **Dialog for customer and supplier data**
> The Parameters dialog is the same for customers and suppliers. It will therefore be described just once in this document.

### Identification

Choose an option to define the partners and products to which the settings in section Parameters should apply:

- **Customer group, Supplier group:** The settings apply to the selected group.
- **Customer number, Supplier number:** The settings apply to the selected partner.
- **Product group:** The settings apply to the selected product group. Any of the three product group levels can be selected.
- **Article number:** The settings apply to the selected product.

### Parameters

**Enter customer item/supplier item** You can define that the option Input control > Enter customer item is overwritten at item entry.

> The settings in dialog Document Management for the partner or group of partners will not be changed.
> The cursor automatically moves to the Consignment field when item entry is opened.

### Explicit display of price/surcharge

You can change the price display settings defined in product master data.
- The settings from product master data will not be changed.
- The price is displayed explicitly. This means that all elements of the price are shown separately if the selected combination consists of partner and product group or product.
> ⇨ Tutorial 1, "Price view Implicit in price per QU" on page B-284

### Table

The column headers in this table are based on the settings in section Identification.

The checkboxes are checked according to the settings in section Parameters.

## Customer Individual Products

**Master Data > Partners > Customer > Customer Individual Products**

*Abb. B-511 Customized products*

This dialog is used to enter products that should only be available for a certain customer. This can also be e.g. glass provided by a customer for producing his orders.

> **Customized products at item entry**
> To be able to enter customized product numbers at item entry you have to choose the option Customized article search.
>
> As an alternative for customized products, an item can be saved as a macro. Apart from the sizes, the price and discount will be saved also. The macro can be defined for a single customer or in general.

Whether or not the customized product name should be printed, can be set in management of forms.
> ⇨ "Form Management" on page B-1068

### External product

**Customer** Number of the customer to whom this product belongs.

**Article** Alpha-numerical article number (product number) used for this product by the customer. This number can be used for this product at order entry.

> **Example**
> A customer regularly orders coated toughened glass of a size of x 1800 mm. Enter this product in master data and allocate it to the customer as a customized product. Use bronze as the article number.
>
> At item entry, enter bronze as the product number. The product is displayed together with the sizes entered in product management.

**Name (1-3)** Name and a short description of the product. The name appears at item entry and is analyzed for the printing of forms.
For single lites that are to be assembled in an IG unit, only the first name appears.

**EAN** EAN code (European Article Number) or GTIN code (Global Trade Item Number). In the US, this field can be used for the UPC code (Universal Product Code).

**Additional text** You can allocate text to the product to which the system refers at item entry.

### Own product

**Article** Article number by which the product is listed in A+W Business.

### Overview

The list shows all customers for which customized products have been entered.

## Delivery Time (Customer, Supplier)

**Master Data > Partners > Customer, Supplier > Delivery time**

*Abb. B-512 Delivery time for customers or suppliers*

Use this dialog to define the delivery sequence per route and the time required for delivery.

> **Dialog for customer and supplier data**
> Dialog Delivery time is the same for customers and suppliers. It will therefore be described just once in this document.

The delivery time for customers only refers to the actual delivery. Delivery date calculation is based on the delivery time and the lead time used for producing an order. The lead time is set in company data.
> ⇨ "Company Data > System" on page B-997

### Selection

**Customer, supplier** Customer or supplier for whom the delivery time is defined.

**Route** Route allocated in the customer's master data. You can change this setting if required.

**Priority** Sequence number allocated to the partner in master data. You can change this number if required.

> **Details on the route priority in two dialogs**
> Please note that the route and the route priority can be entered in this dialog and in dialog Partner management > Order tab. You can open the Route priority overview in both dialogs to make sure that the entries are identical.

**Delivery time (days)** The delivery date is automatically calculated at order entry. The delivery time per customer will be taken into account.
If a route can be handled in one day, enter 0 in field Delivery time.
For customers who are farther away, enter the actual number of days required, e.g. including the time for customs clearance and sea crossings for cross-border routes.

**[Route list]** Opens the dialog Route list, listing all partners whose goods are delivered on the same route.

## Projects (Customer, Supplier)

**Master Data > Partners > Customer, Supplier > Projects**

Projects are available only if project management is active in company data, and if projects have been defined.
> ⇨ "Projects" on page B-801

The tabs in the Invoicing dialog depend on the type of project management enabled in the company data. The following descriptions point out the project management types in which the tabs and fields are available.
> ⇨ Tutorial 2, "Project/invoice management" on page B-568

Dialog Invoicing also appears in module Documents. This is where projects are invoiced.
> ⇨ Sales, "Invoicing" on page C-1783

> **Dialog for customer and supplier data**
> Dialog Invoicing is the same for customers and suppliers. It will therefore be described just once in this document.

This section provides information on the following subjects:

- "Project Management / Invoicing Menus" on page B-862
- "Projects - Invoices" on page B-863
- "Invoices - Blanket Order" on page B-867
- "Invoices - Allocated Orders" on page B-867
- "Invoices - Allocated Purchase Orders" on page B-868
- "Invoices - Totals" on page B-869
- "Invoices - Estimated Quantities" on page B-870
- "Invoices - Table" on page B-871

### Project Management / Invoicing Menus

**Master Data > Partners > Customer, Supplier > Projects**

You can use the invoicing menus to make the standard settings for the dialog and open other dialogs without closing the invoicing dialog.

The entries in the menus depend on the active project management mode.

#### Functions Menu

**Master Data > Partners > Customer, Supplier > Projects > Functions menu**
**Documents > Order > Project invoicing > Invoicing > Functions menu**

Use this menu to open other dialogs without closing the current one. The available functions depend on the selected project management mode.

The following entries are displayed:

- **Add hours required:**
  Opens the dialog Hours required in which you can enter e.g. the fees for assembly work (only Invoicing).
  > ⇨ "Purchase Hours" on page B-872
- **Add purchases required:**
  Opens the Purchasing dialog in which you can e. g. enter the cost of fitting material (only Invoicing management).
  > ⇨ "Purchase" on page B-873
- **Claims calculation:**
  Opens the Claims calculation dialog in which you can issue and check invoices.
  > ⇨ "Claims Calculation" on page B-874

#### Print Menu

**Documents > Order > Project invoicing > Invoicing > Print menu**

Use this menu for drawing up lists of invoices. The entries are only available if the Invoicing mode is active.

The following entries are displayed:

- **Status report:**
  Produces a list of all projects to be invoiced, including the current claims and current balance.
- **List:**
  Lists the estimated sums and the accumulated costs for the selected project to be invoiced.

### Projects – Invoices

**Master Data > Partner > Customer, Supplier > Projects > Invoices tab**

The fields available on this tab depend on the project management mode enabled:

- "Standard Project Management" on page B-864
- "Extended Project Management" on page B-864
- "Invoice management with allocated orders" on page B-865

### Standard Project Management

*Abb. B-513 Invoices - Invoices (standard project management)*

This dialog can be used to restrict the project to a certain period and define maximum values for this project.

#### Selection

The fields **Project** and **Customer, Supplier** are the same for all types of project management and invoicing.

**Project** Project defined in **Partners > General > Projects**.
Standard project management also allows entering a new name and thus create a new project.
> ⇨ "Projects" on page B-801

**Customer, supplier** Partner involved in this project. At document entry, only projects will be shown to which the partner stated in this document has been assigned.

**[Documents/Info]** Pressing this button will open a dialog that shows the number of orders entered for the selected project.
> ⇨ "Projects - Documents" on page B-871

#### Validity

**From, to** Start and end date of the period during which documents can be entered for this project. When the end date has been reached, the project can no longer be selected for document management.

#### Maximum values

You can enter maximum values for every customer project. When you close the order entry, a list of the orders entered plus the accumulated totals will be displayed.

**Net turnover** Maximum amount for this project.
This entry only serves for information in standard project management. The button [Documents/Info] can be used to display the orders actually entered for this project.

**Sqm.** Maximum amount of glass to be used.

**Qty.** Maximum number of lites or products to be used.

**Info** Additional information.

### Extended Project Management

*Abb. B-514 Invoices - Invoices (extended project management)*

You can use this dialog to add details for a project, e. g. an alternative shipping address and alternative payment terms.

**Quotation, No. customer order** Here you can enter the numbers of the quotation and of the order sent by the customer.
These fields are identical for all invoicing versions.

**Insert date** Date on which the number has been entered.

#### Definition

**Address** Alternative shipping address, e. g. another access point to a large construction site.

**Invoicing** Invoice date or number.

**Phone** Phone number of a contact for this project, e. g. the site manager.

**Employee** Employee responsible for the partner.

**Status** State of the project:
- **Current:**
  Documents can be entered for this project.
- **Completed:**
  The project has been completed. No additional documents can be entered for this project.
  This status is set automatically when the agreed maximum values have been reached. It can also be set manually ahead of time.

#### Terms

**Valid from, to** Start and end date of the period during which documents can be issued for this project.

**Salesman** Salesman responsible for this partner. The turnover will be used for calculating the sales commission.

**Payment terms** Payment terms, in case these differ from the terms defined in partner management or in the document. This setting will be saved in the document when the project is allocated.

**Net turnover, sqm., quantity** You can enter maximum values for every customer project. When you close the order entry, a list of the orders entered plus the accumulated totals will be displayed.

**Info** Additional information.

### Invoice management with allocated orders

*Abb. B-515 Invoices - Invoices (invoicing of allocated orders)*

This is where you enter an (invoicing) project for a blanket order.

**Invoicing** Invoice number.

**Customer** Number of the customer for whom this order has been entered.

**Blanket order** Number of the blanket order.

**Quotation, No. customer order** Here you can enter the numbers of the quotation and of the order sent by the customer. These fields are identical for all invoicing versions.

**Insert date** Date on which the number has been entered.

**Address** Alternative shipping address for the project to be allocated to the blanket order.

**Invoicing** Invoice date or number.

**Phone** Phone number of a contact for this project, e. g. the site manager.

**Employee** Employee responsible for the partner.

**Status** State of the project:
- **Current:**
  Documents can be entered for this project.
- **Completed:**
  The project has been completed. No additional documents can be entered for this project.
  This status is set automatically when the agreed maximum values have been reached. It can also be set manually ahead of time.

**Memo** Field for additional information.

### Invoices - Blanket Order

**Master Data > Partners > Customer, Supplier > Projects > Blanket order tab**

*Abb. B-516 Invoices - Blanket Order*

This tab is only displayed if the function *Invoicing of allocated orders* is active. The items and quantities of the blanket orders are displayed.
> ⇨Tutorial 2, "Invoicing of blanket orders" on page B-582

Use the context menu (right-click) to open the **History of claims** dialog in order to view a list of existing claims.
> "History of Claims" on page B-875

### Invoices - Allocated Orders

**Master Data > Partners > Customer, Supplier > Projects > Allocated orders tab**

*Abb. B-517 Invoices - allocated orders*

Use this tab to display the allocated orders and credit notes. This tab is only available if *Invoicing of allocated orders* or *Extended project management + Invoicing of allocated orders* is active.

> **Allocated documents**
> Standard project management allows you to view orders and purchase orders by clicking on the button [Documents/Info] on the Invoices tab.

### Invoices - Allocated Purchase Orders

**Master Data > Partners > Customer, supplier > Projects > Allocated purchase orders tab**

*Abb. B-518 Invoices - Allocated Purchase Orders*

Use this tab to view the allocated purchase orders. This tab is only available if *Invoicing of allocated orders* or *Extended project management + Invoicing of allocated orders* is active.

This tab is not shown if *Extended project management* is active.

**Order-related P.O.s** You can change the view by checking this checkbox.
- Manually entered purchase orders for this project are displayed.
- Referenced purchase orders for the project are displayed.

### Invoices - Totals

**Master Data > Partners > Customer, Supplier > Projects > Totals tab**

*Abb. B-519 Invoices - Totals*

This tab shows the totals accumulated for the selected project so far. This tab is only accessible if *Extended project management* is active.

The totals are shown in red if the estimated quantities have been reached or exceeded.
> ⇨ "Invoices - Estimated Quantities" on page B-870

#### Products, Product groups

The lists show the current values for products and/or product groups.

### Invoices – Estimated Quantities

**Master Data > Partners > Customer, Supplier > Projects > Estimated quantities tab**

*Abb. B-520 Invoices - Estimated Quantities*

Use this tab to enter details on the estimated quantity for a project. These details will be used for calculating the totals. This tab is only accessible if *Extended project management* is active.

#### Overview

The list shows all products or product groups for which estimated quantities have been entered.

#### Buttons

The buttons can be used to add or delete entries. When you add an entry, the fields for the estimated quantities are enabled. Please make sure you select the appropriate option (product, PGR) before adding a new line.

#### Selection

Choose an option to define the subject of your quantity estimation:

- **Product:**
  If you enter a product number, the product name appears automatically.
- **PGR:**
  If you enter a product group number, the name of the product group will be displayed automatically. You can select just one PGR. An MPG or SPG cannot be selected.

**Estim. Sqm.** Maximum amount of glass to be used.

**Estim. qty.** Maximum number of lites or products to be used.

**Estim. Turnover** Maximum net amount for this project. When you close the order entry, a list of the orders entered plus the accumulated totals will be displayed. The values will be used for calculation on the Totals tab.

### Invoices - Table

**Master Data > Partners > Customer > Projects > Table tab**

*Abb. B-521 Invoices – table*

This tab shows all projects matching the defined criteria.

## Projects – Documents

**Master Data > Partners > Customer > Projects > Allocated orders, Allocated P.O.s tab > [Documents/Info]**

To the dialog description:
> ⇨ "History of Claims" on page B-875

*Abb. B-522 Projects - Documents*

This dialog lists all documents allocated to the current project.

The dialog also appears if item entry is closed in module Documents. In this case, however, only orders that have been entered for this project for the selected customer will be listed.

## Purchase Hours

**Master Data > Projects > Functions menu > Add required hours**
**Documents > Order > Contract Calculation > Calculation > Functions menu > Add required hours**

*Abb. B-523 Add required hours*

This dialog is used for entering the amount to be invoiced for additional work, e.g. for assembly. The amount is added to the selected project.

This function is only available if the mode *Invoicing of allocated orders* has been enabled.

**Invoice no.** Number of the invoice to which these hours will be added.

**Value** Amount of the additional hours.

## Purchase

**Master Data > Projects > Functions menu > Add required hours**
**Documents > Order > Project invoicing > Invoicing > Functions menu**

*Abb. B-524 Adding a purchase*

Use this dialog to enter the amount spent on additional purchases, e. g. for fitting material. The amount is added to the selected project.

This function is only available if the mode *Invoicing of allocated orders* has been enabled.

**Invoice no.** Number of the invoice to which this purchase amount will be added.

**Value** Amount of this purchase.

## Claims Calculation

**Master Data > Partner > Customer > Projects > Functions menu > Issue partial invoice**

*Abb. B-525 Invoicing with allocated orders – claims invoice*

This dialog shows the amounts that are already covered by claims invoices. You can issue additional invoices for the remaining amounts by entering the required value in the column *Quantity to be calc*.

For the defined value, a document of the type Claim will be issued that can be accessed and edited in document management for orders. The number of the new document can be displayed in the history of claims.
> ⇨ "History of Claims" on page B-875

## History of Claims

**Master Data > Partner > Customer > Projects > Blanket order tab > Context menu for one of the items displayed**

*Abb. B-526 Projects - history of claims*

This dialog shows the amounts that are already covered by claims invoices.

The details displayed depend on the entry in the context menu:

- **History of claims based on documents:**
  All documents for the blanket order are displayed.
- **History of claims based on items:**
  Only the documents for the current item are displayed.

## Rounding (Customer, Supplier)

**Master Data > Partners > Customer, Supplier > Rounding**

*Abb. B-527 Rounding for customers or suppliers*

These dialog can be used to enter alternative roundings for customers or suppliers.

> **Dialog for customer and supplier data**
> Dialog Rounding is identical for customers and suppliers. Here, it is described in connection with customers.

**Customer, supplier** Partner to which the rounding has been allocated.

**Rounding point** The rounding points defined in dialog Rounding points. For every rounding point you can enter an alternative rounding to be used for calculation.
> ⇨ "Rounding Points" on page B-912

**Net price flag** Currently not used.

**Prod.type/class** Product type and product class to which the rounding refers.

**Price unit** Unit used for rounding the prices.

**Rounding table** The roundings defined in dialog Rounding.
> ⇨ "Rounding" on page B-910

### Table

The table lists all roundings allocated to the customer or supplier in question.

### Customers, Suppliers

The table shows all customers or suppliers matching the selection criteria.

## Rounding for Customer/Supplier Groups

**Master Data > Partners > Customer, supplier > Rounding for customer groups, supplier groups**

*Abb. B-528 Rounding for customer or supplier groups*

These dialogs are used for entering different roundings for customer or supplier groups.

The fields are described in detail in connection with dialog Rounding.
> ⇨ "Rounding (Customer, Supplier)" on page B-876

> **Dialogs for customer and supplier data**
> Dialog Rounding is identical for customer and supplier groups. In this document it is described in connection with customer groups.

### Table

This section lists all roundings allocated to the customer or supplier group in question.

## Logo Position

**Master Data > Partners > Customer > Logo position**

*Abb. B-529 Logo Position*

This dialog is used to define the position of the logo on the lites. The defined position is transferred to A+W Production but does not control any machine. The worker can see the position however.

To transfer the logo, check the checkbox Logo input in Company data > Parameters tab.
> ⇨ "Logo entry" on page B-959

> **No automatic positioning on the shop floor**
> The transferred data do not serve to control any machines. The data are transferred to A+W Production. The worker in charge of the logo printing can view these data in A+W Production and can position the logo in the appropriate place.

### Definition

**Customer** Customer for whom the data should be entered.

**Product group** Main product group (MPG) for which the settings should be used. This detail serves to distinguish IG and toughened glass because these are different with regard to logo printing. The details for these two MPGs have to be made separately.

**Shape No.** The number appears automatically when you select one of the shapes in section Shape. Enter zero (0) if the entry should be used for rectangular lites.

**Up to width, Up to height** You can enter the size of lites starting from which no logo should be printed.

**Type** This setting defines whether your company logo should be printed, or the customer's. If there are several logos for the same customer, you have to enter the logo number in field No..

**Logo**

**Article** Every logo must be defined as an article (product) so that it can be entered in an order.

**No.** Logo number if there are several logos.

**Corner** Number of the corner in which the logo should be applied. The corners are counted anti-clockwise, starting from 1 (bottom left corner).

**A/B** These entries define the size of distance A and B from the reference corner (X, Y).

**Side** On single lites, the logo can be applied on the outside or on the inside. For IG and multiple IG, choose the level on which it should be applied.

**On coating side** All logos applied automatically are always applied to the coating side (if present). If a glass includes several coated glass types, the first coated glass is always selected as the destination. With use of this option, the Position field is ignored if a coating is present.

**Without logo** If your logo is usually printed on all lites, you can define that no logo should be printed for this customer.
- The logo will be applied as defined for this customer or in general.
- No logo will be printed for this customer.

**Shape**

You can use the icons to choose the shape for which the settings should be used.

### Selection

The table lists all customers for which logo settings have been made.

## Different Customer/Supplier Groups

**Master Data > Partners > Customer, supplier > Different customer groups, Different supplier groups**

*Abb. B-530 Suppliers, customers - different supplier/customer groups*

These dialogs define the partner group to which a partner should belong if different prices or discounts should be applied for certain product groups.

> **Dialogs for customer and supplier data**
> The dialogs Different customer groups and Different supplier groups are structured identically for customers and suppliers. In this document, they are described in connection with supplier groups.

### Selection

**Customer, supplier** Partner for whom the prices of another group should be valid.

**Product group** Product group for which the prices of another group should be valid.

**Customer group, Supplier group** Different group that is to be used for products of the defined product group.

### Data

This list shows all partners for which different groups have been defined.

## Credit Limit Analysis

**Master Data > Partners > Customer > Credit limit analysis**
**Master Data > Partners > Customer > Customers > Balance tab > [Snapshot]**

*Abb. B-531 Credit limit snapshot*

This dialog allows analyzing the development of certain financial data of your customers for a certain period.

The data for the credit limit analysis are imported by Workflow Task via A+W Commercial Exchange Service. The snapshot can be displayed for all customers in general or just for a single customer.

### Functions menu

- **Delete snapshots:**
  This function is used to delete all snapshots. After that, the data have to be loaded into the database again.

### Selection

**Creation date, from - to** Period for which snapshots should be shown.
This option defines the customers for which a credit limit snapshot should be created:

- **Customer from - to:**
  You can create the snapshot for a single customer or several snapshots for a series of customers. The name of the first and last customer appears automatically.
- **Customer group from - to:**
  You can create the snapshot for a single customer group or several snapshots for a series of customer groups. The name of the first and last customer group appears automatically.

### Snapshots

This list shows all snapshots created by selecting customers or customer groups. The following data are displayed:

- **Customer #:**
  Customer number.
- **Name:**
  Customer name.
- **Date:**
  Date on which the data were imported.
- **Credit limit 1 / Credit limit 2:**
  Credit limit that has been granted.
- **Unsettled accounts:**
  Total amount of unsettled accounts.
- **Liabilities:**
  Current value of liabilities.
- **Orders (not shipped):**
  Total amount of all new orders that were entered but have not been shipped yet (status < print shipping note).
- **Orders (shipped but not invoiced):**
  Total amount of all orders that have been shipped but have not been invoiced (yet) (status < print invoice).
- **Orders (invoiced, not transferred to financial accounting):**
  Total amount of orders that have been shipped and invoiced but no transferred to financial accounting (so far) (status < FinAcc transfer).
- **Orders (total):**
  Volume of all shipped, not shipped, invoiced, and not invoiced orders that have not been transferred to financial accounting yet.
- **Balance 1/ balance 2:**
  Balances.
- **Customer locked:**
  Lock code from customer master data.
- **Salesman:**
  Name of the salesman in charge as defined in customer master data.
- **Last 12 months' turnover:**
  Total amount of orders within the past 12 months.
- **Payment terms:**
  Payment terms acc. to customer master data.

## Marginal Income Limits

**Master Data > Partners > Customer > Marginal income limits**

*Abb. B-532 Marginal income limits*

This dialog is used to allocate the limits for analyzing the marginal income. These limits must be defined for every customer/customer group and PGR.

For all customer/product group combinations that have not been explicitly defined, the standard entries will be loaded from company data.
> ⇨ "Default MI" on page B-1004

### Selection

Choose an option to specify for who these limits should be valid:

- **Customer:**
  Marginal income limits for customers.
- **Customer, customer group:**
  Marginal income limits for customer group.

The appropriate fields for selecting the customer or the customer group are accessible.

**Product group** Product group for which the marginal income limits should be used.

**Minimum marginal income** Bottom limit for the marginal income.

**Maximum marginal income** Upper limit for the marginal income.

### Marginal incomes

The list shows all marginal incomes that differ from the standard value defined in company data.

## Exceeds Amount

**Master Data > Partner > Customer > Exceeds amount**

*Abb. B-533 Exceeds Amount*

This dialog is used to enter the percentage for commercial surplus the customer will usually accept for certain products.
In product master data you can also enter a percentage for a surplus/shortfall to be taken into account for serial orders.
When the production software reports surplus or a shortfall, the actually produced quantity will be adopted for the order item. The order will then be recalculated.
> ⇨ "Default values for different quantities" on page B-674

> **Requirements**
> You should use surplus only if the following requirements are met:
> - Transfer to production in OrderXML format
> - File-less production reports

### Selection

**Customer** Customer who accepts surplus or shortfall.

**Product** Product for which the definition should be used. If a customer accepts surplus or shortfall for several products, you can enter different percentages for every product.

### Differing quantities

The values will be used for calculating the order quantity. The surplus or shortfall (expressed in units) appears at item entry on tab **Further details**.

**Surplus, Shortfall** Percentage for the surplus and shortfall.

### Data

The list shows all customers who will accept surplus or shortfall for certain products.

## Calendar (Customer)

**Master Data > Partners > Customer > Calendar**

*Abb. B-534 Customer calendar*

This dialog is used for entering (per customer) the days to be omitted when calculating the payment terms, e.g. company holidays. The due date will be postponed if it lies within the define period.
The type of postponement must also be set in customer master data.
> ⇨ Tutorial 1, "Editing Customer's Calendars" on page B-165
> ⇨ "Partner Management - Finances" on page B-822

### Functions menu

The entries in this menu define the postponement for all the days marked in the overview (calendar). You can check several checkboxes.

- **Skip payment:**
  Checks the checkbox of the selected days in skip payment column.
- **Do not skip payment:**
  Removes the check from the checkboxes of the selected days.
- **Skip delivery:**
  Checks the checkbox of the selected days in skip delivery column.
- **Do not skip delivery:**
  Removes the check from the checkboxes of the selected days.
- **Transfer dates:**
  Opens the dialog Transfer calendar data in order to copy the dates to another customer calendar.
  > ⇨ "Transfer Calendar Dates" on page B-885

### Identification

**Number** Number of the customer for whom holidays should be entered.

**Year** Year in which the postponement is entered.

**Name, Street, ZIP/Town** Customer details are automatically adopted from customer master data.

### Overview

The list shows the selected calendar. The days on which no payments must be due can be selected in columns **Skip payment** and **Skip delivery**.

You can check individual checkboxes or select several lines using the menu **Functions > Skip payment**.

When saving an order, the system checks whether the delivery to the customer on the selected date is desired or not. If delivery is not desired on the selected date, a message is output and the delivery date must be changed. The delivery date is also checked when copying orders.

> **Transfer dates**
> When you have entered the dates for postponing a due date and a delivery date you can transfer them to another customer. This function is available in menu Functions. Only the selected data will be transferred, not the entire calendar.

### Table

The table lists all customers for whom details for postponing due dates and/or the delivery date have been entered. You cannot enter a customer without checking at least one date (checkbox).

## Transfer Calendar Dates

**Master Data > Partner > Customer > Calendar > Functions menu > Transfer data**

*Abb. B-535 Customer calendar - Transfer calendar dates*

This dialog is used for transferring the calendar settings from one customer to one or more other customers so that these will not get any invoices during the defined periods.
> ⇨ Tutorial 1, "Editing Customer's Calendars" on page B-165

## Supplier

**Master Data > Partners > Supplier**

This program section serves to enter data that can be allocated to your suppliers. The actual supplier data are entered in dialog **Partner management**.

The following dialogs are the same for customers and suppliers and are therefore described just once:

- "Partner Management" on page B-808
- "Discount Management (Customers, Suppliers)" on page B-847
- "Parameters (Customers, Suppliers)" on page B-856
- "Delivery Time (Customer, Supplier)" on page B-860
- "Projects (Customer, Supplier)" on page B-861
- "Rounding (Customer, Supplier)" on page B-876
- "Rounding for Customer/Supplier Groups" on page B-876
- "Different Customer/Supplier Groups" on page B-878

Menu Supplier offers the following, additional entries:

- "Supplier List" on page B-888
- "Declaration" on page B-892

### Supplier

**Master Data > Partners > Supplier > Suppliers**

*Abb. B-536 Partner management - Suppliers*

This dialog is used for entering master data for your suppliers.

This dialog is the same for all partners. It is described in detail in connection with customers.
> ⇨ "Partner Management" on page B-805

## Supplier List

**Master Data > Partners > Supplier > Supplier List**

The dialog is used to define the suppliers of the individual products or product groups as well as the corresponding delivery times. If entries are made for a product as well as for the corresponding product group, the settings for the product will be used with priority at P.O. transfer.

The supplier file is checked when orders that include purchased articles are directly transferred to purchasing. Since this is done without using the purchase pool, a standard supplier must be defined.

Price comparison in the purchase pool is also based on the data in the supplier file.
> ⇨ Sales, "P.O. transfer" on page C-1751

This dialog offers the following tabs:

- Supplier List – Products
- Supplier List - Product Groups
- Supplier List - Conditions

### Supplier List – Products

**Master Data > Partner > Supplier > Supplier List > Products tab**

*Abb. B-537 Supplier list – Products*

This tab is used to define the suppliers who can provide a certain product.

### Products

Normally, there is just one standard supplier per product for standard orders. However, if customers order large quantities of a certain product, one that the standard supplier is unable to produce, a standard supplier for serial orders can be defined as well.

**Standard orders, Serial orders** Choose an option to define the type of orders for which these settings should be used:
- **Standard orders:**
  Standard orders are orders of the type <n.e.>, work order, internal order.
- **Serial orders:**
  Serial orders are orders of the type Serial order.

**Client, Order area** Choose a client and/or an order area to define the number area from which order numbers for internal orders should be taken.

**Supplier, Product** Choose an option to define whether the settings should apply to a supplier or a product:
- **Supplier:**
  The settings refer to a certain supplier. The fields for selecting the supplier are accessible.
- **Product:**
  The settings refer to a certain product.

**Color** Color variant of the product in question.

**Max. width, Max. height** Size up to which the supplier can provide the product in question.

**Description 1-3** Product names used by the supplier. These will be printed on the P.O. forms instead of the names defined in product master data.

**Del. time/days** Number of days it usually takes the supplier to deliver the product in question. In the price comparison of the purchase order batch, the delivery time is used as another selection criterion..

**Priority of supplier** The supplier with ranking 1 is considered to be the standard supplier.
This definition is important if there are several suppliers for a product. Direct purchase orders are always placed with the standard supplier. If no standard supplier has been defined, the purchased element or the purchase order will be transferred to the purchase pool so that you can choose a supplier.

### Internal orders/Profit center invoicing

Choose an option to define the order type:

- **None:**
  The settings apply to customer orders.
- **Internal orders:**
  Internal orders serve for filling up one's own stock. An internal customer must be defined instead of the standard supplier. In lieu of purchase orders, orders will be created automatically.
- **Profit center:**
  Choose this option for profit center invoicing. Please contact A+W Software GmbH if you want to use this option.

### Create internal orders with / in

The fields in this section are locked if the option **None** has been selected.

**Customer** Number of the internal customer. This field is locked if you have chosen the option **Profit center**.

**Client** Client to whom the internal order should be sent as a P.O.

**Order area** Order area to be used for the invoicing of the internal order.

### Product - Supplier

This list shows all suppliers of the product in question. You can use the arrow keys to change their ranking.

### Products

This is a list of products for which several suppliers have been entered.

## Supplier List – Product Groups

**Master Data > Partner > Supplier > Supplier List > Product Groups tab**

*Abb. B-538 Supplier file - product groups*

This tab is used to define the suppliers for whole product groups.

The fields are explained in connection with Products tab.
> ⇨ "Supplier List – Products" on page B-888

**Supplier, Prod. grp.** Choose an option to define whether the settings should apply to a supplier or a product group:
- **Supplier:**
  The settings refer to a certain supplier.
- **Prod. grp.:**
  The settings refer to a certain product group.

### Product Group - Suppliers

This list shows all suppliers for the product group in question.

### Product groups

This is a list of product groups for which several suppliers have been entered.

## Supplier List - Conditions

**Master Data > Partners > Supplier > Supplier List > Conditions**

*Abb. B-539 Supplier list - Conditions*

On this tab, you specify the condition with which a supplier is assigned. The defined conditions are checked again when determining the supplier during order transfer.
If an appropriate supplier was found, it is determined whether there are other conditions for the supplier assignment that must be fulfilled. If a condition is not relevant, the supplier is not assigned automatically.

**Max. width, Max. height** Specification of the dimensions that the supplier can deliver.

**Product type** Specification whether the selected product type should be checked.
- **=:** The product ordered is part of the specified product type.
- **!=:** The product ordered should not be part of the specified product type.

**Product group** Specification whether the selected product group should be checked. The field is only activated if a product type should be checked.
- **=:** The product ordered is part of the specified product group.
- **!=:** The product ordered should not be part of the specified product group.

**Product group** Specification whether the selected product group should be checked.
- **=:** The product ordered is part of the specified product group.
- **!=:** The product ordered should not be part of the specified product group.

**Formula** Selection of a formula with which the suppliers are checked. The formula is stored on the Formulas dialog.
> ⇨ "Formulas" on page B-1051

## Declaration

**Master Data > Partners > Supplier > Supplier's declaration**

*Abb. B-540 Supplier's declaration for export customs*

This dialog is used for printing the supplier's declaration form required for exporting products.

*Abb. B-541 Example of supplier declaration's (page 2)*

## Shipping

**Master Data > Shipping**

This program section serves to enter the data required to allocate shipments to your customers.

Menu Dispatch offers the following entries:

- "Delivery Conditions" on page B-893
- "Routes" on page B-894
- "Truck" on page B-896
- "Driver" on page B-896
- "Customs Routes" on page B-897
- "Customs ID" on page B-898

### Delivery Conditions

**Master Data > Shipping > Delivery Conditions**

*Abb. B-542 Delivery Conditions*

This dialog is used for defining the ways in which orders can be shipped. Every customer can be allocated one of the defined terms of delivery in customer data.
> ⇨ "Partner Management - Address" on page B-809

The terms of delivery can be changed in the order.

**Name** Name of the delivery terms.

**External key** The external key can be used for communicating with other programs, e.g. for transfer to production or for statistical analysis.

**Locked** A delivery term can be locked so that it cannot be allocated to a customer or in an order.
- The delivery term can be allocated.
- The delivery term is locked and cannot be allocated. If it has been allocated, it will still be displayed.

## Routes

**Master Data > Shipping > Routes**

*Abb. B-543 Routes*

You can use this dialog to enter the actual routes. You can also enter the weekdays, shifts, and departure times. Based on the mileage, the freight costs can be calculated.

Module Production allows planning the routes and vehicle loads.
> ⇨ Production, "Logistics" on page E-2269

### Overview

**No.** Route number.

**Name** Name of the route, e.g. North.

**Mon-Sun** Valid days for the route in question.
- These days will not be used for that route.
- These days will not be used for that route. These days are marked at order entry. You can still enter another delivery date.

**External key** External key for communicating with other programs, e.g. for transfer to production.

**No shipping fee** A surcharge for shipping can be automatically added to the order. This requires input of the corresponding surcharge article in product management. The surcharge for this product number must also be entered in dialog **Product allocation surcharges**.
- No shipping fee will be applied. This setting can be used e.g. for orders to be collected.
- The shipping fee will be applied. Calculation of the fee has to be enabled for this customer in partner management.
> ⇨ "Partner Management - Order" on page B-813
> ⇨ "Surcharge Product Assignment" on page B-1049

**Delivery time** Store a delivery time here that is used by default for the calculation of the dispatch date, if no delivery date is stored in the customer or supplier.

**Calendar week** Select in which calendar week the route should be driven:
- 0 - none
- 1-even: The route will be driven in the even calendar week.
- 2-odd: The route will be driven in the odd calendar week.

**Serial sample (monthly)** With monthly serial samples, you determine whether a route should be driven on the first, second, third, fourth, or last day of the week of a month. This setting applies for the set weekly rhythm (Mo, Tu, We, Th, Fr, Sa, and/or Su) of the route. The settings on the route dialog affect the calendar - Tool off with which you select the route day.

**Shift Mon-Sun** If your capacity planning is run on shifts and a route leaves e.g. in the third shift, enter 3 for the corresponding route day.
- **No entry:** First shift. This means that the order has to be finished the day before.
- **2:** Second shift. The route starts with the second shift. The order can be completed during the first shift.
- **3:** Third shift. The route starts with the third shift. Production of the order can be completed during the second shift.

**Depart. Mon-Sun** If you are using capacity planning you can also define the time at which the route is started on the individual weekdays.

**€/m** Mileage. Together with distance defined in customer data, this is used for calculating the freight costs.
> ⇨ "Partner Management - Production" on page B-831

**Locked** A route can be locked so that it cannot be allocated to a customer, in an order, or in route planning.
- The route can be allocated.
- The route is locked and cannot be allocated. If it has been allocated, it will still be displayed.

## Truck

**Master Data > Shipping > Trucks**

*Abb. B-544 Transport vehicles*

You can use this dialog for entering the data of your vehicles. You can allocate a lorry in the order and in route planning.

### Selection

**Name** Number plate of the vehicle.

**Driver** Name of the usual driver of this vehicle.

**Tare** Tare (in kg) of the vehicle.

**Total weight** Gross vehicle weight. If this weight is exceeded at picking, the actual weight will be shown in red.

**Locked** A vehicle can be locked for input in route planning if it is no longer required.
- The vehicle can be allocated.
- The vehicle is locked and cannot be allocated. If it has been allocated before, it will still be displayed.

### Table

The list shows all vehicles.

## Driver

**Master Data > Shipping > Driver**

*Abb. B-545 Driver*

Enter the names of all drivers. Drivers can be allocated to a lorry, in the order, and at picking.

**Name** Driver's name.

**External key** The external key can be used for communicating with other programs, e.g. for transfer to production or for statistical analysis.

**Locked** A driver can be locked for input in route planning if he should not drive any more.
- The driver can be allocated.
- The driver is locked and cannot be assigned. If he has been assigned before in route planning, he will still be shown however.

## Customs Routes

**Master Data > Shipping > Customs Routes**

*Abb. B-546 Customs Routes*

This dialog serves to define the routes for cross-border business. You can specify border crossings or the name of the route. These entries can be selected in module Production.

**Name** Name of the customs route or border crossing point.

**External key** The external key can be used for communicating with other programs, e.g. for transfer to production or for statistical analysis.

**Locked** A customs route can be locked for input in dispatch if it is no longer required.
- The customs route can be assigned.
- The customs route is locked and cannot be allocated. If it has been allocated, it will still be displayed.

## Customs ID

**Master Data > Shipping > Customs ID**

*Abb. B-547 Customs ID*

This dialog is used to enter the customs IDs for Intrastat reports. The customs numbers appear on the customs management lists in module Production.
Every product to be exported into a third country has to be classified by product number (so-called customs tariffs) according to the German customs tariff.

> **Example**
> 70080081 = IG glazing
> 70099200 = framed mirrors

### Identification

Choose an option to define what these settings should be used for:

- **Product:**
  The settings apply to a single product.
- **Product group:**
  The settings apply to a product group. You can select all three product group levels.

**Currency** Currency in which the prices are defined.

**Customs ID export, Customs ID import** Customs tariff ID for export or import.

**Text** Short, descriptive text.

**Third country product** You can define whether you have imported the product as a BOM elements for instance.
- The product has not been imported.
- The product was imported from a third country (non EU).

### Table

This list shows all product or product groups for which customs IDs have been defined.

## Production

**Master Data > Production**

This program section is used to enter the data required for communicating with the production software.

Menu Production offers the following entries:

- "Optimization” on page B-899
- "Registration Points - Production" on page B-900
- "Glass Type - Jumbos - Tables" on page B-903
- "Cutting Tables" on page B-904
- "Processes" on page B-908
- "Breakage Reasons" on page B-909

The settings for data transfer are made in company data and in the interface service.
> ⇨ "Company Data" on page B-942
> ⇨ "Interface service" on page B-1051

### Optimization

**Master Data > Production > Optimization**

*Abb. B-548 Optimization*

You can use this dialog to enter the product numbers used by AWPool. These product numbers can be allocated to the A+W Business products in dialog **Product Management > Production tab**.
> ⇨ "Optimization key" on page B-675

This allocation is necessary because AWPool uses different racks for processing for example. Based on the AWPool number assigned in A+W Business, AWPool can organize the processed lites on the shop floor acc. to individual rules.

**Code** Code or product number.

**Name** Optimization name or number.

## Registration Points - Production

**Master Data > Production > Registration point production**

*Abb. B-549 Registration point for production reports*

This dialog is used for entering the registration points for analyzing reports from A+W Production in A+W Business. These registration points are necessary for production reports and barcode reports.
In A+W Production, data are collected from all vital registration points (RP) on the shop floor, and are passed on as report files.
Production reports can be transferred file-less. The appropriate settings are made in company data.
> ⇨ "Company Data – Production" on page B-1009

| Registration point: A+W Production examples | Meaning |
| :--- | :--- |
| 0 | unscheduled |
| 100 | scheduled in batch |
| 150 | detailed scheduling |
| 200 | released for production |
| 300 | in production |
| 350 | breakage on the shop floor |
| 700 | produced |
| 800 | ready for shipment |
| 900 | delivered |

These production reports serve for monitoring the production progress in A+W Business. This permits to check the actual status of an order.

The registration point from which on an order is considered to be produced is defined in company data.
> ⇨ "Company Data - Stock/Purchasing/EDI" on page B-981

### Registration point

**Name** Name of the registration point in A+W Business.

**Status point** Status point allocated to the order or to the item based on the report.

**Registration point** Number of the registration point issuing the report.

**Barcode type** Type of report from shop floor data collection (barcoding). Choose the barcode type to define who is expected to issue the report:
- **0 = <n.e.>.**: Reports per Interface Service.
- **1 = receipt of goods:** A+W Capacity Planner (EL) only (entry level).
- **2 = completion report:** A+W Capacity Planner (EL) only (entry level).

**Type** Report type:
- **0-AWBar, STSP:** These setting is made for the old reports AWB_STAT, AWKUSTAT, and STSP.
- **Other:** This setting is used for all other report formats.

**Status increase** Time at which the status should be raised:
- **0 - first lite completed:** The status will be raised when the first lite of the order has been reported complete.
- **1 - first item completed:** The status is raised when the entire first item of the order is reported complete.
- **2 - all lites completed:** The status is raised when all lites of the order have been reported complete.

**P.O. code** By default, no registration point will be set in A+W Production for the receipt of purchased items. This is why purchased items cannot be reported.
- This checkbox is unchecked by default. Purchased products will be ignored for raising the order status. If an order includes purchased items, the order status will be raised even if not all of the ordered items have been received.
- The registration point should report purchased articles. This means that the status in the order header is updated only when the order is ready to be shipped.

### Product Types

This selection lists all product types defined in A+W Business. The settings for the registration point only apply to the checked product types. No reports will be expected for the unchecked product types.

### Selection

This selection lists all registration points from which reports will be expected and processed.

## Glass Type - Jumbos - Tables

**Master Data > Production > Glass type - jumbos - tables**

*Abb. B-550 Glass Type - Jumbos - Tables*

This dialog is used for defining the table on which the stock sizes or jumbos of the individual glass types and thicknesses can be cut. These data are transferred to A+W Production.

This dialog can be accessed only if you have established the connection with the A+W Production server in company data.
> ⇨ "Company Data - Production" on page B-1009

### Key

**Glass type** A+W Production glass type number. Usually matches the A+W Business product number.

**[Directory icon]** Opens the Glass types dialog where a glass type can be entered or selected. This button is accessible only in input mode.
> ⇨ "Glass Types" on page B-706

**Thickness** Glass thickness that can be cut on this table.

**Jumbo number** Number per cutting table.

### Jumbo values

**Width/Height** Width and height of the stockplates that can be cut on this table.

**Priority for opti.** Optimization sequence. The higher the price of a stockplate, the higher priority.

### Subplate flag

Choose an option to define the direction in which subplate should be made:
- **X direction:** The subplate must be vertical to the bottom edge of the plate.
- **Y direction:** The subplate runs parallel to the bottom edge of the lite.
- **Random:** Cutting optimization can choose one of the directions for the subplate.

*Abb. B-551 XYZ cuts on the stock plate*

### Table allocation

The list shows all cutting tables defined in dialog **Cutting tables**.
> ⇨ "Cutting Tables" on page B-904

**Table** Table name.

**Allocated** The selected glass type is allocated to one or more tables.
- The glass type should not be cut on this table.
- The glass type can be cut on this table.

**Autom. loader code** The automatic loader code is imported from table data. You can enter another code if another loader should be used for the glass type in question.

**Quantity** Number of stockplates that can be simultaneously processed by this table.

### Table

This list shows all glass types allocated to the tables.

## Cutting Tables

**Master Data > Production > Cutting tables**

*Abb. B-552 Cutting tables*

This dialog serves to enter the production-relevant data for the cutting tables. The tables are displayed in dialog **Glass type-Jumbos-Tables** and are used for allocating glass types.
> ⇨ "Glass Type - Jumbos - Tables" on page B-903

This dialog can be accessed only if you have established the connection with the A+W Production server in company data.
> ⇨ "Company Data – Production" on page B-1009

### Key

**Table number** Number of the cutting table.

**Name** Name of the cutting table.

### Dimensions

**Width, height** Maximum stockplate size (in mm) that can be cut on this table.

### Values

**Reference point** Reference point for the cutting code. The reference point of the table marks the position of the coordinates 0/0 from where the cutting code starts. It is important in order to cut shapes correctly.
The reference point does not have to match the neutral position of the cutting head. Bystronic for example offers reflected tables with a reference point front left while the cutting head's neutral position is front right. For some tables, this can be set as a parameter.

**Z cut** Position of the Z cuts. The entry bottom or top defines the position on the cutting plan.
It is usually better to position the Z cuts near the top, i.e. away from the working area so that individual subplates can be broken across the whole width of the plate and stacked right away.
If Z cuts are planned in the sections above, there will be enough space on the breakout table to turn the lite for breaking out the Z cut.

**Start of breakout** The start of breakout depends on the spatial conditions on the shop floor. It determines the position of the residue plate as well as - to some extent - the cutting sequence (break bottom or top lite first).

**Special** A+W Production distinguishes the following two options:
- **0 = Normal:** Standard setting
- **1 = Bystronic sorter:** Choose this setting only if you are using a Bystronic sorter at all.

**Racks per cycle** Number of racks available within a cycle. Entries are necessary only if you are using cyclic optimization.

**Hierarchy** Priority for selecting the table on which the specified glass type is cut. The table with the highest priority will be used. This field will be analyzed only if A+W Production is run without machine allocation.

### Distance between cuts

*Abb. B-553 XYZ cuts on the stock plate*

**Min. dist. Y-Y cuts** The minimum distance between Y-Y cuts depends on the use of the automatic breakout line and on the distance of the Y cutting heads. For cutting tables with several Y cutting heads, the minimum distance matches the distance of the cutting wheels of two cutting heads moved together, e.g. Bystronic XYZVA = 300 mm.

**Min. dist. X-X cuts** Minimum distance between X-X cuts in case of automatic breakout.

**Max. Dist. Y-Y cuts** Maximum distance between Y-Y cuts in case of automatic breakout.

**Max. Dist. X-X cuts** Maximum distance between X-X cuts in case of automatic breakout.

### Maximum waste

**X direction** Maximum length of waste permitted for a stockplate. This is the distance in mm from outermost X cut to the edge.

**Y direction** Maximum length of waste permitted for a subplate. This is the distance in mm from outermost Y cut to the edge.

**Z direction** Maximum length of waste permitted on a Y strip. This is the distance in mm from outermost Z cut to the subplate.

### Settings

**Auto breakout** The lites can be broken automatically if the cutting table is equipped with a breakout device.
- Cut lites will not be broken automatically.
- Cut lites should be broken automatically.

**Auto. loader** The lites can be loaded automatically if the cutting table is equipped with an automatic loader.
- The lites will not be loaded automatically, e.g. in case of manual cutting.
- The lites will be loaded automatically. Every stockplate must be allocated a loader code in this case.
> ⇨ "Autom. loader code" on page B-904

**Shapes** Shapes can only be cut on tables that are appropriately equipped, e.g. for manual cutting.
- Shapes are not to be cut on this table.
- Shapes can also be cut on this table.

**Max. subplate can be enlarged** The maximum subplate width can be exceeded for some tables.
- The maximum subplate width must not be extended.
- The maximum subplate width can be extended on this table.

**LAMI** Laminated glass can only be cut on tables that are equipped appropriately.
- Laminated glass cannot be cut on this table.
- The table can be used for laminated glass cutting.

**Edge deletion** Edge deletion is only possible on suitably equipped tables.
- This table cannot handle edge deletion.
- This table can handle edge deletion.

**Manual cutting** Manual cutting is possible on tables that are suitably equipped.
- This table cannot be used for manual cutting.
- This table can also be used for manual cutting.

### Table

This list shows all cutting tables.

## Processes

**Master Data > Production > Processes**

*Abb. B-554 Work processes*

This dialog is used for compiling the processes to be transferred to production. The processing steps are loaded from module A+W Business Capacity Planner.

The dialog functions are released only for specified customers. If you want to use this dialog please contact A+W Software GmbH.

## Breakage Reasons

**Master Data > Production > Processes**

*Abb. B-555 Breakage reasons*

Use this dialog to assign the causes of complaints to the reasons for complaints. With this information, you can create evaluations for the different causes of breakage.
> ⇨ "Complaint Cause" on page B-653
> ⇨ "Complaint Reasons" on page B-654

## Order

**Master Data > Order**

This program section serves to enter the data that are necessary for managing orders and other documents.

Menu Order offers the following entries:

- "Rounding" on page B-910
- "Rounding Points" on page B-912
- "Rounding Allocation" on page B-913
- "Status Management" on page B-913
- "Status Points" on page B-914
- "Status Allocation" on page B-915
- "Business Type" on page B-915
- "Quantity Limits" on page B-916
- "Priority" on page B-916
- "Number Ranges" on page B-918
- "Lock Code" on page B-923
- "Document Type" on page B-925
- "Categories" on page B-926
- "Reasons for change of delivery date" on page B-927

### Rounding

**Master Data > Order > Rounding**

*Abb. B-556 Rounding*

Use this dialog for entering the roundings you require. These roundings will be used for all values that should be rounded, e.g. amounts, surfaces, lengths, etc.

When you enter special roundings for individual partners or whole partner groups, these have to be allocated to the partner or to the group afterwards.
> ⇨Tutorial 2, "Roundings" on page B-515
> ⇨ "Rounding (Customer, Supplier)" on page B-876
> ⇨ "Rounding for Customer/Supplier Groups" on page B-876

**Number** ID of the rounding.

**Name** Name of the rounding.

**Rounding value** Value to which the figure(s) should be rounded.

**Digits** Number of decimals to be rounded to.

> **Example**
>
> **Consider 1 digit:**
> For a value of 0.14, the 4 will be rounded, e. g. to 0.1.
>
> **Consider 2 digits:**
> For a values of 0.147, the 7 will be rounded, e. g. to 0.15.

**Rounding method** Rounding type to be applied:
- **Commercially:** Amounts from 0 to 4 will be rounded downwards and amounts from 5 to 9, upwards.
- **Upwards, downwards:** All amounts will be rounded upwards or downwards as indicated.

Rounding types have to be allocated to the rounding points in dialog Rounding allocation.
> ⇨ "Rounding Allocation" on page B-913

## Rounding Points

**Master Data > Order > Rounding points**

*Abb. B-557 Rounding points*

This dialog is used for defining the rounding points. They describe the units in which the values should be rounded, i.e. amounts, surfaces, and lengths.

Rounding points have to be allocated to the appropriate roundings in dialog Rounding allocation.
> ⇨ Tutorial 2, "Roundings" on page B-515
> ⇨ "Rounding Allocation" on page B-913

## Rounding Allocation

**Master Data > Order > Rounding allocation**

*Abb. B-558 Rounding Allocation*

Use this dialog to allocate the rounding to the corresponding rounding points. These rounding allocations are generally applicable.

If you have defined customer- or supplier-specific roundings you have to allocate them to the partners.
> ⇨ "Rounding (Customer, Supplier)" on page B-876
> ⇨ "Rounding for Customer/Supplier Groups" on page B-876

**Client** Client for whom the rounding allocation should be valid. If you are using several clients, the roundings have to be allocated to each of them.

**Rounding points** Rounding point to which a rounding should be allocated.
> ⇨ Tutorial 2, "Roundings" on page B-515
> ⇨ "Rounding Points" on page B-912

**Prod.type/class** Product type and product group for which the allocation should be valid. The entry `<n.e.>/<n.e.>` means that the rounding allocation should be generally applicable.
This way, you can allocate different rounding types per product type and product class to every rounding point.

**Price unit** Price unit to which the rounding allocation refers, e.g. for different price rounding per meter and millimeter or for the energy surcharge which is calculated with three decimals.

**Net price flag** In customer/supplier management, you can define whether or not net prices should be calculated. The setting can be changed in the order. To make sure that the correct rounding is applied, you have to allocate a rounding in both cases.
- The rounding allocation does not apply to net prices.
- The rounding allocation applies to net prices.

**Rounding table** Rounding to be allocated to the rounding point.
You can define further roundings.
> ⇨Tutorial 2, "Roundings" on page B-515
> ⇨ "Rounding" on page B-910

### Table

The table shows all allocations for the client in question.

## Status Management

**Master Data > Order > Status management**

*Abb. B-559 Status Administration*

This dialog serves to enter the processing points (user status) a document passes on its way through your company. Every user status can be assigned an A+W Business status point to make sure that the status is automatically changed according to your business processes.
> ⇨Tutorial 2, "Status administration" on page B-492
> ⇨ "Status Allocation" on page B-915

> **Change of user status**
> Please contact A+W Software GmbH before changing a user status according to your ideas or before entering a new one. This will help to avoid system errors or incompatibilities.

## Status Points

**Master Data > Order > Status points**

*Abb. B-560 Status Points*

In this dialog you can use the process numbers and names defined in A+W Business. These so-called status points are used for the automatic processing of documents. They signal the end of various, internal processes a document passes from input up to the printing of an invoice, including complaints or credit notes.

The status points are fixed in the system and are used to define conditions for further processing, e.g. for printing invoices. Every status point can be assigned a user status per document.
> ⇨Tutorial 2, "Roundings" on page B-515
> ⇨ "Status Allocation" on page B-915

> **Do not change status points**
> The status points must not be changed.
> New status points can only be added in agreement with A+W Software GmbH.

The different status points are always described in connection with the circumstances in which the processes occur, e.g. printing of forms.

**Identifier** Status point (process) number. The numbering has nothing to do with the sequence of processes.

**Type** The type indicates the document type to which the status point should apply:
- **0: all documents**
- **1: quotation**
- **2: order**
- **3: credit note**
- **4: purchase order request**
- **5: Ρ.Ο.**

**Name** Internal name of the process.

## Status Allocation

**Master Data > Order > Status Allocation**

*Abb. B-561 Status Allocation*

This dialog is used to allocate the internal processes (stats points) to your business processes (user status).

### Status allocation table

This table lists all status points managed by A+W Business.
> ⇨ "Status Points" on page B-914

### Status allocation

**Status point** Status points managed by A+W Business. The status points appear in numerical sequence. The numbering has nothing to do with the sequence of processes.

**Document type** Document type for which the allocation is valid. You can thus restrict the automatic status allocation so that e.g. an order can be transferred to the purchase pool while a quotation can not.

**User status** Allocated user status. All entries defined in status management are presented for selection.
> ⇨ "Status Management" on page B-913

**Min. status** Minimum status the document has to have to reach the selected status point.

**Lock status** Status for which the corresponding document is locked, e.g. a P.O. should be not be changed after receipt of the ordered goods has been booked.

## Business Type

**Master Data > Order > Business type**

*Abb. B-562 Business types*

This dialog is used to define the different business types. These are used for differentiating revenue accounts and for statistics.

Business types can be allocated in the following dialogs:

- **Proceeds accounts:** Allocation for financial accounting (FinAcc).
  > ⇨ "Proceeds Accounts" on page B-934
- **Order areas:** Allocation for internal invoicing.
  > ⇨ "Order Areas" on page B-1040
- **Order header:** Allocation for booking to proceeds accounts.
  > ⇨Sales, "Header data - document" on page C-1543
- **Turnover statistics:** Selection and sorting criterion.
  > ⇨ Statistics, "Turnover sales – restrictions" on page F-2400

**Name** Name, e.g. trade or drop shipment.

**External key** External key for communicating with other programs.

**Locked** A business type can be locked for entry in partner management and in documents if it is no longer needed.
- The business type can be allocated.
- The business type is locked and cannot be allocated. If it has been allocated to products and in documents, it will still be shown however.

## Quantity Limits

**Master Data > Order > Quantity limits**

*Abb. B-563 Quantity Limits*

This dialog shows the defined quantity limits, e.g. square meters, units, linear meters, thickness, airspace.

Quantity limits are used for defining prices and surcharges.
> ⇨Tutorial 1, "Defining a Graduated Price with Limits" on page B-324
> ⇨"Prices" on page B-770
> ⇨ "Miscellaneous Surcharges" on page B-728

> **Dialog locked**
> Only the system administrator can access this dialog.
> Amendments have to be approved by A+W Software GmbH.

**Name** Name of the quantity limit.
**Code** Internal identification number.

**External key** External key for communicating with other programs, e.g. for transfer to production or financial accounting.

**Locked** A quantity limit can be locked for the definition of prices if it is no longer needed.
- The quantity limit can be used.
- The quantity limit is locked and cannot be used any more. If it has been allocated, it will still be displayed.

## Priority

**Master Data > Order > Priority**

*Abb. B-564 Priority*

This dialog serves to enter the priorities for controlling the transfer to production. The priority defined for the order is transferred to capacity planning.

The priorities are predefined by A+W Business. If you add more levels, these have to be defined in A+W Production as well.

Priorities can be allocated in the following dialogs:

- **Order:** The priority loaded from partner management can be changed.
- **Capacity planning:** Determination of production dates and times depending on the priority of the order.

**Name** Name of the priority.

**Production priority** The numbers are predefined by A+W Business and must not be changed.
- **0 - Urgent:** These orders will be produced with top priority.
- **1 - Common:** These orders will be fitted into the usual schedule.
- **4 - Extra:** This priority means that the order should be produced from residue (plates) left over from cutting other orders.
- **9 - On call:** Orders are produced on call.

**External key** External key for communicating with other programs, e.g. for transfer to production.

**Locked** A priority can be locked for allocation if it is no longer needed.
- The priority can be set.
- The priority is locked and cannot be set. If it has been allocated, it will still be displayed.

## Number Ranges

**Master Data > Order > Number Ranges**

Number ranges are logical organization units as well as a means to combine work processes triggered by a so-called number manager.

Dialog Number Ranges offers the following tabs:

- Number Ranges – Documents
- Number Ranges - Production
- Number Ranges - Financial Accounting
- Number Ranges – Table
> ⇨ Tutorial 2, "Number areas" on page B-506

> **Do not reset the number range during operation**
> Resetting or changing the number ranges during operation can cause problems if old document numbers should exist in a new number range. This is why you should carefully check beforehand to make sure that all documents with old numbers have been archived.

### Functions menu

Menu Functions permits to check whether the (newly) defined number ranges clash. If so, the system will issue a message to that effect.

## Number Ranges – Documents

**Master Data > Order > Number Ranges > Documents tab**

*Abb. B-565 Number Ranges – Documents*

You can use this dialog for setting up the number ranges for allocating consecutive numbers. You can allocate 8-digit numbers.

**Client, Order area** For every client, you can define special number ranges by order area. Use tab Table to choose the client and OM area the number areas of which you want to check or change.

> **Example**
> Different number ranges have been set up for the order areas for toughened and IG production. Based on the order number, the workers can see whether the order in question concerns toughened or IG production.

The number ranges of the different clients and order areas must not overlap.

**Employee** For documents, you can define different number ranges by employee.
If you do not want to bother with this, just leave the entry at `<n.e.`. In user management, every user can be allocated to the appropriate order area. The document number will be automatically loaded from the corresponding number range.

### From, Current, To

**From, to** First and last number of the number range. The document number ranges must not overlap.
To lock a document for an order area, enter 0 in both fields and 1 in field current.

**Current** Last number allocated by the system.

**By period** This field is filled by the Number ranges print program.
> ⇨ Sales, "Number ranges" on page C-1815

> **Example**
> Field by period shows the number 181 for orders. The current order number has meanwhile reached 218. If you start the print program, all orders from 182 to 218 on this list will be printed. After printing, the value in field by period will be set to 218.

> **Note**
> When entering new number ranges please make sure that number ranges do not overlap. This also applies to documents, e.g. quotations that can be entered in different order areas.

**Prefix** A separate prefix can be used per document type, e.g. for clients or order areas.

**Quotations** Quotations are independent documents. The system checks this number range at order entry.

**Orders** Orders are independent documents. The system checks this number range at order entry. Partial deliveries as well as complaints belong to the document Order. For the latter, special number ranges are set up on tab Production. These number ranges must not clash.

**Purchase Orders** Purchase orders are independent documents. The system checks this number range at P.O. entry.

**Supplier enquiries** Enquiries are independent documents. The system checks this number range at order entry.

**Invoices** An order gets an invoice number when the invoice is printed. This will be saved in the order. The invoice number is independent of the order number.

**Credit notes** Credit notes are independent documents. The system checks this number range at credit note entry. Generally, the system expects different number ranges for invoices and credit notes. To use the invoice number range for credit notes you have to check the checkbox **Cred.no. = Doc.no.** in company data.
> ⇨ "Company Data > Documents" on page B-952

**Delivery notes** The delivery note number is assigned when the delivery note is printed, and is saved in the order.

**Batch No. A+W Production archives** When an order is archived, an STST file is created which - among others - includes this batch number. This transfer file is imported by A+W Production and triggers the archiving in A+W Production.
The batch number is analyzed only for the order area defined in **Company data > Archives** in field **Order area for batch number**.
This means that you set up this number range only for the client `<n.e.>` and for the order area selected in company data.
> ⇨ "Company Data > Archives" on page B-989

## Number Ranges - Production

**Master Data > Order > Number Ranges > Production tab**

*Abb. B-566 Number Ranges - Production*

This tab is used to define the number ranges to be checked for data interchange with the shop floor.

The columns **from, current, to** and **by period** are described in connection with the tab **Documents**.
> ⇨ "Number Ranges – Documents" on page B-919

**AWPool batch no.** Start and end numbers for the AWPool batch numbers. The system checks this number area at transfer to production.
> ⇨ Production, "Transfer to Production" on page E-2240

**Partial delivery, Complaint, Complaint when breakage** Start and end numbers for partial deliveries and complaints.

> **Partial delivery, Complaint**
> When editing number ranges, please note that partial deliveries and complaints belong to the document Order. These three number ranges must not clash.

**Rack number** Currently not used.

**S+N File Number** This number range is checked in the following cases:
- If shape processing is saved as a SN file at item entry.
  > ⇨ Sales, "Items - stepping" on page C-1611
- When a SN file is automatically created at transfer to production.
  > ⇨ Production, "Transfer to Production" on page E-2240

## Number Ranges - Financial Accounting

**Master Data > Order > Number Ranges > Financial accounting tab**

*Abb. B-567 Number range - financial accounting*

On tab FinAcc, enter the first batch number for transfer to financial accounting (FinAcc).

The columns **from, current, to** and **by period** are described in connection with the tab **Documents**.
> ⇨ "Number Ranges – Documents" on page B-919

## Number Ranges – Table

**Master Data > Order > Number Ranges > Table tab**

*Abb. B-568 Number Ranges – Table*

This tab shows the order areas (per client) for which different number ranges have been defined. To edit the number ranges, select the required entry. The other tabs will show the appropriate number ranges.
> ⇨ "Number Ranges – Documents" on page B-919
> ⇨ "Order Areas" on page B-1040

## Lock Code

**Master Data > Order > Lock Codes**

*Abb. B-569 Lock Code*

This dialog serves to define the lock codes. Lock codes can be used to lock documents for certain actions while automatically raising their status. This means that the document cannot reach the locked status but is instead diverted to another status point (process).

> **Example: Partial delivery without invoicing**
> If partial deliveries must not be invoiced, the system has to be able to recognize a partial delivery as such. In this case, no partial invoice can be created for the partial delivery. The status of the partial delivery will instead be raised automatically. After the order is diverted to Transfer to archives, the partial delivery cannot be edited any further.

Lock codes for complaints and partial deliveries are preset in the company data.
> ⇨ "Company Data > Documents" on page B-952

> **Please discuss changes with A+W Software GmbH**
> Please discuss any changes of lock codes with A+W Software GmbH beforehand to avoid problems.

**Name** (Descriptive) name of the code.

**Locked** A lock code can be locked for further use if it is no longer needed.
- The lock code can be allocated.
- The lock code is locked and cannot be allocated. If it has been assigned in a document, it will still be shown however.

### Status

**Status restriction** Status that will be diverted to another status.

**Deviation to status point** Status point to which the document should be diverted.

**External key** External key for communicating with other programs, e.g. for transfer to production or financial accounting.

### Table

This list shows all lock codes. Select an entry to change the settings in the fields.

## Document Type

**Master Data > Order > Document type**

*Abb. B-570 Document type*

Use this dialog to check which document types are used by A+W Business.

> **Additional document types**
> The document types are preset by A+W Business. Please discuss any changes or extensions with A+W Software GmbH.

**Name** Document type:
- **Down payment:** This document type is automatically used for down payment invoices.
  > ⇨ Sales, "Down payments" on page C-1767
- **In-house production:** Not used at present.
- **Claim:** This document type is used for issuing invoices for a blanket order.
  > ⇨ "Claims Calculation" on page B-874
- **Release:** Not used at present.
- **Internal invoicing:** This document type is automatically used in connection with module Profit Center Invoicing.
- **Internal order:** This document type is used for P.O. transfer in connection with the module Internal orders (multi-stepped production).
  > ⇨ Sales, "P.O. transfer" on page C-1751
- **Customer material:** This document type must be set by hand. As a result, all items will be automatically set to procurement type Customer's own glass.
- **Stock P.O.:** This document type is automatically used for creating a stock P.O. The code can also be set manually for a P.O.
  > ⇨ Sales, "P.O. transfer" on page C-1751
  > ⇨ Stock Management, "Stock P.O." on page G-2640
- **Work order:** This document type is used for filling up your own stock.
  > ⇨ Production, “Production orders" on page E-2199
- **Blanket order:** This document type is used for creating blanket orders.
  > ⇨ "Projects (Customer, Supplier)" on page B-861
- **Complaint:** This document type is used for entering complaints.
- **Serial order:** This document type is used for creating serial orders.
- **Partial delivery:** This document type is automatically set when partial deliveries are entered.
- **Shipping order:** Not used at present.
- **Value booking:** This document type is used for entering credit notes. Quantities like piece, square meter and linear meter are not transferred to statistics as a result.
  > ⇨ Sales, "Credit note (document management)" on page C-1811

**Locked** A document type can be locked for further use if it is no longer needed.
- The document type can be allocated.
- The document type is locked and cannot be assigned any more. If it has been assigned before in a document, it will still be shown however.

> **Locking a document type**
> Locking a document type has a massive effect on order entry. If you want to lock a document type please contact A+W Software GmbH. This helps to avoid unwanted negative effects on your work with A+W Business.

## Categories

**Master Data > Order > Categories**

*Abb. B-571 Categories*

This dialog serves to define categories that are to be used as criteria for the statistical analysis of documents.

**Name** Name of the category.

**External key** External key for communicating with other programs, e.g. for transfer to production or financial accounting.

**Document type** Document type for which the category can be set.

**Default category** You can assign a standard category for the document.
- The category will not be assigned by default for the corresponding document type.
- The category is assigned by default at document entry. It can be changed in the document.

**Locked** A category can be locked for further use if it is no longer needed.
- The category can be allocated.
- The category is locked and cannot be allocated. If it has been allocated before in a document, it will still be shown however.

## Reasons for change of delivery date

**Master Data > Order > Categories**

*Abb. B-572 Reasons for change of delivery date*

On this dialog, you store reasons for changing a delivery date.
Reasons for the change of delivery date can be entered in the Document entry, Document data, the Route list, and in the Picking.
The reason has to be entered if the *Change of delivery date* setting is activated in the master data.
"Change of delivery date" on page B-954

## Financial Data

**Master Data > Financial Data**

This program section serves to define the data required for invoicing order items and transferring the amounts to accounting.

Menu Finances offers the following entries:

- "Tax" on page B-928
- "Payment Conditions" on page B-930
- "Credit Rating" on page B-930
- "Banks" on page B-932
- "Currency" on page B-932
- "Proceeds Accounts" on page B-934
- "Cost Mode" on page B-937
- "Cost Centers" on page B-938
- "Payment Mode" on page B-939
- "Brazilian Tax" on page B-940

### Tax

**Master Data > Financial Data > Tax**

*Abb. B-573 Tax*

This dialog serves to define the (value added) tax rates. In partner management and in product management, the valid tax rates are allocated to the partners (customers) and products.

This allocation can be changed in the actual documents.
> ⇨ "Product Management - Price/Surcharge" on page B-678
> ⇨ "Partner Management - Finances" on page B-822

**Key** Unique number (identification number).

**Tax rate** Percentage to be calculated as tax. Up to four decimals are possible.

**Remark** Description of the tax rate, e.g. 19% domestic.

**Pr.acc.Debt., Pr.acc.Cred.** Numbers of the proceeds accounts for debtors and creditors managed in financial accounting (FinAcc). The tax amounts will not be booked to the proceeds accounts of the product group but tot the accounts specified here.
If this field is left blank, the tax amount will be booked to the proceeds account of the corresponding product group by default.
> ⇨ Software Reference, "Proceeds Accounts" on page B-934

**External key** The external key is transferred to the financial accounting program. The entry depends on the financial accounting program used. Please refer to the user documentation on the financial accounting program you are using.

**Locked** A tax can be locked for further use if it is no longer needed.
- The tax can be allocated.
- The tax is locked and cannot be allocated. If it has been allocated before in a document, it will still be shown however.

### Payment Conditions

**Master Data > Financial Data > Payment Conditions**

*Abb. B-574 Payment conditions*

This dialog serves to enter the common payment terms, e.g. 2% cash discount for payment within 10 days.

Payment terms are allocated to customers in customer management, tab **Finances**. In the order header, the payment terms are loaded from customer data and can be changed if required.
> ⇨ "Partner Management - Finances" on page B-822

**Name** Name of the payment term. You can use up to 40 alpha-numerical characters. This description can be printed on the invoice forms.

**Rate 1, 2, 3** Percentage to be used for calculating the cash discount. The cash discount rate can be constant, or phased.

**Days 1,2,3** Number of days within which the cash discount may be deducted.

**Due date 1-5** Space of time within which an open invoice should be settled. Various fields from customer master data are used for calculating the due date of an order.
> ⇨ "Due date calculation" on page B-823

**Reminder days** Number of days that can be expire after the invoicing date before a reminder is issued. This entry will be transferred to your financial accounting program (FinAcc).

**External key** The external key can be used for communicating with a financial accounting program.

**Locked** A payment term can be locked for use if no longer required.
- The payment term can be allocated.
- The payment term is locked and cannot be allocated. If it has been allocated before in a document, it will still be shown however.

### Credit Rating

**Master Data > Financial Data > Credit Rating**

*Abb. B-575 Credit Rating*

This dialog is used to define the levels for classifying the credit standing of your customers, e.g. excellent, good, poor.
The credit standing is allocated to the customers in customer management, tab **Finances**.
> ⇨ "Partner Management - Finances" on page B-822

**Name** Description of the solvency level.

**External key** The external key can be used for communicating with a financial accounting program.

**Locked** A solvency level can be locked for further use if it is no longer needed.
- The solvency level can be allocated.
- The solvency level is locked and cannot be allocated. If it has been allocated to a partner before, it will still be displayed.

### Banks

**Master Data > Financial Data > Banks**

*Abb. B-576 Banks*

This dialog is used for entering the data of your business partners' bank accounts.

Banks are allocated to the partners in partner management, tab **Finances**. In partner management, you can have the IBAN determined by the system if at least the following data have been entered for the bank: country code, bank code, account number.
> ⇨ "Partner Management - Finances" on page B-822

**Name** Bank name.

**Short name** Short name by which the bank appears in the dialogs.

**Bank code** Bank code.

**BIC** Bank Identifier Code. (SWIFT-) code of the bank, which is used for international payments.

**Country** Code of the country in which the bank is located.

> **IBAN calculation**
> In partner management, you can have the IBAN determined by the system. This is only possible if you have entered the bank code/BIC and the country code of the bank.

**ZIP, Residence, Street** Bank address.

**External key** The external key can be used for communicating with a financial accounting program.

### Currency

**Master Data > Financial Data > Currency**

*Abb. B-577 Currencies*

This dialog is used to enter all currencies you will need at document entry. The currencies are only necessary if you are using the Foreign currency/Euro module.

The currency is allocated to a business partner in partner management. It can be changed in the document.
> ⇨ "Partner Management - Balance" on page B-826

**Input in national currency, foreign currency, Euro** The display field is filled acc. to the entry in company data.
> ⇨ "Company Data > Tax" on page B-944

The description of the following fields refers to the setting **Default: home currency**.

**National currency** Local currency.

**Euro** The Euro conversion rate is loaded from company data.

**Exchange rate/factor** Exchange rate in relation to the national currency.

**Foreign currency** Foreign currency to be converted to.

**Triangulation** This checkbox has to be checked only if the calculation should be changed to Euro.
Currencies are basically calculated in Euro. Amounts in other currencies are first converted into Euro, then into the target currency, e.g. US$. This method is called triangulation.
- Calculation will not be based on triangulation.
- Triangulation will be used only if a third currency comes into play.

**Decimals** Possible number of decimal places in foreign currency.

**Date** Date starting from which the currency or exchange rate is valid.

**External key 1, External key 2** The external keys can be used for communicating with a financial accounting program.

**Locked** A currency can be locked if it is no longer needed.
- The currency can be allocated.
- The currency is locked and cannot be allocated any more. If it has been allocated, it will still be displayed.

### Proceeds Accounts

**Master Data > Financial Data > Proceeds Accounts**

*Abb. B-578 Proceeds Accounts*

This dialog serves to enter your financial accounting proceeds accounts. These proceeds accounts are used for booking in A+W Business.

#### Functions menu

Menu Functions permits to copy proceeds accounts from one business type to another, or change existing entries.
> ⇨ "Copy Proceeds Accounts" on page B-935

#### Identification

Set up a proceeds account for every combination of product group and VAT code so that you can book the transactions with foreign customers. Allocate proceeds accounts to the product groups to make sure that the turnover for the individual products is booked to the correct accounts.

You can also set up proceeds accounts for individual products. For this purpose, the checkbox **Proceeds accounts per product** must be checked.
> ⇨ "Company Data > Financial Accounting" on page B-947

If no account has been created for a product group/VAT combination, a dialog appears in which you can enter the required account number.

> **Use of the copy function**
> You can use the copy function to set up the proceeds accounts required. This will make your job easier.

**Tax 1-5** If you are using several tax rates in your system you have to allocate each tax rate to at least one main product group. The corresponding tax rate is displayed automatically.
> ⇨ "Tax" on page B-928

**Business type** Business type for which the proceeds account is set up.
If no different tax rates have been allocated to business types, adopt the standard setting `<n.e.>`.
> ⇨ "Business Type" on page B-915

#### Proceeds accounts/Cost centers

Debtor = customer, creditor = supplier

**Debtor, creditor** Numbers of the corresponding proceeds accounts.
- **Invoice:** Numbers of the proceeds accounts for the invoices for customer orders or POs.
- **Credit note:** Numbers of the proceeds accounts for credit notes for customer orders or POs.
- **Cost center:** Number of the cost center of the corresponding debtor or creditor in your financial accounting program. The cost centers are defined in dialog **Cost centers**.

If no other proceeds account for the tax has been entered in dialog Tax, the VAT will also be booked to this proceeds account.

#### Supplement

**Remark** Comments on the proceeds account.

**External key** The external key can be used for communicating with a financial accounting program.

#### Overview

This table shows all proceeds accounts for which product groups or products have been defined.

### Copy Proceeds Accounts

**Master Data > Financial Data > Proceeds Accounts > Functions menu > Copy Proceeds Accounts**

*Abb. B-579 Copy proceeds accounts*

This dialog is used to transfer the proceeds accounts for the tax rates and/or business types to other tax rates or business types.

#### from

**Tax 1-5** Tax proceeds accounts to be copied.

**Business type** Business type for which the proceeds accounts have been set up. Business type for which the proceeds accounts have been set up.

#### to

**Tax 1-5** Tax proceeds accounts to which the accounts should be transferred.

**Business type** Business type for which the proceeds accounts have been set up.

**Overwrite existing records** By default, existing records will not be changed.
- Existing records will not be changed. A message appears if a record already exists. Copying will be aborted.
- Existing records will be overridden by the new data without further checks.

### Cost Mode

**Master Data > Financial Data > Cost Mode**

*Abb. B-580 Cost type*

This dialog serves to define the cost types. These cost types can be analyzed in external programs, e.g. Excel.

You can allocate a cost type to each product. It will be adopted for the documents where it can be changed if required.
> ⇨ "Product Management - Price/Surcharge" on page B-678

**Name** Name of the cost type.

**External key** The external key can be used for communicating with a financial accounting program.

**Locked** A cost type can be locked for further use if it is no longer needed.
- The cost type can be allocated.
- The cost type is locked and cannot be allocated any more. If it has been allocated, it will still be displayed.

### Cost Centers

**Master Data > Financial Data > Cost Centers**

*Abb. B-581 Cost Centers*

This dialog serves to define the cost centers. These cost centers can be analyzed by external programs, e.g. Excel.

You can allocate a cost center to each product. It will be adopted for the documents where it can be changed if required.
> ⇨ "Product Management - Price/Surcharge" on page B-678

**Name** Name of the cost center.

**External key** The external key can be used for communicating with a financial accounting program.

**Locked** A cost center can be locked for further use if it is no longer needed.
- The cost center can be allocated.
- The cost center is locked and cannot be allocated. If it has been allocated, it will still be displayed.

### Payment Mode

**Master Data > Financial Data > Payment Mode**

*Abb. B-582 Payment Mode*

This dialog serves to enter the payment modes accepted by your company, e.g. cheque, bank transfer, cash. This is only for information.
Modes of payments can be allocated to partners in partner management.
> ⇨ "Partner Management – Finances" on page B-822

**Name** Name of the payment mode.

**External key, External key 2** The external keys can be used for communicating with a financial accounting program.

**Locked** A payment mode can be locked for further use if it is no longer needed.
- The mode of payment can be allocated.
- The mode of payment is locked and cannot be allocated. If it has been allocated before, it will still be displayed.

### Brazilian Tax

**Master Data > Financial Data > Brazilian tax**

These dialogs can be used to enter the rates for Brazilian taxation. The following dialogs are available:

- TIPI management
- ICMS mode
- CFOP code
- CST code
- Tax allocation
- Business type work flow
- ICMS reduction
- Product types

These dialogs are accessible only Brazilian tax has been activated in company data.
