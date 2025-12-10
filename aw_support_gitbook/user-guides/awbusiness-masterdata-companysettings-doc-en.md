---
description: "EN_AWBusiness_Master_Data_9_10-2"
---


---
## Company Settings

### Create/update customer also in FinAcc main client
Only for Syska financial accounting system. If customers of a client are transferred to financial accounting, you can define whether these customers should be entered as customers of the main client.
- [ ] The customers of the current client will not be entered as customers of the main client in financial accounting.
- [x] The customers of a client who is not the main FinAcc client, will be created or updated as customers of the client who is the main FinAcc client.

### Read and write files in Unicode format
This setting depends on the system used to exchange data.
- [ ] The files will be read and written in the code in which they were created.
- [x] The files are read and written in Unicode.

### Compare new customer number with FinAcc
Only for Syska financial accounting system. When new customer data are entered, the program can check whether the chosen customer number already exists in the financial accounting system.
- [ ] The new customer number will not be checked.
- [x] When comparing master data in Syska financial accounting, the program checks if the number of the new customer already exists. If so, an error report will be issued. You will have to enter another customer number for this customer in this case.

### FinAcc main client
Only for Syska financial accounting system. If you are using several clients, one of them must be presented to the financial accounting system as the main client.
- [ ] The client whose settings are currently edited is not the main client for financial accounting.
- [x] The current client is the main client for financial accounting.

### Transfer cust. account instead of cust. no.
The customer number will be used as an account number by default. Instead of the customer number, the debtor number can be entered in customer master data.
- [ ] The customer number is transferred to financial accounting.
- [x] The account number is transferred to financial accounting. This account number must be entered in customer data. This setting will overrule the settings in customer master data.
⇨ "Main acct." on page B-776

### FinAcc database
You have to fill in these fields only if you are using SQL financial accounting that allow direct exporting.

**Server**
Name of the server containing the financial accounting database.

**Database Name**
Name of the financial accounting database.

**Login**
User name by which A+W Business registers with the financial accounting database.

**Password**
Password by which A+W Business registers with the financial accounting database.

### Options for open items—report

**Create backup file, path**
This field is accessible only in connection with the import of receivables reports. You can save an additional backup file and enter the number of days for which it is going to be saved.
- [ ] No backup file will be saved for the receivables report.
- [x] A backup file of the receivables reports (including a time stamp) will be saved elsewhere. The fields for selecting the directory and the storage days are made available.

**Storing days for backup files**
This field is available only if a backup file is going to be saved. You can enter the number of days for which this file must remain unchanged.

## Company Data > Documents

This tab is used for defining options for document output.

### Choose shape catalog

**Shape catalog**
A+W Business uses the A+W Software GmbH shape catalog by default. You can choose different catalog for your clients.
⇨ Sales, "Shapes" on page C-71

### Lock code
Lock codes are used to exclude documents from certain steps of automatic processing.
⇨ Tutorial 2, "Lock Code" on page B-425

> **Prerequisite**
> Lock codes must be defined in dialog Lock codes so that they can be selected in the appropriate fields.
> ⇨ "Lock Code" on page B-897

**Complaint**
Lock code for complaints. This can be changed in the individual documents.

**Partial delivery**
Lock code for partial deliveries. This can be changed in the individual documents.

> **Activate setting for customer**
> If a customer should be able to get a partial delivery without partial invoice, define this in customer master data using the checkboxes Partial delivery and Partial invoice.
> ⇨ "Partner Management - Order" on page B-763

### Fax/Email - Options

> **Prerequisite**
> A fax number and email address have to be entered in partner management, and fax and email despatch have to be enabled.
> ⇨ "Partner Management - Order" on page B-763

**Fax dispatch per document**
Documents can be faxed.
- [ ] The documents are collected and faxed to the partner.
- [x] Documents are dispatched individually by default. You should maintain this setting to avoid bottlenecks.

**Email dispatch per document**
Documents can be emailed in various formats.
- [ ] The documents are collected and emailed to the partner.
- [x] Documents are emailed individually to the partner. You should maintain this standard setting to avoid bottlenecks.
Please remember that RTF dispatch will not display shapes and other graphics correctly.

### Compulsory shape dimensioning

> **Avoiding calculation errors**
> To avoid pricing errors, you should enable Compulsory shape dimensioning for all documents if edgework by linear meter is also active on tab Parameters.
> ⇨ "Calculate edgework with exact lm" on page B-934

