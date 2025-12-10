---
description: "EN_AWBusiness_Sales_4_7-4"
---


# Transfer, Document Import/Export

*Software Reference*

- **Transfer external key as currency code**: If you are using several currencies and if you have assigned your financial accounting system's external key to the currencies in the master data, you can transfer this external key to financial accounting. The currency will be identified based on the external key.
  ⇨ Master Data, "Currency" on page B-908

---
### Customer group

- **Customer transfer inactive**: The customer name will not be transferred.
- **Transfer customer account instead of number**: If a receivables account has been defined in the customer data, this will be transferred instead of the customer number.
  ⇨ Master Data, "Partner Management - Finances" on page B-773

### Other group

- **Automatic sorting active (customer/invoice/order)**: The data will be automatically sorted for the transfer, by customer, invoice, and/or order. If sorting is disabled, the sorting will be adopted from the number manager.
- **Change output file**: This function is only necessary if financial accounting uses fixed file names rather than number areas. The output file from the previous transfer will be overwritten. If this function is switched off, the new data will be added to the output file. As a result, this file will increase in size.
- **OEM conversion active**: You can enable the conversion of special characters for transfer to financial accounting, e.g. ä into ae. OEM conversion can be locked in the company data.
  ⇨ Master Data, "Disable OEM/ANSI conversion" on page B-960

## Debit Entry FinAcc

**Path**: Documents > Order, credit note > FinAcc transfer

[Image: Fig. C-357 Transfer to FinAcc – Debit entry FinAcc dialog, showing a list of debit entries ready for transfer, with columns for customer, invoice details, amount, and status.]

In this dialog, define the invoices/credit notes that are to be transferred to financial accounting. The dialog is the same for all financial accounting programs. The header always shows the name of the financial accounting system.
⇨ Tutorial, "Financial Accounting (FinAcc)" on page C-350

### Identification

- **Client**: Client for whom the invoices are transferred.
- **Area**: OM area the documents pertain to.
- **Employee**: Employee logged in to A+W Business.
- **Number manager**: Number manager that includes the invoices or credit notes to be transferred. Prior to financial accounting transfer, the program checks whether at least one document in the number manager includes an invoice number and the necessary status for transfer. A sequential number will only be assigned if this is the case.
- **Check sum**: When the documents have been transferred to financial accounting, the total amount transferred will be displayed as a check sum.
- **Batch**: When the documents have been transferred to financial accounting, the number of the transfer batch is displayed. It will be automatically loaded - in ascending order - from the number area defined for the client and/or order area.
  ⇨ Master Data, "Number Ranges - Financial Accounting" on page B-895

### Output

- **Debtor, creditor**: Path and file in which the data is saved. The information is adopted from the company data.
  ⇨ Master Data, "Path and file name" on page B-924
- **Invoice, credit note**: Path and file in which the data is saved. The information is adopted from the company data.
- **Booking date**: The system date is shown as the booking date. It can be changed if required.
- **Period**: Booking period to which the invoices and credit notes belong.
  ⇨ Master Data, "Booking Periods" on page B-1023
- **Current order**: Order number currently being transferred to financial accounting.
- **Item**: Order item number currently being transferred to financial accounting.
- **Total orders**: Number of documents transferred to financial accounting.
- **Items**: Number of items transferred to financial accounting.

### Overview

The list shows all documents included in the current number manager. Only if invoices and credit notes are transferred via the same number manager will both document types be listed.

### Additional information

⇨ Master Data, "Finances and Balance" on page B-80
⇨ Master Data, "Company Data > Financial Accounting" on page B-923
⇨ Tutorial, "Financial Accounting (FinAcc)" on page C-350

## Settings FinAcc Transfer

**Path**: Documents > Orders, credit, P.O. > FinAc transfer > Functions menu > Settings

[Image: Fig. C-358 FinAcc transfer settings dialog, showing fields for Classifiers, Default accounts, Tax IDs, and Business type for down payments.]

Use this dialog to enter details for the transfer to financial accounting.

- **Classifier 1, 2**: Lists all classifiers for selection that are valid for all market partners. If classifiers with additional customer information have been entered in the master data, these can be transferred to financial accounting, e. g. customer's receivables account, customer type.
  ⇨ Master Data, "Enter a Classifier" on page B-74
  ⇨ Master Data, "Classifiers" on page B-752
