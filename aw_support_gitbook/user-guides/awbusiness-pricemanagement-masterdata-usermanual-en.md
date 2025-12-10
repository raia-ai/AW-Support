---
description: "EN-UM-AWBusiness_9"
---


# Software Reference: Price Management

You can restrict the search to partner- and project-related price tables by selecting the appropriate criteria.

> **Individual prices**
> Individual prices always have priority over all other prices and discounts for the pricing of documents.

---
## Prices - Matrix

**Master Data > Prices > Prices > Matrix tab**

*Abb. B-446 Prices - matrix*

This tab permits to enter a price matrix with up to two limit types.

*   Tutorial 1, "Limit Types for Graduations" on page B-315
*   Tutorial 1, "Defining a Graduated Price with Limits" on page B-324

### Limit type1, Limit type2
The limit types can be used for price graduation. The limit type defines the measure for graduation. You can choose different units for the two limit types, e. g. thickness and weight.
The input field for the limit type is accessible when you add a new column. The limit value refers to the limit type. If `<n.e.>` is entered as a limit type, the price is valid per price unit.

### Min. values
The minimum values are checked at order entry. If the actual entries fail to reach the defined minimum price or quantity, a message appears and/or a surcharge is applied.

**Gross price, Net price**
Minimum price for an order item.

**Quantity**
Minimum order quantity.

### Price specification

**Price unit**
The price unit refers to the details defined in the matrix.

**Currency**
If you are using different currencies you have to define the currency for which the gross and net price should be valid.

**Triangle**
In a matrix or cube, you can enter prices so that the defined limits can be exchanged, e.g. width and height.

- The limit types may not be switched. In this case, a price must be entered for every column/line in all fields. You should choose this setting for lites for which the cutting direction is important.
- The limit types may be switched. In this case, the price has to be entered only for one of the combinations of limit types.
⇨ Tutorial 1, "Triangle" on page B-322

### Matrix
Enter - in every field per line and column - the price that will be applied to the corresponding combination of limit types.
⇨ Tutorial 1, "Matrix" on page B-321

> **Copying & inserting from price matrices from Microsoft Excel**
> This function can be used to take over matrices and levels of the cube directly from Excel. The copy & insert function is in the upper left corner of the table, where the properties can also be changed. This way, it is possible to take over the content of the table with its titles directly into Microsoft Excel.

## Prices - Vector

**Master Data > Prices > Prices > Vector tab**

*Abb. B-447 Prices - vector*

Define the price and a limit type.
Prices can also be graduated by the number of lites for example. The quantity limit Number of lites determines the number of lites on the levels below the parent glass. If the parent glass has no children, 1 will be returned. This kind of graduation is suitable for surcharges on gas for example.
⇨ Tutorial 1, "Vector" on page B-320
⇨ Tutorial 1, "Defining a Graduated Price with Limits" on page B-324

The fields are described on the Matrix tab.
⇨ "Prices - Matrix" on page B-772

## Prices - Individual Price

**Master Data > Prices > Prices > Individual price tab**

*Abb. B-448 Prices - Individual Price*

This tab is used to define the individual price, e.g. for fittings or for single annealed per sqm.
⇨ Tutorial 1, "Unit Price" on page B-296
⇨ Tutorial 1, "Input of Unit Prices" on page B-301

## Prices - Shape

**Master Data > Prices > Prices > Shape tab**

*Abb. B-449 Prices - Shape*

This tab is used to define the price of a shape, considering a limit type if required.
Shape prices are usually a surcharge on the glass price. These surcharges can be defined for all glass types used for the production of shapes.
⇨ Tutorial 1, "Defining a Shape Price" on page B-306
The fields are described on the Matrix tab.
⇨ "Prices - Matrix" on page B-772

## Prices – Grills

**Master Data > Prices > Prices > Grills tab**

*Abb. B-450 Prices – Grills*

This tab is used to define the price of grills, considering a limit type if required.
This list shows all grill elements for which prices can be entered. You can enter a separate price per element or a total price for the pattern.
⇨ Tutorial 1, "Grill Price" on page B-299
The fields are described on the Matrix tab.
⇨ "Prices - Matrix" on page B-772

## Prices - Cube

**Master Data > Prices > Prices > Cube tab**

*Abb. B-451 Prices – Cube*

This tab is used to enter a price in the shape of a cube, considering up to three limit types, e.g. width, height, and thickness.
⇨ Tutorial 1, "Cube" on page B-323
⇨ Tutorial 1, "Limit Types for Graduations" on page B-315
The fields are described on the Matrix tab.
⇨ "Prices - Matrix" on page B-772

## Prices - Price Formula

**Master Data > Prices > Prices > Price formula tab**

*Abb. B-452 Prices - Price formula*

Enter the price in the shape of a formula. The formula can be directly entered in the formula editor.

### Formula editor
**[Syntax check]** When you have entered a formula you can use this button to check its syntax. Only correct formulas can be used for pricing.
**[Insert formula]** Use this button to open the dialog Formula management from where you can copy a formula in order to modify it.
⇨ "Formulas" on page B-1051

## Change Prices

**Master Data > Prices > Prices > Functions menu > Change prices**

*Abb. B-453 Change prices - Price type, price change*

This dialog is used for changing individual prices. You can increase or reduce the price or surcharge by a fixed amount or a percentage.
⇨ Tutorial 1, "Copying and Changing Prices" on page B-311

### Price selection
**From no., to**
Number(s) of the price list(s) to be changed.

**Quantity**
Number of records.

**Price list, key**
Choose the price list and the key for which price lists should be amended.

**Price units**
Generally, all price units will be adopted. You can however adapt the selection to your requirements.

### Price type
Choose an option to define the price type to be changed:

- **General:**
  The general price tables will be changed.
- **Customer group, Supplier group:**
  The price tables for a customer group or supplier group will be changed. This option releases the field Group from where you can select the required group.
- **Customer, Supplier:**
  The price tables for a customer or a supplier should be changed. This option releases the field Partner from where you can select the required partner.

**Project**
This field is locked if you have selected the option General. When you select a group or a partner, you can also define the project for which the price table should be changed.

### Price change
**Surcharge, Deduction**
This option determines whether the defined value should be added to or deducted from the prices in the price tables.

**Per cent, Absolute**
If the actual prices are to be changed, enter a percentage or an absolute value.

**Rounding**
You can change the rounding for the selected price table.

## Copy Prices

**Master Data > Prices > Prices > Functions menu > Copy prices**

### To the dialog description:
⇨ Delete Prices
⇨ Copy Exchange Prices
⇨ Copy Prices per Exchange Product Completely
⇨ Delete Exchange Surcharges
⇨ Change Exchange Prices
⇨ Copy Price Group Allocation (Copy Key) (Copy Key)
⇨ Copy Group Surcharges
⇨ Delete Group Surcharges
⇨ Change Group Surcharges

*Abb. B-454 Copy Prices*

This dialog serves for selecting one or more price tables to be transferred to other price tables or rates. You can increase or reduce the prices by a fixed amount or a percentage.
To copy prices to new tables you have to create these tables first. The prices can then be copied to the empty tables.
⇨ Tutorial 1, "Copying and Changing Prices" on page B-311

### Source
**From no., to**
Number(s) of the price list(s) to be copied.

**Price list, key**
Price list and key (rate) the prices of which are to be copied.

**Misc. surcharge**
Miscellaneous surcharge to be copied.

### Target
**Number**
Number of the price list to which the new prices should be copied.

**Change prices**
If you want to transfer the prices to a filled-in price table you have to decide whether the prices in the target table should be changed.
- The prices in the target table will not be changed. The additional prices from the source table will be added.
- All existing prices in the target table will be replaced.

**Price list, key**
Choose the price list and the key for which price lists should be amended.

**Key text**
The name of the (price) key must be the same as the key text.
⇨ "Key text" on page B-771

**Misc. surcharge**
Miscellaneous surcharge to be changed.

### Price units
Generally, all price units will be adopted. You can however adapt the selection to your requirements.

### Source price type, Target price type
Choose an option to specify the price type to be copied, and the target price type to which it should be transferred:
- **General:**
  The general price tables will be changed.
- **Customer group, Supplier group:**
  The price tables for a customer group or supplier group will be changed. This option releases the field Group from where you can select the required group.
- **Customer, Supplier:**
  The price tables for a customer or a supplier should be changed. This option releases the field Partner from where you can select the required partner.

**Project**
This field is locked if you have selected the option General. When you select a group or a partner, you can also define the project for which the price table should be changed.

### Price change
**Per cent, Absolute**
If the actual prices are to be changed, enter a percentage or an absolute value.

**Surcharge, Deduction**
This option determines whether the defined value should be added to or deducted from the prices in the price tables.

**Rounding**
You can change the rounding for the selected price table.

## Delete Prices

**Master Data > Prices > Prices > Functions menu > Delete prices**

*Abb. B-455 Delete prices*

This dialog can be used to delete individual prices or a sequence of prices.

### Price type
Choose an option to define the price type to be deleted:
- **General:**
  The general price tables will be deleted.
- **Customer group, Supplier group:**
  The price tables for a customer group or supplier group will be deleted. This option releases the field Group from where you can select the required group.
- **Customer, Supplier:**
  The price tables for a customer or a supplier should be deleted. This option releases the field Partner from where you can select the required partner.

**Project**
This field is locked if you have selected the option General. When you select a group or a partner, you can also define the project for which the price table should be deleted.

### Price selection
**From no., to**
Number of the price table. If you enter the same number in both fields, only this price list will be deleted.

**Quantity**
Number of records (price tables) to be deleted.

**Price list, key**
Price list and price key from which the prices should be deleted.

## Import Price Matrix

**Master Data > Prices > Prices > Functions menu > Data exchange group > Automatic import**

### To the dialog description:
⇨ Export Price Matrix
⇨ Import Price Matrix

*Abb. B-456 Import Price Matrix*

You can use this dialog for selecting the rate and the file for the import of prices.
If the file has not been saved in the standard directory you have to select the command **Data exchange > Interactive import**. This opens the dialog Prices from which you can select the directory and the file.

---

**Master Data > Prices > Prices > Functions menu > Data exchange group > Interactive import**

### To the dialog description:
⇨ Export Price Matrix

*Abb. B-457 Import price matrix – interactive*

These tabs are used for importing a price matrix that has been saved as a file.
Go to tab **File** and select the file to be imported.
Go to tab **Matrix** and enter the details of the import.

## Export Price Matrix

**Master Data > Prices > Prices > Functions menu > Data exchange group > Export**

*Abb. B-458 Export price matrices*

This dialog is used for exporting a price matrix to save it as a file.

### Parameters
**Price list, key**
Price list and price key from which the prices should be exported.

**Key text**
The name of the (price) key must be the same as the key text.

### Pricing
**Consider individual prices**
You can define whether the customized price tables should be exported as well.
- Customized price tables will not be exported.
- Customized price tables will be exported. Field **Customer number** is accessible.

**Customer number**
If customized price tables are to be exported as well you have to select the customers in question.

**Name, Customer group**
Name and customer group appear automatically when you select a customer.