### Quotation, Order, P.O.
Usually, sizes are entered in the documents. Input of sizes should be compulsory for orders and purchase orders while they may be omitted from quotations.
- [ ] You do not need to enter shape sizes in documents. The sizes are checked when copying from Quotation to Order; the system will ask you to enter sizes if necessary.
- [x] Sizes have to be entered in documents (quotation, order, P.O.). For Order and P.O. the checkboxes should remain enabled by default (necessary for production).

### Mixed calculation factors
If you are using mixed calculation, you can enter factors for price calculation.
⇨ Tutorial 2, "Mixed Calculation" on page B-533
⇨ "Items - Supplement" on page C-502

**Double IG**
The factors for double IG can be chosen at random, e.g. 0.5 / 0.5.

**Triple IG**
The factors for triple IG can be chosen at random, e.g. 0.5 / 0.8 / 0.5.

### Allocate numbers per page

**Delivery note printing, Invoice printing**
Certain countries require that every page of a delivery note or invoice gets its own number.
- [ ] By default, delivery notes and invoices will be numbered by document.
- [x] Every page of the delivery note or invoice will get its own number.

### Credit note/invoice number
Separate number ranges will be set up per document type.

**Credit note number = document number**
By default, credit notes are independent documents with a separate number range.
- [ ] Numbers from the invoice number range will be used for credit notes.
- [x] Numbers from the credit note number range will be used for credit notes.
⇨ Tutorial 2, "Definition of Number Ranges" on page B-437
⇨ "Number Ranges" on page B-890

### Change of delivery date
You can prescribe a mandatory reason for a change of delivery date for orders. The specification of a reason will be required in the following cases:
- Order entry if order will not be entered anew
- Document Data
- Route list
- Consignment

In the manual note of the order history, the old and new delivery dates and the reason entered are visible. If more than one order is changed, the dialog appears per changed order. However, it is filled with the value previously entered and can be taken over with the same reason.

If the order is shifted by the production system during scheduling, the entry is made automatically with the reason `Delivery date calculation with A+W Production`. If the delivery date shift is made due to a rescheduling in the production system, the comment entered there is used as text.

**Entry in history with comment starting with status**
For a manual change of the delivery date, the specification of a reason can be made mandatory.
- [ ] The change of the delivery date does not have to be justified in the history.
- [x] In the history, an entry is created if the delivery date was changed starting with the set status. The entry of the reason is mandatory and cannot be canceled. The setting applies for the following program areas: Order transfer, Document data, OC supplier, Receipt of goods, and in the Picking.
The field for selecting the status is activated.

### Turning shapes

**Shapes can be turned on processing dialog**
Shapes with shape numbers smaller than 137 can be turned on the processing dialog. Excluded here are the shape numbers 0, 24, 98, 99, 60, 61, and 81.
- [ ] The shapes cannot be turned.
- [x] The shapes can be turned: here, the available angles are 90, 180, and 270 degrees. The printout reflects the turned shape.

### Glass door system data source
The field refers to the module AWDoor.

**ODBC DSN**
Enter the name of the database connection configured in Windows.

### Price below minimum

**Password**
Enter a password to avoid that minimum prices are not inadvertently. The system will automatically ask for this password if the defined minimum price is not met at order entry.
By passing on this password you can control how many users should be entitled to negotiate individual prices.

### Project management

**Active project management**
Different settings are available for using the project management functions.
- None
- Invoice management (customized setting)
- Invoice management with allocated orders
- Extended project management
- Standard project management
- Standard project management + invoice management with allocated orders

The differences between the settings are described in detail in the tutorial.
⇨ Tutorial 1, "Projects" on page B-123
⇨ Tutorial 2, "Project/Invoice Management" on page B-494

### Product ID
You can set the appropriate modes for CEKAL classification or quality text. Prerequisite is a valid licence for the corresponding method. If product identification is inactive, the user will be informed accordingly when selecting the dialog in question.

**Active marking**
Product code:
- **None:** With this setting, the product code will not be checked.
- **CEKAL classification:** With this option, the spacer text will be set acc. to CEKAL classification.
- **Quality code:** With this option, the restrictions from dialog Quality text will be taken into account.
⇨ "Quality Text" on page B-581

### File attachments
Files can be attached in partner and document management.

**Path Path**
Enter the path for saving file attachments. In this directory, a subdirectory will be created by customer or order to save the annexes in.
Please make sure that this directory is available on a central computer, accessible to the users.

### Declaration of Performance

**Sending of declarations of performance**
You can specify whether declarations of performance should be sent.
- [ ] No declarations of performance will be dispatched.
- [x] Declarations of performance are dispatched for the allocated partners and products.
The field for selecting the standard declaration of performance is released.

**Standard Declaration of Performance**
You can define a declaration of performance (DoP) to be dispatched by default if no specific DoP is allocated in the order.