- **Default proceeds account, cash discount, rounding differences**: These fields only are analyzed for Golden Soft financial accounting. They refer to the input in field Cuenta.
- **Old, new tax ID**: This information is only needed if documents are transferred to financial accounting after the tax code has been changed.
- **Business type for down payments**: The business type from the order can be changed.

## Import/Export of Payments

**Path**: Documents > Orders > Import/export of payments

[Image: Fig. C-359 Import/export of payments dialog, with tabs for Export and Import, showing fields for date range, status, sorting, and interface selection for payment transactions.]

Use this dialog for Brazilian payment transactions via the bank. With the export, the invoices (payment information) are transferred to the bank. With the import, reports on payments made are imported.

The following prerequisites must be met for the import/export of payment information:

- For each bank, individual customizing formulas must have been created for the import and export for payment transactions.
- Each bank must be assigned with these formulas: Master data > Finances > Banks.
- For each currency, the international currency code must be entered as the external key.
- The following settings must be enabled in the company data:
  - **Parameter tab**:
    - Brazilian tax and Import/Export of payments
  - **NFE tab**:
    - Company's tax number (CNPU tab)

## Transfer to Archives

**Path**: Documents > Quotation, order, credit, inquiry, P.O. > Transfer to archive

[Image: Fig. C-360 Transfer to archives > Sales dialog, showing a list of documents with options to transfer them to commission statistics, turnover statistics, archives, and to delete them.]

Use this dialog to manually transfer documents to archives.

### Identification

- **Client**: Client whose documents should be archived.
- **Employee**: Employee logged in to A+W Business.
- **Number manager**: Number manager containing the documents to be archived.

### Documents

The fields show the number of transferred data records.

- **Commission statistics**: Documents can be transferred to commission statistics individually.
  - ☐ Documents will not be transferred to commission statistics.
  - ✔ Documents will be transferred to commission statistics.
- **Turnover statistics**: Documents are transferred to turnover statistics by default.
  - ☐ Documents will not be transferred to turnover statistics.
  - ✔ Documents will be transferred to turnover statistics.
- **Archives**: Documents are transferred to current archives by default. After that, the documents should be deleted from the main database.
  - ☐ Documents will not be transferred to archives.
  - ✔ Documents will be transferred to archives.
- **Delete**: Documents should be deleted from the main database after they have been transferred to archives.
  - ☐ Documents will not be deleted from the main database.
  - ✔ Documents will be deleted from the main database.
  ⇨ Master Data, "Company Data > Archives" on page B-962

### Defaults

- **Statistics year**: Define the statistics year to which the documents will be transferred. If there is no entry, this will be based on the document date.
- **Monthly statistics**: Define the statistics month to which the documents will be transferred. If there is no entry, this will be based on the document date.
- **Transfer empty sales commission**: Usually, only those documents that include a commission of > 0 are transferred for commission calculations.
  - ☐ All documents will be transferred to commission calculations.
  - ✔ The documents will be transferred to commission calculation even if no commission is included.
- **Reverse booking**: If a document has been transferred to the wrong statistics month, for instance, this can be undone.
  - ☐ All selected documents will be transferred to the statistics and archives defined in the fields.
  - ✔ The documents will be retrieved from the wrong statistics or archives. Subsequently, they have to be transferred to the correct statistics or archives.

### Documents

The list shows all documents included in the selected number manager.

## Import

**Path**: Documents > Order > Import

The Import dialog is the same for orders, quotations, and credits. It is described here using the example of an Order.

[Image: Fig. C-361 Import dialog with two tabs. The first tab 'Import pool' lists importable documents. The second tab 'Create document' shows documents being created and a logbook of the import process.]

On this dialog, you can put imported documents from the import directory into the associated number manager.
⇨ Tutorial, "Document Import" on page C-373

You can open and correct documents that could not be imported due to incorrect data via the External document management dialog.
⇨ "External Document Management" on page C-684

## External Document Management

**Path**: Documents > Order > Import > Double-click document > External document management

The External document management dialog is the same for orders, quotations, and credits. It is described here using the example of an Order.