### Adopt description from
These three options are only enabled if you have selected the Copy mode. The options are accessible only if you have selected format **Klaes** or **Klaes 5.0**. You can choose whether the name should be adopted from price data or from product data.

### Target file
**[Directory]**
Use this button to open the dialog Export file in which you can select the storage location.

**Shape**
The formats are predefined. If you choose the option **Drees**, a CSV file will be created while choosing the option **Adulo** will produce an ASC file (ASCII).

## History of Changes

**Master Data > Customer management, Supplier management, Price management, Discount management > History menu > Evaluation**

*Abb. B-459 Analysis - History*

This dialog is only available if you are using a Gupta database. It can be accessed from the following dialogs:
- Customer management
- Supplier management
- Price Management
- Discount management

In the corresponding dialog, set up the analysis for the current program section, e.g. for prices. The results of the analysis can be displayed on screen or printed.
Analyses can only be displayed if the changes to be monitored and displayed have been defined in module **Utilities > Sys-tem > Monitoring of changes**.
⇨ Tutorial 2, "Monitoring of changes" on page B-601

> **Analyses always refer to the current database table**
> In discount and price management, the data displayed can refer to different modes, e.g. standard prices, prices for customers or for customer groups. If standard prices are shown for example, analysis only takes those into account.

### Selection
The following settings can be selected, depending on the mode the dialog to be monitored is in when analysis is started:
- **Current record:**
  If records are shown in the dialog, amendment history can be analyzed for a single record. Only the tagged record will be analyzed.
- **Current selection:**
  The records are analyzed by the criteria defined in QBE mode.
- **All:**
  All records of the current database table will be analyzed.

### Filter
**Employee**
User who has entered the monitored changes.

**from date, to date**
Space of time during which the monitored changes have been entered.

**Show details**
Details can be displayed only if the detailed monitoring and the required fields have been defined in dialog **Monitoring of changes - management**.
- Details will not be displayed. The list of changes shows the number, e.g. customer number, the date, time, and the name of the user who has changed the record.
- The analysis also shows the details that have been changed, e. g. the old and the new description and new quantity limits.
⇨ Tutorial 2, "Monitoring of changes" on page B-601

**Former price**
This combo box is only available in price management. It will be displayed only if there is an old price.

# Stock

**Master Data > Stock**

This program section is used for entering the master data for stock management.
Menu Stock offers the following entries:
- "Packing” on page B-788
- "Level 1 to 4" on page B-788
- "Stock Definition" on page B-789
- "Stock Categories" on page B-791
- "Stock Location for Machines" on page B-792
- "Search Machines" on page B-792
- "Booking Type" on page B-793

## Packing

**Master Data > Stock > Packing**

*Abb. B-460 Packing types*

This dialog is used for entering the packing types, e.g. rack, box, pallet.
The packing can be allocated in dialog **Document management > Supplement. tab**
⇨ "Header data - supplement" on page C-1551

### Table
**Name**
Name or description of the means of packing, e.g. rack, box, pallet.

**External key**
External key for communicating with other programs, e.g. for transfer to production.
⇨ Production, "Transfer external packing code" on page E-2253

**Locked**
A means of packing can be locked for input in price management and in documents if it is no longer required.
- The means of packing can be allocated.
- The packing is locked and cannot be allocated. If it has been allocated in the shipping area and in documents, it will still be shown however.

## Level 1 to 4

**Master Data > Stock > Level 1, Level 2, Level 3, Level 4**

*Abb. B-461 Level*

The dialogs for the levels 1 to 4 are used to enter the descriptions of the different levels of your stock.
Dialog **Stock definition** serves to allocate the individual levels to each other.
⇨ "Stock Definition" on page B-789

## Stock Definition

**Master Data > Stock > Stock definition**

### To the dialog description:
⇨ Stock Levels

*Abb. B-462 Stock Definition*

This dialog serves to allocate the stock levels to each other, thus describing the structure of your stock.
Module **Stock > Stock Management** serves to allocate the stock articles to the defined storage places.
⇨ Stock management, "Define Storage Location" on page G-2447

### Levels
You can define the names in dialog Stock levels. The following names are therefore only meant as examples.

- **Warehouse** = Level 1
- **Aisle** = Level 2
- **Shelf 1** = Level 3
- **Slot** = Level 4

**Name**
Name of the storage place, e.g. external warehouse, gate A.

### Parameters
**Locked**
- The storage place can be locked.
- The storage place is not locked.
- The storage place is locked and cannot be allocated.

**Warehouse type**
Selection of the warehouse type. If you work with the warehouse connection to Hegla, the entry Hegla must be selected. This will release the field **Stock for goods receipt**.

**Stock for goods receipt**
Stock location to which the goods receipt should be booked. The field is only enabled if you have selected the entry **Hegla** as warehouse type.
In addition, in the stock definition, a stock with the Warehouse type Hegla and an assigned goods receipt stock must be defined.
⇨ "Stock Definition" on page B-789

> **Allocation of supplier article numbers**
> To manage products correctly all articles have to be allocated: **Master Data > B2B > Supplier > Products**.

**Cutting table (1;2;)**
Specification of the cutting table on which the glass can be cut. You can specify several tables and separate them with semicolons.

## Stock Levels

**Master Data > Stock > Stock Definition > Definition menu**

*Abb. B-463 Stock levels*

This dialog is used for specifying the names of the stock levels.
⇨ Stock management, "Define Storage Location" on page G-2447

## Stock Categories

**Master Data > Stock > Stock Category**

*Abb. B-464 Stock Categories*

This dialog serves for defining the stock categories, e.g. boxes, stock sizes, fittings, sqm articles.
The stock categories are allocated to stock articles in dialog **Stock management**. The stock articles are summed up in groups (stock categories) that can be used as search criteria.

**ID**
The ID (identification number) can be chosen at random, e.g. numbers or descriptions like raw material, boxes, production.

**Comment**
Short description of the stock category

## Stock Location for Machines

**Master Data > Stock > Stock locations for machines**

*Abb. B-465 Stock Location for Machines*

This dialog serves to allocate storage places to a machine or a production area. These details are used by A+W Business capacity planning.

> **Example**
> The stock article float glass is kept in the storage places A and B. Storage place A is closer to cutting table 44.
> If storage place A is allocated to cutting table 44, the float glass is taken from stock A and is withdrawn. Only if there is no suitable glass available on stock A, the glass will be taken from stock B, which is farther away.

The actual machines are entered in module **Capacity planning**.

### Machine / Production Area
Choose an option to define the area:
- **Machine:**
  Machine where the material from the storage place is needed.
- **Production area:**
  Production area where the material from the storage place is needed.

### Storage place
**Storage place**
Storage place allocated to the product and machine or production area.
⇨ "Stock Definition" on page B-789

### Article / Product Group
Choose an option to specify the material:
- **Articles:**
  A specific product from the selected storage place will be allocated.
- **Product type:**
  A specific product type from the selected storage place will be allocated.

**Product class**
Allocation of the product type can be restricted to a certain product group. The field is accessible only if the option **Product type** has been selected.

### Overview
The list shows all storage place allocations matching the selection criteria.

## Search Machines

**Master Data > Stock > Stock location for machines > Search**

*Abb. B-466 Search machines*

This dialog is for searching for a machine you have entered in module **Capacity Planning**.

### Filter
**From machine no., to**
Machine number of sequence of machine numbers

**Name**
Name of the machine you are looking for. Enter at least the first letter.

### Machines
The list shows the machines resulting from the search.
**[Search (F2)]** Filters the display by the defined search criteria.

## Booking Type

**Master Data > Inventory > Booking type**

*Abb. B-467 Stock booking types*

This dialog shows the booking types used on stock, e.g. reserved, ordered, received, shipped. They are preset in A+W Business.
⇨ Stock management, "Show Booking Journal" on page G-2513

> **Enter new booking type**
> Booking types must not be changed or completed. Please agree any required changes with A+W Software GmbH.

# Partners

**Master Data > Partners**

This program section specifies the details for entering partner data.
A+W Business distinguishes customers, suppliers, and partners:
- Customers place orders with you and are provided with goods by you.
- Suppliers are those partners from which you order the products you cannot produce yourself.
- Partners are all those who fit in neither category. This can be your paper or beverage supplier.

Menu Partners offers the following entries:
- "General" on page B-795
- "Customer" on page B-846
- "Supplier" on page B-887

## General

**Master Data > Partners > General**

Use this program section to define the details for entering customer and supplier data. You can also enter the data for those partners who are neither customers or suppliers.

Menu General offers the following entries:
- "Partner Groups" on page B-796
- "Customer Groups" on page B-797
- "Supplier Groups" on page B-797
- "Transactions" on page B-798
- "Titles" on page B-799
- "Title (Function)" on page B-799
- "Branches" on page B-800
- "Projects" on page B-801
- "State" on page B-802
- "Partners" on page B-803
- "Classifiers" on page B-803

### Partner Groups

**Master Data > Partners > General > Partner Groups**

*Abb. B-468 Partner Groups*

This dialog is used for defining partner groups, e.g. Catering for all partners supplying food and beverage.
The partners are allocated to a partner group in partner management.
⇨ "Partner Management - Address" on page B-809

**Name**
Name of the partner group.

**External key**
External key for communicating with other programs, e.g. for statistical analysis.

**Locked**
Partner groups can be locked for entry in partner management if no longer needed.
- The partner group can be allocated.
- The partner group is locked and cannot be allocated. If it has been allocated, it will still be displayed.

### Customer Groups

**Master Data > Partners > General > Customer Groups**

*Abb. B-469 Customer Groups*

This dialog serves to specify the customer groups, e.g. Customer group 1, Customer group A, Craftsman, Private customers, Others ... A customer group can be used for allocating prices. It also serves as a sorting criterion in customer turnover statistics.
⇨ "Price Group Allocation" on page B-746
In partner management, customers are allocated to a customer group.
⇨ "Partner Management - Address" on page B-809

**Name**
Name of the customer group.

**External key**
The external key can be used for communicating with other programs, e.g. for transfer to production or for statistical analysis.

**Locked**
If it is no longer required, a customer group can be locked for input in partner management, for discounts, rounding, and prices.
- The customer group can be allocated.
- The customer group is locked and cannot be allocated. If it has been allocated, it will still be displayed.

### Supplier Groups

**Master Data > Partners > General > Supplier Groups**

*Abb. B-470 Supplier Groups*

This dialog is used for defining supplier groups, e.g. glass trade, metal works. The supplier groups serve as a sorting criterion in supplier turnover statistics.
In partner management, suppliers are allocated to supplier groups.
⇨ "Partner Management - Address" on page B-809

**Name**
Name of the supplier group.

**External key**
The external key can be used for communicating with other programs, e.g. for transfer to production or for statistical analysis.

**Locked**
If it is no longer required, a supplier group can be locked for input in partner management, for discounts, rounding, and prices.
- The supplier group can be allocated.
- The supplier group is locked and cannot be allocated. If it has been allocated, it will still be displayed.

### Transactions

**Master Data > Partner > General > Transactions**

*Abb. B-471 Transactions*