**[Directory]**
Opens the dialog Declaration of performance management where you can enter the declaration of performance (DoP).
⇨ "Declaration of Performance, Management" on page B-583

**[Zoom]**
Opens the dialog Search declaration of performance from which you can select the standard declaration of performance.

**Size restriction for email dispatch ... MB**
For the sending of declarations of performance, you can specify an upper limit in MB. For documents that exceed this value, the e-mail is split in several parts.

**Use A+W SLT interface**
For data transmission in the B2B module, A+W's own interface can be installed.
- [ ] The A+W SLT interface is not used.
- [x] The A+W SLT interface is used. With this setting you can specify where the interface file is stored if a different installation path was used.

**Different installation path**
Specification whether a different installation path was used for the A+WSLT.exe interface file.
The field is only enabled if the A+W SLT interface is activated.
- [ ] The interface file is installed in the standard installation path.
- [x] The interface file is installed in a different installation path. For this, you must specify the path.

**(Path)**
Specification of the installation directory for the interface file A+WSLT.exe.

### CEKAL parameters
These settings are only used in France.

**Default text**
These fields refer to the CEKAL module.
There are two ways of allocating a general standard CEKAL text:
- Enter the standard text at this point. This text will appear automatically whenever you enter an item.
- Or leave the fields in dialog Text allocation blank and allocate the standard text. This text will appear only if no other CEKAL definition is found.
⇨ “CEKAL” on page B-1070

**Center no.**
Company number in connection with CEKAL certification. This number can differ from the company number on tab Client.

## Company Data – Parameters

This tab is used for defining the options for the documents. Amendments on this tab will overrule the standard calculation in A+W Business.

### Parameters for document entry

**Calculate edgework with exact lm**
Depending on the national customs, edgework can be rounded by default.
- [ ] Edgework will be calculated with linear meters rounded.
- [x] Edgework calculation is based on the exact sizes.
⇨ "Rounding" on page B-880
⇨ "Compulsory shape dimensioning" on page B-929

**Logo entry**
To print a logo you have to define the logo position for shapes and rectangular lites in master data, for every customer.
- [ ] The logo will be added to the BOM by default.
- [x] The logo is automatically printed on the (toughened) lite. This setting can be changed by customer.
⇨ "Logo Position" on page B-841

**Actual product groups for BOM search**
The logo can be entered in master data for a main product or for the product group. For items with a bill of material, the automatic search for a logo can be started from the main product or from the product group.
This checkbox is accessible only if logo entry is active.
- [ ] By default, the program will search for the logo based on the main product.
- [x] For elements on the first BOM level, the program searches for the logo by means of the BOM element's product group.
With this setting, the program will search e.g. for the logo of a laminated lite irrespective if it is entered as a main item or if it is exchanged in the IG's BOM.

**Do not delete partial delivery item**
Orders can be executed as partial deliveries, with or without partial invoicing. This setting can also be made by customer.
- [ ] By default, the items of a partial delivery will be deleted from the original order after the item has been completely shipped.
- [x] If partial delivery is combined with partial invoicing, the shipped items will not be deleted from the original order. Completely shipped items will be set to 0.
⇨ "Partner Management - Order" on page B-763

**Adopt partial delivery date from original order**
For partial deliveries, the order date can be updated in the delivery note.
- [ ] By default, today's date is entered as entry date of the partial delivery for each creation of a partial delivery.
- [x] The entry date of the original order will be used for the partial delivery.

**Raise status when credit limit is exceeded**
The customer's credit limit is checked when the order is saved at order entry.
If the credit limit is exceeded at order entry, the following actions can be released:
- The system issues a message but the order can be entered completely.
- The order cannot be entered.
These settings are made in every customer's master data.
⇨ "Credit limit" on page B-778

If the credit limit is exceeded at order entry, the system will automatically set the order status to `700 Credit limit exceeded`.
These orders can be selected via number manager. After that, you have to decide if the order can be released for production, or remains locked for further processing.
⇨ Tutorial 1, "Credit Limit for Customers" on page B-90

> **Assign user status**
> There has to be an appropriate user status for status point 700; this is allocated in dialog Status allocation. If an order has been automatically set to status 700, and you reset the status manually, the system will not automatically raise it again.
> ⇨ Tutorial 2, "Status Administration" on page B-418
> ⇨ "Status Allocation" on page B-886

**Enable deviating procurement type per client/order area**
If you are working with clients, the procurement type of the product can be set per client.
- [ ] The procurement type is set across the board for all clients.
- [x] The procurement type can be set per client. For this, in the product master data, the deviating product code per product and client must be specified.