[Image: Fig. C-362 Import - external document management dialog, showing detailed fields for a single external document, including source file, address, parameters, and status.]

This dialog displays the details for the import of the external documents. Normally, these settings do not have to be edited.
Imported documents are loaded according to the defined rules, and are saved as new orders.
⇨ Tutorial, "Document Import" on page C-373

# Project Invoicing

**Path**: Documents > Order > Project invoicing

The dialogs for project invoicing are only available if the corresponding project management has been activated in the company data and if the projects have been created and assigned.
⇨ Master Data, "Company Data > Documents" on page B-928

This chapter provides information on the following subjects:

- "Invoicing” on page C-685
- "Projects - Documents" on page C-696
- "Hour Claim" on page C-697
- "Purchase" on page C-698
- "Claims Calculation" on page C-699
- "History of Claims" on page C-701

## Invoicing

**Path**: Documents > Order > Project invoicing > Invoicing

The tabs in the Invoicing dialog depend on the type of project management enabled in the company data. The following descriptions point out the project management types in which the tabs and fields are available.
⇨ Tutorial 2, "Project/Invoice Management" on page B-494

> **Dialog for customer and supplier data**
> The Projects dialog is identical for customers and suppliers. We are going to describe it in connection with an Order in this manual.

This chapter provides information on the following subjects:

- "Functions menu" on page C-686
- "Print menu" on page C-686
- "Projects - invoicing" on page C-687
- "Projects - Blanket Order" on page C-690
- "Projects - Allocated Orders" on page C-691
- "Projects - Allocated POs" on page C-692
- "Projects - Totals" on page C-693
- "Projects - Estimated Quantities" on page C-694
- "Projects - Table” on page C-695

### Functions menu

**Path**: Documents > Order > Project invoicing > Invoicing > Functions menu

Use this menu to open other dialogs without closing invoice management. The available functions depend on the activated project management mode. The following entries are displayed:

- **Add hours required**: Opens the Hours required dialog in which you can enter e. g. the fees for assembly work (only Invoicing management).
  ⇨ "Hour Claim" on page C-697
- **Add purchases required**: Opens the Purchasing dialog in which you can e. g. enter the cost of fitting material (only Invoicing management).
  ⇨ "Purchase" on page C-698
- **Claims calculation**: Opens the Claims calculation dialog in which you can issue and check invoices.
  ⇨ "Claims Calculation" on page C-699

### Print menu

**Path**: Documents > Order > Project invoicing > Invoicing > Print menu

Use this menu for drawing up lists of invoices. The entries are only available if the Invoicing mode is active.

#### Screen group, printer group

- **Print by PGR**: Items are sorted by product groups for printing.
- **Print by product**: Items are sorted by product groups for printing.

#### Status report group

- **Status report**: Produces a list of all projects to be invoiced, including the current claims and current balance.
  - **Screen**: An individual document is displayed on the screen and can be checked.
  - **Printer**: Documents are sent directly to the printer and printed.

#### List group

- **List**: Lists the estimated sums and the accumulated costs for the selected project to be invoiced.
  - **Screen**: An individual document is displayed on the screen and can be checked.
  - **Printer**: Documents are sent directly to the printer and printed.

## Projects - invoicing

**Path**: Documents > Order > Project invoicing > Invoicing > Invoices tab

[Image: Fig. C-363 Projects - invoicing tab, showing fields for project selection (Quotation, Customer order no.) and definition (Title, Name, Address, etc.).]

Use this tab to add additional details for a project, e. g. an alternative shipping address and alternative payment terms.

### Selection

- **Quotation**: Quotation number if the quotation has been entered.
- **Customer order no.**: Number of the order that has been sent by the customer.
- **Insert date**: Date on which the number has been entered.
- **Project, invoicing**: Number of the project or invoice that has been entered for the blanket order.
- **[Documents/Info]**: Opens a list of the orders that have been entered for the selected project (only standard project management).
  ⇨ "Projects - Documents" on page C-696
- **Customer**: Customer involved in this project. When you enter a document, only those projects that have been assigned to the customer in the master data are displayed.
- **Blanket order**: Number of the basic order for which the invoice is entered (only project management + accounting management).

### Terms

This area is only displayed if you have activated the Extended project management in the company data.
⇨ "Extended Project Management" on page B-825