This dialog is serves to enter names for documents that can be used for recurring tasks in the contact with customers. In partner management, these documents can be selected for an action and followed up.
⇨ "Transaction Management" on page B-842

> **Example**
> One of your sales representatives wants you to revise the customer file for his territory. This necessitates the dispatch of a circular.
> In this case you want to check whether letters were sent to the customers and if their data have been updated afterwards. This action can be given a name that is entered here.

**Name**
Name of the document.

**External key**
External key for communicating with other programs, e.g. for statistical analysis.

### Titles

**Master Data > Partners > General > Titles**

Enter the possible titles for your business partners and employees in this dialog.

**Name**
Form of address, e.g. Messrs, Mrs, Mr in all languages used for communicating with your partners.

**External key**
Currently not used.

**Locked**
A form of address can be locked for entry in partner management and in documents if it is no longer needed.
- The form of address can be allocated.
- The form of address is locked and cannot be allocated. If it has been allocated to partners and documents, it will still be shown.

### Title (Function)

**Master Data > Partners > General > Title**

This dialog serves to enter all possible titles or functions you may want to assign to your contacts or employees, e.g. Manager, Production Manager.

**Name**
Title or function in all languages used for corresponding with your partners.

**External key**
External key for communicating with other programs, e.g. for the transfer to financial accounting or statistical analysis.

**Locked**
A function (title) can be locked for input if it is no longer needed.
- The function can be assigned.
- The function is locked and cannot be assigned. If it has been assigned to partners, it will still be shown.

### Branches

**Master Data > Partner > General > Branches**

*Abb. B-472 Branches*

This dialog can be used to enter the lines of business you are dealing with. The line of business is an additional analysis and sorting criterion for statistics. Every customer and supplier can be allocated to a line of business, e. g. glass dealer, window manufacturer, joiner.
Lines of business are allocated in partner management.
⇨ "Partner Management - Address" on page B-809

**Name**
Name of the line of business.

**External key**
External key for communicating with other programs, e.g. for statistical analysis.

**Locked**
A line of business can be locked for entry in partner management and in documents if it is no longer needed.
- The line of business can be allocated.
- The line of business is locked and cannot be allocated. If it has been allocated to partners and documents, it will still be shown.

### Projects

**Master Data > Partners > General > Projects**

*Abb. B-473 Projects*

This dialog is used for defining projects, e.g. building projects for which you want to use special prices and discounts. This dialog is accessible only if project management is enabled in company data.
⇨ "Company Data > Documents" on page B-952
The projects are allocated to the customers or suppliers, defining the general conditions for project in question.
⇨ "Projects (Customer, Supplier)" on page B-861
You can select the required project in the document. The prices and discounts defined for this project will be applied automatically.
The different types of projects are described in detail in the Tutorial.
⇨ Tutorial 2, "Project/invoice management" on page B-568

**Name**
Project name.

**External key**
External key for communicating with other programs, e.g. for transfer to production or financial accounting.

**Locked**
A project can be locked for document input if it is no longer required.
- The project can be allocated.
- The project is locked and cannot be allocated. If it has been assigned in a document, it will still be shown however.

### State

**Master Data > Partners > General > State**

*Abb. B-474 States*

This dialog can be used to enter the states that can be allocated to your partners.
States are required if different VAT codes are valid in different parts of a country.

**Name**
Name of the state.

**Tax code**
VAT code valid for this state.

**External key**
External key for communicating with other programs, e.g. for transfer to production or financial accounting.

**Locked**
A state can be locked for entry in partner management and in documents if it is no longer needed.
- The state can be allocated.
- The state is locked and cannot be allocated. If it has been allocated to products and in documents, it will still be shown however.

### Partners

**Master Data > Partners > General > Partners**

Dialog **Partner Management** allows entering data for the partners. Partners serve for managing address data that belongs neither to the category of customers nor to the supplier category, e.g. the tax advisor. You cannot enter documents for partners.
This dialog is the same for all partners. It is described in detail in connection with customers.
⇨ Tutorial 1, "Customer Data" on page B-95
⇨ "Partner Management" on page B-805

### Classifiers

**Master Data > Partners > General > Classifiers**

Enter the classifiers for partners and products in this dialog. Enter the technical parameters for glass products in this dialog. Apart from the name and a comment you have to define the value that can be allocated to each classifier.
⇨ Tutorial 1, "Enter a Classifier" on page B-135
⇨ Tutorial 1, "Allocate Classifier Value" on page B-137

#### To the dialog description:
⇨ Employee Classifiers
⇨ Classifier Value Allocation

The **Classifiers** dialog offers the following tabs:
- Classifiers - all market partners, customers, suppliers
- Classifiers - Product

#### Classifiers - all market partners, customers, suppliers

**Master Data > Partners > General > Classifiers > Market Partner Shared, Customers, Suppliers**

*Abb. B-475 Classifiers - Partners*

On this tab, you store the names of classifiers. The classifiers on the **All Market Partners** tab apply for all market partners. You must define classifiers that only refer to customers on the **Customers** tab.

> **User classifiers**
> Classifiers for users are managed separately in partner management where the corresponding value is entered.
> ⇨ "Employee Classifiers" on page B-842

**Name**
Unique name of the classifier.

**Remark**
Comment, e.g. regarding the use of the classifier.

**No.**
Only numerical values can be allocated here, e.g. the turnover.
- This value is invalid for this classifier.
- This value can be allocated to the classifier.

**Alpha-num.**
Numbers and letters can be allocated, e.g. exhibition give-away 2010.
- This value is invalid for this classifier.
- This value can be allocated to the classifier.

**Date**
Only dates must be allocated.
- This value is invalid for this classifier.
- This value can be allocated to the classifier.

Every alpha-numerical classifier can be allocated a value in dialog **Classifier value allocation**.
⇨ "Classifier Value Allocation" on page B-843

#### Classifiers - Product

**Master Data > Products > General > Classifiers > Products**
**Master Data > Partners > General > Classifiers > Products**

*Abb. B-476 Classifiers - products*

This tab is used for entering products of classifiers.
Apart from the name and a comment you have to define the value that can be allocated to each classifier.
⇨ "Product Management - Attachments / Classifiers" on page B-697

## Partner Management

**Master Data > Partners > Customer, Supplier > Customers, Suppliers**
**Master Data > Partners > General > Partner**

Dialog **Partner Management** is used for entering the details of your customers, suppliers, and/or partners.

> **Dialogs for Partner Management**
> This dialog is the same for all partners. In this document, it is described for an example customer. Fields that are displayed only for suppliers or for partners will be marked accordingly.

This section provides information on the following subjects:
- "Menus in Partner Management" on page B-805
- "Partner Management" on page B-808
- "Free Numbers / Areas" on page B-835
- "Telecommunication Data" on page B-836
- "Invoicing Surcharge/Minimum Value per Order Area" on page B-837
- "Route Priority" on page B-838
- "Text Search" on page B-839
- "Subsidiary" on page B-840
- "Employee" on page B-840
- "Transaction Management" on page B-842
- "Employee Classifiers" on page B-842
- "Classifier Value Allocation" on page B-843
- "Check Receivables" on page B-844
- "Copy Master Data" on page B-845
- "Partner Change" on page B-845
- "Terms" on page B-845

### Menus in Partner Management

**Master Data > Partners > Customer, Supplier > Customer, Suppliers**
**Master Data > Partners > General > Partner**

The partner management menus can be used to define the default settings for the dialog and to open other dialogs without closing partner management.

This section provides information on the following subjects:
- "Functions Menu" on page B-806
- "Options Menu" on page B-807
- "Print Menu" on page B-807

#### Functions Menu

**Master Data > Partners > Customer, Supplier > Customer, Suppliers > Functions menu**

You can use this menu to open other dialogs or setting codes without closing the dialog.
The menu is organized in the following groups:
- "Details group" on page B-806
- "Classifiers group" on page B-806
- "Accounting group" on page B-806
- "Global Changes group" on page B-806
- "Other group" on page B-807

**Details group**
- **Subsidiary:**
  Opens dialog Subsidiary to enter or change the dates of a subsidiary.
  ⇨ "Subsidiary" on page B-840
- **User:**
  Opens dialog User to enter or change user data.
  ⇨ "Employee" on page B-840
- **Documents:**
  Opens dialog Document management to enter or change documents.
  ⇨ "Transaction Management" on page B-842

**Classifiers group**
- **Classifier values:**
  Opens the dialog Classifier values where you can enter or change the values for an alpha-numerical classifier.
  ⇨ "Classifier Value Allocation" on page B-843
- **Classifier definition:**
  Opens the dialog Classifier definition where you can enter or edit classifiers.
  ⇨ "Classifiers" on page B-803

**Accounting group**
- **Check receivables:**
  Opens dialog Receivables that states the customer's unsettled accounts.
  ⇨ "Check Receivables" on page B-844

**Global Changes group**
- **Copy master data:**
  Opens dialog Master Data to transfer the settings from one partner to another.
  ⇨ "Copy Master Data" on page B-845
- **Change selected partners:**
  Opens dialog Change Partners to change the allocation of automatic surcharges or special discounts.
  ⇨ "Partner Change" on page B-845

**Other group**
- **Create IBAN:**
  You can use this function for determining the IBAN on tab Finances.
  ⇨ "Bank” on page B-822
- **Terms:**
  Opens dialog Terms/Individual Prices showing the discount and price agreements for the customer in question.
  ⇨ "Terms" on page B-845
- **Release documents:**
  Opens the Release documents dialog on which you can release locked orders, of individual customers or all together.

#### Options Menu

**Master Data > Partners > Customer, Supplier > Customers, Suppliers > Options menu**
**Master Data > Partners > General > Partners > Options menu**

This menu allows you to define the default settings for this dialog. The options can be enabled or disabled. The settings will not be reset when you close the dialog. The following entries are displayed:

- **Cursor position in search mode:**
  When you open partner management in search mode, the cursor can be either on field **Number** or on field **Mode**.
- **Sort state by external key:**
  If you have defined different states, you can sort them by external key.

#### Print Menu

**Master Data > Partners > Customer, Supplier > Customers, Suppliers > Print menu**
**Master Data > Partners > General > Partners > Print menu**

You can use this menu to print the customer data shown in section **Table**. The data can be displayed on screen or transferred to a printer. After you have chosen the printing mode, the following options are shown:

- **Short list:**
  Includes the customer number, customer name, address, phone and fax numbers.
- **File:**
  Includes all data.

### Partner Management Dialog

**Master Data > Partners > Customer, Supplier > Customers, Suppliers > Customers/Suppliers**
**Master Data > Partners > General > Partners**

#### To the dialog description:
⇨ Free Numbers / Areas
⇨ Route Priority
⇨ Invoicing Surcharge/Minimum Value per Order Area
⇨ Turnover/Order Area
⇨ Copy Master Data
⇨ Partner Change

> **Dialogs for Partner Management**
> This dialog is the same for all partners. In this document, it is described for an example customer. Fields that are displayed only for suppliers or for partners will be marked accordingly.