> **Example**
> The company has the production scheduling TSG and IGU. The IGU production scheduling IGU orders a TSG for the production scheduling TSG, e.g. a 6 mm TSG.
> This product 6 mm TSG has the procurement type `Production` in the production scheduling TSG and the procurement type `Purchase order` in the production scheduling IGU.
> ⇨ "Product Codes" on page B-608

**Enable search by product code**
Procurement types are allocated to products in product management. You can also allocate other procurement types by client and order area in dialogue Product code management.
- [ ] You should disable this checkbox if you do not use different procurement types for the same product. This will help to relieve the system.
- [x] The program checks if different procurement types are allocated to the same product. Depending on the order area, the product will be produced or ordered.
⇨ "Product Management - Stock/Purchase" on page B-606
⇨ "Product Code Management" on page B-630

**Interactive sales commission**
By default, the sales commission is calculated when documents are transferred to archives. Checkbox `Transfer to commission statistics` must be active on tab Archives for this purpose.
The sales commission can be entered or changed by item at order entry.
- [ ] The commission rate will not be displayed at order entry. At transfer to commission statistics, the commission rates defined in master data will be used to calculate the commission.
- [x] The commission rate will be displayed at order entry. To calculate the commission, you still have to transfer the orders to commission statistics via dialog Transfer to archives.
⇨ "Automatic options" on page B-966
⇨ "Commission" on page B-1017
⇨ Sales, "Transfer to Archives" on page C-684

**Save manual changes in reference document**
If the supplier's price is changed in a reference P.O., it can be saved in the order.
- [ ] Changed entries will not be saved in the reference document by default.
- [x] The changed entries should be adopted for the reference document:

**Referencing document**
Specification of how the changed values should be taken over.
- **Yes, No:** The changed value is only saved if the additional query displayed has been confirmed with [Yes].
- **Always:** The changed entry is saved always, without checking.
- **Never:** The changed entry will not be saved. No question will be displayed.

**BOM transmission of variants**
If a BOM element is replaced by a variant on top or medium BOM level, the variants of the related elements can be replaced automatically.
- [ ] Changes made to a BOM element will not be passed on to the sub-elements.
- [x] If e.g. the color of a product containing BOM elements is changed at item entry, the color of all sub-elements will change automatically.
⇨ "Product Variants" on page B-641

**Enter rectangular cut-outs as width x height**
The marking of corner cut-outs can be reversed.
- [ ] Sizes are entered sequentially after the pattern A-B-A-B.
- [x] Edge cut-outs are entered according to the standard pattern, i. e. A always represents the width and B, the height.

**Check number ranges in orders**
You can enter the order area in existing orders.
- [ ] The order area can be changed no matter whether a number range exists for the (new) order area.
- [x] The order area can be changed only if there is a number area for the (new) order area. The document number remains unchanged.

**Exchange spacer with BOM (gas)**
The airspace can be entered as a product with the BOM element gas. You can define what should happen when the airspace is changed.
- [ ] The gas will not be changed automatically if the airspace changes. It does not matter whether or not the gas is allocated to the airspace.
- [x] When you change the airspace, the BOM element gas will be changed too. This setting is useful if you have defined airspaces with gas.

**Lock documents after printing the invoice**
An order can be edited until the lock status `Document changed` has been reached.
- [ ] By default, the order is locked against changes by means of the lock status. This status can be reset.
- [x] After printing the invoice, the order is locked and cannot be edited. The lock refers to the invoice number created at printing. It cannot be undone.
⇨ Tutorial 2, "Lock status" on page B-423
⇨ "Status Allocation" on page B-886

**Lock documents starting from status point**
A document can be locked for editing after it has reached a defined status.
The document will be locked completely from the defined status on. Items cannot be edited either.

**Automatic scheduling**
Automatic scheduling does not pass on orders to capacity planning or production.

> **Automatic scheduling vs. capacity planning**
> You must not enable this function when working with A+W Business Capacity Planner.

- [ ] Orders will not be passed on to automatic scheduling by default.
- [x] Orders are automatically passed on to automatic scheduling (in the background).

**Tax calculation on item/BOM level**
The tax is usually calculated when the order is saved and the dialog closed.
- [ ] The tax is calculated for the entire order value.
- [x] The tax is calculated on BOM level, for every BOM element. This calculation type is quite tedious and should be enabled only if legislation requires.

**Create product description from BOM**
In product definition, you have to enter a name for the product in field `Name 1`. This name can be created automatically for IG and laminated glass products with bills of materials.
- [ ] The name of the main product will be kept as a standard.
- [x] Name 1 for the main product consists of the names of the individual BOM elements.