- **Valid from, to**: Start and end date of the period during which documents can be issued for this project.
- **Salesman**: Representative who is responsible for the market partner. The turnover will be used for calculating the sales commission.
- **Payment terms**: Payment terms, in case these differ from the terms defined in partner management or in the document. This setting will be saved in the document when the project is allocated.
- **Net turnover, sqm., quantity**: You can enter maximum values for every customer project. When you close the order entry, a list of the orders entered plus the accumulated totals will be displayed.

### Definition

- **Title**: Form of address to be printed on documents, e.g. Messrs.
- **Name 1-3**: The three fields allow entering the name plus supplements, e.g. group of companies.
- **Street**: Customer's street address.
- **State/Country**: Province and country abbreviation that should be printed on documents for correct designation of the address. The State field is intended for USA and Canada.
- **ZIP/City**: Postal code and city.
- **Invoicing**: Invoice date or number.
- **Phone**: Phone number of a contact for this project, e. g. the site manager.
- **Employee**: Employee responsible for the partner.
- **Status**: State of the project:
  - **Current**: Documents can be entered for this project.
  - **Completed**: The project has been completed. No additional documents can be entered for this project. This status is set automatically when the agreed maximum values have been reached. It can also be set manually ahead of time.
- **Distance**: Distance (one-way, in kilometers) to be charged per delivery round. Together with the mileage fee for the allocated route, this value is used for calculating the freight charges.
- **Take over in order**: The fields in the Definition area can be taken over into the order.
  - ☐ The fields are not taken over into the order.
  - ✔ The fields are taken over into the order.

### Info, memo

Additional information.

## Projects - Blanket Order

**Path**: Documents > Order > Project invoicing > Invoicing > Blanket order tab

[Image: Fig. C-364 Projects - blanket order tab, displaying a list of items from a blanket order with columns for description, quantity, calculated quantity, percentage, and calculated amount.]

This tab is only displayed if the function Invoicing of allocated orders is active. The items and quantities of the blanket orders are displayed.
⇨ Tutorial 2, "Invoicing of Blanket Orders" on page B-508

Use the context menu (right-click) to open the History of claims dialog in order to view a list of existing claims.
⇨ "History of Claims" on page C-701

### Totals

In this section, the total SP and total PP for the blanket order are displayed.
In addition, the amount already invoiced and the percentage are shown that comprise this amount of total SP.
These two values are updated with each additional invoice. However, they do not reflect whether the amount has already been paid.

## Projects - Allocated Orders

**Path**: Documents > Order > Project invoicing > Invoicing > Allocated orders tab

[Image: Fig. C-365 Projects - allocated orders tab, showing two sections. The top section lists allocated documents (orders/credit notes), and the bottom section lists the items within the selected document.]

Use this tab to display the allocated orders and credit notes. This tab is only available if Invoicing of allocated orders or Extended project management + Invoicing of allocated orders is active.

> **Allocated documents**
> Standard project management allows you to view orders and purchase orders by clicking on the button [Documents/Info] on the Invoices tab.

## Projects - Allocated POs

**Path**: Documents > Order > Project invoicing > Invoicing > Allocated P.O.s tab

[Image: Fig. C-366 Projects - allocated POs tab, showing a list for allocated purchase orders with columns for P.O. number, supplier, dates, and totals.]

Use this tab to view the allocated purchase orders. This tab is only available if Invoicing of allocated orders or Extended project management + Invoicing of allocated orders is active.

This tab is not shown if Extended project management is active.

- **Order-related P.O.s**: Switch display.
  - ☐ Manually entered purchase orders for this project are displayed.
  - ✔ Referenced purchase orders for the project are displayed.

## Projects - Totals

**Path**: Documents > Order > Project invoicing > Invoicing > Totals tab

[Image: Fig. C-367 Projects - totals tab, showing two lists: 'Products' and 'Product groups'. Both lists display estimated vs. actual quantities, square meters, and turnover, along with fulfillment percentages.]

This tab shows the totals accumulated for the selected project so far. This tab is only accessible if Extended project management is active.
The totals are shown in red if the estimated quantities have been reached or exceeded.
⇨ "Projects - Estimated Quantities" on page C-694

### Products, product groups

The lists show the current values for products and/or product groups.