Dialog Partner management offers the following tabs:
- Partner Management - Address
- Partner Management - Order
- Partner Management - Employee/Subsidiaries/Transactions
- Partner Management – Text
- Partner Management - Classifiers
- Partner Management - Finances
- Partner Management – Balance
- Partner Management - Sales
- Partner Management – Production
- Partner Management - Attachments

Dialog Partner Management opens in selection mode by default. You can decide whether you want to edit the data of an existing partner or enter the data of a new partner.

#### Partner Management – Address

**Master Data > Partners > Customer, Supplier > Customers, Suppliers > Address tab**
**Master Data > Partners > General > Partners > Address tab**

*Abb. B-477 Partner Management - Address*

This tab serves to enter the data for the address, communication, and shipment.
⇨ Tutorial 1, "Input of Partner Master Data" on page B-110

**Identification**
- **Number ... to**: Customer numbers for the search. If you enter just one customer number, only the data of the corresponding customer will be displayed. The customer number can be selected only in mode New or in selection mode. When you enter new partner data you can use the zoom function to view the numbers that are still free.
  ⇨ "Free Numbers / Areas" on page B-835
- **Matchcode**: The matchcode is an alpha-numerical search key.
- **Client**: If you are using clients, every customer must be allocated to a client. This is necessary for client- or proceeds account-related bookings in financial accounting.
  ⇨ "Company Data - Client" on page B-943

**Address**
- **Header**: Form of address to be printed on documents, e.g. Messrs. The forms of address are defined in the dialog of that name.
  ⇨ "Titles" on page B-799
- **Name**: The three fields allow entering the name plus supplements, e.g. group of companies.
- **Standard**: This checkbox is only accessible in connection with subsidiaries. If you have to enter several addresses for the same company you can define the address to be used as the shipping address. The standard shipping address is entered as a subsidiary in A+W Business.
  - The subsidiary should not be used as the standard shipping address.
  - The subsidiary should be used as the standard shipping address for this customer. It can be changed in the order.
- **[Selection]**: Select the business area to which this partner belongs. This information can be used for external analyses for instance.
- **Street**: Customer's street address. If a subsidiary has been defined as the standard shipping address, shipments will be sent to this street address.
- **Miscell.**: You can bill minor customers as so-called **Miscellaneous customers** using a collective account in your financial accounting system for this purpose. There is no need to create individual accounts for this purpose.
  - These customer's orders will not be booked onto a collective account.
  - These customer's orders will be booked onto a collective account, together with other customers' orders.
- **(Country, state)**: Country code and state to be printed on documents. The State field is intended for USA and Canada. Missing codes can be added in the following dialogs:
  ⇨ "Country Code" on page B-638
  ⇨ "State" on page B-802
- **ZIP/Town**: Post code and place of residence.
- **ZIP/P.O. box**: Post code and P.O. box number. These fields can be used to control the printing of forms for the individual customers. You can also enter the bank details. This information will be printed on the form if the option **Read customer data (bank)** is active.
  ⇨ "Form Management - Options 2" on page B-1076

**Connections**
- **Phone 1 and 2**: Phone numbers including area code and country code (if applicable).
- **[Icon]**: You can use the Telecom button to display a list of phone and fax numbers defined for the subsidiaries and staff of this customer.
- **Fax and fax invoice**: Fax numbers including area code and country code (if applicable). The second field is meant for the fax number to which only invoices should be sent.
- **Email**: Email address to which documents should be sent. You can email documents to a customer or supplier only if an email address is defined here.
- **[Icon]**: You can use this icon to start your email system.
- **Homepage**: Partner's internet address.
- **[Icon]**: This icon can be used to access the partner's homepage.

**Company**
- **Back to main comp.**: The [Directory] icon is accessible only if you are editing the data of a subsidiary. Use this button to return to the main company. The customer number is shown for identification.
- **Independent subsidiary**: This checkbox is only accessible for editing the data of a subsidiary.
  - "No order can be entered for this subsidiary. It only serves as a shipping address for example.
  - If the shipping address is to be used as the standard shipping address, the checkbox **Standard** must be checked on tab **Address** in section **Address**. This shipping address will be used automatically at order entry.
  - The data refers to an independent subsidiary for which orders can be entered, and invoices issued. The subsidiary will also be displayed as a search result.

**Specification**
- **Line of business**: The line of business is used as a sorting criterion in turnover statistics. Missing lines of business can be defined by means of the directory icon, without leaving the partner management dialog.
  ⇨ "Branches" on page B-800
- **Language**: Language used for printing the document forms.
  ⇨ "Languages" on page B-636
- **Consultant**: Consultant in charge. This name will appear at order entry and can be changed if required.
  ⇨ "Employee" on page B-1031
- **Group**: Customer group to be used for discount allocation. The customer group can also be used as a sorting criterion in statistics.
  ⇨ "Customer Groups" on page B-797
- **Route 1, Route 2**: Route and alternative route for deliveries to this customer. When entering the routes, also enter the days on which this route will be driven. At document entry, the system automatically checks whether the delivery date matches the route date.
  ⇨ "Routes” on page B-894
- **Del. terms**: Delivery type, e.g. collection, lorry. This detail can be changed at order entry.
  ⇨ "Delivery Conditions" on page B-893
- **Display**: Define how the short info for this customer should be displayed at document entry:
  - **Never:** No details will be shown.
  - **Possible:** Information can displayed via [i].
  - **Always:** Information will be displayed whenever you load a document of this customer.
- **Info**: Information displayed at document entry, e.g. details regarding delivery terms, discounts, and payment terms.

#### Partner Management – Order

**Master Data > Partners > Customer, Supplier > Customers, Suppliers > Order tab**

*Abb. B-478 Partner Management – Order*

> **No documents for partners**
> This tab is relevant only for customers and suppliers for whom documents can be entered. You cannot enter documents for other partners.

This is where you can enter details on order entry. The settings can be amended in the order.
⇨ Tutorial 1, "Order and Sales Invoice" on page B-113
The fields in sections **Identification** and **Address** are described in tab **Address**.
⇨ "Partner Management - Address" on page B-809

**Standard rounding**
- **Width, height**: Pricing in Germany is usually based on rounding to thirty. This means that calculation is based on the next edge length that can be divided by 30. In France, calculation is based on rounding to 10 for example.
  > **Example**
  > Rounding 30:
  > For a lite of 1000 x 1000 mm, a surface of 1.04 (= 1020 x 1020) will be calculated.
  The specified size rounding can be changed in the order. The search for roundings starts with the individual prices and goes on to discounts, prices, products, and partners. The search comes to an end once a value has been found.

**Document dispatch**
Documents can be faxed or emailed only if the required function is active for the document type in question. You also have to enter the fax number and/or email address on the **Address** tab.
This function can be enabled separately for the following documents:
- Order confirmation (OC)
- Quotation (QU)
- Invoice (IN)
- Credit note (CR)

The appropriate form is selected at printout. The documents codes are checked in the number manager after which the documents are faxed or emailed via automatic printing of forms.
⇨ Tutorial 2, "Forms" on page B-545
⇨ "Form Management" on page B-1068
> **Fax dispatch**
> Fax dispatch requires a special software.

**Invoicing surcharge / minimum value**
A surcharge can be applied for invoicing and if the defined minimum value is not met. If a surcharge should be calculated for invoicing or the minimum value, the appropriate products or surcharges must be defined including the corresponding price tables.
The settings are valid for the present customer. You can use the [Order area] button for defining different settings for the individual order areas.
- **Mode**: Choose a mode to define the surcharge to be applied:
  - **No surcharge:** No surcharge will be applied to the invoice or order value.
  - **For first invoice of the month:** The invoicing surcharge will only be applied for the first invoice of the month. The following surcharges issued in the current month will not be subject to this surcharge.
  - **For every invoice:** The invoicing surcharge will be applied to every invoice.
  - **Minimum invoice amount (as an item):** The surcharge is applied to the order total including the surcharges, and is added as a separate item.
  - **Minimum value (as an item):** The surcharge is checked for every item and is added as a separate item. The surcharges will not be taken into account for calculating the difference.
  - **Minimum value (split):** The surcharge is distributed to the order items but not to the surcharges.
  ⇨ Tutorial 1, "Invoice Settings" on page B-115
- **[Order area]**: This button is used to open the dialog **Invoicing surcharge/minimum value per order area** where you can make individual settings for every order area.
  ⇨ "Invoicing Surcharge/Minimum Value per Order Area" on page B-837
- **Value**: Minimum value (amount) starting from which a surcharge should be applied. Please obey the selected mode. The amount for every invoice will be raised to the minimum value.
- **Last calc.**: Shows the last date on which the invoicing surcharge has been applied.

**Order**
- **Priority**: You can define the priority with which orders from this customer should be produced in general. The setting can be changed in the order.
  - **On call:** Orders are produced on call. An order is entered for this purpose with a delivery date that lies far ahead. When the customer calls for this order, the delivery date will be amended.
  - **Express:** These orders are produced with top priority. The priority is analyzed on the shop floor. The express surcharge is only based on the limit days however.
  - **Common:** These orders are fitted into the usual schedule.
  - **Extra:** This priority means that the order should be produced from residue (plates) left over from cutting other orders.
- **External number**: External number for electronic data transfer. In Supplier Data, enter the customer number you have been assigned by your supplier. This field is irrelevant in connection with customer data.
- **Route priority**: Sequence in which the customers of a route will get their goods:
  - 0 means that the deliveries will be automatically sorted by order number.
  - To sort the orders by customer number, enter the customer number in this field.
Order entry will analyze the entries in dialog **Delivery time** first.
  ⇨ "Delivery Time (Customer, Supplier)" on page B-860
Use the button next to the field to open an overview of the sequence of customers for this route.
  ⇨ "Route Priority" on page B-838
- **Pre-settings pattern side IG**: Position of the pattern side generally required by the customer. This setting overrules the settings made in product management:
  - **No default:** The settings from product data will be applied to the order.
  - **Pattern outside:** The patterned side should be facing outward by default.
  - **Pattern inside:** The patterned side should be facing inward by default.

**Units of measurement**
Defines the measure used for this customer:
- **metric (mm):** For European customers.
- **imperial (inch):** For American customers.

**Document parameters**
You can set the following calculation parameters for the document:
- **Monthly invoice:** If you are using the **Monthly invoices** module, invoices for a customer can e. g. be issued once a month or once every two weeks. Orders from this customer automatically get the **Monthly invoice** code when delivery notes are printed based on which they can be selected for invoicing. The corresponding print point and status point must be entered in company data, section **Monthly invoices** for this purpose.
  ⇨ "Company Data - Print" on page B-1005
- **Felt pads:** Felt pads will be automatically fitted for this customer. The setting can be changed in the order.
  ⇨ Sales, "Grill pads" on page C-1556
- **Weight rounded:** The weight should be rounded for calculating the energy surcharge.

**Surcharges/discounts**
All automatic surcharges are listed. Only the active surcharges or discounts will be considered for pricing for this customer.
⇨ "Miscellaneous Surcharges" on page B-728