**Duplicate check if credit limit exceeded**
The system automatically checks when a document is entered or edited whether another document exists that includes the same product, product structure, and sizes.
- [ ] The duplicate check is not performed if the credit limit is exceeded.
- [x] When exceeding the customer credit limit, a duplicate check is performed and the status adjusted if necessary.

**Quotation entry for locked customers**
Customers can be locked via the customer master data so that no documents for them can be entered.
- [ ] For locked customers, quotations can only be entered if the lock is lifted in the customer master data.
- [x] Quotations can be entered for locked customers without lifting the lock in the customer master data. When entering the customer number, a warning message is displayed. No order can be generated from a quotation that was entered despite the lock as long as the customer is locked.

**No copy of quotations after orders if credit limit exceeded**
Orders can be generated from quotations for locked customers with the copy function.
- [ ] For customers with credit limit lock, orders can be generated from quotations nevertheless. For the new order, the corresponding status is set, `Locked credit limit`.
- [x] For customers, no orders can be generated from quotations if the credit limit is exceeded and the customer is therefore locked. When starting the copy process, an appropriate message is output.
With this setting, orders via quick entry are also possible.

**Maintain production BOM structure in case of changes**
In case of a change, you can adopt the BOM structure of a glass if the new glass has no a BOM with production BOM structure.
- [ ] The exchanged (new) product will be adopted including its production BOM structure.
- [x] If the new glass has no BOM, the BOM structure of the original production BOM will be kept.
⇨ Tutorial 1, "Price- and/or Production-Relevant" on page B-181

**No shipping/delivery on weekends**
You can define the calculation type for dates. You also have to enter the corresponding lead days.
- [ ] Weekends will not be considered as dates for possible shipments and deliveries. Goods will not be shipped or accepted on weekends.
- [x] Goods can be shipped and accepted on weekends.
⇨ "Lead days" on page B-972

**Use virtual item numbers**
Receipt of boxes with an item quantity of >1 has to be booked for each box separately. Virtual item numbers are defined for every box for this purpose.
- [ ] Virtual item numbers will not be used.
- [x] Upon receipt, every box gets a virtual item number so that it can be registered and booked with its own ID.
➡ Kistenmanagement, "Lagerverwaltung von Kisten" auf Seite K-49

**Change procurement type if maximum stocksize is exceeded**
The procurement type of products can be automatically changed to P.O. if the maximum stock size is exceeded at order entry.
- [ ] The procurement type will not be changed automatically if the maximum stocksize is exceeded in the order.
- [x] The procurement type will be changed automatically if the maximum stocksize is exceeded in the order.

**Always adopt product text from BOM**
Product management allows to enter product text to be displayed in field `Article info`.
- [ ] Only the main product text will be displayed as article info.
- [x] The text for the BOM elements will be displayed as well.

**Adopt P.O. text 1 and customer item for document references**
Document references can be created on item level for electronic data interchange. These are necessary for automatically referring order items to the corresponding P.O. items.
- [ ] References will not be created on item level.
- [x] When an order is entered by hand, document references are automatically created from the `Purchase order 1` field in the order header, and the customer item field at item entry.

**Laminated glass production BOM breakdown based on the procurement type**
Laminated glass can be produced or cut. Based on the procurement type, individual lites or the entire laminated unit has to be processed.
- [ ] The production BOM will always be broken down.
- [x] If the procurement type is `Cutting`, the production BOM will not be broken down for the processing steps.

**Determine tax, salesman, and VAT ID based on the shipping address**
You can define whether the shipping address determines the VAT ID.
- [ ] The shipping address is determined based on the main customer's data.
- [x] The shipping address is chosen based on the VAT ID. For printing collective invoices this means that a new collective invoice will be started when the VAT ID changes. For printing collective invoices, invoices have to be sorted by shipping address.

**Print code in case of exchange**
The print code for BOM elements can be controlled in general.
- **Standard:** The print code is kept as defined for the main product.
- **Always active:** The print code is enabled with every exchange.
- **Acc. to exchange product:** The print code will be set as defined for the basic product of the exchange article.

> **Example**
> The print code can be disabled for toughened glass arrissing in the BOM because this processing step is done by default. If this processing step is replaced by the processing step `Polishing`, the changed processing should be printed on the forms however.

**Order-related purchase orders can be changed**
Changes in reference purchase orders can refer to the shipping and production dates as well as to the quantities ordered.
- [ ] Reference purchase orders cannot be changed.
- [x] Reference purchase orders can be changed. The changes will be saved in the order.

