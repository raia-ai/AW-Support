---
title: "EN-UM-AWBusiness_11"
source: "EN-UM-AWBusiness_11.pdf"
tags: ["A+W Business", "Software Reference", "Master Data", "Company Configuration", "ERP", "Financial Accounting", "Purchasing", "EDI", "Capacity Planning", "Document Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the 'Company' module within the A+W Business ERP system. It details the configuration of master data, including company details, financial settings, document management, pricing rules, and system parameters."
long_description: "This comprehensive software reference manual provides detailed instructions for configuring the 'Company' master data in the A+W Business software. It serves as a guide for system administrators and power users to set up core company-wide parameters. The document is structured around the various sub-menus and tabs within the 'Company' module, such as 'Company Data,' 'Employee,' 'Banks,' and 'Subsidiaries.' Each section, like 'Company Data,' is further broken down into tabs including Client, Tax, Financial Accounting, Documents, Parameters, Price Calculation, Stock/Purchasing/EDI, Archives, and more. For each tab, the manual presents a user interface screenshot followed by a detailed explanation of every field and option. This includes settings for currency, tax calculation (including Avalara WebService integration), financial accounting interfaces, document output formats, pricing logic, inventory management, and production transfer settings. The guide is essential for ensuring the A+W Business system is correctly configured to match the company's specific operational and financial workflows."
---

# Company

*Master Data > Company*

This part of the program serves to enter data concerning your company.

Menu Company offers the following entries:
- "Company Data" on page B-942
- "Portuguese Certification" on page B-1030
- "Employee" on page B-1031
- "Employee Groups" on page B-1036
- "Employee Rights" on page B-1037
- "Copy rights" on page B-1039
- "Status Management per Employee (Group)" on page B-1040
- "Order Areas" on page B-1040
- "Field Services" on page B-1041
- "Commission” on page B-1043
- "Sales Representatives - Copy Commission Rates" on page B-1045
- "Banks" on page B-1045
- "Subsidiaries" on page B-1047
- "Booking Periods" on page B-1048
- "Surcharge Product Assignment" on page B-1049
- "Formulas" on page B-1051
- "Interface service" on page B-1051
- "Customizing" on page B-1061
- "Data Container" on page B-1062

---
## Company Data

*Master Data > Company > Company Data*

Enter the basic settings to be adopted as defaults for document entry.

When you open the dialog Company data, tab Client appears.

Module Clients can be used to define several clients. If you are using several clients you can select the required client from tab Table. The following tabs have to be edited for every individual client.

On each tab, the navigation buttons keys can be used to scroll through the client list to view the corresponding data.

Dialog Company data offers the following tabs:
- Company Data - Client
- Company Data > Tax
- Company Data > Financial Accounting
- Company Data > Documents
- Company Data – Parameters
- Company Data > Price Calculation
- Company Data – Stock/Purchasing/EDI
- Company Data > Archives
- Company Data – Daily Closing
- Company Data > System
- Company Data > Calculation
- Company Data - Print
- Company Data – Production
- Company Data – Shipment
- Company Data - Capacity Planning
- Company Data - Miscellaneous

## Company Data - Client

*Master Data > Company > Company > Client tab*

Enter the clients for your company plus their addresses and communication data.
⇨ Tutorial 1, "Financial accounting (FinAcc)" on page B-440
⇨ Tutorial 1, "Management of Employees" on page B-453

### Address

**Number** Client number. Can be chosen at random.

**Sender's company number** Company number of the client. It is used e.g. for group statistics and for importing and exporting purchase orders and orders.

**Matchcode** Matchcode for the client (mandatory field)

**Name, Street, Country/Zip/Town, Province** Address as shown in the commercial register.

### Contact

**Phone 1-4, Fax** Communication numbers.

**Email** Enter the email address from where messages received should be passed on to the individual contacts.

### General settings for email dispatch

**Server** Name of the server controlling the dispatch of emails.

**Port** Number of the port for email dispatch.

**Sender's address, Recipient's address, cc:** Email addresses to be used by default.

**E-mail** Sends a test mail for checking the settings.

**Authentication** An authentication can be used for data transfer.
- The transmission confirmation will not be sent without authentication.
- The transmission confirmation requires authentication. The fields for entering the registration data are accessible.

**Use SSL encryption** Secure Sockets Layer (SSL); encryption program for safe data transfer in the Internet.
- The transmission confirmation will not be encoded.
- The transmission confirmation will be encoded acc. to the SSL log.

**User, Password** Registration data the sender uses for authentication.

## Company Data > Tax

*Master Data > Company > Company > Tax tab*

This tab is used to enter the data for your inland revenue and define the currency.

### Revenue office / Tax

**Name, Street, ZIP/Town** Address of the inland revenue.

**Bank code, Acct. no.** Bank code and account number you are using for your tax payments.

**Tax number, Subsidiary number** Your tax and registration number.

**VAT ID** Tax number for the turnover tax payments.

### Currency settings

Choose the standard currency for document entry.
⇨ Tutorial 2, "Currencies" on page B-530
⇨ "Currency" on page B-932
⇨ "Company Data > Price Calculation" on page B-970

> **Working with three currencies**
> If you are working with three different currencies, you have to define whether the currency defined in master data should be taken into account.
> ⇨ "Obey currency in price master data" on page B-976

**National currency** Your national currency. This detail refers to the setting in section Currency displayed at order entry.
⇨ "Show currency at order entry" on page B-945

**Euro rate** Official Euro exchange rate referring to your national currency. If the national currency is Euro, enter 1.

### Default currency

Choose an option to define the currency in which the documents are entered:
- **No currency:** This setting allows to enter orders only in your national currency, i.e. you will not be able to switch from national to foreign currency at document entry.
- **National currency:** With this setting, you can enter orders in national currency, switching to foreign currency if required. Pricing will be based on the price lists in national currency and on the defined exchange rates.
⇨ Sales, "Header data - terms" on page C-1554
- **Foreign currency:** With this setting, you can enter order in foreign currency, switching to national currency if required. Pricing is based on the price lists in foreign currency. No exchange rates will be defined.

> **No exchange rates for prices in foreign currency**
> If the prices are entered in foreign currency, exchange rates must not be kept.
> Prices will be automatically converted into Euro by default. If an exchange rate was defined, prices would be converted twice.

### Show currency at order entry

Choose an option to define the currency to be displayed in document management:
- **None:** With this setting, order entry automatically uses the currency set in field National currency. If the Euro is not your country's national currency please choose the option None.
- **Euro:** Choose this setting if your country's currency has not been converted to Euro but price lists have been entered in Euro. If you have defined your national currency in field National currency you can enter the prices in Euro in the order, and display them in your national currency, e.g. SFR.
- **Old currency:** If the conversion to Euro has been completed, select Euro in field National currency and enable the option Old currency. Select your former national currency as well.

### Access Data VAT Calculation Avalara WebService

A+W Business can transfer all relevant information for a document to the Avalara WebService and receives the tax rates, the tax basis amounts, and the tax calculated in return. The transfer of the data to the Avalara tax service is done on the item level. This way, it is possible in states such as Florida to perform a tax calculation with a tax base rate per article of maximum $5000.

For the correct tax accounting, so-called tax codes must be entered for each product group.
⇨ "PGR" on page B-644

You specify how the system should log into the Avalara Webservice. With the selection of the option, the corresponding input fields are activated:
- User name/password
- Account number/license key

**Tax (0=no total)** Select the tax code from the combo box. A+W Business can process up to five Avalara taxes. For tax codes greater than 0, the Avalara tax is totaled up and one tax amount determined. By default, the tax code is 0, which means that up to five taxes are entered individually into the documents.

> **Setting up transfer**
> The call of the Avalara WebService is done via a customizing for the tax accounting. For this, a formula must be assigned in the customizing management to the program point 52-Tax accounting. Contact your planner at A+W Software GmbH if you want to use this function.

## Company Data > Financial Accounting

*Master Data > Company > Company > Financial Accounting tab*

State the financial accounting program you are using.
The details depend on the corresponding financial accounting program. The necessary data are entered by A+W Software GmbH when the system is installed.

When you select an interface, the following information are displayed for configuring the interface:
- Valid document types, e.g. order, credit note, P.O.
- Number and name of the interface file for documents and customer master data.
- Number and name of the interface file for receivables import.
- Necessary external codes, e.g. tax, payment terms, currency.
- Other necessary settings, e.g. booking area, FinAcc client.
⇨ Tutorial 1, "Financial accounting (FinAcc)" on page B-440

### Financial Accounting

**Export** The selected interface exports invoices and master data.

**Import** Receivables are imported via the selected interface.
⇨ Tutorial 1, "Credit Limit Analysis" on page B-156

**Account / external key** Number of the account or external key used to identify the data.

**FinAcc client** Financial accounting number of the client for whom this settings are made.

**Booking range** If you have defined company codes for your clients in your FinAcc program, you can maintain the accounting of the individual clients separately. You need to define the corresponding booking areas in A+W Business for this purpose.
If you are working with different bookings areas, please enter the valid area for this client.

### Path and file name

The settings in this area are made at installation and usually require no changes.

**Export documents** Path and name of the file to which the transaction data are exported. Please note the example with regard to the spelling.

**Export market partners** Path and name of the file to which the customer and supplier master data are exported. Please note the example with regard to the spelling.

**Batch file** Path and name of the batch file to be started after the transfer. An error report will be issued if you enter a file that cannot be executed.

**Import receivables report** Path and name of the receivables file to be processed by the batch file.

### Options

The entries in this section depend on the financial accounting program A+W Business communicates with by means of this interface. The necessary data are entered by A+W Software GmbH when the system is installed.

**Create standard output** The export file for financial accounting is created depending on the interface. Apart from that, you can create the standard output.
- Only the export file for financial accounting will be created.
- Apart from the export file for financial accounting, the system creates a file in AWStandard2 format.

**Cost accounting active** Cost accounting records can be created for the transfer. This works only if the financial accounting program can handle cost accounting.
Apart from cost and surcharge calculation in A+W Business, you can write cost accounting records for your financial accounting system based on which you can check and revise your calculations.
- No cost accounting records will be written.
- Special cost accounting records will be created if your financial accounting program can handle cost accounting.
⇨ Tutorial 2, "Cost and surcharge calculation" on page B-613

**Update receivables balance after transfer** The customer's credit limit can be displayed at order entry. To update the receivables, unsettled accounts have to be reported and updated in A+W Business.
- Transferring an invoice to financial accounting will not update the customer's account.
- The customer's account will be increased when the invoice is transferred to financial accounting.

**Single receivables report** A customer's receivables can be reported individually, or accumulated.
- By default, receivables are reported accumulated.
- Receivables are reported by invoice.

**Proceeds accounts per product** The proceeds accounts can be set up and booked for products and PGR.
- ☐ Proceeds accounts are only booked for PGR.
- Proceeds accounts can be booked for products and PGR.
⇨ "Proceeds Accounts" on page B-934

> **Requirements**
> For the following three functions, one of the clients has to be marked as the main financial accounting client. The function must also be enabled for all clients.

**Create/update customer also in FinAcc main client** Only for Syska financial accounting system. If customers of a client are transferred to financial accounting, you can define whether these customers should be entered as customers of the main client.
- The customers of the current client will not be entered as customers of the main client in financial accounting.
- The customers of a client who is not the main FinAcc client, will be created or updated as customers of the client who is the main FinAcc client.

**Read and write files in Unicode format** This setting depends on the system used to exchange data.
- The files will be read and written in the code in which they were created.
- ☑ The files are read and written in Unicode.

**Compare new customer number with FinAcc** Only for Syska financial accounting system. When new customer data are entered, the program can check whether the chosen customer number already exists in the financial accounting system.
- The new customer number will not be checked.
- ☑ When comparing master data in Syska financial accounting, the program checks if the number of the new customer already exists. If so, an error report will be issued. You will have to enter another customer number for this customer in this case.

**FinAcc main client** Only for Syska financial accounting system. If you are using several clients, one of them must be presented to the financial accounting system as the main client.
- The client whose settings are currently edited is not the main client for financial accounting.
- ☑ The current client is the main client for financial accounting.

**Transfer cust. account instead of cust. no.** The customer number will be used as an account number by default. Instead of the customer number, the debtor number can be entered in customer master data.
- The customer number is transferred to financial accounting.
- ☑ The account number is transferred to financial accounting. This account number must be entered in customer data. This setting will overrule the settings in customer master data.
⇨ "Main acct." on page B-825

**Enter credit limit in net and convert to gross** With this option, it is possible to enter the credit limits per customer in net or gross.
- The credit limits are entered gross including taxes.
- ☑ The existing amounts are converted to net amounts with the tax rate assigned to the customer. Right now, the credit limits can be entered net and converted immediately to the gross amount. All checks associated with this are still conducted with the gross amounts.

### FinAcc database

You have to fill in these fields only if you are using SQL financial accounting that allow direct exporting.

**Server** Name of the server containing the financial accounting database.

**Database name** Name of the financial accounting database.

**Login** User name by which A+W Business registers with the financial accounting database.

**Password** Password by which A+W Business registers with the financial accounting database.

### Options for open items-report

**Create backup file, path** This field is accessible only in connection with the import of receivables reports. You can save an additional backup file and enter the number of days for which it is going to be saved.
- ☐ No backup file will be saved for the receivables report.
- ☑ A backup file of the receivables reports (including a time stamp) will be saved elsewhere. The fields for selecting the directory and the storage days are made available.

**Storing days for backup files** This field is available only if a backup file is going to be saved. You can enter the number of days for which this file must remain unchanged.

## Company Data > Documents

*Master Data > Company > Company data > Documents tab*

This tab is used for defining options for document output.

### Choose shape catalog

**Shape catalog** A+W Business uses the A+W Software GmbH shape catalog by default. You can choose different catalog for your clients.
⇨ Sales, "Shapes" on page C-1189

### Lock code

Lock codes are used to exclude documents from certain steps of automatic processing.
⇨ Tutorial 2, "Lock code" on page B-499

> **Prerequisite**
> Lock codes must be defined in dialog Lock codes so that they can be selected in the appropriate fields.
> ⇨ "Lock Code" on page B-923

**Complaint** Lock code for complaints. This can be changed in the individual documents.

**Partial delivery** Lock code for partial deliveries. This can be changed in the individual documents.

> **Activate setting for customer**
> If a customer should be able to get a partial delivery without partial invoice, define this in customer master data using the checkboxes Partial delivery and Partial invoice.
> ⇨ "Partner Management - Order" on page B-813

### Fax/Email - Options

> **Prerequisite**
> A fax number and email address have to be entered in partner management, and fax and email despatch have to be enabled.
> ⇨ "Partner Management - Order" on page B-813

**Fax dispatch per document** Documents can be faxed.
- ☐ The documents are collected and faxed to the partner.
- ☑ Documents are dispatched individually by default. You should maintain this setting to avoid bottlenecks.

**Email dispatch per document** Documents can be emailed in various formats.
- ☐ The documents are collected and emailed to the partner.
- ☑ Documents are emailed individually to the partner. You should maintain this standard setting to avoid bottlenecks.
Please remember that RTF dispatch will not display shapes and other graphics correctly.
For PDF dispatch, the documents will appear in individual PDF files attached to a mail. This way, you get a better overview of the attachment documents, you can rename these if necessary, and it is easier to handle the documents.

### Compulsory shape dimensioning

> **Avoiding calculation errors**
> To avoid pricing errors, you should enable Compulsory shape dimensioning for all documents if edgework by linear meter is also active on tab Parameters.
> ⇨ "Calculate edgework with exact Im" on page B-958

**Quotation, Order, P.O.** Usually, sizes are entered in the documents. Input of sizes should be compulsory for orders and purchase orders while they may be omitted from quotations.
- ☐ You do not need to enter shape sizes in documents. The sizes are checked when copying from Quotation to Order, the system will ask you to enter sizes if necessary.
- ☑ Sizes have to be entered in documents (quotation, order, P.O.). For Order and P.O. the checkboxes should remain enabled by default (necessary for production).

### Mixed calculation factors

If you are using mixed calculation, you can enter factors for price calculation.
⇨ Tutorial 2, "Mixed calculation" on page B-607
⇨ "Items - supplement" on page C-1623

**Double IG** The factors for double IG can be chosen at random, e.g. 0.5/0.5.

**Triple IG** The factors for triple IG can be chosen at random, e.g. 0.5 / 0.8. / 0.5.

### Allocate numbers per page

**Delivery note printing, Invoice printing** Certain countries require that every page of a delivery note or invoice gets its own number.
- ☐ By default, delivery notes and invoices will be numbered by document.
- ☑ Every page of the delivery note or invoice will get its own number.

### Credit note/invoice number

Separate number ranges will be set up per document type.

**Credit note number = document number** By default, credit notes are independent documents with a separate number range.
- ☐ Numbers from the invoice number range will be used for credit notes.
- ☑ Numbers from the credit note number range will be used for credit notes.
⇨ Tutorial 2, "Definition of number ranges" on page B-511
⇨ "Number Ranges" on page B-918

### Change of delivery date

You can prescribe a mandatory reason for a change of delivery date for orders (also internal orders). The specification of a reason will be required in the following cases:
- Order entry if order will not be entered anew
- Document Data
- Route list
- Consignment

In the manual note of the order history, the old and new delivery dates and the reason entered are visible. If more than one order is changed, the dialog appears per changed order. However, it is filled with the value previously entered and can be taken over with the same reason.

If the order is shifted by the production system during scheduling, the entry is made automatically with the reason Delivery date calculation with A+W Production. If the delivery date shift is made due to a rescheduling in the production system, the comment entered there is used as text.

**Entry in history with comment starting with status** For a manual change of the delivery date, the specification of a reason can be made mandatory.
- ☐ The change of the delivery date does not have to be justified in the history.
- ☑ In the history, an entry is created if the delivery date was changed starting with the set status. The entry of the reason is mandatory and cannot be canceled. The setting applies for the following program areas: Order transfer, Document data, OC supplier, Receipt of goods, and in the Picking.
The field for selecting the status is activated.
- ☐ for POs: For a delivery date shift, the entry of a reason in a PO is not required.
- ☑ for POs: For a delivery date shift, the entry of a reason also in a PO is required.

### Turning shapes

**Shapes can be turned on processing dialog** Shapes with shape numbers smaller than 137 can be turned on the processing dialog. Excluded here are the shape numbers 0, 24, 98, 99, 60, 61, and 81.
- ☐ The shapes cannot be turned.
- ☑ The shapes can be turned: here, the available angles are 90, 180, and 270 degrees. The printout reflects the turned shape.

### Glass door system data source

The field refers to the module AWDoor.

**ODBC DSN** Enter the name of the database connection configured in Windows.

### Price below minimum

**Password** Enter a password to avoid that minimum prices are not inadvertently. The system will automatically ask for this password if the defined minimum price is not met at order entry.
By passing on this password you can control how many users should be entitled to negotiate individual prices.

### Project management

**Active project management** Different settings are available for using the project management functions.
- None
- Invoice management (customized setting)
- Invoice management with allocated orders
- Extended project management
- Standard project management
- Standard project management + invoice management with allocated orders

The differences between the settings are described in detail in the tutorial.
⇨ Tutorial 1, "Projects" on page B-185
⇨ Tutorial 2, "Project/invoice management" on page B-568

### Product ID

You can set the appropriate modes for CEKAL classification or quality text. Prerequisite is a valid licence for the corresponding method. If product identification is inactive, the user will be informed accordingly when selecting the dialog in question.

**Active marking** Product code:
- **None:** With this setting, the product code will not be checked.
- **CEKAL classification:** With this option, the spacer text will be set acc. to CEKAL classification.
- **Quality code:** With this option, the restrictions from dialog Quality text will be taken into account.
⇨ "Quality Text" on page B-660

### File attachments

Files can be attached in partner and document management.

**Path** Enter the path for saving file attachments. In this directory, a sub-directory will be created by customer or order to save the annexes in.
Please make sure that this directory is available on a central computer, accessible to the users.

### Declaration of Performance

**Sending of declarations of performance** You can specify whether declarations of performance should be sent.
- ☐ No declarations of performance will be dispatched.
- ☑ Declarations of performance are dispatched for the allocated partners and products. The field for selecting the standard declaration of performance is released.

**Standard Declaration of Performance** You can define a declaration of performance (DoP) to be dispatched by default if no specific DoP is allocated in the order.

**[Directory]** Opens the dialog Declaration of performance management where you can enter the declaration of performance (DoP).
⇨ "Declaration of Performance, Management" on page B-661

**[Zoom]** Opens the dialog Search declaration of performance from which you can select the standard declaration of performance.

**Size restriction for email dispatch ... MB** For the sending of declarations of performance, you can specify an upper limit in MB. For documents that exceed this value, the e-mail is split in several parts.

**Use A+W SLT interface** For data transmission in the B2B module, A+W's own interface can be installed.
- ☐ The A+W SLT interface is not used.
- ☑ The A+W SLT interface is used. With this setting you can specify where the interface file is stored if a different installation path was used.

**Different installation path** Specification whether a different installation path was used for the A+WSLT.exe interface file.
The field is only enabled if the A+W SLT interface is activated.
- ☐ The interface file is installed in the standard installation path.
- ☑ The interface file is installed in a different installation path. For this, you must specify the path.

**(Path)** Specification of the installation directory for the interface file A+WSLT.exe.

**Fill product description 3** Controls the text replacement of the name 3 for IGU from the technical values of the BPV2. Prerequisite for this is a license for the BPV2.
- ☐ The product name 3 is not filled with the technical values from the BPV2.
- ☑ The product name 3 is filled with the technical values from the BPV2.

### CEKAL parameters

These settings are only used in France.

**Default text** These fields refer to the CEKAL module.
There are two ways of allocating a general standard CEKAL text:
- Enter the standard text at this point. This text will appear automatically whenever you enter an item.
- Or leave the fields in dialog Text allocation blank and allocate the standard text. This text will appear only if no other CEKAL definition is found.
⇨ "CEKAL" on page B-1091

**Center no.** Company number in connection with CEKAL certification. This number can differ from the company number on tab Client.

## Company Data – Parameters

*Master Data > Company > Company Data > Parameters tab*

This tab is used for defining the options for the documents. Amendments on this tab will overrule the standard calculation in A+W Business.

### Parameters for document entry

**Calculate edgework with exact Im** Depending on the national customs, edgework can be rounded by default.
- ☐ Edgework will be calculated with linear meters rounded.
- ☑ Edgework calculation is based on the exact sizes.
⇨ "Rounding" on page B-910
⇨ "Compulsory shape dimensioning" on page B-953

**Logo entry** To print a logo you have to define the logo position for shapes and rectangular lites in master data, for every customer.
- ☐ The logo will be added to the BOM by default.
- ☑ The logo is automatically printed on the (toughened) lite. This setting can be changed by customer.
⇨ "Logo Position" on page B-877

**Actual product groups for BOM search** The logo can be entered in master data for a main product or for the product group. For items with a bill of material, the automatic search for a logo can be started from the main product or from the product group.
This checkbox is accessible only if logo entry is active.
- ☐ By default, the program will search for the logo based on the main product.
- ☑ For elements on the first BOM level, the program searches for the logo by means of the BOM element's product group.
With this setting, the program will search e.g. for the logo of a laminated lite irrespective if it is entered as a main item or if it is exchanged in the IG's BOM.

**Do not delete partial delivery item** Orders can be executed as partial deliveries, with or without partial invoicing. This setting can also be made by customer.
- ☐ By default, the items of a partial delivery will be deleted from the original order after the item has been completely shipped.
- ☑ If partial delivery is combined with partial invoicing, the shipped items will not be deleted from the original order. Completely shipped items will be set to 0.
⇨ "Partner Management - Order" on page B-813

**Adopt partial delivery date from original order** For partial deliveries, the order date can be updated in the delivery note.
- ☐ By default, today's date is entered as entry date of the partial delivery for each creation of a partial delivery.
- ☑ The entry date of the original order will be used for the partial delivery.

**Raise status when credit limit is exceeded** The customer's credit limit is checked when the order is saved at order entry.
If the credit limit is exceeded at order entry, the following actions can be released:
- The system issues a message but the order can be entered completely.
- The order cannot be entered.
These settings are made in every customer's master data.
⇨ "Credit limit" on page B-826
If the credit limit is exceeded at order entry, the system will automatically set the order status to 700 Credit limit exceeded.
These orders can be selected via number manager. After that, you have to decide if the order can be released for production, or remains locked for further processing.
⇨ Tutorial 1, "Credit Limit for Customers" on page B-152

> **Assign user status**
> There has to be an appropriate user status for status point 700; this is allocated in dialog Status allocation. If an order has been automatically set to status 700, and you reset the status manually, the system will not automatically raise it again.
> ⇨ Tutorial 2, "Status administration" on page B-492
> ⇨ "Status Allocation" on page B-915

**Enable deviating procurement type per client/order area** If you are working with clients, the procurement type of the product can be set per client.
- ☐ The procurement type is set across the board for all clients.
- ☑ The procurement type can be set per client. For this, in the product master data, the deviating product code per product and client must be specified.
> **Example**
> The company has the production scheduling TSG and IGU. The IGU production scheduling IGU orders a TSG for the production scheduling TSG, e.g. a 6 mm TSG.
> This product 6 mm TSG has the procurement type Production in the production scheduling TSG and the procurement type Purchase order in the production scheduling IGU.
⇨ "Product codes" on page B-685

**Enable search by product code** Procurement types are allocated to products in product management. You can also allocate other procurement types by client and order area in dialogue Product code management.
- ☐ You should disable this checkbox if you do not use different procurement types for the same product. This will help to relieve the system.
- ☑ The program checks if different procurement types are allocated to the same product. Depending on the order area, the product will be produced or ordered.
⇨ "Product Management - Stock/Purchase" on page B-683
⇨ "Product Code Management" on page B-704

**Interactive sales commission** By default, the sales commission is calculated when documents are transferred to archives. Checkbox Transfer to commission statistics must be active on tab Archives for this purpose.
The sales commission can be entered or changed by item at order entry.
- ☐ The commission rate will not be displayed at order entry. At transfer to commission statistics, the commission rates defined in master data will be used to calculate the commission.
- ☑ The commission rate will be displayed at order entry. To calculate the commission, you still have to transfer the orders to commission statistics via dialog Transfer to archives.
⇨ "Automatic options" on page B-992
⇨ "Commission" on page B-1043
⇨ Sales, "Transfer to archives" on page C-1779

**Save manual changes in reference document** If the supplier's price is changed in a reference P.O., it can be saved in the order.
- ☐ Changed entries will not be saved in the reference document by default.
- ☑ The changed entries should be adopted for the reference document:

**Referencing document** Specification of how the changed values should be taken over.
- **Yes, No:** The changed value is only saved if the additional query displayed has been confirmed with [Yes].
- **Always:** The changed entry is saved always, without checking.
- **Never:** The changed entry will not be saved. No question will be displayed.

**BOM transmission of variants** If a BOM element is replaced by a variant on top or medium BOM level, the variants of the related elements can be replaced automatically.
- ☐ Changes made to a BOM element will not be passed on to the sub-elements.
- ☑ If e.g. the color of a product containing BOM elements is changed at item entry, the color of all sub-elements will change automatically.
⇨ "Product Variants" on page B-710

**Enter rectangular cut-outs as width x height** The marking of corner cut-outs can be reversed.
- ☐ Sizes are entered sequentially after the pattern A-B-A-B.
- ☑ Edge cut-outs are entered according to the standard pattern, i. e. A always represents the width and B, the height.

**Check number ranges in orders** You can enter the order area in existing orders.
- ☐ The order area can be changed no matter whether a number range exists for the (new) order area.
- ☑ The order area can be changed only if there is a number area for the (new) order area. The document number remains unchanged.

**Exchange spacer with BOM (gas)** The airspace can be entered as a product with the BOM element gas. You can define what should happen when the airspace is changed.
- ☐ The gas will not be changed automatically if the airspace changes. It does not matter whether or not the gas is allocated to the airspace.
- ☑ When you change the airspace, the BOM element gas will be changed too. This setting is useful if you have defined airspaces with gas.

**Lock documents after printing the invoice** An order can be edited until the lock status Document changed has been reached.
- ☐ By default, the order is locked against changes by means of the lock status. This status can be reset.
- ☑ After printing the invoice, the order is locked and cannot be edited. The lock refers to the invoice number created at printing. It cannot be undone.
⇨ Tutorial 2, "Lock status" on page B-497
⇨ "Status Allocation" on page B-915

**Lock documents starting from status point** A document can be locked for editing after it has reached a defined status.
- ☑ The document will be locked completely from the defined status on. Items cannot be edited either.

**Automatic scheduling** Automatic scheduling does not pass on orders to capacity planning or production.

> **Automatic scheduling vs. capacity planning**
> You must not enable this function when working with A+W Business Capacity Planner.

- ☐ Orders will not be passed on to automatic scheduling by default.
- ☑ Orders are automatically passed on to automatic scheduling (in the background).

**Tax calculation on item/BOM level** The tax is usually calculated when the order is saved and the dialog closed.
- ☐ The tax is calculated for the entire order value.
- ☑ The tax is calculated on BOM level, for every BOM element. This calculation type is quite tedious and should be enabled only if legislation requires.

**Create product description from BOM** In product definition, you have to enter a name for the product in field Name 1. This name can be created automatically for IG and laminated glass products with bills of materials.
- ☐ The name of the main product will be kept as a standard.
- ☑ Name 1 for the main product consists of the names of the individual BOM elements.

**Duplicate check if credit limit exceeded** The system automatically checks when a document is entered or edited whether another document exists that includes the same product, product structure, and sizes.
- ☐ The duplicate check is not performed if the credit limit is exceeded.
- ☑ When exceeding the customer credit limit, a duplicate check is performed and the status adjusted if necessary.

**No copy of quotations after orders if credit limit exceeded** Orders can be generated from quotations for locked customers with the copy function.
- ☐ For customers with credit limit lock, orders can be generated from quotations nevertheless. For the new order, the corresponding status is set, Locked credit limit.
- ☑ For customers, no orders can be generated from quotations if the credit limit is exceeded and the customer is therefore locked. When starting the copy process, an appropriate message is output.
With this setting, orders via quick entry are also possible.

**Copy of order in credit note for locked customer** Customers can be locked via the customer master data so that no documents for them can be entered.
- ☐ For locked customers, quotations can only be copied if the lock is lifted in the customer master data.
- ☑ Quotations can be copied for locked customers without lifting the lock in the customer master data. When entering the customer number, a warning message is displayed.

**Quotation entry for locked customers** Customers can be locked via the customer master data so that no documents for them can be entered.
- ☐ For locked customers, quotations can only be entered if the lock is lifted in the customer master data.
- ☑ Quotations can be entered for locked customers without lifting the lock in the customer master data. When entering the customer number, a warning message is displayed. No order can be generated from a quotation that was entered despite the lock as long as the customer is locked.

**Copy from order to credit note for blocked customers** Customers can be locked via the customer master data so that no documents for them can be entered.
- ☐ For locked customers, orders can only be copied to credit notes if the lock is lifted in the customer master data.
- ☑ Orders can be copied to credit notes for locked customers without lifting the lock in the customer master data. When entering the customer number, a warning message is displayed.

**Enter credit notes for locked customers** Customers can be locked via the customer master data so that no documents for them can be entered.
- ☐ For locked customers, credit notes can only be entered if the lock is lifted in the customer master data.
- ☑ Credit notes can be entered for locked customers without lifting the lock in the customer master data. When entering the customer number, a warning message is displayed.

**Maintain production BOM structure in case of changes** In case of a change, you can adopt the BOM structure of a glass if the new glass has no a BOM with production BOM structure.
- ☐ The exchanged (new) product will be adopted including its production BOM structure.
- ☑ If the new glass has no BOM, the BOM structure of the original production BOM will be kept.
⇨ Tutorial 1, "Price- and/or Production-Relevant" on page B-244

**No shipping/delivery on weekends** You can define the calculation type for dates. You also have to enter the corresponding lead days.
- ☐ Weekends will not be considered as dates for possible shipments and deliveries. Goods will not be shipped or accepted on weekends.
- ☑ Goods can be shipped and accepted on weekends.
⇨ "Lead days" on page B-999

**Due date calculation for February (28 or 29 days)** With this option, the due date is calculated in more detail. An invoice from 30.01.20xx, with a payment term of 30 and a payment day on the 30th now has the due date calculated as the 23.02.20xx. Without this option, the 30.03.20xx would be calculated since February only has 28 days.
- ☐ The due date is not calculated in more detail.
- ☑ The due date is calculated in more detail.

**Use virtual item numbers** Receipt of boxes with an item quantity of >1 has to be booked for each box separately. Virtual item numbers are defined for every box for this purpose.
- ☐ Virtual item numbers will not be used.
- ☑ Upon receipt, every box gets a virtual item number so that it can be registered and booked with its own ID.
⇨ Box Management, "Stock management of boxes" on page K-3044

**Change procurement type if maximum stocksize is exceeded** The procurement type of products can be automatically changed to P.O. if the maximum stock size is exceeded at order entry.
- ☐ The procurement type will not be changed automatically if the maximum stocksize is exceeded in the order.
- ☑ The procurement type will be changed automatically if the maximum stocksize is exceeded in the order.

**Always adopt product text from BOM** Product management allows to enter product text to be displayed in field Article info.
- ☐ Only the main product text will be displayed as article info.
- ☑ The text for the BOM elements will be displayed as well.

**Adopt P.O. text 1 and customer item for document references** Document references can be created on item level for electronic data interchange. These are necessary for automatically referring order items to the corresponding P.O. items.
- ☐ References will not be created on item level.
- ☑ When an order is entered by hand, document references are automatically created from the Purchase order 1 field in the order header, and the customer item field at item entry.

**Laminated glass production BOM breakdown based on the procurement type** Laminated glass can be produced or cut. Based on the procurement type, individual lites or the entire laminated unit has to be processed.
- ☐ The production BOM will always be broken down.
- ☑ If the procurement type is Cutting, the production BOM will not be broken down for the processing steps.

**Determine tax, salesman, and VAT ID based on the shipping address**
You can define whether the shipping address determines the VAT ID.
- ☐ The shipping address is determined based on the main customer's data.
- ☑ The shipping address is chosen based on the VAT ID. For printing collective invoices this means that a new collective invoice will be started when the VAT ID changes. For printing collective invoices, invoices have to be sorted by shipping address.

**Print code in case of exchange** The print code for BOM elements can be controlled in general.
- **Standard:** The print code is kept as defined for the main product.
- **Always active:** The print code is enabled with every exchange.
- **Acc. to exchange product:** The print code will be set as defined for the basic product of the exchange article.

> **Example**
> The print code can be disabled for toughened glass arrissing in the BOM because this processing step is done by default. If this processing step is replaced by the processing step Polishing, the changed processing should be printed on the forms however.

**Order-related purchase orders can be changed** Changes in reference purchase orders can refer to the shipping and production dates as well as to the quantities ordered.
- ☐ Reference purchase orders cannot be changed.
- ☑ Reference purchase orders can be changed. The changes will be saved in the order.

**Outside coating/pattern facing away from airspace/film as from 2nd lite**
You have to define the way in which coated and patterned lites are to be fitted into multiple IG or multiple laminated glass lites. You can define a default for this which can be changed in the order if required.
- ☐ The lites will be fitted as defined in glass master data. When exchanged in an IG or laminated glass unit, the coated or patterned side will be turned from the second lite on, to face the airspace or the film layer.
- ☑ If the coating or the pattern has been defined as outside in master data, the program must check in case of an exchange whether these lites should be actually facing away from the airspace or the film layer.

**Enable Brazilian tax** This setting is only valid for Brazilian taxation.
- ☐ The tax will be calculated according to the settings in product master data.
- ☑ The tax will be calculated according to the tax matrix and to the formulas for Brazilian tax.

**Import/export of payments** This setting only applies to the Brazilian payments. This field is accessible only if Brazilian taxation is active.
- ☐ Import and export of payments to the bank is not enabled.
- ☑ Payments to banks are made by data transfer. The appropriate formulas have to be defined for this purpose.

**Enable Portuguese certification** For the Portuguese market, invoices and credit notes can get a digital signature that is certified acc. to certain parameters. This function can only be enabled by the system administrator.
- ☐ Portuguese certification is inactive.
- ☑ The [Parameter management] button is accessible.

**[Parameter management]** Opens the dialog Portuguese certification where you can set the parameters for the certification (signature). This button is accessible only if Portuguese certification is active.
⇨ "Portuguese Certification" on page B-1030

**Apply product exchange rules for BOM exchange** You can specify that in IGU and LSG, only glass, spacers, and foils can be installed that are intended and suitable for these products.
- ☐ No rules are specified for the product exchange in IGU and LSG.
- ☑ For the exchange of BOM elements, the rules are applied that are specified on the Exchange groups and Exchange allocations dialogs.
⇨ "Exchange Groups" on page B-662
⇨ "Exchange Allocations" on page B-662

**Edge processing on LAMI creates size allowance in order** Specification whether a size allowance is calculated if a LAMI with edge processing is ordered.
- ☐ The PO is forwarded unchanged.
- ☑ For the generation of the PO, there is a check whether an edge processing (block grinding) affects an ordered part within the block. If this is the case, the size allowances of the processing are added to the dimension of the glass ordered. Here it doesn't matter whether or not the processing is also ordered.

**Show only levels valid for processings** Specification of whether a dimension surcharge is calculated if an LSG with edge processing is ordered.
- ☐ The purchase order is forwarded unchanged.
- ☑ During the generation of the purchase order, it is checked whether an edge processing (block grinding) affects an ordered part within the block. If this is the case, the dimension surcharges for the processing are added to the dimensions of the glass ordered. Here it does not matter whether the processing is also ordered or not.

**"No layer" selectable** Specification of whether layers are shown for coatings if only valid layers for processings are shown.
- ☐ The setting for processing layers is not expanded.
- ☑ The setting for processings is expanded for coatings to include the selection No layer. This setting only makes sense if the display is restricted for processing layers.

**Delete inferior edge processing** Specification of whether for edge processings all processings should be executed if they differ only in the quality, e.g. seaming and polishing on the TG.
- ☐ All edge processings are executed as they are entered.
- ☑ Only the superior edge processing is executed. The inferior edge processing is ignored.
If an edge processing should therefore affect no edge, then the whole processing is deleted from the BOM.
In the import settings for customers, you can also activate the Delete inferior edge processing on the glass option for this.
⇨ "Customer, Supplier - Parameters" on page B-1114

**CRM document reference** Specification whether or not the field for entry of a CRM project number should be displayed.
- ☐ Field will be hidden.
- ☑ Field will be shown.
⇨ Sales: Software Reference, "CRM reference/project" on page C-1548

**A+W iQuote history only with exact status** Restriction to documents that have precisely the status that was enabled under Master Data > Order > Status Points. The status point is not checked, but rather the status that is assigned to this status point.
- ☐ In A+W iQuote, all documents of the customer are displayed and stati that are not enabled are shifted to the next smaller status that is enabled in the display.
- ☑ In A+W iQuote, only the documents are displayed that correspond to this status assignment.

## Company Data > Price Calculation

*Master Data > Company > Company Data > Price calc. tab*

This tab is used to adapt the pricing to your company's or country's requirements.
Amendments on this tab will overrule the standard calculation in A+W Business.
⇨ Tutorial 1, "Price Master Data" on page B-276
⇨ "Price Management" on page B-768

### Pricing parameters

**Price calculation for orders**
You can define different prices and discounts for the same product for a customer. Individual prices will always override discount agreements.
The standard rates will always be used if the program cannot find any discount agreement.

**Several individual prices permitted** You can enter customized prices in addition to standard prices.
- ☐ You can enter just one individual price per customer and product in price management. This will be automatically determined at document entry.
- ☑ You can enter several individual prices per customer. If you have entered several individual prices, the program first checks (in discounts) which rate has been defined as the standard price and if there is an individual price. If no individual price has been defined, the standard rate will be used for pricing.

> **Pricing with several individual prices**
> Prices will not be inserted automatically at document entry if several individual prices have been defined.
> You have to enter the required price key by hand. For this purpose, item entry offers a list of all prices defined for the customer.

**Calculation of supplier prices for purchased items** Purchase prices will be managed only if module Purchasing has been installed and released.
- ☐ The system will not show the supplier's individual prices.
- ☑ Individual prices will be displayed. The purchase price will be calculated right away at order entry.
This checkbox should be active for purchasing.

**No discount search for default records** Standard prices will always be used for pricing unless an individual price has been defined. Automatic pricing follows the hierarchy below (downward priority):
- Individual price
- Discounts
- Standard prices
- ☐ Prices including the defined discounts will be used for standard prices (default rates).
- ☑ The defined discount should not be taken into account. The following hierarchy applies in this case:
    - Total product price
    - sqm + individual item (French pricing)
    - Individual prices for IG and laminated glass

**PGR combination for discounts valid only if discount exists** The product group discounts will be used for pricing at order entry.
- ☐ If you have entered a product group combination for an IG unit with a grill for example, this will be used at item entry no matter if there is a discount rate for this price key or not.
- ☑ In this case, the product group combination will be used only if a discount rate has been entered for this price key.
⇨ Tutorial 1, "PGR Combination" on page B-205
⇨ Tutorial 1, "Combine Product Groups" on page B-214
⇨ "Combined PGR" on page B-647

**Create PGR combinations using complete BOM** If a product includes a BOM, the turnover of the BOM elements can be analyzed by means of product group combinations.
- ☐ With this settings, the product group combination valid for the corresponding product will be used.
- ☑ Irrespective of the combination rule for the next processing steps, all BOM elements will be booked to the last combination found for this item.
⇨ Tutorial 1, "Create PGR combinations with full BOM" on page B-209
⇨ Tutorial 1, "Combine Product Groups" on page B-214
⇨ "Combined PGR" on page B-647

**Search discounts for mixed IG calculation** If the price for IG is calculated by mixed calculation using different price lists, discount calculation can be permitted or forbidden.
- ☐ Discount search is switched off by default for IG mixed calculation.
- ☑ The system searches for discount rates for the corresponding IG price list.
⇨ Software Reference, "Mixed Price Calculation" on page B-756

**Search individual price for mixed IG calculation** If the price for IG units is calculated by means of different price lists, using mixed calculation, the search for customized prices can be permitted or forbidden.
- ☐ The search for individual prices is disabled by default for mixed IG calculation.
- ☑ The system will search in price management for individual prices for the corresponding combination of IG lites.
⇨ "Product Management - Price/Surcharge" on page B-678

**300 mm min. edge length for IG in PP and SP** This setting is valid for IG pricing in purchasing and sales.
- ☐ Pricing is based on the actual lite size.
- ☑ If the width and/or height of an IG unit lies below 300 mm, pricing will be based on a minimum edge length of 300 mm (sales and purchase price).

**IG + LG single price calculation** A+W Business offers three price calculation types:
- Total product price
- sqm + individual item (French pricing)
- Individual prices for IG and laminated glass
- ☐ The defined total price is used for pricing. The individual prices of the elements will not be taken into account.
- ☑ Pricing is controlled by product master data. The price for the main product is calculated for every single element, and then added up.

> **Elements have to be price-relevant**
> If this checkbox is checked, the codes Price-relevant SP and Price-relevant PP must be checked for the BOM elements in product management. If this code is inactive, the corresponding element will not be calculated.
> ⇨ "Product Management – BOM" on page B-691

**Calculate min. grill length per pattern** Minimum quantities can influence pricing. It is therefore necessary to define what the minimum bar length refers to.
- ☐ By default, the minimum length is calculated by bar.
- ☑ The minimum bar length is calculated by grid (total of all bars).
⇨ Tutorial 1, "Pricing Codes" on page B-232
⇨ "Surcharge Product Assignment" on page B-1049

**Calculate min. edge length per edge** Minimum quantities can influence pricing. It is therefore necessary to define what the minimum edge length refers to.
- ☐ By default, the total of all edge lengths is calculated as the minimum length for processing.
- ☑ The minimum processing length is calculated by edge.

**Commercial size rounding** Size roundings can be calculated in different ways.
- ☐ By default, sizes are rounded upwards.
- ☑ In case of commercial rounding, rounding goes four downwards and five upwards.
⇨ Tutorial 2, "Rounding" on page B-516
⇨ "Rounding" on page B-910

**Calculate foreign currency amount from unit price x quantity** This setting allows to control the calculation of foreign currency accounts on item level.
- ☐ The foreign currency amount for the item is calculated from the item price, in national currency. This is done multiplying the item price by the conversion factor.
- ☑ The amount in foreign currency for the item is the net unit price in foreign currency. This means that the individual prices are converted into foreign currency, then multiplied by the quantity.
⇨ Tutorial 1, "Price Tables" on page B-295
⇨ Tutorial 2, "Pricing in connection with foreign currency" on page B-531

**Use main item discount rather than processing discount 0%** Discounts can be applied to the main item as well as processing.
- ☐ If a separate discount of 0% is defined for processing, the discount for processing will not be adopted from the main item.
- ☑ If a separate discount of 0% is defined for processing, the discount from the main item will also be applied to processing.
This means that the appropriate entry has to be selected for processing in field Adopt from main item.
⇨ "Price parameters" on page B-678

**No fixed adoption of item discount in case of exchange surcharge** Discounts for replacement products can be considered as a separate discount, or replaced by the discount defined for the main item.
- ☐ If no other discount has been defined for exchanged glass in IG units, the discount for the main item will be adopted for the exchanged lites.
- ☑ The discount will not be applied to the replacement product. In this case, only the discount for the replacement product (if defined) will be taken into account.

**Recursive quantity calculation in BOM** This checkbox defines if the processing step should be calculated once for the entire product, or for every BOM element.
- ☐ By default, the processing will be calculated for the entire product. In this case, you have to enter the processing item and the required quantity at order entry, e.g. 12 x edgework for a CD stand with two side panels and four shelves. The edgework is defined per glass.
- ☑ For processing, the total net amount for a BOM element is calculated from the number of processing steps of all parent products.

> **Recalculation of orders**
> If this option is switched on later, orders with the corresponding constellation have to be recalculated.
> ⇨ Sales, "Recalculate" on page C-1770

**Adopt rate/discount from main item if rate is changed** In product master data you can define whether and how the discount from the main item should be applied to the BOM elements if these are price-relevant and discountable. This checkbox defines how the discounts should be applied if the rate or price key are changed.
- ☐ If prices are changed, the discount is loaded from product definition.
- ☑ If no discount has been defined for a BOM element in product master data, the discount from the main item is basically adopted when the rate is changed. Discounts on BOM level will not be taken into account.

**Use real shape size for price calculation** Pricing of shapes can be based on the surface.
- ☐ By default, the surrounding rectangle will be used to calculate the sqm price.
- ☑ For shapes, the actual surface will be used to calculate the square meter price.
⇨ "Shape Processing Surcharges" on page B-757
⇨ "Quantity Limits" on page B-916

**Misc. surcharges (% gross/net) with surcharge types** Other surcharges generally refer to quantity limits and measures.
- ☐ For all BOM elements defined with a surcharge, the surcharge is used as a calculation basis, irrespective of the surcharge type.
- ☑ The surcharge types of the BOM elements will be taken into account by default.
⇨ Tutorial 1, "Miscellaneous Surcharges" on page B-374
⇨ "Miscellaneous Surcharges" on page B-728

**Do not calculate energy surcharge by item weight** The energy surcharge refers to the weight of the shipment.
- ☐ The energy surcharge is generally calculated by total weight, including fittings, spacers, grill, etc.
- ☑ The energy surcharge is applied only to the glass weight.
⇨ "Surcharge Product Assignment" on page B-1049

**Energy surcharge on rounded weight, then with item area** The energy surcharge can be calculated on the rounded area of the item.
- ☐ The energy surcharge is not calculated on the rounded weight.
- ☑ The energy surcharge is calculated on the rounded area of the item. This may also affect any defined minimum quantities. The setting is important if BOM glass is not price-relevant, but TG with float decisive for the energy surcharge is included in the BOM.

**Calculate surcharges with rounded quantities** Even if prices are calculated with rounded quantities, the surcharge can refer to the actual surface.
- ☐ Surcharges are applied to the actual surface as a standard, i.e. before the quantity is rounded.
- ☑ Surcharges and services are calculated based on rounded quantities. The dimension rounding of the item is transferred to the dimension rounding of the non price-relevant BOM glass, which prevents that the main product has a different dimension rounding than the non price-relevant BOM glass.
This calculation type can be changed in the order by selecting the price unit sqm (act.).

**Order minimum value incl. partial deliveries** The minimum order value can refer to the total order or the individual partial deliveries.
- ☐ The partial deliveries are not regarded for the determination of the minimum order value.
- ☑ The minimum order value applies for each partial delivery.

**No dev. customer/supplier group in case of group change (header)**
Here it is controlled whether with deviating customer group in the order than the assigned customer group in the customer master data there should be a search for product group-dependent customer groups. If this deviates, then there is no more search and the order's customer group is decisive.
- ☐ The price calculation is done as previously.
- ☑ There is no product group-dependent change of the customer group if the customer group in the document header deviates from the customer group in the customer master data. This also applies for supplier groups in the POs.

**Expanded exchange price search for assembly position (LAMI)** For LAMI, the exchange price can also depend on the assembly position.
- ☐ The search for an exchange price does not consider the assembly position.
- ☑ The price calculation for the surcharge on exchange glass considers the assembly position. This way, in LAMI an additional foil can be installed and nevertheless the product/thickness-related exchange surcharge for the 2nd glass found. This also applies for the exchange surcharge for a glass in LAMI of an IGU.

**Delete glass, gas, and airspace surcharges if price/unit is defined (not for French pricing)** Surcharges can be suppressed in case of manual price changes. The corresponding option is displayed at item entry.
- ☐ This option is active at item entry by default.
- ☑ This option is disabled at item entry.
⇨ "Options menu" on page C-1539

> **French Pricing**
> With French pricing, you can choose any option at item entry.

**Spacer does not get discount PGR of IG** If a special product group has been entered for discounts on IG units, you have to define whether this should be applied to all BOM elements.
- ☐ Generally, the IG discount product group is applied to all BOM elements.
- ☑ The discount product group for IG will not be used for spacers.

**Obey currency in price master data** Currencies can be taken into account in price lists and orders. You can even take into account a third currency.
- ☐ By default, price lists are entered in national currency so that no special settings are required. An exchange rate is defined for conversions into foreign currency.
- ☑ You have to choose this setting if orders are entered in foreign currency. This function needs to be enabled if the price list is not entered in national currency and if orders are also entered in a third currency, or converted into a third currency. You also have to enter the exchange rate in this case.
⇨ Tutorial 2, "Currencies" on page B-530
⇨ "Currency" on page B-932
⇨ "Currency settings" on page B-944

**CPIP creation** Characteristic Performance Identification Paper (characteristics of features and of the performance). The CPIP code can be created automatically at order entry provided that the parameters have been defined in the CE code dialogs. This function is only required in France. It can be used only if the complete master data for CE codes have been entered.
- ☐ No CPIP code will be created.
- ☑ When documents are entered, the CPIP code will be determined, to be printed on the forms. The program also checks the defined restrictions and issues a message if they are not met.
⇨ "CE Code" on page B-1098

**Extended pricing (reference price, manual change)** Prices can usually be changed in the order. You have to define if customized price lists are still to be used in case of price changes.
- ☐ If prices are changed by hand in an order, the price entered in customer master data will not be loaded.
- ☑ If prices are changed by hand, the system checks if the price entered lies below the standard price defined for this customer. If so, an additional dialog appears where a reason for the new price has to be given.
The setting enables the Mandatory reason for price change checkbox.
⇨ "Customer Individual Products" on page B-858

**Mandatory reason for price change** For a manual price change in the order, the specification of a reason can be made mandatory.
The checkbox is only enabled if the Ex. pricing (reference price, man. change) checkbox is enabled.
- ☐ The specification of a reason for a manual price change is not required.
- ☑ In case of a manual price change, a reason must absolutely be specified.

**Check min. qty. mainly by price unit** Minimum quantities are usually calculated based on the quantity unit.
- ☐ The quantity unit defined for the product will be applied by default when checking the minimum quantity.
- ☑ The minimum quantity check is based on the price unit.
⇨ Tutorial 1, "Pricing Codes" on page B-232
⇨ Tutorial 1, "Limit Types for Graduations" on page B-315

**Calculate total order price for BOM** The amounts of the individual order items are multiplied by the quantity, provided that amounts should be displayed and printed at all.

**Total per PGR combination** The total quantity for the BOM can also be calculated by means of the PGR combination. This checkbox is accessible only if checkbox Calculate total order price for BOM has been checked.
- ☐ The total quantity will not be calculated by PGR combination.
- ☑ The total quantity will be calculated by PGR combination. This allows e.g. distinguishing total quantities with and without processing.

**Sort individual prices by price list** You can control the sorting of individual prices.
- ☐ The program will first find the individual price the price list of which has the lowest ID, i.e. which has been entered first.
- ☑ The program will find the price list with the highest ID first.

**Delete surcharges only if SP+PP are zero** The surcharge can be deleted if no price has been entered for an item.
- ☐ The surcharge will be deleted if zero (0) is entered for the sales price.
- ☑ The surcharge will be deleted only if zero has been entered for the sales and the purchase price.

**Calculate external PGR key as an inexact quantity limit** The quantity limit 140 Exact external PGR key can be used as an exact quantity limit for the external PGR key.
If the quantity limit is External PGR key, item price and price list price will be calculated in different ways.
- ☐ The quantity limit 140 Exact external PGR key will not be treated as a system-wide quantity limit.
- ☑ The quantity limit 140 Exact external PGR key will be treated as a system-wide quantity limit.
⇨ Tutorial 1, "Price Calculation by PGR" on page B-330

**Enable pricing based on macro prices** The search for prices can also include macro prices.
- ☐ No macro prices will be checked when searching for prices. This setting makes sense only if macro prices are not used at all.
- ☑ Macro prices, e.g. for specific IG structures, will be checked when searching for prices. The price macro can be valid for a customer or in general. Macro prices will be shown in customer terms at item entry.

**SP relevance of customer's own glass** Glass supplied by the customer can be entered with or without a price. This depends on the supply type Customer's own glass or on document type Customer's material.
- ☐ Glass supplied by the customer is entered without a price.
- ☑ A sales price will be calculated for glass supplied by the customer.

**PP relevance of customer's own glass** Glass supplied by the customer can be entered with or without a price. This depends on the supply type Customer's own glass or on document type Customer's material.
- ☐ Glass supplied by the customer is entered without a price.
- ☑ A purchase price will be calculated for glass supplied by the customer.

**Apply misc. surcharges to price/PU in case of manual entries** A miscellaneous surcharge that is applied to the price/the price unit, will be added to the price. For prices entered by hand, you can define how the price should be displayed in connection with miscellaneous surcharges.
- ☐ The increased value is shown in the price/price unit.
- ☑ The miscellaneous surcharge is included in the gross price. If the gross price is not shown on the form, the price cannot be explained.

**Qty. limit on BOM level for French pricing (gas and spacers)** In connection with French pricing, the search for the quantity limit can be set to Exact variant no.
- ☐ For French pricing, a spacer with limit type Exact variant no.
- ☑ French pricing also takes into account a spacer with limit type Exact variant no.

**For French. price calc. calculate the min. price on BOM** For the French price calculation, the minimum price can refer to the BOM components.
- ☐ The minimum price is calculated on the main product.
- ☑ In the French price calculation, the BOM is incorporated if the setting XX+PU is activated in the item.

**Exact calculation of surface/circumference for surface treatment** Surface and circumference calculation can be based on rounded or actual sizes.
- ☐ Surface and circumference will be calculated based on rounded sizes.
- ☑ Surface and circumference will be calculated based on the exact (actual) sizes.

**Calculate delivery fee by delivery date instead of by shipping date** The delivery fee can be calculated by shipping date or by delivery date. These dates can differ e.g. if shipping is done via an intermediate store.
- ☐ The delivery fee will be calculated by shipping date.
- ☑ The delivery fee will be calculated by delivery date.

**Price relevance for Shaping+Nesting shape rectangle acc. to master data** Shape 0 that has been defined for creating a SN file can adopt the code price-relevant from master data, or can be set to not price relevant.
- ☐ The code will be set to not price relevant.
- ☑ The code is adopted from master data. This means that you can enter prices and costs for shape 0 that will not be changed when a SN sketch is created.

**Master data rounding Price per quantity unit Foreign currency** The prices per quantity unit can be rounded off for foreign currencies.
- ☐ The prices per quantity unit are not rounded off using the settings in the master data of the foreign currency.
- ☑ The prices per quantity unit in foreign currency are rounded off. The number of places after the decimal point is taken over from the management of the currencies.
⇨ "Currency" on page B-932

## Company Data – Stock/Purchasing/EDI

*Master Data > Company > Company Data > Stock/Purchasing/EDI tab*

This tab serves to define how the purchase price of inventory products is to be calculated, and how inventory P.O.s should be reserved. You can also enter details for the EDI interface.

### Purchasing

**Calculate purchase price** Check this checkbox if the purchase price for stock products should be calculated automatically. This releases the option buttons. The following options are available for selection:
- **Average PP:** The average purchase price will be recalculated in the following cases:
    - Whenever the receipt of stock P.O.s is booked.
    - With every invoice check.
    - After reallocations (stock movements).
    - After an inventory value adjustment.
    The updated average purchase price is saved in the standard price table of the product.
- **Last PP:** The last purchase price booked on stock after receipt of goods or an invoice check, will be saved in the standard price table.
⇨ Stock Management, "Stock management - prices" on page G-2615

**Ignore combined stock articles without sizes** You can define that combined stock articles for which no sizes have been defined should be ignored when calculating the average purchase price. In this case, only the average cost of the stock sizes will be calculated.
- ☐ Stock articles without sizes will not be ignored.
- ☑ Check this checkbox if combined stock articles without sizes should be ignored when calculating the average purchase price. You should choose this setting if you are using production reports.
⇨ Stock management, "How should stock be managed" on page G-2440

**Include spacers in grill orders** Whenever the BOM or the procurement type is changed, the system checks if the BOM includes grill that have to be ordered.
- ☐ The procurement type for the spacer is loaded from product data. It can be changed in the order. Transfer to purchasing will only check the procurement type defined in the order.
- ☑ If the BOM includes grill of supply type P.O., the spacer's supply type is set to P.O. as well. This setting is adopted for the second grid if the first grid has been copied to the second spacer.

> **Order spacers and grill from the same supplier**
> If the spacer is set to procurement type P.O. in the order, it will be listed as a separate item at transfer to purchasing. If a supplier for grill has been entered in the supplier file, this will be used for spacers too.
> In case of manual changes please make sure that spacers and grills are ordered from the same supplier.

**IG as a purchased article (processing can be done in-house)** Purchased articles are ordered according to their procurement type.
- ☐ If the BOM of an IG unit includes processing of the procurement type In-house production, these will not be ordered.
- ☑ The entire IG unit including processing will be ordered even if the BOM includes processing steps with procurement type In-house production.

**Show items w/o inventory code for stock P.O.s are receipt of goods**
Goods received will be entered based on their stock code.
- ☐ In stock P.O.s, items without stock code will not be marked at receipt of goods as a standard.
- ☑ If items are entered at receipt of goods for which no stock code has been defined, these items will be shown in red letters.

**Purchasing suggestions for articles without sizes** Automatic creation of stock P.O.s can also take into account sqm stock articles (size 0 x 0 mm).
- ☐ Stock articles without sizes will not be taken into account.
- ☑ Stock articles without sizes will be taken into account when creating automatic purchasing suggestions for stock P.O.s.

**Weight in lbs** Via the OrderXML interface, by default, weights are transferred in the unit kilograms to production.
- ☐ The weight is transferred in the measurement system in kilograms.
- ☑ The weight is converted to imperial pounds (lbs.) during the transfer to production.

**In case of incomplete P.O., process complete BOM** Specification for how purchase orders are transferred to standard suppliers.
- ☐ If for an order a standard supplier is entered for the whole order, the item must be set to Purchase order (complete) so that the BOM elements of an item to be ordered are also processed. If the item is only set to Purchase order, the BOM elements are not transferred to the purchase order.
- ☑ This item is treated as if no standard supplier is entered. Thus the BOM elements to be ordered are transferred to the purchase order pool.

**Change PO and order if surplus/shortfall accepted**
On receipt of goods of ordered order items, surplus/shortfall can be delivered.
- ☐ Surpluses or shortfalls are not written back.
- ☑ If on goods receipt a deviating quantity for an item is specified and accepted, the new quantities in the order are entered as surplus or shortfall.
    - If the order is already in production, the quantity change is transferred to the production system.
    - If the order is not yet in production, the over/excess quantity is reported to the production system with the production transfer.

**Always include supplier project in purchase order** Transfer of the supplier projects from the order to the PO.
- ☐ The supplier projects are not transferred.
- ☑ The supplier objects are also transferred to the PO if no header supplier is specified. This way, an order with supplier projects can include several suppliers. These can be assigned per item or entered in the order transfer. In the PO pool, the Supplier project column can be inserted above the Properties.

### Stock control mode

**Update inventory in case of reservations** Selection of whether the inventory should be updated in case of reservations.
- **w/o:** When you enter an order, the quantity of the product entered will be reserved but not withdrawn from the stock on hand.
- **with:** The reserved quantity is withdrawn from the stock on hand when the delivery note or invoice is printed.
If no other storage place has been entered in the stock search, the order quantities are allocated to the standard storage place.
The decision about the stock location from which the product is withdrawn is made with reports from the optimization by the bar code registration.

**Stock control on BOM level** Products can be kept on stock even if they are part of a BOM.
- ☐ By default, products are only added and withdrawn on main product level in A+W Business.
- ☑ Additions and withdrawals are also made on BOM element level.
⇨ Stock management, "Stock control on BOM level" on page G-2484

**Execute stock booking before printing the document** The stock on hand is usually updated when a delivery note or invoice is issued; this is recorded in stock history. You can define that withdrawals should always be recorded.
- ☐ Stock withdrawals are booked when the form is printed.
- ☑ Stock withdrawals will be booked separately from the printing of forms.

**Delete articles with ID if there is no stock on hand** When boxes are received, they get an identification number (ID) that is usually deleted when the box is withdrawn from stock. If boxes are broken up internally it can happen that the box is still kept on stock with this ID.
- ☐ Stock articles (boxes) with ID and stock = 0 have to be deleted by hand.
- ☑ Stock articles with an ID and stock = 0 will be deleted automatically.

**Stock control even without document type Stock P.O.** Partial deliveries can be created for stock P.O.s.
- ☐ An (independent) partial P.O. for stock articles cannot be issued. The quantity delivered for a stock P.O. will be adopted for the partial P.O. however if part of the goods received have been booked already.
- ☑ A partial P.O. can be issued for partial receipt of goods if the P.O.'s document type is not Stock P.O.
A partial invoice can be booked for such a partial P.O. In the order, the costs will be updated based on the average costs from all partial P.O.s. The costs will be saved as unit costs.

**Consumption of BOM elements in production orders** For production orders, the consumption of BOM elements in stock can be booked.
- ☐ The consumption of BOM elements is not withdrawn automatically from the stock.
- ☑ In production orders, a stock-kept BOM element is withdrawn from stock automatically and the product for the main item is added to the stock.

> **Example**
> In a production order, an IGU with a TSG is entered. After reporting of the production order, the IGU is booked into the stock, the TSG is withdrawn from the stock.
> If for the same IGU with TSG a normal customer order is entered, only the IGU is withdrawn from the stock. The TSG is not kept in the stock since it has already been withdrawn from the stock by the production order.

**XTV feedback for stock sizes only (w.o. reservations)** Also for products with the stock-keeping mode size-dependent, automatic withdrawals can be made with feedback from the optimization.
- ☐ Products with the stock-keeping mode size-dependent are not withdrawn automatically from stock with feedback from optimization.
- ☑ Products with the stock-keeping mode size-dependent are withdrawn automatically from stock with feedback from optimization. The quantity entered is not marked as reserved in the qm record. Only the stock sizes from the optimization feedback are withdrawn.
⇨ "Stock control mode" on page B-983

**Always calculate area according to circumscribed rectangle** Size-dependent lites can be booked differently in stock.
- ☐ By default, lites that are not kept in stock depending on size are always booked with the actual area or waste in stock.
- ☑ The area of the circumscribing rectangle is booked.

**Include foot surcharges in the purchase price of boxes** Percentage costs can also be considered for boxes with ID, e.g. energy surcharges, transport costs.
- ☐ The percentage costs are not calculated in the box PU.
- ☑ For boxes with ident number, the percentage costs are calculated in the PU.

### Stock preview

**No. of workdays** The stock preview shows the availability of products for a certain period in the future. The number of days represents the number of days to be shown in the preview. The display starts from the current date.

### Dorma web service

The data in this section have to be entered if BMECat is to be downloaded from the Dorma website. These data match those for automatic Dorma purchase orders.

**Address** Internet address of the Dorma web service.

**[Globe]** When you have entered or changed the Internet address you can use this icon to check whether the connection can be established.

**User, Password** Registration data that entitles you to access the Dorma web service.

**Save costs in the order** The actual costs of a purchase order can differ from the costs defined in supplier data.
- ☐ The costs will not be saved. The P.O. still shows the costs defined in master data.
- ☑ The actual cost of the ordered articles will be saved in the order.

**[A+W test login]** This button can be used to change the access data to the A+W Software GmbH test login. This allows to check whether the connection can be correctly established based on these data.

### Confirm Dorma transmission by email

You can have a transmission confirmation issued automatically to make sure that your online P.O. has been sent.

**Server** Name of the server controlling the transmission confirmation.

**Port** Number of the port for the transmission confirmation.

**Sender's address, Recipient's address, cc:** Email addresses to be used by default for the transmission confirmation.

**Authentication** An authentication can be used for the transmission confirmation.
- ☐ The transmission confirmation will not be sent without authentication.
- ☑ The transmission confirmation requires authentication. The fields for entering the registration data are accessible.

**Use SSL encryption** Secure Sockets Layer (SSL); encryption program for safe data transfer in the Internet.
- ☐ The transmission confirmation will not be encoded.
- ☑ The transmission confirmation will be encoded acc. to the SSL log.

**User, Password** Registration data the sender uses for authentication.

### EDI interface

Documents can be exchanged electronically (as files); the data will be imported into another system right away. The following settings are important only if you are using EDI interfaces.

**Disable OEM/ANSI conversion** For transfer, the interface converts the data into a format that can be read by all other programs.
- ☐ The data of the file to be transferred are automatically converted to ANSI format by default, e.g. ä becomes ae.
- ☑ In special cases, data conversion has to be switched off, e.g. in connection with certain interfaces.

**Disable automatic scheduling in capacity planning** This setting only applies to A+W Business capacity planning. It is necessary to transfer order data electronically. The data are usually transferred by means of a work flow task.
- ☐ Generally, the data of the imported orders are automatically scheduled in capacity planning if automatic scheduling is active.
- ☑ Automatic scheduling of imported orders is disabled. This permits to check imported orders before scheduling.
If you are using A+W Business capacity planning, the checkbox for automatic scheduling must be disabled.
⇨ "Automatic scheduling" on page B-963

**Use architect from header record for article reference** During
- ☐ During EDI import, no article reference in the header record is used.
- ☑ During EDI import, the article reference to the architect is entered in the header record.
The architect number used for import is transferred to the order with import in order to distinguish the eCommerce orders from the rest of the orders later on.

### Reg. point allocation

**Order produced at** When an item has been registered at the selected registration point, its status will be set to produced in A+W Business. The corresponding batch number will be saved with the order item.
If AWBar or A+W Production reports are sent to the files of the types STSP, STSL, STSD, STSB, STSG, you have choose a registration point that is allocated to a status point. If such a registration point was not assigned, the report generates an error.
Order information shows this item on tab Produced. The production date is updated in the order header.
⇨ Statistics, "Order information" on page F-2382

**Goods receipt in/for** Specification of registration point.

**Check the P.O. parts in purchasing** The goods receipt of purchase order parts can be checked from a registration point or in purchasing.
- ☐ Goods receipts from partial delivery items are checked through the packaged quantity reported by STSG. The reported quantities are queried for the generation of partial deliveries. The parts delivery can only be created for the quantity reported.
- ☑ The goods receipt of purchase order parts is checked in purchasing.

## Company Data > Archives

*Master Data > Company > Company Data > Archives tab*

This tab defines how data and documents should be archived.
⇨ Tutorial 1, "Database" on page B-440
⇨ Tutorial 1, "Statistics" on page B-441

### Global settings

The settings in this area refer to automatic archiving that can be enabled in section Automatic options.

**Archives database** Name of the A+W Business archiving database. Usually, the customer code is used as the name. The name of the archives database is completed by the corresponding year. This allows to manage several years in one database.

> **Create new archives**
> Please remember to have A+W Software GmbH create new archives for the next year.

**Consider complaints for sales commission** Complaints can be taken into account when calculating the sales commission.
- ☐ Complaints will not be considered as a standard. The commission will not be reduced.
- ☑ Complaints will be considered in the salesman's turnover. The sales commission will not be diminished however.

**Complaints without quantities (pc., sqm., lin.m.) to turnover statistics**
Complaints can be analyzed with regard to prices and quantities.
- ☐ Apart from the amounts, quantities (piece, sqm, linear meter, etc.) are also transferred to turnover statistics. This can mean that the quantities from uninvoiced complaints will reduce the total result.
- ☑ Only the price is transferred to turnover statistics by default.

**Export super statistics** This option refers to module Group statistics. Group statistics are designed for groups of companies who are using different servers with separate databases, but need comprehensive statistics for all companies of the group.
- ☐ This checkbox must be disabled for the main company running the analysis.
- ☑ The checkbox has to be active for the client supplying the statistical data.
⇨ Statistics, "Super statistics" on page F-2404

**Transfer to statistics w/o printing an invoice/credit note** Turnover and quantities can be analyzed before or after printout of invoices and credit notes.
- ☐ The invoice number created at printout has to be available to release transfer to statistics.
- ☑ Orders can be transferred to statistics even if no invoice or credit note is printed. Transfer is released by the defined minimum status.
⇨ Tutorial 2, "Lock status" on page B-497

**Transfer to statistics only after invoice check** This option only refers to module Invoice check in purchasing.
- ☐ By default, purchase orders are transferred to purchase statistics without an invoice check.
- ☑ Purchase orders can be transferred to statistics only after the invoice has been checked.

**Transfer BOM glass turnover to main product** The turnover from exchanged lites can be analyzed together with the main product, or separately.
- ☐ By default, the replacement surcharge is included in the turnover of the new element.
- ☑ The replacement surcharge is included in the main product's turnover. The checkbox for cost analysis is accessible.

**Transfer cost of BOM glass elements to main product** The cost of exchange glass can be evaluated in statistics separately or together with the main product.
This checkbox is accessible only if the checkbox for turnover evaluation has been checked.
- ☐ By default, the costs of replaced lites are included in the costs of the replacing element.
- ☑ The costs of the replaced lites should be included in the costs of the main product.

**Book transfer to statistics of box qty./surface to item** The size and quantity included in a box can be analyzed in statistics on BOM element level or on item level.
- ☐ The contents of boxes is booked to statistics on BOM element level by default.
- ☑ The contents of boxes should be booked to statistics on item level. With this setting, the analysis depth in statistics must refer to items only. The analysis depth Item and BOM would falsify the size on product group level otherwise because the size is calculated for the glass and the processing.

> **Statistics update**
> If you have chosen the setting Book transfer to statistics of box qty./surface to item, statistics must be drawn up anew via Utilities > System > Statistics update.

**Transfer to archives by input date** Documents are archived based on their input date.
- ☐ Archiving is based on the invoice date by default.
- ☑ The order input date is used as a basis for archiving.

**Delete documents without checking the reference** This setting only refers to documents created by transfer to purchasing.
- ☐ Usually, a P.O. can be deleted only if the corresponding order has been archived, and deleted from the main database.
- ☑ When deleting a document, the system does not check if there are reference documents. The archiving year does not depend on the order but on the P.O.

**Delete documents only if already archived** Documents can be deleted from the main database to keep its size at bay.
- ☐ The document can be deleted without checking archives.
- ☑ A document (order, P.O., etc.) can be deleted (by hand) only if it has been transferred to archives before. The system will search for the corresponding history entry.

**Multiple archiving** The document is archived when the order is completed, i.e. when the invoice has been transferred to financial accounting and statistics.
- ☐ Every document can be archived just once.
- ☑ Documents can be archived several times. This setting makes sense only if a document is fetched from archives to be amended. In this case, the original document will be deleted; only the amended one will be archived.

**Book complaint orders only in turnover statistics** Orders based on complaints can falsify turnover statistics.
- ☐ By default, the turnover of orders and the corresponding complaint orders are booked in turnover statistics.
- ☑ Orders based on complaints are only booked in turnover statistics. A reason for the complaint has to be entered for this purpose.

> **Example**
> A customer complains about an order. The operator enters a complaint order of the document type Complaint without a reason for the complaint. An invoice will be issued for the complaint order; it is booked in statistics like a standard order.
> If the complaint is justified, a complaint credit note will be issued as a third document (credit note of the document type Complaint and reason for complaint). This document corrects turnover statistics by the corresponding sales price (cost and surface remain unchanged); unlike the standard booking, positive amounts will be booked in complaint statistics.
>
> | Document | SA | Costs | Surface |
> | :--- | :--- | :--- | :--- |
> | Order | 100 € | 50 € | 1,0 sqm |
> | Complaint order | 100 € | 50 € | 1,0 sqm |
> | Complaint credit note | 100 € | 50 € | 1,0 sqm |
>
> **Booking in turnover statistics:**
>
> | Document | SA | Costs | Surface |
> | :--- | :--- | :--- | :--- |
> | Order | 100 € | 50 € | 1,0 sqm |
> | Complaint order | 200 € | 100 € | 2,0 sqm |
> | Complaint credit note | 100 € | 100 € | 2,0 sqm |
>
> **Booking in complaint statistics:**
>
> | Document | SA | Costs | Surface |
> | :--- | :--- | :--- | :--- |
> | Order | - | - | - |
> | Complaint order | - | - | - |
> | Complaint credit note | 100 € | 50 € | 1,0 sqm |

**Document archiving without items** Documents can be archived even if they contain no items.
- ☐ Documents without items will not be archived.
- ☑ Documents without items will also be archived.

### Complaint statistics for credit notes

**Entry of complaint cause obligatory** When a complaint is entered, both the place and complaint and the cause of complaint can be defined.
- ☐ Generally, input of the complaint cause is optional.
- ☑ The document cannot be saved if no cause of complaint has been entered.
⇨ Software Reference, "Complaint Cause" on page B-653

**Default complaint place** The place of complaint can be entered for statistical purposes. If there are several places of complaint, one of them can be used as a default.
- ☐ Usually, no default place of complaint is set.
- ☑ You can choose the most frequently stated place of complaint as default. This can be changed in the document.

### Document settings

The settings in this area are valid for the selected document type.

**Document type** Choose the document type for which you are going to set automatic options in the following fields. The settings can differ for the individual document types.
⇨ Sales, "Transfer to archives" on page C-1779

### Automatic options

The settings in the following fields refer to the document type selected in field Document type. This means that you can enter different archiving settings for every document type.
Usually, documents are transferred to both statistics and archives at (automatic) archiving, and will then be deleted from the main database. Generally, transfer to statistics is based on the month in which the document was issued while archiving is based on the year.

> **Settings for transfer to archives**
> Document management allows to set the details for automatic transfer to archives.
> Documents can also be transferred to archives by hand.
> ⇨ Sales, "Transfer to archives" on page C-1779

**Transfer to commission statistics** This checkbox refers to module Sales commission.
- ☐ Data are not transferred to commission statistics.
- ☑ Automatic archiving will also transfer the data to commission statistics.
With this settings, you should also check the field Process complaints in sales commission in section Global settings.

**Transfer to turnover statistics** This checkbox refers to the module Turnover statistics.
- ☐ Data will not be transferred to turnover statistics.
- ☑ Automatic archiving will also transfer the data to turnover statistics.
With these settings, you should also check the field Complaint w/o quantities in section Global settings.

**Transfer to archives** This checkbox refers to the module Document archiving. Archives are set up by year. At the change of year, the system archives the documents in the old or in the new archives, based on the invoice date.
- ☐ Documents will not be archived automatically. Documents can be transferred to archives by hand however.
- ☑ Documents will be archived automatically. Enter the archiving year as well.
With this setting you should also check the checkbox Delete document.

**Delete document** Documents should be deleted from the main database in regular intervals in order to keep its size at bay.
- ☐ Documents will not be automatically deleted upon archiving.
- ☑ Documents will be deleted from the main database after transfer to archives.

> **Relieve main database**
> Delete the archived documents from the main database. This will relieve your database and will improve its speed. Archived documents can be retrieved from archives any time.

**Deleting document from iQuote** This checkbox allows you to delete documents from A+W iQuote if an Order or Quotation is deleted via the A+W Business. Here, the associated configuration entries are also removed from the database. This reduces the quantity of data saved in the database.
- ☐ Documents will not be deleted from the main database.
- ☑ Documents will be deleted from the main database.

### Archiving mode

The settings in the following fields refer to the document type selected in field Document type. You can enter different archiving settings for every document type. Choose an option to define the mode:
- **Minimum status:** Status from which on documents should be archived automatically. Status 820-Auto. archiving is selected by default for automatic archiving.
- **Document older than x days:** If automatic archiving should depend on the document date, you can enter the number of days that have to elapse after the given date before the document can be archived.
- **Status + document older than:** With these settings, both criteria must be fulfilled: The corresponding status must be reached and the document has to have reached the defined age.

### A+W Production

**Path for report file** File in which the report file should be saved. It includes the list of orders archived in A+W Business. A+W Production uses this information for deleting the corresponding orders from its system.

**Order area for batch number** The batch numbers are only analyzed for the defined order area. The batch number is selected from the corresponding number range in dialog Number ranges in field Alcim archives batch number.
⇨ "Number Ranges - Production" on page B-921

**Version** If different versions have been defined for an order area, you can choose the current one.

## Company Data – Daily Closing

*Master Data > Company > Company Data > Daily Closing tab*

Enter the deadlines after which files are finally deleted from the main database.

### Storage days

The following fields serve to enter the number of days for which data should be saved in the main database for statistics and backup purposes before they are automatically deleted for good. This helps to keep the database small and fast.

All data older than the defined number of days will be deleted. This does not include the archived data.

**Statistics** To create annual overviews you should enter more than 365 days to have ample time for creating the reports.
⇨ Statistics, "Purchasing Statistics" on page F-2414
⇨ Statistics, "Turnover purchase statistics" on page F-2414

**Commission statistics** Long periods allow to analyze the commission for several years.
⇨ Statistics, "Commission Statistics" on page F-2424

**Time management** Long periods allow to analyze time management statistics for several years.
⇨ Capacity Planning, "Statistics" on page H-2901

**EDI backup file** Backup files for interfaces are practical until data processing has been successfully completed by the connected programs.
⇨ "Interface service" on page B-1051

**History entries** Number of days for which a document history will be saved.

**Order information** You should choose a longer saving time for analysis purposes. You should choose a longer saving time for analysis purposes.
⇨ Statistics, "Order information" on page F-2382

**Stock logbook** Inventory history shows the goods received and withdrawn, purchase orders, etc. You can keep this list at bay by deleting the entries after a reasonable time.
⇨ Stock Management, "Stock history" on page G-2627

**Rack history** You should choose a longer saving time for analysis purposes.

**Credit limit snapshots** Credit limit snapshots can be used for analyzing the development of certain financial data for a customer within a defined period.
⇨ "Credit Limit Analysis" on page B-879

**OderXML data records** You should choose a longer saving time for analysis purposes.

### System logbook

**Age of entries when deleted** Number of days for which an entry should be saved in the logbook before it is automatically deleted for good.

**Archives path/name** Directory and name of logbook archives.

## Company Data > System

*Master Data > Company > Company data > System tab*

This tab serves to adjust the measurement system, lead days for production, the transfer to A+W Production, and time management.

### Units of measurement

The measurement system does not have to be the same for the two areas.

**Database metric, imperial** Unit of measurement to be used by default. You can enter your documents based on metric (=cm) or imperial measures (=Inch).

**Thickness metric, imperial** Although you may usually enter sizes in inch, it may be necessary to enter the thickness in mm.

> **Choose measurement system by customer**
> You can change the predefined measurement system by customer. In this case, the measures will be converted in the customer-bound documents.

**Size precision = 1/** If imperial measurements are activated for the database, enter 32, 64 or 128 in this field, depending on the factor to be used for calculation.
If you are using metric sizes, enter 1 in field Size accuracy.

**Metric digits after colon** Number of places after the decimal point of the circumscribed rectangle for shapes if the measurement system is set to metric.

### Formats

**Date** Display the date as:
- dd.MM.yyy
- MM.dd.yyyy
- MM/dd/yyyy
- yyyy-MM-dd
(d = day, M = month, y = year)

**Time** Display the time as:
- hh:mm
- hh:mm AMPM (English 24 hour format)
- hhhh/mm/ss
- hhhh-mm-ss
(h = hour, m = minute, s = second)

**French keyboard support (. to,)** On keyboards with a French layout, the decimal separator on the number block is a dot. In the country settings for the operating system, however, the comma is entered as decimal separator.
- ☐ The decimal separator matches the settings in the operating system (Windows country settings).
- ☑ The decimal separator is converted:
    - For countries using the colon as a decimal separator, dots will be changed into colons.
    - For countries using the dot as a decimal separator, colons will be changed into dots.
When the Caps Lock key is active, the decimal separator of the numeric keypad is redirected to the dot.

### Customer version

**Producer, Trade** Depending on the setting, the document header will show different fields for the dates. Calculation of dates is based on the settings in section Lead days.
Based on these options, you should fill in the fields Start of production and Supplier's delivery in section Lead days (see below).

**Code** The customer code is used to check which parts will be enabled in this A+W Business installation.

> **Changing the customer code**
> If you change the customer code, you will lose access to the functions specially developed for your company.

**Edition** If different editions of A+W Business are available, the version matching the customer code will be displayed. This is usually the standard edition however.

### Lead days

The fields in this area refer to the fields in section Customer version. The lead days can be changed at order entry.
The tutorial offers examples for scheduling of dates (customer's delivery date, shipping date, start of production, etc.) in the order header.
⇨ Tutorial 1, "Delivery Time" on page B-183

**Start of production** Number of days to be deducted by default from the shipping date shown in the order header in order to determine the start of production.
This detail is required if you have selected the option Producer in section Customer version.
Start of production = shipping date - Start of production

**Production LG** Number of days to be deducted by default from the shipping date shown in the order header in order to determine the start of production for laminated glass.
This field is displayed only if you have chosen Producer for the customer version.

**Delivery from supplier** Number of days to be deducted by default from the start of production shown in the order header in order to determine the date for the supplier's delivery.
This field is displayed only if you have selected Trade for the customer version.
Supplier's delivery date = Start of production – Supplier's delivery

### Lead days for resubmission

**(Document)** Selection whether quotations or orders are checked for resubmission.

**(Days)** Enter the number of days after which the system should automatically remind you of following up a quotation.
When you enter a new quotation, the resubmission date is automatically determined based on the input date and the days defined here.

### Settings

**Use Windows registration for A+W Business login** This setting is valid for all users. It cannot be linked with certain users.
- ☐ A+W Business can be started only by separate registration.
- ☑ After the Windows registration, A+W Business can be started without an additional registration (SSO: Single Sign On). User name and password have to be identical for this purpose.
A client-/server installation also requires input of the domain.

**Customizing activated** This setting refers to customized amendments.
- ☐ A+W Business can be used in the version installed.
- ☑ Additional forms, variables, or fields can be used. If you do not need those, you should uncheck the checkbox to relieve your database.

**Enable Exchange Service for Workflow** For the execution of workflows and the processing of production reports, the new A+W Commercial Exchange Service is now available. It replaces the A+W Business 6 Interface Service.
- ☐ The A+W Commercial Exchange Service is not supported.
- ☑ The A+W Commercial Exchange Service is used.

**openTrans Export in Thread** Number of open Trans transfers per export process.

### A+W CAD Designer (Shapes)

**View** View for the SN file:
- **End product (sketch):** This is the standard setting if you are using the SN-Editor.
- **Edgework (sketch):** With this setting, only the edgework will be shown.

**Color depth** Color setting for displaying SN files:
- **1 Bit:** This setting is used for line drawings. The display is monochrome.
- **4 Bit:** This setting means that 16 colors or shades of grey can be displayed.
- **8 Bit:** This is the standard setting. Up to 256 colors can be displayed with this setting.

**lite background** This setting refers to the display of the sketch.
- **Filled:** The lite appears as a colored area.
- **Unfilled:** Only the outline of the lite is shown.

**Pattern size, segment text, sizes** Size in which the SN file is displayed at item entry. Standard settings:
- Pattern size: 12 px
- Segment text: 14 px
- Sizes: 16 px

**File path** Storage place for the SN file. For the transfer to production, this directory must be known to A+W Production. To be on the safe side, always start the path with a double backslash and enter the complete address (IP).

**Only processings broken down in the production BOM** The production BOM breakdown for processing steps can be adopted from the SN file. Production BOM breakdowns from macros will always be adopted.
- ☐ The entire production BOM breakdown will be adopted.
- ☑ Only the production BOM breakdown for processing steps will be adopted.

**In case of structural changes** The SN files are regenerated after changes. This function only makes sense for structural changes.
- ☐ With each change, a new SN file is generated. This also affects changes that are not production-relevant.
- ☑ Only for structural changes is a new SN file generated, e.g. if the dimensions were changed.

**Edge processings and drillings on shape 99** Edge processings and drillings can be applied to free shapes and imported SN files.
- ☐ With the shape 99, no additional processings can be entered in the associated SN file.
- ☑ The edge processings and drillings are saved in the SN drawing.
This function only refers to the dimension type circumscribed rectangle and to the program version 6 of A+W CAD Designer (Shapes).
With a free shape (shape 99), edge processings cannot be applied selectively, but rather only on all edges. Drillings can only be dimensioned with reference to the circumscribing rectangle.
If during import of the SN files into A+W Business there is a change to a standard shape, edge processings on individual edges can be entered if there is an edge numbering (1, 2, 3, 4) in the SN or DFX file.

### URL for AWSOA services

Specification of the A+W SOA service. With this service, among other things, capacity overviews from A+W Capacity Planner (EL) can be imported, in order to view the free and occupied capacities.

### Customer logo

Path for the files containing the customer logos. The customer logo is defined in dialog Logo position.
⇨ "Logo" on page B-877

### Path for product images

Path for the directory containing the product images assigned to a product. These images will be used for the printing of forms.
⇨ "Article sketch" on page B-672

### Replication

Replication means that master data are copied from the headquarters' database to the subsidiaries' databases.
The replication is started in module Utilities > Replication management.

**Replication recipient** You will need this function only if you have several subsidiaries with separate databases.
- ☐ This checkbox must not be checked at headquarters.
- ☑ This checkbox must be checked in the subsidiaries. This will lock all master data fields that are maintained in the main database.

**Language** Dialog Replication shows the descriptions in tables and fields in the selected language.

### Database parameters

**Isolation level** The transaction mode of the database can be changed:
- **RL:** Release Lock (restrictive transaction mode). This is the setting for the older versions of A+W Business.
- **RC:** Read Committed (restrictive transaction mode). This setting increases the performance. It will be adopted for all terminals after the system is rebooted.

### A+W CAD Designer (Bars)

**Show clear field sizes** For grill patterns, the clear sizes of the fields can be displayed.
- ☐ The clear sizes of the fields will not be shown.
- ☑ The sizes of the glass without the grill width (clear fields) will be displayed.

**Sum up grill quantities from macros** Prices can be adopted from A+W CAD Designer (Bars) macros.
- ☐ Prices will not be adopted.
- ☑ The prices from A+W CAD Designer (Bars) will be adopted and added to the existing quantities. If e.g. a sun consisting of three fields is added, the extra fields will be added to number of fields.

**AWD20.INI for construction printing** The true-to-scale grill sketch can be printed according to the configuration for CAD Designer Bars.
- ☐ The grill sketch is printed according to the A+W Business standard.
- ☑ The configuration for CAD Designer Bars is used if in the order a true-to-size sketch for grills with the setting Output grill cutting list is printed.
⇨ Sales, "Print dimensioned sketch" on page C-1747

### Database

**Transactions** The database support for SQL server also allows transactions. Thus, SQL commands that follow one another and change the data can be undone as long as the transaction has not been completed.
- ☐ Database transactions are only possible for the SQL Base database system.
- ☑ Database transactions are possible for SQL Server. This setting is important for the Microsoft SQL Server database system.
For the SQL Base database system, the transaction logic is always active.

## Company Data > Calculation

*Master Data > Company > Company Data > Calculation tab*

This tab is used to enter the surcharges for cost calculation.
⇨ Tutorial 2, "Cost and surcharge calculation" on page B-613

### Cost and surcharge calculation

The costs calculated at document entry can be displayed at order and item entry.

### Material overheads

**Procurement type** Supply types are preset by A+W Business.

**% surcharge** Proportional surcharge to be used for the corresponding procurement type.

**Ancillary labour costs** Proportional surcharge on ancillary labour costs.

**Sales overheads** Proportional surcharge for the overhead cost of sales.

**Administrative overheads** Proportional surcharge for the administrative overheads.

**Profit margin** Proportional surcharge for the expected profit.

### Capacity areas

**Weekday, IG, LG, TG** This table only refers to module Customer-based capacity information system.
You can define total capacities for the three main product types (IG, toughened, laminated glass). Shares of those can be reserved for key customers. These shares are defined in customer master data.
⇨ "Partner Management - Production" on page B-831
Customers for whom no capacities have been defined, will be collected in a group to which the remaining capacity is allocated. At order entry, the function Capacity info by customer shows the remaining production capacity.
⇨ Sales, "Document - header data" on page C-1542

### Default MI

**Minimum MI** Percentage of marginal income that must be reached when an order is changed.

**Maximum MI** Percentage of marginal income that must not be exceeded when an order is changed.

## Company Data - Print

*Master Data > Company > Company data > Printing tab*

This tab serves to define the settings for printing documents.

### Monthly invoices

The fields in this section refer to the module Monthly invoices.
The checkbox Monthly invoice has to be checked in customer master data.
⇨ "Partner Management - Finances" on page B-822
All customer orders with the code Monthly invoice are automatically allocated the status point 73-Monthly invoice.
The corresponding user status in your A+W Business version depends on your own status organization. Based on this status, you can select the orders for each customer and invoice them together.
⇨ Tutorial 2, "Status administration" on page B-492
⇨ Sales, "Monthly invoice" on page C-1149

**Print point** Print point for the printing of forms. Standard setting: 103-Invoices.

**Mail, Fax, Email** For the print of monthly invoices you can define at which print point the invoice will be printed.
- ☐ The print point is not used.
- ☑ The print point is relevant for the print of monthly invoices. With the print, the status of the document is set. For this, the status point 73-Monthly invoice must be set.

**Status point** Standard setting: 73-Monthly invoice. Orders for customers with monthly invoicing that are invoiced by mistake will be automatically set to status 73-Monthly invoice.

### Print sketches

**Extended grill sketch on printed forms** Sketches can be printed schematically or true to scale. The setting can be changed in the order.
- ☐ By default, grills will be printed schematically.
- ☑ Grill sketches can be printed in detail. This requires that the sketch size is increased in management of forms for the detailed display. The function for true-to-scale printing must also be set in the order.
⇨ Tutorial 2, "Printing sketches" on page B-552
⇨ "Shape sketch, grill sketch" on page B-1081

### BOM

**Maximum quantity** Number of BOM entries to be transferred to printing of forms. You should make sure that your BOMs can be actually processed.
If an order has got a more extensive BOM, all entries exceeding the maximum number will not be printed.
An input of 15-20 has proved sensible. A higher number will impede the processing speed considerably.

### Print server

This field refers to the module Print server.
⇨ "Print Jobs" on page B-1083

**Server name** Enter the name of the server on which the print server has been installed.

### Printer list

**Check available printers via Windows API** If you are using several printers, these can be offered for selection when forms are printed. Printing via print server requires the creation of print jobs.
- ☐ The forms will be sent to the standard printer.
- ☑ You can choose one of the available printers. This setting allows to decide whether a form is printed as a PDF file, as a fax, or as a hardcopy (on paper).

### Reprint for document archiving

**Printer** Choose the standard printer.
If an automatic reprint should e.g. be started for the DMS system ELO (electronic Leitz file), you have to select the ELO printer.

### DMS

**DMS archives path** Path for saving the document files. All documents that can be archived in A+W Business will thus be archived in the document management system Saperion (DMS) at the same time.

### Primary form/report search

Clients may be using different forms for printing and for reports. Enter a path for the primary search for forms/reports. Printing of forms and printing of reports will search for the report and the form in this directory.
If the forms cannot be found there, the program will fall back on the standard installation directory.

**Path** Path in which the forms for the current client can be found. This path may also include amended standard reports.
This field can be left blank if all clients are using the same forms or if just one client has been entered.

### Crystal Reports ODBC

**DSN** Name of the domain server on which the application is installed.

**User, Password** Login data for accessing Crystal Reports.

### Form printing

**Form printing via Crystal Reports** As an alternative to the internal report forms, the reports can also be printed via Crystal Reports.
- ☐ Crystal Reports is not used.
- ☑ The forms are output via Crystal Reports.

**Path** Path in which the forms can be found.

**Email** Printer with which the reports will be output.

### Document management

**Enable archiving system** If you are using a document management system (DMS), e.g. in Saperion, documents can be archived. An appropriate interface has to be installed.
- ☐ Documents will not be transferred to a document management system.
- ☑ The documents are transferred automatically to the connected DMS. For this, you have to active the document archiving in the form management for each form.
With this setting, e.g. when printing the invoice, the invoice is first sent automatically and then transferred to the document archive.
⇨ "Archiving of documents" on page B-1074

**(Path)** Specification of the archiving path.

## Company Data – Production

*Master Data > Company > Company Data > Production tab*

This tab serves to enter the settings for the transfer to production.

### Transfer to production

**Profit center invoicing active** Profit center invoicing allows to invoice internal services between different clients or order areas.
- ☐ Profit center invoicing will not be used.
- ☑ When an order of the first client is transferred to production, a P.O. will be automatically issued for the corresponding client.
In product management, the corresponding procurement types have to be entered for every product, per client/OP area.
After that, the work performed by the corresponding client/order area will be invoiced.
⇨ "Product codes" on page B-685

**[Orders]** Opens the dialog Settings – Transfer to production where various transfer parameters for orders can be set.
⇨ Production, “Settings for Transfer to Production" on page E-2244

**[Quotations]** Opens the dialog Settings – Transfer to production where various transfer parameters for quotations can be set.
⇨ Production, “Settings for Transfer to Production" on page E-2244
⇨ Production, “Optimization of Quotations" on page E-2349

**Creation of follow-up orders enabled** If your production areas (IG, laminated and toughened glass) are distributed to different clients or order areas, this module allows the automatic creation of follow-up orders for internal orders for the corresponding production area.
- ☐ No follow-up order will be issued for internal orders.
- ☑ At transfer to purchasing, all internal orders and follow-up orders for the corresponding client or order area will be created automatically.
⇨ "Product Management - Stock/Purchase" on page B-683

**Extended workbench (Light)** IG and LAMI can be ordered completely in A+W Business. These items are then transmitted via purchasing to the supplier; they are regarded as purchased parts (usually only for dispatch) in production. If, however, insulated glass from internally cut glass or lamination of a LAMI should be ordered, in the past there was no solution for this since the production transferred the insulated glass a purchased part to the glass and thus there was no cutting.
- ☐ The glass is ordered.
- ☑ The glass is transferred with the procurement type 16 (cutting before order) and the glass is cut. Only the assembly or the lamination is purchased.
In the solution, it is not considered that the lites have to go to the supplier; this has to be organized manually internally.

**Creation of SN files (incl. EDI import)** SN files can be created automatically at transfer to production.
- ☐ SN files (A+W CAD Designer) will not be created automatically.
- ☑ At transfer to production or at EDI import, the system automatically creates a SN file for rectangles and standard shapes including the following processing steps for every item that includes e.g. single annealed or toughened glass: edgework, cut-off corners, rounded corners, notches, and drill holes. This procedure allows to print true-to-scale sketches on your production papers.
When a SN file is created, the user status SN file checked will be assigned so that the following transfer to production can use this user status as a minimum status.

**Prioritize import according to delivery date** With this option, you control whether the delivery date in the form `<yyyy-MM-dd>` is appended to the OrderXML file name. This way, the production import can import files with earlier delivery date with priority. This makes particular sense if a large number of orders come into the system via EDI, which will burden the import in production for a long time. This way, early deliveries would be scheduled too late. The condition for this is that a delivery date for the orders is transferred via EDI.
- ☐ The delivery date is not appended to the OrderXML file name.
- ☑ The delivery date is appended to the OrderXML file name.

**Generation of shape 0** You can select the shape that should be inserted automatically for the creation of SN files for rectangular lites. If no item is selected here, the shape to be attached is determined as previously.
The field is only enabled if the automatic generation of SN files is activated.

**Production Manager** With this setting, you switch on the program variant A+W Business Pro.
If you are working with the Production Manager module, partial deliveries can be booked with fileless reporting.
- ☐ The production manager is not used.
- ☑ The production manager is activated. With this setting, stock residual lites are considered for batch optimizations in the production manager. The program does not establish a connection to A+W Production. Instead, production planning is available in the Production module.

**File path** Path for saving the files.

### A+W Production connection

**PPS Webservice URL** Address for the PPS Webservice. PPS Webservice is required for the following transfers:
- Production release after capacity transfer
- Goods received report to A+W Production
- Cancellation

**[Globe]** Checks whether a connection can be established by means of the defined URL.

**Cancellation of production transfer via PPS WebService** File-less transfer to production offers two ways of cancelling orders.
- ☐ Orders to be cancelled are transferred to production by hand, with a cancellation code.
- ☑ Orders to be cancelled are transferred to production via PPS Webservice. The quantities for the corresponding order items are manually set to 0 in the order.

**Cancellation of the production transfer only up to status ready for dispatch**
The cancellation and thus the decreasing of the status can be suppressed if the order has already been produced.
- ☐ Orders to be cancelled are transferred to production by hand, with a cancellation code.
- ☑ Orders can only be cancelled up to the status ready for dispatch. For this, the registration point for the status Order produced at must be defined.
⇨ "Reg. point allocation" on page B-988
At the registration points, a status assignment must be present for this registration point and the assigned status defined whether the order is produced if it is greater than or equal to.

**Message about P.O.** Receipt of ordered goods can be directly reported to production so that the corresponding orders can be produced with the purchased articles.
- **None:** With this setting, receipt of goods will not be reported to the shop floor.
- **By AWPool transfer:** You should choose this setting if production data are saved in a file (AW-Pool or OrderXML).
- **By PPS Webservice:** You should choose this setting for file-less transfer of production data.

### ERP Webservice

**URL** Address for the ERP Webservice. PPS Webservice is required for the following transfers:
- OrderXML production transfer
- Scheduling reports from A+W Capacity Planner
- File-less production reports
- AWPort connection

### Master data transfer and language A+W Production

Master data only have to be maintained in A+W Business and can be transferred to A+W Production.

**Server name** Glass, processing, grills, fillings, articles, spacers, glass type groups, glass types, tables, jumbos, and jumbo/table allocations can be synchronized between A+W Business and A+W Production.
Enter the name of the A+W Production server (DNS name or IP address).
In product management, you also have to define which data will be transferred.
⇨ "Product Management - A+W Production" on page B-693

> **Complete the master data input**
> Enter the server name only after you have entered the corresponding master data. If this field is left blank you can e.g. enter products without transferring data.

**Diff. Diff. production language** OrderXML can transfer product names and text from A+W Business in a language that differs from the language used in A+W Production, e.g. because different languages are used for order entry and for production. The field for selecting the target language is accessible only if this checkbox is checked.
- ☐ The language is the same in both programs.
- ☑ Product names and text from A+W Business will be transferred in a different language and should be translated into the target language. Text changed by hand at order entry will not be translated.

### Online production overview in

With the online production overview, it is possible to generate a report from the PPS Webservice. This production overview can be displayed for several orders at once if it is called from a Number Manager. For this, in the Report parameters field of the Crystal Report, specify the report that should be used for the production overview.
The online production overview draws the data directly from the PPS Webservice.

**Report parameter** Specification of the report parameter in the following form: Report=//awbawp60/Trans/Reports/BDE/AUW_OrderList_Status.rpt&Unterteile_anzeigen=1&Auftrag=[OrderList]
For this, specify the rpt file to be used under report and link the report parameter with &. The text [OrderList] is replaced with the corresponding order numbers before transfer to the PPS Webservice.

### Production report

**[Settings]** Opens the dialog Production reports (interface service) where various parameters for reports per file can be set.
⇨ "Interface service" on page B-1051

**Fileless production feedback** The feedback is stored by A+W Production via the ERP Webservice and booked by A+W Commercial Exchange Server.
- ☐ Feedback from production is not imported online.
- ☑ Reports from production will be imported online. For this, no files are saved. On the tab Stock/PU/EDI, the control elements for management of the individual STS files are deactivated.
⇨ Production, "Reports from Production" on page E-2127

**Book feedback in partial deliveries** The fileless feedback can also book production feedback in partial deliveries with partial invoices.
- ☐ Fileless feedback is not booked in partial deliveries.
- ☑ Fileless feedback is booked in partial deliveries.
For feedback for an order, initially all partial deliveries are sought. The quantities reported are distributed accordingly across the documents found. Here, feedback is booked first to the documents whose delivery date is earliest. This means that the documents should have different delivery dates.
If the feedback of a registration point for a document is complete, it is booked to the following document. Breakage messages always apply only for the original order, excess quantities for the document with the latest delivery date.
Feedback already made is divided up according to the quantities selected when creating a partial delivery. Thus it is not relevant for the booking at what time of production a partial delivery is created.

**Production release for order if sub-order has been produced (STSP)**
This field is accessible only if production reports are imported.
Partial orders can be created for an order. If a production report refers to such a sub-order, the status of the whole order can be changed.
- ☐ An order is not automatically set to the Production release status.
- ☑ When the sub-orders are reported as produced, the status of the main order is automatically raised to Production release.

**Adopt batch no. from order header (STSP)** This field is accessible only if production reports are imported.
If the defined registration point has no status allocated, the report is processed by A+W Business capacity planning, and the status is changed accordingly.
- ☐ The batch numbers of the items are updated separately from the batch number in the order header.
- ☑ After the order header has been updated, all items with an item status over/equal with the status of the registration point produced will get the order number's batch number.
⇨ "Reg. point allocation" on page B-988

**Adopt production rack number for item (STSD)** This field is accessible only in connection with the import of barcode reports.
If the barcode report includes rack numbers of items, these can be allocated to the items in A+W Business.
- ☐ Rack numbers will not be adopted for the item.
- ☑ The reported rack numbers will be saved in the order and allocated to the corresponding item.

**Update production list through registration point (STSG)** The STSG report defines the rack that is allocated to the corresponding order item and the quantities produced. The rack number is printed on the delivery note.
In this field, choose the registration point used by the rack reports to raise the status. Based on the selected registration point, the production list in dialog List of status reports will be updated.
For this, the production status must be selected or defined via the folder symbol.
⇨ Sales, "Status message overview" on page C-1683

**Quantity > Allow item quantity (STSB, STSD, STSG, STSL, STSP)** This field is accessible only if production reports are imported. If the produced quantity is greater than the quantity of the order item, the produced quantity can be taken over.
- ☐ Produced surpluses are not taken over into the order.
- ☑ Produced quantities are taken over into the order item.

**Capacity planning feedback (STSD/STSB)** STSD and STSB reports can be processed by capacity planning (time management).
- ☐ Capacity planning processes no data from STSD and STSB files.
- ☑ Capacity planning will process STSD and STSB files. So that the reporting of A+W Production can be processed correctly, on the Stock/PU/EDI tab, the registration point 700 must be selected.
⇨ "Reg. point allocation" on page B-988

**Create complaint orders (STSB)** This field is accessible only in connection with the import of breakage reports.
- ☐ Complaint orders will not be created automatically.
- ☑ A complaint order will be automatically created based on a breakage report. This function can be allocated a standard cause and a standard reason that can be changed for the individual complaint order.

**Cause** This field is accessible only in connection with the automatic creation of complaint orders.
You can select a cause that is adopted for the automatically created complaint order. It will be loaded irrespective of the settings in Company Data > Archives tab.
⇨ "Default complaint place" on page B-992

**Reason** This field is accessible only in connection with the automatic creation of complaint orders.
You can select a reason that is adopted for the automatically created complaint order.

**Order area** This field is released only in connection with the automatic creation of complaint orders. You can select an order area: the order number will be taken from its number range.

**Target NM** This field is released only in connection with the automatic creation of complaint orders. You can select a number manager to which the automatically created complaint order should be transferred.

**Free** This checkbox is available only in connection with the automatic creation of complaint orders.
- ☐ Automatically created complaint orders are not free of charge as a standard.
- ☑ Automatically created complaint orders are free of charge by default. The setting can be changed in the complaint order.

## Company Data – Shipment

*Master Data > Company > Company data > Shipment tab*

This tab is used to define the settings for rack management and dispatch.

### Number areas

**Rack No. from, to** First and last number of the number range for racks. The number range applies to the current client.
To lock racks for a client, enter 0 in both fields and 1 in field Current.

**Current** Field actual shows the last number assigned by the system.

**Ident. no from, current, to** These numbers define the IDs that can be assigned to racks, and the last assigned rack number.

### Rack load

**for packaging type** Packaging type for which L rack numbers can be assigned. This field refers to module L racks.

### Rack Management

Choose an option to define the type of rack management you are using:
- **A+W Business** This option enables the common rack management of A+W Business.
- **AWRack:** This option enables the rack management (Rack Manager) and gives access to the following fields.

**No writing back of remarks for pick up** Pick-up information can be transmitted in STSK feedback.
- ☐ The pick-up information is written to the remark field for the rack. Thus, manual entries in this field are overwritten.
- ☑ Pick-up information is not written back.

**AWRack Webservice** Complete Internet address for the Webservice Rack Manager.

**CommonBase client** 0 is entered here by default; this has to be changed only if you are using Rack Manager.
The specified values are the IDs for the CommonBase interface.

**CommonBase company group** 0 is entered here by default; this has to be changed only if you are using Rack Manager.

**Default order area for invoices** Select the order area for which rack invoices are issued on a regular basis. You can overwrite this setting when creating invoices in Rack Manager.

**Current client is the default client for invoices** You can specify whether the client for which you are currently setting the company data should be stored in Rack Manager as default.
- ☐ The current client is not the default client.
- ☑ The current client is stored in Rack Manager as default. You can overwrite this setting when creating invoices in Rack Manager.

### Freight costs

If you are using imputed freight costs, you can enter a limit beyond which freight costs become unviable.

**Critical freight cost limit %** Critical freight cost limit. Critical freight cost limit in per cent. If the specified value is exceeded, the figures in dialog Imputed freight costs are shown in red.
⇨ Production, "Freight costs" on page E-2208

**Surcharges/freight revenues** You can specify which surcharges form the freight revenues. This way, you also specify how freight revenues arise for the orders that are sent to the A+W Logistics Optimizer.

### Route optimization

**A+W Logistics Optimizer** In order to work with the A+W route optimizing, you must activate this module.
- ☐ The A+W Logistics Optimizer is not used.
- ☑ The A+W Logistics Optimizer is enabled.

**Changing the shipping date** Update of the shipping date after change in the A+W Logistics Optimizer.
- ☐ The shipping date for the customer is not updated.
- ☑ The shipping date for the customer will be updated after confirmation by the A+W Logistics Optimizer in the order header.

**Changing delivery** Update of the delivery date after change in the A+W Logistics Optimizer.
- ☐ The delivery date for the customer is not updated.
- ☑ The delivery date for the customer will be updated after confirmation by the A+W Logistics Optimizer in the order header.

### MQTT

The settings in this area relate to the feedback service for MQTT. A MQTT-based broker serves as a general data interface to which both client systems and services of A+W Software GmbH are connected. So that the feedback service works, all participants must be logged into the broker. If a client is offline, he receives the message as soon as he is back online. To activate the service, click Activate the Feedback service for MQTT. There are two options available:
- **Delivery:** If this checkbox is enabled, the changes of the delivery date are forwarded to the feedback service and then to the MQTT broker.
- **Shipping:** With processing of the shipping data, the concern is to report order data and its item quantities as well as the information about on which rack the order items should be placed. If the item quantity reported does not equal the original quantity, a partial delivery is generated automatically and set to the reported rack. If the reported quantity is complete, no partial delivery must be generated. Only the order item is assigned to the rack.

Only one of these options can be enabled.

> **Installation and configuration**
> The installation and configuration of this service is done by A+W Software GmbH. If you are interested, please contact your responsible partner.

## Company Data - Capacity Planning

*Master Data > Company > Company data > Capacity Planning tab*

This tab serves to enter the details for capacity planning.

### Automatic scheduling

> To use capacity planning you have to switch off automatic scheduling. Go to tab Parameters and uncheck the checkbox Automatic scheduling.
> ⇨ "Automatic scheduling" on page B-963

### Capacity planning

**Version** For the selection of the program for capacity planning, you must pay attention to how you receive reports from production. You can choose from the following settings:
- **None:** Orders will not be transferred to capacity planning. With this setting you can use both the file reports and online reports.
- **A+W Business capacity planning:** This setting means that you can also use online reports.
- **ALCIM capacity planning:** With this setting you can exchange the following data:
    - Order information, e.g. route.
    - Order status is set by A+W Capacity Planner.
    - Order/time costs for items and BOM elements are set by A+W Capacity Planner.
    - Stock availability check in A+W Capacity Planner.
    - Stock reservations in A+W Capacity Planner.

> **Necessary status allocations**
> A+W Capacity Planner can allocate the status Scheduled and Scheduling error in A+W Business only if the status points 38 and 39 have been allocated.

### Error report from automatic capacity planning

With the selection of this option, you specify to whom error reports are sent.
- **To operator:** This setting means that error reports will be sent to the user who has entered the order in question. These error reports usually refer to dates that cannot be kept because of capacity bottlenecks. This is the default setting.
- **To employee:** This setting releases the field so that an employee can be selected. Select this option if only a single employee processes the orders that cannot be scheduled without problems.

### A+W Business Capacity Planner

**Number of shifts** Number of shifts per day. You specify the shift times in the Capacity planning module on the Calendar dialog.
⇨ Capacity Planning, "Calendar" on page H-2860

**Production scheduling mode** You have to define whether you are going to use open or closed capacities.
- **Automatically normal capacity:** Orders are scheduled according to the shift times available. Overbooking is not possible. This is the default setting.
- **Automatic full days:** With this setting, the specifications on the calendar for the number of shifts and hours are ignored. Scheduling is based on a workday of 24 hours. However, this only applies for regular workdays, not for holidays.
- **Change machine only:** With utilized capacities, there should be an automatic search only for another machine. If it is also at capacity, the scheduling is interrupted and you must intervene manually.
- **Schedule without check:** This setting corresponds to the open shift. This means, for example, that despite the shift time of 8 hours, 16 hours can also be scheduled. Here no message is output if a day is fully utilized.

**Fill shift in case of item splitting** Large items can be divided across several machines, shifts or days. Enter the percentage up to which the machine's shift(s) can be filled by split items in order to leave room for other orders.

**Machine alignment** If you are using several machines that can perform the same work types, scheduling can consider these machines in different ways:
- **Automatic:** The program automatically searches for the most cost- and time-effective machine and schedules the orders on this machine. This is the default setting.
- **Semi-automatic:** The program offers the alternative machines for selection.
- **Manual:** Alternative machines can only be selected for manual scheduling or re-scheduling.

**Scheduling priority** Priorities defined in the order can be taken into account for scheduling:
- **Standard:** The capacities of the required machines are checked and the orders are scheduled according to the priority entered.
- **Low priority:** By default, all orders are scheduled with low priority.
- **Apply changed priority in order:** If the priority is changed during scheduling, it should be written back to the order automatically.

**Max. shift for autom. delivery date calculation (days)** You can specify how many days in the future the delivery date may be shifted automatically.

**Scheduling of P.O. items (only main products)** With A+W Business Capacity Planning, PO articles can be scheduled.
- ☐ P.O. items are not scheduled.
- ☑ The P.O. items are scheduled. can report time costs.

**Scheduling of stock items (only main products)** With the A+W Business Capacity Planning, you can schedule stock items. Thus the time costs can be determined for such items.
- ☐ Stock items are not scheduled.
- ☑ Stock items are scheduled. The time costs can be determined.

**Scheduling of manually entered service items (only main products)**
With A+W Business Capacity Planning, manually entered service items from the main item can be scheduled. The time costs for the items can be determined.
- ☐ Service items entered manually are not scheduled.
- ☑ Manually-entered service items are scheduled. The time costs can be determined.

**Fill history table for completion reports** In the program variant A+W Business Pro, completion reports can be written to the history.
- ☐ Completion reports are not written into the history.
- ☑ The completion reports are written into the history. In addition, the work processes reported complete implicitly with a booking are logged, as well as STSD reports if there is no booking in the capacity planing. STSD reports are logged if no booking is made in the capacity planning. The history can be evaluated in the Statistics module and printed out.

**Autom. delivery date search by route** In case of bottlenecks, it is possible to search for a new delivery date automatically.
- ☐ The next possible date is chosen as delivery date no matter if this is a route day or not. This is the default setting.
- ☑ The program searches for a new delivery date based on the customer's route days. Automatic scheduling selects the new delivery date and saves it in the order.

**Do not split order** Large orders have to be split into smaller portions if processing of the whole item cannot be completed in one day.
- ☐ The orders can be split for automatic scheduling. This is the default setting.
- ☑ The orders can only be split manually. Automatic scheduling of large orders triggers a message to that effect so that you can intervene.

**Reduced scheduling check if structure identical** An order may contain items with the same BOM structure, which differ only according to the dimensions.
- ☐ The entire BOM structure is checked for each item.
- ☑ If the BOM structure is the same, scheduling is based on the previous item without checking the BOM again. This is the default setting.

**Schedule for delivery date** Automatic scheduling generally schedules the orders for the delivery date. The searches for a new delivery date only if there is no free capacity.
- ☐ Orders are scheduled with delivery date search. This is the default setting.
- ☑ Orders are scheduled without searching for an alternative delivery date no matter whether or not there are free capacities.

**Automatic completion report for invoiced orders** Orders can be automatically reported completed.
- ☐ Orders will not be automatically reported completed.
- ☑ Orders will be automatically reported completed if the invoices have already been issued. This setting makes only sense if transfer to production is triggered after the invoice has been issued.

**Transfer to production (OrderXML) incl. planning data** At transfer to production, data can be transferred by OrderXML or Pool.asc.
- ☐ The data should not be saved in the OrderXML file.
- ☑ A+W Business capacity planning data should also be saved in the OrderXML file.

**Use change of shifts table** A 'change of shifts' table can be used for the automatic changing of shifts.

**[Settings]** Opens the dialog in order to define the shift change.
⇨ Capacity Planning, "Shift settings" on page H-2837

**Product classes without status change**
The raising of the item status (order status) can be prevented by completion reports for product classes. Just select the appropriate entries on the list.

**Order areas without scheduling**
You can define that certain order areas are excluded from automatic scheduling. This means that orders for the selected order areas can be scheduled manually only.

### Feedback settings regarding A+W Production Capacity Planner

**Update time costs** A+W Capacity Planner can report time costs.
- ☐ Time costs will not be updated.
- ☑ Time costs will be updated.

**Check stock availability** Capacity planning checks if enough of the materials required are available on stock.
- ☐ Availability of stock articles will not be checked.
- ☐ Availability of stock articles will be checked. If there is a shortage on stock, a task will be entered for the user.
- ☑ Stock information will highlight any articles of which there is not enough stock and which might therefore endanger the scheduled delivery date.

**Barcode reports** Fileless reporting of completion messages can be imported from A+W Business Pro and imported into the A+W Barcodescanner.
- ☐ Reports are not imported via barcode.
- ☑ Reports about the lites are imported via barcode. This settings must be activated both in the purchasing and supplying companies.
For this, barcodes in all participating operations must be identical. The barcode is transferred and also written back to the order in the Complete Scheduling report.

**Update production date** If capacity planning realizes that the original production date cannot be kept, a new date will be reported.
- ☐ The production date will not be updated in the order.
- ☑ Based on the report, the dates for the start and end of production will be updated in the order header. The earliest date for all products of the order will be used as the start-of-production date. For the end of production, the program will use the latest date defined for any of the order items.

**Check replacement time for purchased products** Capacity planning checks if there is sufficient time for replacing the necessary materials so that the order can be produced in time.
- ☐ The replacement time for stock articles will not be checked.
- ☑ The replacement time for stock articles will be checked.

**Don't check whether all items have been reported** For the feedback for the scheduling in A+W Production it is possible to check in the ERP Webservice whether all necessary items have been reported back.
- ☐ The completeness of the feedback is not checked.
- ☑ The completeness of the feedback is checked. Here, partially-delivered items are also considered. The following items are not reported back:
    - Service or surcharge items
    - Items with numbers greater than or equal to 900
    - Article items if no item transfer is activated
The check also considers partially-delivered items.

**Del. date can be changed indep. from scheduling** By default, the delivery date of scheduled orders can only be shifted to an earlier date if the status of the order was changed in advance.
- ☐ The delivery date can only be changed if the order status is reset.
- ☑ The delivery date can be changed after scheduling and production beginning.
    - Here it is not checked whether this is still possible in production. The order is not canceled automatically.
    - If the order has already been transferred to A+W Capacity Planner (EL), an entry is written to the order history.

**Direction of the delivery date update** If the delivery date may be changed, you can specify whether an earlier or later delivery date is calculated automatically and written back to the order.

**Evaluate A+W Production document type in case of feedback from Capacity Planner**
Choose an option to define how documents should be transferred by A+W Business:
- **Search for quotation or order:** Both orders and quotations are transferred to production. With this setting, the two document types have to have separate number areas.
- **Always as order (must be active for capacity transfer):** You have to choose this setting if you are using OrderXML transfer and A+W Capacity Planner (EL).

## Company Data – Miscellaneous

*Master Data > Company > Company > Miscellaneous tab*

This tab is used for making the settings for importing products from the suppliers Dorma, KI-Megla, and Schlechtendahl. The settings are read by the module BMECat import.

You can also make the settings for the connection with MS Outlook.
Automatic purchase orders for Dorma and the export of invoices, delivery notifications, and order confirmations in openTrans format are exchanged via A+W Commercial Exchange Service.

> **Data import**
> Import of data is started via module BMECat. To import data from Dorma's website you have to enter the URL and access data on tab Stock/PCH/EDI.
> ⇨ "Company Data – Stock/Purchasing/EDI" on page B-981

### Settings for BMECat import

The following settings can be made for the suppliers who provide their product catalogs in BMECat format.

**Template product** Number of the product based on which the imported articles should be set up.

**Matchcode prefix for product** Code for the supplier in question. The supplier codes must be different, e.g. D. for Dorma, M. for Megla, S. for Schlechtendahl.

**Product number from** Product number from which on products should be imported.

**Price list, Price key** Price list and key valid for the products of the supplier in question.

**Variants from table number** Number of the price table for colors (variants).

**Import of short descriptions, product info, pictures** You can import further product data from the corresponding suppliers.
- ☐ Short description, product info, and/or pictures will not be imported.
- ☑ Short description, product info, and/or pictures will be imported.

### Link to Outlook

Outlook contacts can be linked with A+W Business so that these data do not have to be entered again.

**Import customers, suppliers, partners** You can import the Microsoft Outlook data from your business partners to make them available in A+W Business
- ☐ Data will not be imported.
- ☑ Data can be imported.

**Exchange name and surname of market partners, employees** You can exchange the names and surnames in the email addresses of your business partners or of their employees at data import in order to adjust the display.
- ☐ First and last names will not be exchanged.
- ☑ First and last names will be exchanged.

**No transfer of market partners if email address/phone number is missing** You can prevent the export of partner data to Outlook if no email address and/or phone number has been entered for the contact.
- ☐ All data will be exported.
- ☑ Data will not be exported if there is no email address and/or phone number.

**Transfer all market partners (not only those assigned to the person in charge)** The export of market partners can be based on the employee they are assigned to.
- ☐ Only data assigned to the current employee/user will be exported.
- ☑ All market partner's data will be exported.

## Portuguese Certification

*Master Data > Company > Company Data > Parameter tab > [Parameter Management]*

This dialog serves to make the settings for Portuguese certification.
In dialog Form/label printing you can create digital signatures for the print mode Invoices (orders) and Credit notes.
When printing is started, the private key is used to create the signature in the background; among other things, the signature includes the invoice number and invoice date. The certification code plus four digits of the signature will be printed.
The document status is changed to Invoice printed. After that, the invoices must not be changed.

> **Requirements**
> You have to define a lock status for printing invoices. In addition to that, the right to change invoices must be withdrawn for all users in management of rights. At least one user must be entitled however to cancel the invoice in document management.
> If the current document is part of a collective invoice, all documents belonging to this collective invoice will be cancelled.

**Private key, Public key** When you open the dialog for the first time, the private and the public keys for the digital invoice signature will be created. These will be saved in the current user's temporary Windows directory, and in the database.

**Certification code** The certification code is assigned by the Portuguese government.

> **Parameters cannot be changed**
> These three parameters cannot be changed after saving.

### SAFT-PT export parameter

All printed invoices and credit notes referring to a certain period can be exported to a XML file. This file can be created in module Documents in dialog SAFT-PT Export.
The business year, the start and end date, and the file path must be defined there. Based on the defined business year, even archived documents can be exported.

**Audit file version, Company identification, Territory** Enter the data in the appropriate fields. These will be included in the signature.
The remaining fields will be filled from the system data entered at installation.

## Employee

*Master Data > Company > Employees*

This dialog is used for entering and maintaining details on your staff.

> **Prerequisite**
> Employees' data can only be entered or amended by the system administrator.

Dialog Staff offers the following tabs:
- Employees - Employees
- Employees - Specification
- Employees > Settings

### Employees – Employees

*Master Data > Company > Employees > Employees tab*

This tab is used for entering new employee data. All fields with blue lettering are mandatory fields. To edit the data of an employee, select the corresponding entry on tab Table.

> **Observe data protection**
> Personal data are subject to data protection. Please make sure that this kind of data is protected from misuse by means of the appropriate access rights.

#### Identification

**Name (plain)** Complete name of the employee. Once saved, it cannot be changed.
This name will be saved for every action this employee performs in A+W Business. We recommend entering the full name for clarity's sake.

**Login name** Name the employee uses for logging into A+W Business.

**Domain** Name of the domain if A+W Business is installed in a network.

#### Address

**First/last name** Name of the employee as kept in the personal file.

**Street, Country/Post code/City** The employee's address.

#### Contact

**Extension** Internal phone number by which the employee can be reached.

**Phone 2-4** Further phone numbers, e.g. the mobile phone number for sales representatives.

**Fax** Fax number the employee uses for sending and receiving faxes.

**Email** The employee's email address.

#### Overview

The list shows all employees specified in A+W Business.

## Employees – Specification

*Master Data > Company > Employees > Specification tab*

This tab serves to enter further details on the employee, e.g. position, title, authorization group.
The fields in section Identification are described in connection with the tab Employees.
⇨ "Employees - Employees" on page B-1031

### Access rights

**PASSWORD** Password the employee uses for logging into A+W Business. If the Windows login has been enabled in company data, login by means of a specific A+W Business password is impossible.
Access via A+W Business Connect requires a password in any case.

**Ext. customer no.** This field is used with module A+W Business Connect. For all internal users, the entry is 0 (<n.e.>).
If one of your customers wants to use document entry via A+W Business Connect, he has to be registered as an employee. Select his company's customer number in this field so that he can only view the documents related to his company.
Access rights can be restricted further in management of rights, e.g. for the input of credit notes.

**Locked** A user can be locked for logging into A+W Business. This is e.g. necessary when an employee leaves the company. The employee's data cannot be deleted from the database because they refer to various documents etc.
- ☐ The user is been locked.
- ☑ The user is locked and cannot access A+W Business. His name will still appear in documents though.

### Specification

**Function** The employee's position in the company. You can choose from all positions entered in master data.
⇨ "Title (Function)" on page B-799

**Titles** Titles entered in master data.
⇨ "Titles" on page B-799

**Group** Employees can be allocated to user groups. By means of groups, certain rights in A+W Business can be easily controlled. Groups are defined and maintained in dialog User groups.
⇨ "Employee Groups" on page B-1036

**Birthday** The employee's birth date.

### Menu + A+W CAD Designer

**Language** Language in which the menus appear in A+W Business and A+W CAD Designer. This does not include the display in the dialogs or entries in the fields.

### Documents

**Restrict documents to client** You can assign a user to a client.
- ☐ The user is not assigned to any client.
- ☑ The field is accessible for selecting a client. The user is assigned to the selected client. He will be able to enter and edit documents only for this client.

### Output

**Printer** Printer to be used by default. You can choose another printer if the user should not use the standard printer for his documents and lists.

**Fax** Fax used by default, e.g. Twinfax. If you do not use the A+W Business fax module please enter the standard printer.

### Time registration

**Employee no.** The user's employee number. It serves just for information and will not be analyzed by A+W Business.

### Interface service

**User for interface service** You have to enter a (virtual) user for logging into the interface service.

## Employees > Settings

*Master Data > Company > Employees > Settings tab*

This tab serves to allocate a document type and/or order area to the user.
⇨ Tutorial 1, "Input of User Data" on page B-462
The fields in section Identification are described in connection with the tab Employees.
⇨ "Employees - Employees" on page B-1031