**Express surcharge**
- **Limit days**: The number of days refer to the delivery date. If an order is to be shipped before the calculated delivery date, an express surcharge will be applied.
  > **Example: Limit days = 2**
  > Input date = 21st of the month
  > Calculated delivery date = 23rd of the month: no surcharge.
  > Delivery date entered = 22nd of the month: express surcharge will be applied automatically.
The express surcharge will be applied only if it has been enabled in field **Surcharges/discounts**. A **Express surcharge** product with the corresponding price table must be defined for this purpose.
⇨ "Miscellaneous Surcharges" on page B-728

**(Invoicing)**
- **Collective invoice**: Customer invoices can be combined in collective invoices. The setting can be changed in the order.
  - For this customer, an invoice is issued for every order.
  - Invoices for this customer will be combined in collective invoices.
  > **Settings for collective invoices**
  > With certain settings, no collective invoices will be printed although the code **Collective invoice** has been set for the order.
  > ⇨ Sales: Tutorial, "Printing of collective invoices" on page C-1149
  > ⇨ Tutorial 1, "Invoice Settings" on page B-115
- **Partial delivery**: Partial deliveries are permitted for this customer. The checkbox **Partial invoice** is checked only if partial delivery is permitted. This checkbox does not appear for suppliers in partner management.
  - You cannot enter partial deliveries for this customer. The setting can be changed in the order. Checkbox **Partial invoice** is locked.
  - You can enter partial deliveries for this customer. Checkbox **Partial invoicing** is released. The setting can be changed in the order.
  Partial deliveries are created by hand.
  ⇨ Sales, "Partial deliveries" on page C-1377
- **Partial invoice**: Partial invoicing is possible only for partial deliveries. This checkbox does not appear for suppliers in partner management.
  - Partial invoices will not be issued even if a partial delivery is entered for an order. The original order is locked for invoicing until the last partial delivery has been made. You have to enter a lock code for this purpose. The lock code has to be entered in company data.
  - A partial invoice is automatically created for every partial delivery. The amount and quantity of this partial invoice will be deducted from the original order.
  ⇨ "Lock Code" on page B-923
  ⇨ "Company Data > Documents" on page B-952
- **Print prices**: This setting will be used for all forms printed for this customer. If prices should be printed, the settings in management of forms have to be taken into account.
  ⇨ Tutorial 2, "Management of forms: Settings for printing prices" on page B-550
  ⇨ "Form Management – Options 1" on page B-1072
  The following settings can be applied:
  - **No printing:** No prices will be printed on the forms for this customer.
  - **All prices:** All item prices and totals can be printed.
  - **Totals only:** Only the totals can be printed.
- **Net prices**: Define how the prices should be printed on the document. The setting can be changed in the order.
  - Gross prices will be shown.
  - Prices are shown as net prices without discounts.

#### Partner Management – Employee/Subsidiaries/Transactions

**Master Data > Partner > Customer, Supplier > Customers, suppliers > Employee/Subsidiaries/Transactions tab**

*Abb. B-479 Partner management – Employee/Subsidiaries/Transactions*

This tab is used for defining the employees, subsidiaries, and documents of your partners. Employees and documents of the subsidiaries are neglected for the main company.
⇨ Tutorial 1, "Add Employees" on page B-126
⇨ Tutorial 1, "Add Subsidiaries" on page B-124

Double-click on a user, subsidiary or document to open the corresponding dialog.
⇨ "Employee" on page B-840
⇨ "Subsidiary" on page B-840
⇨ "Transaction Management" on page B-842

The fields in the sections **Identification** and **Address** are described in connection with the tab **Address**.
⇨ "Partner Management - Address" on page B-809

#### Partner Management – Text

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Text tab**
**Master Data > Partner > General > Partners > Text tab**

*Abb. B-480 Partner Management – Text*

These tabs can be used to enter text to be printed on forms as well as spacer text.
You can allocate existing text or enter new text.
⇨ Tutorial 1, "Entering Text in Customer Master Data" on page B-130
⇨ "Text" on page B-1063

The fields in section **Identification** are explained in tab **Address**.
⇨ "Partner Management - Address" on page B-809

> **Do not change text numbers by mistake**
> Please be careful not to change the (standard) text and text numbers by mistake.

**Block overview**
- **Number**: You can choose a standard text module by entering the text number. To enter a special text for this customer please keep the entry 0.
- **Buttons**: Use these buttons to add or remove text.
  ⇨ Tutorial, "Enter text" on page C-1170
- **Text code**: This text code controls the forms on which the text will be printed. The text code is automatically displayed when you select a text module. If you change the text code, the text corresponding with the new text code will be printed on the forms.
  ⇨ Master data, "Text Code" on page B-1063
  ⇨ Master data, "Text" on page B-1064
- **Overview (table)**: The table shows all text modules assigned to the customer. These text modules will always be printed, based on the text codes. Text output can be changed in the document.

**Text block**
- **Buttons**: You can change the font type and size and add hyperlinks, images and tables.
  ⇨ Tutorial, "Enter text" on page C-1170
- **Text field**: Click on the 'add text' button to release the text field. You can type directly into the text field to enter or change the text.

**Spacer Text**
- **Spacer Text**: Spacer text to be printed on the spacers for this customer by default.
- **[Icon]**: Opens dialog **Text** where spacer text can be entered or edited.
  ⇨ "Text" on page B-1064

#### Partner Management – Classifiers

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Classifiers tab**

*Abb. B-481 Partner Management – Classifiers*

This tab is used for entering the classifier values for your partners. Available classifiers are those defined for the corresponding partner type - e.g. for customers - or for all partners.
⇨ Tutorial 1, "Enter a Classifier" on page B-135

> **User classifiers**
> Classifiers for employees are managed separately from the classifiers defined for the customer's company.
> ⇨ "Employee Classifiers" on page B-842

The fields in sections **Identification**, **address**, and **Connections** are explained in connection with tab **Address**.
⇨ "Partner Management - Address" on page B-809

**Classifiers (list)**
This list shows all classifiers that can be allocated to the partner.
- **A (alpha-numerical):**
  To make an entry here, open the dialog **Classifier value allocation** by double-clicking on the **Value** field.
  ⇨ "Classifier Value Allocation" on page B-843
- **N (numerical):**
  You can make this entry right in the **Value** field.
- **D (date):**
  You make this entry directly in the **Value** field.

#### Partner Management – Finances

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Finances tab**

*Abb. B-482 Partner Management - Finances*

You can use this tab to enter the settings for the invoices to be issued for this customer.
⇨ Tutorial 1, "Finances and Balance" on page B-141

The fields in sections **Identification** and **Address** are described in connection with the **Address** tab.
⇨ "Partner Management - Address" on page B-809

**Bank**
- **Bank code/BIC**: Customer's bank account. Bank code, BIC (Business Identifier Code), and the name of the bank appear automatically when the bank is selected, provided that all bank details have been entered.
  The zoom function can be used to search for the required bank.
  You can use the directory icon for entering further bank accounts or for completing the existing details.
  ⇨ "Banks" on page B-932
- **Direct debiting**: You can use direct debiting to get payment for this customer's invoices. This code will be transferred to financial accounting. This checkbox does not appear for suppliers in partner management.
  - Invoices will be paid in the agreed way.
  - Invoices will be paid by direct debiting.
- **Acct. No.**: Customer's account number, e.g. for credit notes.
- **IBAN**: International Bank Account Number. If the customer number and the bank details are correctly entered in dialog **Banks**, you can use the menu **Functions** to determine the IBAN.
  ⇨ "Banks" on page B-932

**Due date calculation**
You can set the due date calculation for every single customer. Calculation will be based on the due date stated in the order. Only mode 11 is based on the delivery date.
⇨ Tutorial 1, "Due Date Calculation" on page B-143
- **Mode**: The mode defines how due dates should be calculated for this customer. When you select a mode, a short text appears along with the calculation. The following calculation modes are available:
  - **0: Date of issue:** Invoice is due immediately.
  - **1: Date of issue + payment term:** By default this is invoice date + 30 days but other payment terms can be entered if required.
  - **2: Date of issue + payment term rounded to 1. Date of payment or month's end:** If a date of payment is defined, the due date is calculated from the rounded total of date of issue + payment term. If no date of payment is defined, the month's end is used for rounding.
  - **3: Date of issue + payment term, rounded to the 15th day of the month or end of month:** Like 2, rounded to the 15th day of the month or to month's end.
  - **4: Date of issue + payment term rounded to the 10th or 20th of the month:** Like 2, rounded to the 10th or 20th of the month, or to month's end.
  - **5: Date of issue + month's end + payment term:** The payment term is calculated starting from the first day of the month following the date of invoice.
  - **6: Date of issue + month's end + payment term rounded to first payment date:** Like 5, rounded to the first payment date.
  - **7: Date of issue + payment term, rounded to first, second, or third payment date:** Like 5, rounded to the next payment date in line.
  - **8: Date of issue + payment term depending on the second payment date, rounded to the first or third payment date:** Like 5, rounded to the first or third payment date.
  - **11: Due date = delivery date + payment term:** Delivery date + payment term.
- **Invoice date**: Date of invoice that is to be generally used for this customer. The setting can be changed in the order.
- **Due dates (gross days)**: Payment term agreed with the customer.
- **Payment days**: Payment days agreed with the customer.
- **Payment day postponement**: You can define that the calculation of the payment date should be postponed, e. g. to make sure that invoices do not become due during the customer's works holidays. The time of the postponement is set in the customer calendar. The type of postponement is valid irrespective of the days defined in the customer calendar:
  - **0 - No postponement:** The payment date will be calculated without postponement.
  - **1 - Equal distribution:** One due date lies within a certain period before the original due date and another due date lies within a certain space of time after the original due date.
  - **2 - Postpone by period:** Due dates will be postponed by a certain space of time.
  - **3 - Postpone by period + surcharge:** Like option 2 plus a surcharge.
  ⇨ Tutorial 1, "Editing Customer's Calendars" on page B-165

**General**
You can use the directories to proceed to the corresponding dialogs in order to enter more data.
- **VAT ID**: VAT ID. The number must not contain blanks. It can be printed on the forms.
- **Tax number**: Customer's tax number.
- **Paymt. terms**: Payment terms agreed with the customer. The setting can be changed in the order.
  ⇨ "Payment Conditions" on page B-930
- **Paymt. mode**: Payment mode agreed with the customer, e.g. invoice, cheque, bank transfer, etc. This setting can be changed in the order.
  ⇨ "Payment Mode" on page B-939
- **Solvency**: Information on the customer's credit standing. Further solvency levels can be defined in the directory. This field will not be shown for suppliers.
  ⇨ "Credit Rating" on page B-930
- **Lock code**: Options for the lock code are:
  - **Not locked:** Orders can be entered for this customer.
  - **Locked:** The customer does not appear in the partner search and orders cannot be entered for him either. A message to that effect is displayed.
  - **Replicated:** Customer data are kept in the master database and cannot be changed in the slave database.
- **No reminders**: You can define whether the customer should get reminders at all. This code is transferred to financial accounting (FinAcc). This checkbox does not appear for suppliers.
  - The customer can get reminders.
  - No reminders should be sent to the customer even if there are unpaid invoices.