**Outside coating/pattern facing away from airspace/film as from 2nd lite**
You have to define the way in which coated and patterned lites are to be fitted into multiple IG or multiple laminated glass lites. You can define a default for this which can be changed in the order if required.
- [ ] The lites will be fitted as defined in glass master data. When exchanged in an IG or laminated glass unit, the coated or patterned side will be turned from the second lite on, to face the airspace or the film layer.
- [x] If the coating or the pattern has been defined as outside in master data, the program must check in case of an exchange whether these lites should be actually facing away from the airspace or the film layer.

**Enable Brazilian tax**
This setting is only valid for Brazilian taxation.
- [ ] The tax will be calculated according to the settings in product master data.
- [x] The tax will be calculated according to the tax matrix and to the formulas for Brazilian tax.

**Import/export of payments**
This setting only applies to the Brazilian payments. This field is accessible only if Brazilian taxation is active.
- [ ] Import and export of payments to the bank is not enabled.
- [x] Payments to banks are made by data transfer. The appropriate formulas have to be defined for this purpose.

**Enable Portuguese certification**
For the Portuguese market, invoices and credit notes can get a digital signature that is certified acc. to certain parameters. This function can only be enabled by the system administrator.
- [ ] Portuguese certification is inactive.
- [x] The [Parameter management] button is accessible.

**[Parameter management]**
Opens the dialog Portuguese certification where you can set the parameters for the certification (signature). This button is accessible only if Portuguese certification is active.
⇨ "Portuguese Certification" on page B-1001

**Apply product exchange rules for BOM exchange**
You can specify that in IGU and LSG, only glass, spacers, and foils can be installed that are intended and suitable for these products.
- [ ] No rules are specified for the product exchange in IGU and LSG.
- [x] For the exchange of BOM elements, the rules are applied that are specified on the Exchange groups and Exchange allocations dialogs.
⇨ "Exchange Groups" on page B-584
⇨ "Exchange Allocations" on page B-585

**Edge processing on LAMI creates size allowance in order**
Specification whether a size allowance is calculated if a LAMI with edge processing is ordered.
- [ ] The PO is forwarded unchanged.
- [x] For the generation of the PO, there is a check whether an edge processing (block grinding) affects an ordered part within the block. If this is the case, the size allowances of the processing are added to the dimension of the glass ordered. Here it doesn't matter whether or not the processing is also ordered.

**Placing the edge processing at the Lamy leads to size correction in the P.O.**
Specification of whether a dimension surcharge is calculated if an LSG with edge processing is ordered.
- [ ] The purchase order is forwarded unchanged.
- [x] During the generation of the purchase order, it is checked whether an edge processing (block grinding) affects an ordered part within the block. If this is the case, the dimension surcharges for the processing are added to the dimensions of the glass ordered. Here it does not matter whether the processing is also ordered or not.

**"No layer" selectable**
Specification of whether layers are shown for coatings if only valid layers for processings are shown.
- [ ] The setting for processing layers is not expanded.
- [x] The setting for processings is expanded for coatings to include the selection No layer. This setting only makes sense if the display is restricted for processing layers.

**Delete inferior edge processing**
Specification of whether for edge processings all processings should be executed if they differ only in the quality, e.g. seaming and polishing on the TG.
- [ ] All edge processings are executed as they are entered.
- [x] Only the superior edge processing is executed. The inferior edge processing is ignored.
If an edge processing should therefore affect no edge, then the whole processing is deleted from the BOM.
In the import settings for customers, you can also activate the Delete inferior edge processing on the glass option for this.
⇨ "Customer, Supplier - Parameters" on page B-1096

## Company Data > Price Calculation

This tab is used to adapt the pricing to your company's or country's requirements.

> Amendments on this tab will overrule the standard calculation in A+W Business.
> ⇨ Tutorial 1, "Price Master Data" on page B-211
> ⇨ "Price Management" on page B-710

### Pricing parameters

**Price calculation for orders**
> You can define different prices and discounts for the same product for a customer. Individual prices will always override discount agreements.
> The standard rates will always be used if the program cannot find any discount agreement.

**Several individual prices permitted**
You can enter customized prices in addition to standard prices.
- [ ] You can enter just one individual price per customer and product in price management. This will be automatically determined at document entry.
- [x] You can enter several individual prices per customer. If you have entered several individual prices, the program first checks (in discounts) which rate has been defined as the standard price and if there is an individual price. If no individual price has been defined, the standard rate will be used for pricing.

> **Pricing with several individual prices**
> Prices will not be inserted automatically at document entry if several individual prices have been defined.
> You have to enter the required price key by hand. For this purpose, item entry offers a list of all prices defined for the customer.