## Projects - Estimated Quantities

**Path**: Documents > Order > Project invoicing > Invoicing > Estimated quantities tab

[Image: Fig. C-368 Projects - estimated quantities tab, allowing users to define estimated quantities, square meters, and turnover for specific products or product groups for a project.]

Use this tab to enter details on the estimated quantity for a project. These details will be used for calculating the totals. This tab is only accessible if Extended project management is active.

### Overview

The list shows all products or product groups for which estimated quantities have been entered.

### Selection

Choose an option to define the subject of your quantity estimation:

- **Product**: If you have entered a product number, the product name is automatically displayed.
- **PGR**: If you have entered a product group number, the name of the product group will be displayed automatically. You can select just one PGR. An MPG or SPG cannot be selected.

- **Est. sqm**: Maximum amount of glass to be used.
- **Estim. quantity**: Maximum number of lites or products to be used.
- **Estim. turnover**: Maximum net amount for this project. When you close the order entry, a list of the orders entered plus the accumulated totals will be displayed. The values will be used for calculation on the Totals tab.

### Buttons

The buttons can be used to add or delete entries. When you add an entry, the fields for the estimated quantities are enabled. Please make sure you select the appropriate option (product, PGR) before adding a new line.

## Projects - Table

**Path**: Documents > Order > Project invoicing > Invoicing > Table tab

[Image: Fig. C-369 Projects - table tab, showing a table overview of all projects matching the defined criteria, with columns for Invoice No., Project, Customer, and Status.]

Depending on the project management, this tab shows all projects or invoices matching the defined criteria. If no criteria are defined, all projects will be displayed.

## Projects – Documents

**Path**: Documents > Order > Project invoicing > Invoicing > Invoices tab > [Documents/Info]

[Image: Fig. C-370 Projects - documents dialog, displaying totals for the current project, such as net turnover and quantity, compared against maximum object values.]

This dialog lists all documents allocated to the current project. It is only available in standard project management.
The dialog is also displayed if item entry is closed. In this case, however, only orders which have been entered for this project for the selected customer will be listed.

## Hour Claim

**Path**: Documents > Order > Project invoicing > Invoicing > Functions menu > Add hour claim

[Image: Fig. C-371 Add hour claim dialog, showing a list of invoices with fields to enter the value of an hour claim, along with estimated and real hours.]

Use this dialog to enter the amount to be invoiced for additional work, e. g. for assembly. The amount is added to the selected project.
This function is only available if the mode Invoicing of allocated orders has been enabled.

- **Invoice number**: Number of the invoice to which these hours will be added.
- **Value**: Amount of the hour claim.

## Purchase

**Path**: Documents > Order > Contract calculation > Calculation > Functions menu > Add purchases required

[Image: Fig. C-372 Adding a purchase dialog, showing a list of invoices with a field to enter the value of a purchase.]

Use this dialog to enter the amount spent on additional purchases, e. g. for fitting material. The amount is added to the selected project.
This function is only available if the mode Invoicing of allocated orders has been enabled.

- **Invoice no.**: Number of the invoice to which this purchase amount will be added.
- **Value**: Amount of this purchase.

## Claims Calculation

**Path**: Documents > Order > Project invoicing > Invoicing > Functions menu > Create claims invoice

This dialog is displayed differently depending on the activated project management:

- "Invoice management and allocated orders" on page C-699
- "Invoice management" on page C-700

### Invoice management and allocated orders

[Image: Fig. C-373 Invoicing with allocated orders – claims invoice dialog, showing a list of items with their total values and the quantity or amount to be calculated for the claim.]

This dialog shows the amounts that are already covered by claims invoices. You can issue additional invoices for the remaining amounts by entering the required value in the column Qantity to be calc.

For the defined value, a document of the type Claim will be issued which can be accessed and edited in document management for orders. The number of the new document can be displayed in the history of claims.
⇨ "History of Claims" on page C-701

This tab is also shown if Standard project management + Extended project management has been activated.

### Invoice management

[Image: Fig. C-374 Invoice management – claims invoice dialog, with options to create a claim by selection, date, or without an order, and fields for turnover and purchasing values.]

Use this dialog to enter claims that have been incurred for an invoicing project. The dialog is enabled for individual customers only.