- **(Reminder text)**: Way in which the customer should be reminded, e.g. common, severe. This code is used for transfer to financial accounting.
- **Main acct.**: Customer number of the main debtor. The customer number will be used as an account number by default. There are the following exceptions:
  - If an alternative invoice address has been defined as a subsidiary or an independent customer, this customer number can be used as the account number.
  - The main account matches the main debtor's customer number in this case. If this field is blank, the number of the current customer will be automatically used as the main account.
  - If the checkbox **Transfer customer account instead of customer number** is checked in 'Options' for the transfer to Microsoft Business Solutions XAL (MBS-XAL) financial accounting, the customer's debtor number will be transferred as the account number.
- **Creditor acct.**: A+W Business permits 8-digit customer numbers that are also used as customer numbers. If you are using a financial accounting program that can handle e. g. only 5-digit customer numbers, you can enter the corresponding number as a reference.

**Tax data**
- **Tax 1-5**: You can assign different tax rates to a customer by selecting the required entries. The tax rate for VAT is usually selected in the first field, e.g. 19%. If you are using Brazilian taxation you have to check the appropriate checkboxes, too. The settings can be changed in the order.
  ⇨ "Tax" on page B-928
  ⇨ "Brazilian Tax" on page B-940
- **Calculate 2. tax based on 1.**: In some countries, the invoice total can be subject to another tax.
  - VAT 2 should be calculated irrespective of VAT 1.
  - VAT 2 will be based on VAT 1.

> **Example**
> | Item | Amount |
> | :--- | :--- |
> | Turnover | 100.00 |
> | Tax 1 (7%) | 7.00 |
> | **Subtotal** | **107.00** |
> | Tax 2 (8%) | 8.56 |
> | **Total** | **115.56** |

#### Partner Management – Balance

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Balance tab**

*Abb. B-483 Partner Management – Balance*

This tab shows the credit limit. If the system reports receivables to financial accounting (FinAcc), the balance will be updated automatically.
⇨ Tutorial 1, "Finances and Balance" on page B-141

The fields in sections **Identification** and **Address** are described in connection with the **Address** tab.
⇨ "Partner Management - Address" on page B-809

**Credit limit**
If you define a credit limit for the customer, you have to enable the check as well. If the credit limit check is active and the credit limit is exceeded, this customer will be locked for order entry.
If the check is disabled, the system will not check the unsettled accounts against the credit limit. Order entry will not be locked.

- **Comprehensive check**: The credit limit check can be run for the main customer or for the individual subsidiaries:
  - **None:** There will be no credit limit check.
  - **by subsidiary:** The credit limit of every independent subsidiary will be checked. Only if subsidiaries are marked as independent, orders can be entered and checked by subsidiary. You have to set the check and the values in fields **Credit limit 1/2** for every independent subsidiary.
  - **By main account:** The main account's credit limit will be checked. If no independent subsidiaries have been defined, this includes all orders entered for this customer. If you have defined independent subsidiaries and have entered a main account for each of them, the check will include all subsidiaries.
- **Check**: The credit limit check is based on the entries in fields **Credit limit 1/2**. You can select one of the following methods:
  - **No check:** There will be no credit limit check.
  - **Limit 1 + report limit 2:** The entry in field **Credit limit 1** defines the lock. The entry in field **Credit limit 2** is only checked.
  - **Limit 2 + report limit 1:** The entry in field **Credit limit 2** defines the lock. The entry in field **Credit limit 1** is only checked.
  - **Check limit 1:** Only the entry in field **Credit limit 1** defines the lock.
  - **Check limit 1+2:** The entries in fields **Credit limit 1** and **Credit limit 2** define the lock.
  - **Check limit 2:** Only the entry in field **Credit limit 2** defines the lock.
  - **Cash in advance:** Orders will be produced only after the invoice amount has been received.
- **Receivables (due since...)**: If the credit limit should be checked, you can define how old the unsettled accounts to be checked have to be.

> **No check at item entry**
> The credit limit will be checked only when the order header is entered. There will be no check at item entry.

**Cost and surcharge calculation**
> **Prerequisite**
> Cost and surcharge calculation can be shown only if the checkbox **Production cost calculation** is checked in allocation of rates, and the surcharges are defined in company data.
> ⇨ "Rate allocation" on page B-726
> ⇨ "Cost and surcharge calculation" on page B-1004

- **Special surcharge**: Special surcharge to be taken into account for cost and surcharge calculation for this customer.

**Financial values (check by subsidiary)**
- **Credit limit 1/2**: Two entries can be made for the credit limit:
  - **Credit limit 1:** This entry defines the secured credit limit.
  - **Credit limit 2:** This entry is an internal credit limit granted to the customer because of his credit standing.
  You have to enable this check to prevent that orders can be entered after the credit limit is exceeded.
  At document entry, the system checks if the customer's credit limit is exceeded. The document status is automatically set to 700.
  ⇨ Tutorial 2, "Status administration" on page B-492
- **Receiv. (FinAcc/date)**: Receivables are reported from financial accounting (FinAcc). These fields will be filled in only if there is an appropriate interface with financial accounting. Apart from the total unsettled accounts, the report date is shown.
- **Liabilities**: Receivables are reported from financial accounting. This field will be filled in only if there is an interface to financial accounting.
- **Orders**: Shows the total orders on hand including the invoices that have not been transferred to financial accounting yet.
- **Balance 1/2**: The balance is calculated from the credit limit - UA (FinAcc) - Orders - Receivables. Balance 1 is insured while Balance 2 depends on your company's scope of discretion.
- **Turnover current year/month**: Customer's turnover in the current year and in the current month. The fields are filled from module **Turnover statistics**.
- **Turnover prev. year**: Customer's turnover from last year. The icon can be used to open the dialog **Turnover/order area** where you can view the turnover by order area, year, and month.

**Currency/rate**
- **Currency**: Standard currency for orders from this customer. The setting can be changed in the order.
  ⇨ Sales, "Header data - terms" on page C-1554
- **Exch. rate fixed**: You can define that the foreign currency amount is calculated only at order entry, according to the current rate.
  - Conversion is based on the current rate, which is maintained in dialog **Currency**.
  - The amount in foreign currency will not be recalculated when the invoice is issued.
  ⇨ "Currency" on page B-932
- Choose an option to define whether documents can be issued in foreign currency.
  - **No currency:** Documents for this customer can be entered in national currency only.
  - **Order entry in national currency:** Documents for this customer are entered in national currency by default. Prices can be shown in home or foreign currency.
  - **Order entry in foreign currency:** Documents for this customer are entered in foreign currency as a standard. Prices can be shown in home or foreign currency.
  ⇨ Sales, "Document group" on page C-1535

**Discount calculation**
> **Prerequisite**
> Cash discount can be calculated only if the checkbox **Cash discountable** is enabled in product master data.
> ⇨ "Suited for discount, cash discount" on page B-682

Choose an option to define how the cash discount is going to be calculated:
- **On gross amount:** Cash discount is calculated from the gross order total.
- **On net amount (gross minus cash discount):** Cash discount is calculated from the net order total, and is deducted from the gross amount.
- **On net amount:** Cash discount is calculated from the net order total.
⇨ Tutorial 1, "Cash Discount" on page B-159

#### Partner Management - Sales

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Sales tab**

*Abb. B-484 Partner Management - Sales*

This tab shows the lists of current orders and quotes for this customer. For suppliers, inquiries and purchase orders are listed. A customer can also be allocated up to two sales representatives.

The fields in sections **Identification**, **address**, and **Connections** are explained in connection with tab **Address**.
⇨ "Partner Management - Address" on page B-809

**Sales data**
The fields **Sales rep. 1** and **2** will not be displayed for suppliers.
- **Sales rep. 1, 2**: The customer can be allocated two sales representatives. The sales representatives are adopted for the order and can be changed if required.
- **Turnover share sales rep. 2**: Share of sales representative 2 in the customer's total turnover. This entry will be adopted for the order and can be changed if required.
> **Commission rate in order**
> The defined commission rate is shown on the order only if interactive sales commission is enabled in company data.
> ⇨ Software Reference, "Interactive sales commission" on page B-961
- **iQuote**: With this option, you have the opportunity to decide for each partner individually whether or not there should be a transfer to the A+W iQuote system.

**Current quotations**: This list shows the quotations for this customer for which no order has been placed (yet).

**Current orders on hand**: This list shows all orders that have not been archived yet.

**Current enquiries**: For suppliers, this list shows all enquiries for which no purchase order has been issued (yet).

**Current purchase orders**: For suppliers, this list shows all purchase orders that have not been archived.

#### Partner Management – Production

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Production tab**

*Abb. B-485 Partner Management – Production*

This tab serves to make the settings for production and dispatch. For your internal list, you can also define the surface capacity you will usually book for this customer.
The fields in sections **Identification** and **Address** are described in tab **Address**.
⇨ "Partner Management - Address" on page B-809
The fields in the sections **Production labels**, **Shipping**, and **Rack optimization** only appear for customers.

**Capacity areas**
Enter the square meters of IG, laminated, and/or toughened glass scheduled for this customer for the individual weekdays. These details will not be transferred to capacity planning or production. They only serve as an internal estimation of production capacity.
Total capacities are defined in company data.
⇨ "Capacity areas" on page B-1004

**Production labels**
- **Layout / Logo**: Only in connection with A+W Production. The fields Layout and Logo are used for printing the customer's logo on the production labels. This requires a thermo transfer printer and has to be discussed with A+W Software GmbH. These fields will not be displayed for suppliers.

**Product code**
This field appears only if CPIP creation is enabled in company data. The CPIP code can be checked only if the appropriate data have been selected in product management.
⇨ "CPIP data" on page B-683
⇨ "CPIP creation" on page B-977
- **CPIP creation**: Characteristic Performance Identification Paper (characteristics of features and of the performance).
  - No CPIP code will be created.
  - At document entry, the CPIP code is determined based on the product data, and entered in **Item entry > Supplement** tab. The restrictions can be disabled. The data will be transferred to A+W Production during export.

**Shipping**
The fields in sections Shipping and Rack optimization do not appear for suppliers.
- **Sorting**: Only in connection with A+W Production.
- **Packing**: Only in connection with A+W Production.
- **Distance**: Distance (one-way, in kilometers) to be charged per delivery round. Together with the mileage fee for the allocated route, this value is used for calculating the freight charges.

**Packing optimization**
- **Packing rule**: Currently not used.
- **Group creation**: Currently not used.

**Grill Entry**
- **Cutback (single)**: For the bender, you can define the distance between outside glass edge and aluminium spacer.
- **Calculation type**: Standard calculation of drilling points for grills for this customer:
  - **Field-symmetrical:** Holes will be calculated so that the fields are symmetrical.
  - **Drill hole-symmetrical:** Drilling will be calculated so that the drill points are symmetrical.
  ⇨ Tutorial 1, "Calculation type for grill construction Prices and Surcharges" on page B-228
  The setting can be changed in the order.

**Spacer settings**
- **Type**: Spacers that are fitted for this customer as a standard. The setting can be changed in the order.
- **Color**: Color (variant) to be used for this customer by default. The setting can be changed in the order.