**Calculation of supplier prices for purchased items**
Purchase prices will be managed only if module Purchasing has been installed and released.
- [ ] The system will not show the supplier's individual prices.
- [x] Individual prices will be displayed. The purchase price will be calculated right away at order entry.
This checkbox should be active for purchasing.

**No discount search for default records**
Standard prices will always be used for pricing unless an individual price has been defined. Automatic pricing follows the hierarchy below (downward priority):
- Individual price
- Discounts
- Standard prices
- [ ] Prices including the defined discounts will be used for standard prices (default rates).
- [x] The defined discount should not be taken into account. The following hierarchy applies in this case:
    - Total product price
    - sqm + individual item (French pricing)
    - Individual prices for IG and laminated glass

**PGR combination for discounts valid only if discount exists**
The product group discounts will be used for pricing at order entry.
- [ ] If you have entered a product group combination for an IG unit with a grill for example, this will be used at item entry no matter if there is a discount rate for this price key or not.
- [x] In this case, the product group combination will be used only if a discount rate has been entered for this price key.
⇨ Tutorial 1, "PGR Combination" on page B-143
⇨ Tutorial 1, "Combine Product Groups" on page B-152
⇨ "Combined PGR" on page B-568

**Create PGR combinations using complete BOM**
If a product includes a BOM, the turnover of the BOM elements can be analyzed by means of product group combinations.
- [ ] With this settings, the product group combination valid for the corresponding product will be used.
- [x] Irrespective of the combination rule for the next processing steps, all BOM elements will be booked to the last combination found for this item.
⇨ Tutorial 1, "Create PGR combinations with full BOM" on page B-147
⇨ Tutorial 1, "Combine Product Groups" on page B-152
⇨ "Combined PGR" on page B-568

**Search discounts for mixed IG calculation**
If the price for IG is calculated by mixed calculation using different price lists, discount calculation can be permitted or forbidden.
- [ ] Discount search is switched off by default for IG mixed calculation.
- [x] The system searches for discount rates for the corresponding IG price list.
⇨ Software Reference, "Mixed Price Calculation" on page B-696

**Search individual price for mixed IG calculation**
If the price for IG units is calculated by means of different price lists, using mixed calculation, the search for customized prices can be permitted or forbidden.
- [ ] The search for individual prices is disabled by default for mixed IG calculation.
- [x] The system will search in price management for individual prices for the corresponding combination of IG lites.
⇨ "Product Management – Price/Surcharge" on page B-601

**300 mm min. edge length for IG in PP and SP**
This setting is valid for IG pricing in purchasing and sales.
- [ ] Pricing is based on the actual lite size.
- [x] If the width and/or height of an IG unit lies below 300 mm, pricing will be based on a minimum edge length of 300 mm (sales and purchase price).

**IG + LG single price calculation**
A+W Business offers three price calculation types:
- Total product price
- sqm + individual item (French pricing)
- Individual prices for IG and laminated glass
- [ ] The defined total price is used for pricing. The individual prices of the elements will not be taken into account.
- [x] Pricing is controlled by product master data. The price for the main product is calculated for every single element, and then added up.

> **Elements have to be price-relevant**
> If this checkbox is checked, the codes `Price-relevant SP` and `Price-relevant PP` must be checked for the BOM elements in product management. If this code is inactive, the corresponding element will not be calculated.
> ⇨ "Product Management – BOM" on page B-614

**Calculate min. grill length per pattern**
Minimum quantities can influence pricing. It is therefore necessary to define what the minimum bar length refers to.
- [ ] By default, the minimum length is calculated by bar.
- [x] The minimum bar length is calculated by grid (total of all bars).
⇨ Tutorial 1, "Pricing Codes" on page B-168
⇨ "Surcharge Product Assignment" on page B-1024

**Calculate min. edge length per edge**
Minimum quantities can influence pricing. It is therefore necessary to define what the minimum edge length refers to.
- [ ] By default, the total of all edge lengths is calculated as the minimum length for processing.
- [x] The minimum processing length is calculated by edge.

**Commercial size rounding**
Size roundings can be calculated in different ways.
- [ ] By default, sizes are rounded upwards.
- [x] In case of commercial rounding, rounding goes four downwards and five upwards.
⇨ Tutorial 2, "Rounding" on page B-442
⇨ "Rounding" on page B-880

**Calculate foreign currency amount from unit price x quantity**
This setting allows to control the calculation of foreign currency accounts on item level.
- [ ] The foreign currency amount for the item is calculated from the item price, in national currency. This is done multiplying the item price by the conversion factor.
- [x] The amount in foreign currency for the item is the net unit price in foreign currency. This means that the individual prices are converted into foreign currency, then multiplied by the quantity.
⇨ Tutorial 1, "Price Tables" on page B-230
⇨ Tutorial 2, "Pricing in connection with foreign currency" on page B-457

