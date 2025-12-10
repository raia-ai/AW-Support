---
title: "EN_AWBusiness_Master_Data_9_8-4"
source: "EN_AWBusiness_Master_Data_9_8-4.pdf"
tags: ["A+W Business", "Master Data", "Partner Management", "Software Reference", "Customer Data", "Supplier Data", "Financial Accounting", "Credit Limit", "Sales Data", "Production Settings"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the Partner Management module within A+W Business Master Data. It details the configuration of customer and supplier data, including financial settings, tax data, credit limits, and sales information."
long_description: "This is a detailed software reference manual for the Partner Management section of A+W Business Master Data. It provides comprehensive instructions and explanations for managing partner (customer and supplier) information within the system. The guide covers a wide range of settings organized into various tabs. Key areas include defining payment terms, solvency, and lock codes for partners. It explains how to configure tax data, including settings for Brazilian taxation and compound taxes. A significant portion is dedicated to the 'Balance' tab, which covers setting and checking credit limits, comprehensive checks for subsidiaries, and managing financial values like receivables and liabilities. The document also details the 'Sales' tab for tracking quotations and orders, and the 'Production' tab for setting up production-related parameters like capacity areas, labels, shipping, and packing optimization. Additional dialogs and functions such as managing subsidiaries, employees, file attachments, and transaction documents are also thoroughly explained. The guide serves as a complete reference for users responsible for maintaining accurate and detailed partner master data in the A+W Business system."
---

# Partner Management

---
## Software Reference

**Paymt. terms**
Payment terms agreed with the customer. The setting can be changed in the order.
⇨ "Payment Conditions" on page B-905

**Paymt. mode**
Payment mode agreed with the customer, e.g. invoice, cheque, bank transfer, etc. This setting can be changed in the order.
⇨ "Payment Mode" on page B-914

**Solvency**
Information on the customer's credit standing. Further solvency levels can be defined in the directory. This field will not be shown for suppliers.
⇨ "Credit Rating" on page B-906

**Lock code**
Options for the lock code are:
-   **Not locked:** Orders can be entered for this customer.
-   **Locked:** The customer does not appear in the partner search and orders cannot be entered for him either. A message to that effect is displayed.
-   **Replicated:** Customer data are kept in the master database and cannot be changed in the slave database.

**No reminders**
You can define whether the customer should get reminders at all. This code is transferred to financial accounting (FinAcc). This checkbox does not appear for suppliers.
-   [ ] The customer can get reminders.
-   [x] No reminders should be sent to the customer even if there are unpaid invoices.

**(Reminder text)**
Way in which the customer should be reminded, e.g. common, severe. This code is used for transfer to financial accounting.

**Main acct.**
Customer number of the main debtor. The customer number will be used as an account number by default. There are the following exceptions:
-   If an alternative invoice address has been defined as a subsidiary or an independent customer, this customer number can be used as the account number.
-   The main account matches the main debtor's customer number in this case. If this field is blank, the number of the current customer will be automatically used as the main account.
-   If the checkbox 'Transfer customer account instead of customer number' is checked in 'Options' for the transfer to Microsoft Business Solutions XAL (MBS-XAL) financial accounting, the customer's debtor number will be transferred as the account number.

**Creditor acct.**
A+W Business permits 8-digit customer numbers that are also used as customer numbers. If you are using a financial accounting program that can handle e. g. only 5-digit customer numbers, you can enter the corresponding number as a reference.

---

# Tax data

**Tax 1-5**
You can assign different tax rates to a customer by selecting the required entries. The tax rate for VAT is usually selected in the first field, e.g. 19%.
If you are using Brazilian taxation you have to check the appropriate checkboxen, too.
The settings can be changed in the order.
⇨ "Tax" on page B-903
⇨ "Brazilian Tax" on page B-915

**Calculate 2. tax based on 1.**
In some countries, the invoice total can be subject to another tax.
-   [ ] VAT 2 should be calculated irrespective of VAT 1.
-   [x] VAT 2 will be based on VAT 1.

**Example**

| | |
| :--- | ---: |
| Turnover | 100.00 |
| Tax 1 (7 %) | 7.00 |
| **Subtotal** | **107.00** |
| Tax 2 (8 %) | 8.56 |
| **Total** | **115.56** |

---

# Partner Management – Balance

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Balance tab**

This tab shows the credit limit. If the system reports receivables to financial accounting (FinAcc), the balance will be updated automatically.
⇨ Tutorial 1, "Finances and Balance" on page B-80

The fields in sections Identification and Address are described in connection with the Address tab.
⇨ "Partner Management - Address" on page B-759

## Credit limit

If you define a credit limit for the customer, you have to enable the check as well. If the credit limit check is active and the credit limit is exceeded, this customer will be locked for order entry.

If the check is disabled, the system will not check the unsettled accounts against the credit limit. Order entry will not be locked.

**Comprehensive check**
The credit limit check can be run for the main customer or for the individual subsidiaries:
-   **None:** There will be no credit limit check.
-   **by subsidiary:** The credit limit of every independent subsidiary will be checked. Only if subsidiaries are marked as independent, orders can be entered and checked by subsidiary. You have to set the check and the values in fields Credit limit 1/2 for every independent subsidiary.
-   **By main account:** The main account's credit limit will be checked. If no independent subsidiaries have been defined, this includes all orders entered for this customer. If you have defined independent subsidiaries and have entered a main account for each of them, the check will include all subsidiaries.

## Check

The credit limit check is based on the entries in fields Credit limit 1/2. You can select one of the following methods:
-   **No check:** There will be no credit limit check.
-   **Limit 1 + report limit 2:** The entry in field Credit limit 1 defines the lock. The entry in field Credit limit 2 is only checked.
-   **Limit 2 + report limit 1:** The entry in field Credit limit 2 defines the lock. The entry in field Credit limit 1 is only checked.
-   **Check limit 1:** Only the entry in field Credit limit 1 defines the lock.
-   **Check limit 1+2:** The entries in fields Credit limit 1 and Credit limit 2 define the lock.
-   **Check limit 2:** Only the entry in field Credit limit 2 defines the lock.
-   **Cash in advance:** Orders will be produced only after the invoice amount has been received.

**Receivables (due since...)**
If the credit limit should be checked, you can define how old the unsettled accounts to be checked have to be.

> **No check at item entry**
> The credit limit will be checked only when the order header is entered. There will be no check at item entry.

## Cost and surcharge calculation

> **Prerequisite**
> Cost and surcharge calculation can be shown only if the checkbox Production cost calculation is checked in allocation of rates, and the surcharges are defined in company data.
> ⇨ "Rate allocation" on page B-663
> ⇨ "Cost and surcharge calculation" on page B-977

**Special surcharge**
Special surcharge to be taken into account for cost and surcharge calculation for this customer.

---

# Financial values (check by subsidiary)

**Credit limit 1/2**
Two entries can be made for the credit limit:
-   **Credit limit 1:** This entry defines the secured credit limit.
-   **Credit limit 2:** This entry is an internal credit limit granted to the customer because of his credit standing.

You have to enable this check to prevent that orders can be entered after the credit limit is exceeded.
At document entry, the system checks if the customer's credit limit is exceeded. The document status is automatically set to 700.
⇨ Tutorial 2, "Status Administration" on page B-418

**Receiv. (FinAcc/date)**
Receivables are reported from financial accounting (FinAcc). These fields will be filled in only if there is an appropriate interface with financial accounting. Apart from the total unsettled accounts, the report date is shown.

**Liabilities**
Receivables are reported from financial accounting. This field will be filled in only if there is an interface to financial accounting.

**Orders**
Shows the total orders on hand including the invoices that have not been transferred to financial accounting yet.

**Balance 1/2**
The balance is calculated from the credit limit - UA (FinAcc) - Orders - Receivables. Balance 1 is insured while Balance 2 depends on your company's scope of discretion.

**Turnover current year/month**
Customer's turnover in the current year and in the current month. The fields are filled from module Turnover statistics.

**Turnover prev. year**
Customer's turnover from last year. The icon can be used to open the dialog Turnover/order area where you can view the turnover by order area, year, and month.

## Currency/rate

**Currency**
Standard currency for orders from this customer. The setting can be changed in the order.
⇨ Sales, "Header data - Terms" on page C-427

**Exch. rate fixed**
You can define that the foreign currency amount is calculated only at order entry, according to the current rate.
-   [ ] Conversion is based on the current rate, which is maintained in dialog Currency.
-   [x] The amount in foreign currency will not be recalculated when the invoice is issued.
⇨ "Currency" on page B-908

Choose an option to define whether documents can be issued in foreign currency.
-   **No currency:** Documents for this customer can be entered in national currency only.
-   **Order entry in national currency:** Documents for this customer are entered in national currency by default. Prices can be shown in home or foreign currency.
-   **Order entry in foreign currency:** Documents for this customer are entered in foreign currency as a standard. Prices can be shown in home or foreign currency.
    ⇨ Sales, "Document group" on page C-408

---

# Discount calculation

> **Prerequisite**
> Cash discount can be calculated only if the checkbox Cash discountable is enabled in product master data.
> ⇨ "Suited for discount, cash discount" on page B-605

Choose an option to define how the cash discount is going to be calculated:
-   **On gross amount:** Cash discount is calculated from the gross order total.
-   **On net amount (gross minus cash discount):** Cash discount is calculated from the net order total, and is deducted from the gross amount.
-   **On net amount:** Cash discount is calculated from the net order total.
⇨ Tutorial 1, "Cash Discount" on page B-97

---

# Partner Management - Sales

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Sales tab**

This tab shows the lists of current orders and quotes for this customer. For suppliers, inquiries and purchase orders are listed. A customer can also be allocated up to two sales representatives.

The fields in sections Identification, address, and Connections are explained in connection with tab Address.
⇨ "Partner Management – Address" on page B-759

## Sales data

> The fields Sales rep. 1 and 2 will not be displayed for suppliers.

**Sales rep. 1, 2**
The customer can be allocated two sales representatives. The sales representatives are adopted for the order and can be changed if required.

**Turnover share sales rep. 2**
Share of sales representative 2 in the customer's total turnover. This entry will be adopted for the order and can be changed if required.

> **Commission rate in order**
> The defined commission rate is shown on the order only if interactive sales commission is enabled in company data.
> ⇨ Software Reference, "Interactive sales commission" on page B-937

**Current quotations**
This list shows the quotations for this customer for which no order has been placed (yet).

**Current orders on hand**
This list shows all orders that have not been archived yet.

**Current inquiries**
For suppliers, this list shows all inquiries for which no purchase order has been issued (yet).

**Current purchase orders**
For suppliers, this list shows all purchase orders that have not been archived.

---

# Partner Management – Production

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Production tab**

This tab serves to make the settings for production and dispatch. For your internal list, you can also define the surface capacity you will usually book for this customer.

The fields in sections Identification and Address are described in tab Address.
⇨ "Partner Management - Address" on page B-759

The fields in the sections Production labels, Shipping, and Rack optimization only appear for customers.

## Capacity areas

Enter the square meters of IG, laminated, and/or toughened glass scheduled for this customer for the individual weekdays. These details will not be transferred to capacity planning or production. They only serve as an internal estimation of production capacity.

Total capacities are defined in company data.
⇨ "Capacity areas" on page B-978

## Production labels

**Layout / Logo**
Only in connection with A+W Production.
The fields Layout and Logo are used for printing the customer's logo on the production labels. This requires a thermo transfer printer and has to be discussed with A+W Software GmbH.
These fields will not be displayed for suppliers.

## Product code

This field appears only if CPIP creation is enabled in company data. The CPIP code can be checked only if the appropriate data have been selected in product management.
⇨ "CPIP data" on page B-606
⇨ "CPIP creation" on page B-951

**CPIP creation**
Characteristic Performance Identification Paper (characteristics of features and of the performance).
-   [ ] No CPIP code will be created.
-   [x] At document entry, the CPIP code is determined based on the product data, and entered in Item entry > Supplement tab. The restrictions can be disabled. The data will be transferred to A+W Production during export.

## Shipping

The fields in sections Shipping and Rack optimization do not appear for suppliers.

**Sorting**
Only in connection with A+W Production.

**Packing**
Only in connection with A+W Production.

**Distance**
Distance (one-way, in kilometers) to be charged per delivery round. Together with the mileage fee for the allocated route, this value is used for calculating the freight charges.

## Packing optimization

**Packing rule**
Currently not used.

**Group creation**
Currently not used.

## Grill Entry

**Cutback (single)**
For the bender, you can define the distance between outside glass edge and aluminium spacer.

**Calculation type**
Standard calculation of drilling points for grills for this customer:
-   **Field-symmetrical:** Holes will be calculated so that the fields are symmetrical.
-   **Drill hole-symmetrical:** Drilling will be calculated so that the drill points are symmetrical.
⇨ Tutorial 1, "Calculation type for grill construction" on page B-163
The setting can be changed in the order.

## Spacer settings

**Type**
Spacers that are fitted for this customer as a standard. The setting can be changed in the order.

**Color**
Color (variant) to be used for this customer by default. The setting can be changed in the order.

---

# Partner Management – Attachments

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Attachments tab**

This tab can be used for attaching files with additional information, e.g. special agreements. The files are linked and are saved in a partner-specific directory.
⇨ Sales, "Attaching documents" on page C-57

The fields in sections Identification, Address are described in connection with the Address tab.
⇨ "Partner Management - Address" on page B-759

## File attachment

All linked files are listed. You can enter a comment for every linked file, e.g. regarding its validity.
Define the path for the storage location in the company data.
⇨ Master Data, "File attachments" on page B-932

## Declaration of performance

The dispatch of declarations of performance can be enabled per partner (customer).
-   [ ] No declaration of performance will be dispatched for the current partner.
-   [x] A declaration of performance will be dispatched for every order item to this partner. A flag will be set after the first dispatch so that the same declaration of performance will not be sent again.
⇨ "Declaration of Performance, Management" on page B-583

---

# Free Numbers / Areas

**Master Data > Partners > Customer, Supplier > Customers, Suppliers > [Zoom]**

This dialog shows the free numbers that can be used for entering new master data.
⇨ Tutorial 1, "Input of Partner Master Data" on page B-50

---

# Telecommunication Data

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Address tab > [Connections]**

This dialog shows the defined phone and fax numbers. If you are using a telephone software system, you can dial a number by double-clicking on it.

---

# Invoicing Surcharge/Minimum Value per Order Area

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Order tab > [Order area]**

You can use this dialog to enter a special minimum invoice value or an invoicing surcharge per order area. The surcharges are described in connection with the tab Order.
⇨ "Mode" on page B-764

---

# Route Priority

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Order tab > [Route priority]**

This dialog shows all partners who belong to the same route. Data are loaded from customer master data and from dialog Delivery time. You can change the route sequence in dialog Delivery time. These entries are used at order entry.

---

# Text Search

**Master Data > Partners > Partner management > Text tab > [Zoom]**

This dialog shows all defined text. Select a text module and press [OK] to adopt it for partner management.
⇨ "Text" on page B-1040

---

# Turnover/Order Area

**Master Data > Partners > Partner Management > Balance tab > [Last year's turnover]**

This dialog shows the previous year's turnover of the customer per order area. The options in section Selection can be used for modifying the display.

---

# Subsidiary

**Master Data > Partners > Customer > Customers > Employees/Subsidiaries/Documents tab > double-click on Subsidiary**

This dialog is used to enter data for your customer's subsidiary. The info section shows the actual subsidiary you are about to enter or change.

The fields in this dialog are described in detail in connection with dialog Partner Management.
⇨ "Partner Management" on page B-757

> **Standard shipping address**
> The customer's standard shipping address is entered as a subsidiary. When you define a subsidiary as the standard shipping address you have to check checkbox Standard on the Address tab.

To finish input or modification of the subsidiary, click on the Back to main company icon.

---

# Employee

**Master Data > Partners > Customer > Customers > Employees/Subsidiaries/Documents tab > double-click on Employees**

This dialog is used for entering the names of your customer's employees plus additional information such as the department in which he/she works, his/her function, phone extension, fax number, and email address.

## Address

**Name 1-3**
Full name of the employee, e.g. Dr Richard Sander.
If this employee's address differs from the company's address you can enter the details at this point.

## Connections

Phone number(s), fax number, email address of the employee.

**Contact (order processing), Contact (sales)**
You can define whether the employee is the only contact in questions of order processing and/or sales. These details can be used for analysis via ODBC interface.
-   [ ] The employee is not explicitly responsible for order processing or sales matters.
-   [x] The employee is the contact for sales and orders.

## Specification

Title and function of the employee.

**Info**
You can enter further details here, e.g. other aspects of his sphere of responsibility.

## Classifiers

This section shows the allocated classifiers.

## Table

List of this customer's employees.

**[Classifier values]**
Opens the dialog Classifier value allocation where an entry can be made or adopted.
⇨ "Classifier Value Allocation" on page B-798

**[Classifier definition]**
Opens the dialog Classifiers where you can make or adopt an entry. Classifiers for employees are managed separately from the classifiers for partners.
⇨ "Employee Classifiers" on page B-797

---

# Transaction Management

**Master Data > Partners > Customer > Customers > Employees/Subsidiaries/Documents tab > double-click on Document**

You can use this dialog for managing and tracing documents, e.g. which of the customer's employees has been asking for information, and when.

You can also record who has tracked and completed this document, and when.

**Done**
This box can be checked when a document is completed. This code appears on tab Empl./Subsid./Documents.
-   [ ] The document is still open and should be traced.
-   [x] The document is completed.

## Tab

-   **Event:** Use this tab to enter a document.
-   **Table:** This tab shows all documents (projects).
-   **Text received, Text sent:** This tab can be used to enter text regarding the corresponding document.
-   **Agreements:** You can use this tab to enter details regarding any agreements that have been made.

---

# Employee Classifiers

**Master Data > Partner > Customer > Customers > Functions menu > Employee > Functions menu > Classifier definition**

This dialog serves for managing the classifiers for your customers' employees. You can define the classifier and the types of values it can have:
-   **No..:** Only numerical values can be allocated, e. g. sales figures.
-   **Alpha-num.:** Numbers and letters can be allocated, e.g. exhibition give-away 2010.
-   **Date:** Only dates can be allocated.

-   [ ] This value is invalid for this classifier.
-   [x] This value can be allocated to the classifier.

Classifiers for employees are managed separately from those for partners. They can only be used for ODBC queries.
⇨ Tutorial 1, "Enter a Classifier" on page B-74

---

# Classifier Value Allocation

-   **Master Data > Partner > Customer > Customers > Classifiers tab > Functions menu > Classifier values**
-   **Master Data > Partners > Customer > Customers > Employee tab > double-click on Employee > [Classifier values]**

You can use this dialog to enter alpha-numerical values for a classifier. The [Adopt] button is used to allocate this value to a customer or employee.
⇨ Tutorial 1, "Allocate Classifier Value" on page B-75

---

# Check Receivables

**Master Data > Partners > Customer > Customers > Functions menu**

This dialog lists all open invoices including the sum due, the reminder date, and the reminder level.

The receivables are imported by a Workflow Task via AIS (A+W Commercial Exchange Service).

The receivables check only works in connection with the SQL financial accounting system Syska. This function is released in company data.
⇨ "Company Data > Financial Accounting" on page B-923

---

# Copy Master Data

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Functions menu > Global Changes group > Copy Master Data**

This dialog is used for copying the master data of a partner, e. g. if you have entered a partner who should be defined as a customer now.

---

# Partner Change

**Master Data > Partner > Customer, Supplier > Customer, Suppliers > Functions menu > Global Changes group > Change selected partner**

This dialog is used to change the allocation of automatic surcharges and special discounts for the current partner.