#### Partner Management – Attachments

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Attachments tab**

*Abb. B-486 Partner management - attachments*

This tab can be used for attaching files with additional information, e.g. special agreements. The files are linked and are saved in a partner-specific directory.
⇨ Sales, "Attaching documents" on page C-1173

The fields in sections **Identification**, **Address** are described in connection with the **Address** tab.
⇨ "Partner Management - Address" on page B-809

**File attachment**
All linked files are listed. You can enter a comment for every linked file, e.g. regarding its validity.
Define the path for the storage location in the company data.
⇨ Master data, "File attachments" on page B-956

**Declaration of performance**
The dispatch of declarations of performance can be enabled per partner (customer).
- No declaration of performance will be dispatched for the current partner.
- A declaration of performance will be dispatched for every order item to this partner. A flag will be set after the first dispatch so that the same declaration of performance will not be sent again.
⇨ "Declaration of Performance, Management" on page B-661

### Free Numbers / Areas

**Master Data > Partners > Customer, Supplier > Customers, Suppliers > [Zoom]**

*Abb. B-487 Free numbers*

This dialogue shows the free numbers that can be used for entering new master data.
⇨ Tutorial 1, "Input of Partner Master Data" on page B-110

### Telecommunication Data

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Address tab > [Connections]**

*Abb. B-488 Telecommunication Data*

This dialog shows the defined phone and fax numbers. If you are using a telephone software system, you can dial a number by double-clicking on it.

### Invoicing Surcharge/Minimum Value per Order Area

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Order tab > [Order area]**

*Abb. B-489 Invoicing surcharge/Minimum value per order area*

You can use this dialog to enter a special minimum invoice value or an invoicing surcharge per order area. The surcharges are described in connection with the tab **Order**.
⇨ "Mode” on page B-814

### Route Priority

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Order tab > [Route priority]**

*Abb. B-490 Route Priority*

This dialog shows all partners who belong to the same route. Data are loaded from customer master data and from dialog **Delivery time**. You can change the route sequence in dialog **Delivery time**. These entries are used at order entry.

### Text Search

**Master Data > Partners > Partner management > Text tab > [Zoom]**

*Abb. B-491 Selection of predefined text*

This dialog shows all defined text. Select a text module and press [OK] to adopt it for partner management.
⇨ "Text" on page B-1064

### Turnover/Order Area