**Use main item discount rather than processing discount 0%**
Discounts can be applied to the main item as well as processing.
- [ ] If a separate discount of 0% is defined for processing, the discount for processing will not be adopted from the main item.
- [x] If a separate discount of 0% is defined for processing, the discount from the main item will also be applied to processing.
This means that the appropriate entry has to be selected for processing in field `Adopt from main item`.
⇨ "Price Parameters" on page B-602

**No fixed adoption of item discount in case of exchange surcharge**
Discounts for replacement products can be considered as a separate discount, or replaced by the discount defined for the main item.
- [ ] If no other discount has been defined for exchanged glass in IG units, the discount for the main item will be adopted for the exchanged lites.
- [x] The discount will not be applied to the replacement product. In this case, only the discount for the replacement product (if defined) will be taken into account.

**Recursive quantity calculation in BOM**
This checkbox defines if the processing step should be calculated once for the entire product, or for every BOM element.
- [ ] By default, the processing will be calculated for the entire product. In this case, you have to enter the processing item and the required quantity at order entry, e.g. 12 x edgework for a CD stand with two side panels and four shelves. The edgework is defined per glass.
- [x] For processing, the total net amount for a BOM element is calculated from the number of processing steps of all parent products.

> **Recalculation of orders**
> If this option is switched on later, orders with the corresponding constellation have to be recalculated.
> ⇨ Sales, "Recalculate" on page C-674

**Adopt rate/discount from main item if rate is changed**
In product master data you can define whether and how the discount from the main item should be applied to the BOM elements if these are price-relevant and discountable.
This checkbox defines how the discounts should be applied if the rate or price key are changed.
- [ ] If prices are changed, the discount is loaded from product definition.
- [x] If no discount has been defined for a BOM element in product master data, the discount from the main item is basically adopted when the rate is changed. Discounts on BOM level will not be taken into account.

**Use real shape size for price calculation**
Pricing of shapes can be based on the surface.
- [ ] By default, the surrounding rectangle will be used to calculate the sqm price.
- [x] For shapes, the actual surface will be used to calculate the square meter price.
⇨ "Shape Processing Surcharges" on page B-697
⇨ "Quantity Limits" on page B-888

**Misc. surcharges (% gross/net) with surcharge types**
Other surcharges generally refer to quantity limits and measures.
- [ ] For all BOM elements defined with a surcharge, the surcharge is used as a calculation basis, irrespective of the surcharge type.
- [x] The surcharge types of the BOM elements will be taken into account by default.
⇨ Tutorial 1, "Miscellaneous Surcharges" on page B-305
⇨ "Miscellaneous Surcharges" on page B-664

**Do not calculate energy surcharge by item weight**
The energy surcharge refers to the weight of the shipment.
- [ ] The energy surcharge is generally calculated by total weight, including fittings, spacers, grill, etc.
- [x] The energy surcharge is applied only to the glass weight.
⇨ "Surcharge Product Assignment" on page B-1024

**Energy surcharge on rounded weight, then with item area**
The energy surcharge can be calculated on the rounded area of the item.
- [ ] The energy surcharge is not calculated on the rounded weight.
- [x] The energy surcharge is calculated on the rounded area of the item. This may also affect any defined minimum quantities. The setting is important if BOM glass is not price-relevant, but TG with float decisive for the energy surcharge is included in the BOM.

**Calculate surcharges with rounded quantities**
Even if prices are calculated with rounded quantities, the surcharge can refer to the actual surface.
- [ ] Surcharges are applied to the actual surface as a standard, i.e. before the quantity is rounded.
- [x] Surcharges and services are calculated based on rounded quantities. The dimension rounding of the item is transferred to the dimension rounding of the non price-relevant BOM glass, which prevents that the main product has a different dimension rounding than the non price-relevant BOM glass.
This calculation type can be changed in the order by selecting the price unit `sqm (act.)`.

**Order minimum value incl. partial deliveries**
The minimum order value can refer to the total order or the individual partial deliveries.
- [ ] The partial deliveries are not regarded for the determination of the minimum order value.
- [x] The minimum order value applies for each partial delivery.

**Expanded exchange price search for assembly position (LAMI)**
For LAMI, the exchange price can also depend on the assembly position.
- [ ] The search for an exchange price does not consider the assembly position.
- [x] The price calculation for the surcharge on exchange glass considers the assembly position. This way, in LAMI an additional foil can be installed and nevertheless the product/thickness-related exchange surcharge for the 2nd glass found. This also applies for the exchange surcharge for a glass in LAMI of an IGU.
