---
title: "EN_AWBusiness_Master_Data_9_9-2"
source: "EN_AWBusiness_Master_Data_9_9-2.pdf"
tags: ["A+W Business Master Data", "Software Reference", "Customer Management", "Invoice Management", "Project Management", "Rounding", "Logo Position", "Credit Limit Analysis", "User Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical reference guide for the A+W Business Master Data software, specifically detailing the 'Customer' module. It covers functionalities such as project and invoice management, handling of allocated orders and blanket orders, setting up customer-specific rounding rules, logo positioning on products, and financial analysis tools like credit limit and marginal income analysis."
long_description: "This document is a comprehensive software reference for the A+W Business Master Data system, version 9.00. It focuses on the setup and management of customer-related master data. The guide provides detailed definitions and instructions for various modules and tabs associated with customer profiles. Key topics include managing customer projects with specific statuses (current, completed), defining terms like payment conditions and validity periods, and handling different types of invoicing, including those for allocated orders and blanket orders. It explains how to track project totals, estimated quantities, and view associated documents. The manual also covers advanced features such as setting up customer-specific rounding for pricing, defining logo positions on products, managing purchase hours and additional purchases for projects, and calculating claims. Financial management tools are also detailed, including credit limit analysis with snapshots, marginal income limit definitions, and handling of surplus/shortfall quantities. The document serves as a practical guide for users to configure and utilize the full range of customer data management features within the A+W software."
---

---
## Customer

### Definition

**Address**
Alternative shipping address, e.g. another access point to a large construction site.

**Invoicing**
Invoice date or number.

**Phone**
Phone number of a contact for this project, e.g. the site manager.

**Employee**
Employee responsible for the partner.

**Status**
State of the project:
*   **Current:** Documents can be entered for this project.
*   **Completed:** The project has been completed. No additional documents can be entered for this project. This status is set automatically when the agreed maximum values have been reached. It can also be set manually ahead of time.

### Terms

**Valid from, to**
Start and end date of the period during which documents can be issued for this project.

**Salesman**
Salesman responsible for this partner. The turnover will be used for calculating the sales commission.

**Payment terms**
Payment terms, in case these differ from the terms defined in partner management or in the document. This setting will be saved in the document when the project is allocated.

**Net turnover, sqm., quantity**
You can enter maximum values for every customer project. When you close the order entry, a list of the orders entered plus the accumulated totals will be displayed.

**Info**
Additional information.

## Invoice management with allocated orders

*Fig. B-166 Invoices - Invoices (invoicing of allocated orders)*

This is where you enter an (invoicing) project for a blanket order.

**Invoicing**
Invoice number.

**Customer**
Number of the customer for whom this order has been entered.

**Blanket order**
Number of the blanket order.

**Quotation, No. customer order**
Here you can enter the numbers of the quotation and of the order sent by the customer. These fields are identical for all invoicing versions.

**Insert date**
Date on which the number has been entered.

**Address**
Alternative shipping address for the project to be allocated to the blanket order.

**Invoicing**
Invoice date or number.

**Phone**
Phone number of a contact for this project, e. g. the site manager.

**Employee**
Employee responsible for the partner.

**Status**
State of the project:
*   **Current:** Documents can be entered for this project.
*   **Completed:** The project has been completed. No additional documents can be entered for this project. This status is set automatically when the agreed maximum values have been reached. It can also be set manually ahead of time.

**Memo**
Field for additional information.

## Invoices - Blanket Order

**Master Data > Partners > Customer, Supplier > Projects > Blanket order tab**

*Fig. B-167 Invoices - Blanket Order*

This tab is only displayed if the function *Invoicing of allocated orders* is active. The items and quantities of the blanket orders are displayed.

⇨ Tutorial 2, "Invoicing of Blanket Orders" on page B-508

Use the context menu (right-click) to open the *History of claims* dialog in order to view a list of existing claims.

⇨ "History of Claims" on page B-838

## Invoices – Allocated Orders

**Master Data > Partners > Customer, Supplier > Projects > Allocated orders tab**

*Fig. B-168 Invoices - allocated orders*

Use this tab to display the allocated orders and credit notes. This tab is only available if *Invoicing of allocated orders* or *Extended project management + Invoicing of allocated orders* is active.

> **Allocated documents**
> Standard project management allows you to view orders and purchase orders by clicking on the button [Documents/Info] on the Invoices tab.

## Invoices – Allocated Purchase Orders

**Master Data > Partners > Customer, supplier > Projects > Allocated purchase orders tab**

*Fig. B-169 Invoices - Allocated Purchase Orders*

Use this tab to view the allocated purchase orders. This tab is only available if *Invoicing of allocated orders* or *Extended project management + Invoicing of allocated orders* is active.

This tab is not shown if *Extended project management* is active.

**Order-related P.O.s**
You can change the view by checking this checkbox.
*   Manually entered purchase orders for this project are displayed.
*   Referenced purchase orders for the project are displayed.

## Invoices – Totals

**Master Data > Partners > Customer, Supplier > Projects > Totals tab**

*Fig. B-170 Invoices - Totals*

This tab shows the totals accumulated for the selected project so far. This tab is only accessible if *Extended project management* is active.

The totals are shown in red if the estimated quantities have been reached or exceeded.

⇨ "Invoices - Estimated Quantities" on page B-832

### Products, Product groups

The lists show the current values for products and/or product groups.

## Invoices – Estimated Quantities

**Master Data > Partners > Customer, Supplier > Projects > Estimated quantities tab**

*Fig. B-171 Invoices - Estimated Quantities*

Use this tab to enter details on the estimated quantity for a project. These details will be used for calculating the totals. This tab is only accessible if *Extended project management* is active.

### Overview

The list shows all products or product groups for which estimated quantities have been entered.

### Buttons

The buttons can be used to add or delete entries. When you add an entry, the fields for the estimated quantities are enabled. Please make sure you select the appropriate option (product, PGR) before adding a new line.

### Selection

Choose an option to define the subject of your quantity estimation:
*   **Product:** If you enter a product number, the product name appears automatically.
*   **PGR:** If you enter a product group number, the name of the product group will be displayed automatically. You can select just one PGR. An MPG or SPG cannot be selected.

**Estim. Sqm.**
Maximum amount of glass to be used.

**Estim. qty.**
Maximum number of lites or products to be used.

**Estim. Turnover**
Maximum net amount for this project. When you close the order entry, a list of the orders entered plus the accumulated totals will be displayed. The values will be used for calculation on the Totals tab.

## Invoices - Table

**Master Data > Partners > Customer > Projects > Table tab**

*Fig. B-172 Invoices - table*

This tab shows all projects matching the defined criteria.

## Projects – Documents

**Master Data > Partners > Customer > Projects > Allocated orders, Allocated P.O.s tab > [Documents/Info]**

*Fig. B-173 Projects - Documents*

This dialog lists all documents allocated to the current project.
The dialog also appears if item entry is closed in module Documents. In this case, however, only orders that have been entered for this project for the selected customer will be listed.

## Purchase Hours

**Master Data > Projects > Functions menu > Add required hours**
**Documents > Order > Contract Calculation > Calculation > Functions menu > Add required hours**

*Fig. B-174 Add required hours*

This dialog is used for entering the amount to be invoiced for additional work, e.g. for assembly. The amount is added to the selected project.
This function is only available if the mode *Invoicing of allocated orders* has been enabled.

**Invoice no.**
Number of the invoice to which these hours will be added.

**Value**
Amount of the additional hours.

## Purchase

**Master Data > Projects > Functions menu > Add required hours**
**Documents > Order > Project invoicing > Invoicing > Functions menu**

*Fig. B-175 Adding a purchase*

Use this dialog to enter the amount spent on additional purchases, e. g. for fitting material. The amount is added to the selected project.
This function is only available if the mode *Invoicing of allocated orders* has been enabled.

**Invoice no.**
Number of the invoice to which this purchase amount will be added.

**Value**
Amount of this purchase.

## Claims Calculation

**Master Data > Partner > Customer > Projects > Functions menu > Issue partial invoice**

*Fig. B-176 Invoicing with allocated orders – claims invoice*

This dialog shows the amounts that are already covered by claims invoices. You can issue additional invoices for the remaining amounts by entering the required value in the column *Qantity to be calc*.

For the defined value, a document of the type *Claim* will be issued that can be accessed and edited in document management for orders. The number of the new document can be displayed in the history of claims.

⇨ "History of Claims" on page B-838

## History of Claims

**Master Data > Partner > Customer > Projects > Blanket order tab > Context menu for one of the items displayed**

*Fig. B-177 Projects - history of claims*

This dialog shows the amounts that are already covered by claims invoices.
The details displayed depend on the entry in the context menu:

*   **History of claims based on documents:** All documents for the blanket order are displayed.
*   **History of claims based on items:** Only the documents for the current item are displayed.

## Rounding (Customer, Supplier)

**Master Data > Partners > Customer, Supplier > Rounding**

*Fig. B-178 Rounding for customers or suppliers*

These dialog can be used to enter alternative roundings for customers or suppliers.

> **Dialog for customer and supplier data**
> Dialog Rounding is identical for customers and suppliers. Here, it is described in connection with customers.

**Customer, supplier**
Partner to which the rounding has been allocated.

**Rounding point**
The rounding points defined in dialog *Rounding points*. For every rounding point you can enter an alternative rounding to be used for calculation.
⇨ "Rounding Points" on page B-882

**Net price flag**
Currently not used.

**Prod.type/class**
Product type and product class to which the rounding refers.

**Price unit**
Unit used for rounding the prices.

**Rounding table**
The roundings defined in dialog *Rounding*.
⇨ "Rounding" on page B-880

### Table

The table lists all roundings allocated to the customer or supplier in question.

### Customers, Suppliers

The table shows all customers or suppliers matching the selection criteria.

## Rounding for Customer/Supplier Groups

**Master Data > Partners > Customer, supplier > Rounding for customer groups, supplier groups**

*Fig. B-179 Rounding for customer or supplier groups*

These dialogs are used for entering different roundings for customer or supplier groups.
The fields are described in detail in connection with dialog *Rounding*.
⇨ "Rounding (Customer, Supplier)" on page B-839

> **Dialogs for customer and supplier data**
> Dialog Rounding is identical for customer and supplier groups. In this document it is described in connection with customer groups.

### Table

This section lists all roundings allocated to the customer or supplier group in question.

## Logo Position

**Master Data > Partners > Customer > Logo position**

*Fig. B-180 Logo Position*

This dialog is used to define the position of the logo on the lites. The defined position is transferred to A+W Production but does not control any machine. The worker can see the position however.

To transfer the logo, check the checkbox *Logo input* in Company data > Parameters tab.
⇨ "Logo entry" on page B-935

> **No automatic positioning on the shop floor**
> The transferred data do not serve to control any machines. The data are transferred to A+W Production. The worker in charge of the logo printing can view these data in A+W Production and can position the logo in the appropriate place.

### Definition

**Customer**
Customer for whom the data should be entered.

**Product group**
Main product group (MPG) for which the settings should be used. This detail serves to distinguish IG and toughened glass because these are different with regard to logo printing. The details for these two MPGs have to be made separately.

**Shape No.**
The number appears automatically when you select one of the shapes in section Shape. Enter zero (0) if the entry should be used for rectangular lites.

**Up to width, Up to height**
You can enter the size of lites starting from which no logo should be printed.

**Type**
This setting defines whether your company logo should be printed, or the customer's. If there are several logos for the same customer, you have to enter the logo number in field No..

### Logo

**Article**
Every logo must be defined as an article (product) so that it can be entered in an order.

**No.**
Logo number if there are several logos.

**Corner**
Number of the corner in which the logo should be applied. The corners are counted anti-clockwise, starting from 1 (bottom left corner).

**A/B**
These entries define the size of distance A and B from the reference corner (X, Y).

**Side**
On single lites, the logo can be applied on the outside or on the inside. For IG and multiple IG, choose the level on which it should be applied.

**Without logo**
If your logo is usually printed on all lites, you can define that no logo should be printed for this customer.
*   The logo will be applied as defined for this customer or in general.
*   No logo will be printed for this customer.

### Shape

You can use the icons to choose the shape for which the settings should be used.

### Selection

The table lists all customers for which logo settings have been made.

## Different Customer/Supplier Groups

**Master Data > Partners > Customer, supplier > Different customer groups, Different supplier groups**

*Fig. B-181 Suppliers, customers - different supplier/customer groups*

These dialogs define the partner group to which a partner should belong if different prices or discounts should be applied for certain product groups.

> **Dialogs for customer and supplier data**
> The dialogs *Different customer groups* and *Different supplier groups* are structured identically for customers and suppliers. In this document, they are described in connection with supplier groups.

### Selection

**Customer, supplier**
Partner for whom the prices of another group should be valid.

**Product group**
Product group for which the prices of another group should be valid.

**Customer group, Supplier group**
Different group that is to be used for products of the defined product group.

### Data

This list shows all partners for which different groups have been defined.

## Credit Limit Analysis

**Master Data > Partners > Customer > Credit limit analysis**
**Master Data > Partners > Customer > Customers > Balance tab > [Snapshot]**

*Fig. B-182 Credit limit snapshot*

This dialog allows analyzing the development of certain financial data of your customers for a certain period.
The data for the credit limit analysis are imported by Workflow Task via AIS (A+W Commercial Exchange Service). The snapshot can be displayed for all customers in general or just for a single customer.

### Functions menu

**Delete snapshots:**
This function is used to delete all snapshots. After that, the data have to be loaded into the database again.

### Selection

**Creation date, from - to**
Period for which snapshots should be shown. This option defines the customers for which a credit limit snapshot should be created:
*   **Customer from - to:** You can create the snapshot for a single customer or several snapshots for a series of customers. The name of the first and last customer appears automatically.
*   **Customer group from - to:** You can create the snapshot for a single customer group or several snapshots for a series of customer groups. The name of the first and last customer group appears automatically.

### Snapshots

This list shows all snapshots created by selecting customers or customer groups. The following data are displayed:
*   **Customer #:** Customer number.
*   **Name:** Customer name.
*   **Date:** Date on which the data were imported.
*   **Credit limit 1 / Credit limit 2:** Credit limit that has been granted.
*   **Unsettled accounts:** Total amount of unsettled accounts.
*   **Liabilities:** Current value of liabilities.
*   **Orders (not shipped):** Total amount of all new orders that were entered but have not been shipped yet (status < print shipping note).
*   **Orders (shipped but not invoiced):** Total amount of all orders that have been shipped but have not been invoiced (yet) (status < print invoice).
*   **Orders (invoiced, not transferred to financial accounting):** Total amount of orders that have been shipped and invoiced but no transferred to financial accounting (so far) (status < FinAcc transfer).
*   **Orders (total):** Volume of all shipped, not shipped, invoiced, and not invoiced orders that have not been transferred to financial accounting yet.
*   **Balance 1/ balance 2:** Balances.
*   **Customer locked:** Lock code from customer master data.
*   **Salesman:** Name of the salesman in charge as defined in customer master data.
*   **Last 12 months' turnover:** Total amount of orders within the past 12 months.
*   **Payment terms:** Payment terms acc. to customer master data.

## Marginal Income Limits

**Master Data > Partners > Customer > Marginal income limits**

*Fig. B-183 Marginal income limits*

This dialog is used to allocate the limits for analyzing the marginal income. These limits must be defined for every customer/customer group and PGR.
For all customer/product group combinations that have not been explicitly defined, the standard entries will be loaded from company data.

⇨ "Default MI" on page B-978

### Selection

Choose an option to specify for who these limits should be valid:
*   **Customer:** Marginal income limits for customers.
*   **Customer, customer group:** Marginal income limits for customer group.
The appropriate fields for selecting the customer or the customer group are accessible.

**Product group**
Product group for which the marginal income limits should be used.

**Minimum marginal income**
Bottom limit for the marginal income.

**Maximum marginal income**
Upper limit for the marginal income.

### Marginal incomes

The list shows all marginal incomes that differ from the standard value defined in company data.

## Exceeds Amount

**Master Data > Partner > Customer > Exceeds amount**

*Fig. B-184 Exceeds Amount*

This dialog is used to enter the percentage for commercial surplus the customer will usually accept for certain products.
In product master data you can also enter a percentage for a surplus/shortfall to be taken into account for serial orders.
When the production software reports surplus or a shortfall, the actually produced quantity will be adopted for the order item. The order will then be recalculated.

⇨ "Default Values for Different Quantities" on page B-597

> **Requirements**
> You should use surplus only if the following requirements are met:
> *   Transfer to production in OrderXML format
> *   File-less production reports

### Selection

**Customer**
Customer who accepts surplus or shortfall.

**Product**
Product for which the definition should be used. If a customer accepts surplus or shortfall for several products, you can enter different percentages for every product.

### Differing quantities

The values will be used for calculating the order quantity. The surplus or shortfall (expressed in units) appears at item entry on tab *Further details*.

**Surplus, Shortfall**
Percentage for the surplus and shortfall.

### Data

The list shows all customers who will accept surplus or shortfall for certain products.

## Calendar (Customer)

**Master Data > Partners > Customer > Calendar**

*Fig. B-185 Customer calendar*

This dialog is used for entering (per customer) the days to be omitted when calculating the payment terms, e.g. company holidays. The due date will be postponed if it lies within the define period.
The type of postponement must also be set in customer master data.
⇨ Tutorial 1, "Editing Customer's Calendars" on page B-103
⇨ "Partner Management - Finances" on page B-773

### Functions menu

The entries in this menu define the postponement for all the days marked in the overview (calendar). You can check several checkboxes.

*   **Skip payment:** Checks the checkbox of the selected days in *skip payment* column.
*   **Do not skip payment:** Removes the check from the checkboxes of the selected days.
*   **Skip delivery:** Checks the checkbox of the selected days in *skip delivery* column.
*   **Do not skip delivery:** Removes the check from the checkboxes of the selected days.
*   **Transfer dates:** Opens the dialog *Transfer calendar data* in order to copy the dates to another customer calendar.
    ⇨ "Transfer Calendar Dates" on page B-851

### Identification

**Number**
Number of the customer for whom holidays should be entered.

**Year**
Year in which the postponement is entered.

**Name, Street, ZIP/Town**
Customer details are automatically adopted from customer master data.

### Overview

The list shows the selected calendar. The days on which no payments must be due can be selected in columns *Skip payment* and *Skip delivery*.

You can check individual checkboxes or select several lines using the menu **Functions > Skip payment**.

When saving an order, the system checks whether the delivery to the customer on the selected date is desired or not. If delivery is not desired on the selected date, a message is output and the delivery date must be changed. The delivery date is also checked when copying orders.

> **Transfer dates**
> When you have entered the dates for postponing a due date and a delivery date you can transfer them to another customer. This function is available in menu *Functions*. Only the selected data will be transferred, not the entire calendar.

### Table

The table lists all customers for whom details for postponing due dates and/or the delivery date have been entered. You cannot enter a customer without checking at least one date (checkbox).