**Master Data > Partners > Partner Management > Balance tab > [Last year's turnover]**

*Abb. B-492 Last year's turnover per order area*

This dialog shows the previous year's turnover of the customer per order area. The options in section **Selection** can be used for modifying the display.

### Subsidiary

**Master Data > Partners > Customer > Customers > Employees/Subsidiaries/Documents tab > double-click on Subsidiary**

*Abb. B-493 Customers - Subsidiary*

This dialog is used to enter data for your customer's subsidiary. The info section shows the actual subsidiary you are about to enter or change.
The fields in this dialog are described in detail in connection with dialog **Partner Management**.
⇨ "Partner Management" on page B-808

> **Standard shipping address**
> The customer's standard shipping address is entered as a subsidiary. When you define a subsidiary as the standard shipping address you have to check checkbox **Standard** on the **Address** tab.
> To finish input or modification of the subsidiary, click on the **Back to main company** icon.

### Employee

**Master Data > Partners > Customer > Customers > Employees/Subsidiaries/Documents tab > double-click on Employees**

*Abb. B-494 Customers - Employees*

This dialog is used for entering the names of your customer's employees plus additional information such as the department in which he/she works, his/her function, phone extension, fax number, and email address.

**Address**
- **Name 1-3**: Full name of the employee, e.g. Dr Richard Sander.
If this employee's address differs from the company's address you can enter the details at this point.

**Connections**
Phone number(s), fax number, email address of the employee.

**Contact (order processing), Contact (sales)**
You can define whether the employee is the only contact in questions of order processing and/or sales. These details can be used for analysis via ODBC interface.
- The employee is not explicitly responsible for order processing or sales matters.
- The employee is the contact for sales and orders.

**Specification**
- **Title and function** of the employee.
- **Info**: You can enter further details here, e.g. other aspects of his sphere of responsibility.

**Classifiers**
This section shows the allocated classifiers.

**Table**
List of this customer's employees.

**[Classifier values]**
Opens the dialog **Classifier value allocation** where an entry can be made or adopted.
⇨ "Classifier Value Allocation" on page B-843

**[Classifier definition]**
Opens the dialog **Classifiers** where you can make or adopt an entry. Classifiers for employees are managed separately from the classifiers for partners.
⇨ "Employee Classifiers" on page B-842

### Transaction Management

**Master Data > Partners > Customer > Customers > Employees/Subsidiaries/Documents tab > double-click on Document**

*Abb. B-495 Customers - Document management*

You can use this dialog for managing and tracing documents, e.g. which of the customer's employees has been asking for information, and when.
You can also record who has tracked and completed this document, and when.

**Done**
This box can be checked when a document is completed. This code appears on tab **Empl./Subsid./Documents**.
- The document is still open and should be traced.
- The document is completed.

**Tab**
- **Event:** Use this tab to enter a document.
- **Table:** This tab shows all documents (projects).
- **Text received, Text sent:** This tab can be used to enter text regarding the corresponding document.
- **Agreements:** You can use this tab to enter details regarding any agreements that have been made.

### Employee Classifiers

**Master Data > Partner > Customer > Customers > Functions menu > Employee > Functions menu > Classifier definition**

*Abb. B-496 Employees - Classifiers*

This dialog serves for managing the classifiers for your customers' employees. You can define the classifier and the types of values it can have:
- **No..:** Only numerical values can be allocated, e. g. sales figures.
- **Alpha-num.:** Numbers and letters can be allocated, e.g. exhibition give-away 2010.
- **Date:** Only dates can be allocated.
- This value is invalid for this classifier.
- This value can be allocated to the classifier.

Classifiers for employees are managed separately from those for partners. They can only be used for ODBC queries.
⇨ Tutorial 1, "Enter a Classifier" on page B-135

### Classifier Value Allocation

**Master Data > Partner > Customer > Customers > Classifiers tab > Functions menu > Classifier values**
**Master Data > Partners > Customer > Customers > Employee tab > double-click on Employee > [Classifier values]**

*Abb. B-497 Classifier Value Allocation*

You can use this dialog to enter alpha-numerical values for a classifier. The [Adopt] button is used to allocate this value to a customer or employee.
⇨ Tutorial 1, "Allocate Classifier Value" on page B-137

### Check Receivables

**Master Data > Partners > Customer > Customers > Functions menu**

*Abb. B-498 Receivables*

This dialog lists all open invoices including the sum due, the reminder date, and the reminder level.
The receivables are imported by a Workflow Task via **A+W Commercial Exchange Service**.
The receivables check only works in connection with the SQL financial accounting system Syska. This function is released in company data.
⇨ "Company Data > Financial Accounting” on page B-947

### Copy Master Data

**Master Data > Partner > Customer, Supplier > Customers, Suppliers > Functions menu > Global Changes group > Copy Master Data**

*Abb. B-499 Copy master data*

This dialog is used for copying the master data of a partner, e. g. if you have entered a partner who should be defined as a customer now.

### Partner Change

**Master Data > Partner > Customer, Supplier > Customer, Suppliers > Functions menu > Global Changes group > Change selected partner**

*Abb. B-500 Change the surcharge/partner allocation*

This dialog is used to change the allocation of automatic surcharges and special discounts for the current partner.

### Terms

**Master Data > Partners > Customer, Supplier > Customers, Suppliers > Functions menu > Miscellaneous group > Terms**

*Abb. B-501 Terms*

This dialog shows the discounts and individual prices that apply to this customer or supplier.
Discounts and prices for product groups are shown in blue and discounts for products in red.
⇨ Tutorial 1, "Discounts" on page B-412

**Discounts**
This dialog shows all discounts valid for this customer. These can refer to the individual customer or to the customer group this customer belongs to.

**Individual prices**
The prices in this section have been especially defined for this customer or customer group. This field is blank if no customer-specific prices have been defined.

## Customer

**Master Data > Partners > Customer**

This program section serves to enter data that can be allocated to your customers. The actual customer data are entered in dialog **Partner management**.
⇨ "Partner Management" on page B-805

> **Dialogs for customer and supplier data**
> Some of the dialogs are the same for customers and suppliers. They will therefore be described just once in this document.

In addition to partner management, menu **Customer** offers the following entries:
- "Discount Management (Customers, Suppliers)" on page B-847
- "Change/Copy Discounts" on page B-853
- "Delete Discounts" on page B-856
- "Parameters (Customers, Suppliers)" on page B-856
- "Customer Individual Products" on page B-858
- "Delivery Time (Customer, Supplier)" on page B-860
- "Projects (Customer, Supplier)" on page B-861
- "Projects - Documents" on page B-871
- "Purchase Hours" on page B-872
- "Purchase" on page B-873
- "Claims Calculation" on page B-874
- "History of Claims" on page B-875
- "Rounding (Customer, Supplier)" on page B-876
- "Rounding for Customer/Supplier Groups" on page B-876
- "Logo Position" on page B-877
- "Different Customer/Supplier Groups" on page B-878
- "Credit Limit Analysis" on page B-879
- "Marginal Income Limits" on page B-881
- "Exceeds Amount" on page B-881
- "Calendar (Customer)" on page B-883

### Discount Management (Customers, Suppliers)

**Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts**

Discounts can be defined for individual customers, suppliers, or for customer or supplier groups. The discounts are defined for the individual product groups and/or for the actual product.
At order entry, the program checks if a discount has been entered for the product and for the customer. If not, it will check the customer group and product group. The same applies to the input of purchase orders.

> **Dialog for customer and supplier data**
> The **Discount management** dialog is the same for customers and suppliers. It will therefore be described just once in this document.

Dialog **Customer discounts** offers the following tabs:
- Discount Management - Discount List
- Discount Management - Divergences
- Discount Management - Graduated Discounts
- Discount Management - Exchange Discounts
- Discount Management - Table

The tabs **Divergences**, **Grad. discount**, and **Exchange discounts** are accessible only if you have selected a discount from the list.

**Additional information**
⇨ Tutorial 1, "The Function of Discounts" on page B-414
⇨ "PGR" on page B-644
⇨ "Product Management" on page B-667

#### Functions menu
**Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu**

This menu allows to copy or delete discounts.
- **Copy discounts, Change discounts:**
  Opens the dialog **Copy discounts** where discounts for the selected partner can be copied or changed.
  ⇨ "Change/Copy Discounts" on page B-853
- **Delete discounts:**
  Opens dialog **Delete discounts** where discounts for the selected partner can be deleted.
  ⇨ "Delete Discounts" on page B-856

#### Discount Management - Discount List

**Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Discount List tab**

*Abb. B-502 Customer discounts - Discount list*

This tab is used for discount input and management. To edit a discount, select it from the list. The corresponding data will be loaded automatically; the appropriate fields will be released.
Discounts for product groups are shown in blue and discounts for products in red.
Discounts can be entered for every price list and price key. You can also enter different discounts for the same product group for example by allocating them to different price lists and/or price keys.
⇨ Tutorial 1, "Discounts" on page B-412

**Discount for**
Choose an option to define for whom the discount should be valid:
- **Group:** Group discounts for customers or suppliers.
- **Customer or supplier:** Discounts for individual customers or suppliers.

**Project**
Discounts can be applied to a certain project. You can select only projects that are allocated to the group, the customer, or the supplier.
⇨ "Projects" on page B-801
⇨ "Projects (Customer, Supplier)" on page B-861

**Price list, Price key**
Discounts are always allocated to a price list and a price key (rate).

**Discount information**
- **Product, Prod. grp.**: The discount always refers to a certain product or product group (MPG, PSG, PGR). If you need discounts for a project with different products, you have to enter a discount for the corresponding products or product groups.
- **Discount**: Discount in percent.
- **Default disc.**: If several discounts have been entered for a product or product group, one of them must be defined as the standard discount.
  - The discount has not been defined as the standard discount.
  - This discount is the standard discount and will be shown by default in the corresponding fields at order entry. It can be changed.
- **Valid from/to**: You can restrict the validity of discounts to a certain period. This is useful if more than one discount has been defined for a customer and a product or product group. After the define time, the discount will not be used any more for pricing, and will not be offered for selection either.

#### Discount Management - Divergences

**Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Divergences tab**

*Abb. B-503 Customer discounts - Divergences*

This tab can be used for defining rounding parameters and referring to other surcharges valid for this customer.
The fields in sections **Discount for** and **Discount information** are described in connection with the tab **Discount list**.
⇨ "Discount Management - Discount List" on page B-848

**Rounding**
- **Size rounding width/height**: You can enter customized size roundings. At pricing, the size roundings will be taken into account in the following order: Individual prices -> Discounts -> Prices -> Products -> Partners. This means that the individual price is decisive.
- **Min. quantity**: Different minimum quantities for this product or product group.
- **Minimum unit price**: Minimum unit price for the product or product group in question, which may not be underrun by the entire product. The price surcharge on the calculated price is distributed proportionally across the sales. The prices of the individual components can therefore become a unit price. The minimum price is indicated by the **Minimum calculation price** flag and can be underrun by assigning a manual unit or item price, but not by manually specifying a price per price unit.

**Group-based surcharges**
The price list and the key for the main item will be automatically used for surcharge calculation.
You can allocate another price list and/or key for surcharge calculation. The system will check whether the corresponding price groups have been defined for the price list, the price key, and the product. If so, A+W Business will search for the appropriate entries in group surcharges. If there are no entries, a message will be issued at order entry saying that no surcharges were found.
⇨ "Price Groups" on page B-745
⇨ "Group Surcharges" on page B-747

**Group-independent surcharges**
These surcharges are managed in A+W Business as **Exchange surcharges**. The principle is the same as for group-independent surcharges.
⇨ "Exchange Surcharges" on page B-729

**Miscellaneous Surcharges**
Different, Miscellaneous surcharge for the customer or customer group.

**PP calculation by supplier**
Purchase price calculation is usually based on all suppliers. If no standard supplier has been defined in the order, the purchase prices can be calculated based on the prices defined for the selected supplier.

#### Discount Management - Graduated Discounts

**Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Grad. discount tab**

*Abb. B-504 Customer discounts - graduated discount*

This tab is used for entering graduated discounts based on quantity limits.
The fields in sections **Discount for** and **Discount information** are described in connection with the tab **Discount list**.
⇨ "Discount Management - Discount List" on page B-848

**Scaling**
- **Quantity limit (unit)**: Unit of the quantity limit on which the graduation is based.
- **Overview**: This list shows all defined grades. To add another grade please double-click on the header of the first line and select the option **Add**.

#### Discount Management - Exchange Discounts

**Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Exchange discounts tab**

*Abb. B-505 Customer discounts - replacement discounts*

You can use this tab for defining discounts on exchange surcharges referring to a product or product class.
The fields in sections **Discount for** and **Discount information** are described in connection with the tab **Discount list**.
⇨ "Discount Management - Discount List" on page B-848

**Products**
This list shows all discounts granted on exchange surcharges for glass.
Whether or not these discounts will actually be used for calculation, depends on the setting **Adopt from main item** in product master data.

> **Example**
> A 5% discount is granted on the surcharge of the exchanged glass.
> A 10% discount is applied for IG.
> - Adopt from main item: 10% discount for IG will be applied.
> - No adoption: 5% discount of the exchange discount will be granted.
> ⇨ "Price parameters" on page B-678

- **Product**: Exchange product for which the discount is defined.
- **Discount**: Discount (in per cent) granted for the exchange product.

**Product Classes**
This list shows all product types and classes including the discounts currently defined.
- **Product type/ Product class**: Product type and class for which the discounts should be granted.
- **Discount**: Discount (in per cent) to be granted for this product type and class.

#### Discount Management - Table

**Master Data > Partner > Customer, Supplier > Customer discounts, Supplier discounts > Table tab**

*Abb. B-506 Customer discounts - table*

You can use this tab to view all customers or suppliers for whom discounts have been entered.
The fields in sections **Discount for** and **Discount information** are described in connection with the tab **Discount list**.
⇨ "Discount Management - Discount List" on page B-848

### Change/Copy Discounts

**Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu > Copy/change discounts**

This dialog is used for changing or copying discounts of the selected partners.
This dialog offers the following tabs:
- Copying Discounts
- Change Discounts

#### Copying Discounts

**Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu > Copy discounts**

*Abb. B-507 Copying discounts*

This tab is use for copying the discounts of the selected partner in order to transfer them to another partner or group of partners.

**Source:**
The fields in this section are the same on both tabs.
> **General change**
> To change existing discounts in general you can leave these fields blank, only entering the new values.

- **Customer/supplier, from/to**: You can select a single partner or several partners in a row. The names of the first and last partner will be displayed automatically. To select just one partner, enter the same number in both fields.
- **Group from/to**: You can select a single partner group or several partner groups in a row. The names of the first and last group will be displayed automatically. To select just one group, enter the same number in both fields.
- **All**: This checkbox is accessible only if you have selected a price list or a price key. In this case you can decide whether the discounts for all customers, suppliers, or groups should be edited or copied.
  - Only the discounts of the selected price list and/or key defined for certain partners or groups will be edited.
  - All discounts of the selected price list and/or key will be edited or copied.
- **Price list, key**: You can restrict the selection to the discounts allocated to a certain price list and/or key. In this case you can use the checkbox **all** to define whether all the appropriate discounts should be edited or just those for certain partners or groups. Please note that the `<n.e.>` entries refer to a price list or a price key. If no price list and/or key is selected, the changes will be valid for all discounts.
- **Product grp./Product - from**: You can restrict the selection to discounts allocated to a certain product group (PGR, SPG, MPG) and/or a certain product. A sequence of product groups or products can be selected in both cases. The names will be shown automatically.

**Target**
- **Customer, supplier**: Partner for whom the discounts should be defined.
- **Group**: Group for which the discounts should be defined.
- **Price list, key**: Price list and/or key to which the discounts should be allocated. These fields will be released only if a price list and/or key has been selected in section **Source**. Please note that the `<n.e.>` entries refer to a price list or a price key.
- **Overwrite existing records**: You have to decide whether existing discounts should be changed.
  - Existing discounts will be ignored.
  - The existing discounts should be changed as defined. Checkbox **Delete all discounts for the target** is locked.
- **Delete all discounts for the target**: You can decide whether the existing discounts should be deleted before new discounts are entered.
  - Existing discounts will not be deleted.
  - Existing discounts will be deleted first. The new discounts (from the source) will be created afterwards as defined. Checkbox **Overwrite existing discounts** is locked.
- **Target discounts get default code**: If discounts have been entered for several rates you can define whether the new discounts should be marked as the standard discounts.
  - The new discounts should not be marked as default discounts.
  - The new discounts should be marked as default discounts.

#### Change Discounts

**Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu > Change discounts**

*Abb. B-508 Change discounts*

This tab is used to change the discounts for the selected partner.
If no restriction has been made in section **Source**, all discounts will be changed as defined.

**Source:**
The fields in this section are the same on both tabs.
> **General change**
> To change existing discounts in general you can leave these fields blank, only entering the new values.

- **Customer/supplier, from/to**: You can select a single partner or several partners in a row. The names of the first and last partner will be displayed automatically. To select just one partner, enter the same number in both fields.
- **Group from/to**: You can select a single partner group or several partner groups in a row. The names of the first and last group will be displayed automatically. To select just one group, enter the same number in both fields.
- **All**: This checkbox is accessible only if you have selected a price list or a price key. In this case you can decide whether the discounts for all customers, suppliers, or groups should be edited or copied.
  - Only the discounts of the selected price list and/or key defined for certain partners or groups will be edited.
  - All discounts of the selected price list and/or key will be edited or copied.
- **Price list, key**: You can restrict the selection to the discounts allocated to a certain price list and/or key. In this case you can use the checkbox **all** to define whether all the appropriate discounts should be edited or just those for certain partners or groups. Please note that the `<n.e.>` entries refer to a price list or a price key. If no price list and/or key is selected, the changes will be valid for all discounts.
- **Product grp./Product - from**: You can restrict the selection to discounts allocated to a certain product group (PGR, SPG, MPG) and/or a certain product. A sequence of product groups or products can be selected in both cases. The names will be shown automatically.

**Discount change**
Choose an option to define how the discounts should be changed:
- **Absolute** and a number, e.g. 5 or -5 to reduce or increase the discounts by 5 Euros.
- **Proportional** plus a number, e.g. 2 or -2 to increase or reduce the prices by 2 per cent.
- **Fixed** if a fixed value should be applied to the discounts, e.g. 5 to set all selected discounts to 5%.

**Rounding**
Rounding to be used for the calculated discounts. Roundings are defined in **Master Data > Order > Rounding**.
⇨ "Rounding" on page B-910

**Price list, key**
Price list and key to which the amended discounts should be allocated. These fields will be released only if a price list and/or key has been selected in section **Source**. Please note that the `<n.e.>` entries refer to a price list or a price key.

**Main discounts, Graduated discounts, Exchange discounts**
You can choose the discounts to be edited. All checkboxes are checked by default.
- These discounts should not be changed.
- These discounts are going to be changed as defined.

**Discounts get default code**
If discounts have been defined for several rates you can specify which of them is going to be marked as the standard discount.
- The selected discounts will not be marked as default discounts.
- The selected discounts should be marked as default discounts.

### Delete Discounts

**Master Data > Partners > Customer, Supplier > Customer discounts, Supplier discounts > Functions menu > Delete discounts**

*Abb. B-509 Delete discounts*

You can use this dialog for deleting the selected discounts.

**Selection**
Choose an option to define the discounts to be deleted:
- **Customer:** The fields for selecting a certain customer are accessible.
- **Group:** The field for selecting the group can be accessed.
- **Rate:** The fields for selecting the price list and the corresponding key are released.

### Parameters (Customers, Suppliers)

**Master Data > Partners > Customer, Supplier > Parameters**

