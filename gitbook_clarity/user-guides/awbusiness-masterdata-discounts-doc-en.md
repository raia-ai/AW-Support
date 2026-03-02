---
description: "EN_AWBusiness_Master_Data_9_4-3"
---


# Tutorial 1: Discounts

---
## The copy function

You can copy discounts while making the following changes:
- Transfer discounts to another price list or price key.
- Transfer discounts to another partner or group.
- Raise or reduce discounts in general by a percentage or by a fixed amount.
- Transfer or change discounts for a product or a PGR.

The copy function also allows changing all discounts at once without copying them to another rate. There are different options:
- Increase by a percentage or an absolute value.
- Reduction by a percentage or an absolute value.
- Increase or reduction to a fixed amount.
- Change rounding.

*(Fig. B-216: Copy function for discounts illustrates the process of copying discounts from one rate (Year 11, Key 11) to another. Options include copying to a different partner/group with a +/- value adjustment, changing within the same rate, or copying and changing to a new rate (Year 12, Key 12).)*

---

## Settings for Discount Calculation (Company Data)

Standard discount calculation can be modified in company data.

This tab is used for defining the options for the documents. Any changes on this tab will overrule the standard calculation in A+W Business.

For a detailed description of the checkboxes please refer to the Software Reference.

*(Fig. B-217: Company data > Pricing shows a screenshot of the "Price calculation parameters" tab within the company data settings. This includes numerous checkboxes to configure how prices and discounts are calculated across the system.)*

**Key Settings for Discount Calculation (A):**
- Several individual prices permitted
- Calculate supplier price for purchased products
- No discount search for default records
- PGR combination for discounts only valid if discount exists
- Create PGR combinations using complete BOM
- Search discounts for mixed IG calculation
- Search individual price for mixed calculation IG
- Calculate min. Georgian bar length per pattern
- Calculate min. edge length per edge
- Commercial size rounding
- Calculate foreign currency from unit price x quantity
- Use main item discount rather than processing discount 0%
- No fixed adoption of item discount in case of exchange surcharge
- Recursive quantity calculation in BOM
- Adopt rate/discount from main item if rate is changed
- Use real shape size for price calculation
- Misc. surcharges (%-gross/net) with surcharge types
- Do not calculate energy surcharge by item weight
- Calculate surcharges with rounded quantities
- Delete glass-, gas-, and airspace surcharge if price/unit is defined
- Spacer does not get discount PGR of IG
- Obey currency in price master data
- Extended pricing (reference price, manual changes)
- Check min. qty. mainly by price unit
- Calculate total order price for BOM
- Total per PGR combination
- Sort individual prices by price list
- Delete surcharges only if SP and PP are zero
- Calculate external PGR key as inexact quantity limit
- Enable pricing based on macro prices
- SP relevance of customer's own glass
- PP relevance of customer's own glass
- Apply misc. surcharges to price/PU in case of manual entries
- Qty. limit on BOM level for French pricing (gas and airspaces)
- Exact calculation of surface/circumference for surface treatment
- Calculate delivery fee by delivery date instead of shipping date
- Price relevance for Shaping+Nesting shape rectangle acc. to master data

---

## Defining a discount

Discounts are defined for customers or suppliers or for customer or supplier groups. In the following example, dialog `Discount management` is opened for customers. The procedure is the same for Suppliers.

> **Copy discounts**
> If discounts have been entered already, you can copy and edit them for new customers or suppliers. In these new discounts, individual values can be changed or can be generally reduced or increased by a certain amount or percentage. This way, new discounts are easy to define. Please note that price year, price key, and rate for the target discount have to be entered before.

### How to define a discount

1.  Go to menu `Master data > Partners > Customers > Customer discounts`. Dialog `Discount management` pops up.
2.  Go to the menu `Start > New` to switch to the input mode.

*(Fig. B-218: Fields for the new discount accessible shows the 'Customer discount' dialog with the following fields marked.)*
-   **A**: Customer for whom the discount is valid
-   **B**: Rate
-   **C**: Product for which the discount is valid
-   **D**: Default discount (standard discount)
-   **E**: Amount of discount

Tabs `Discount list` and `Table` will be released only after the new discount has been saved.

3.  Choose the option `Customer` (A) and select the customer for whom the discount shall be entered.
4.  Select the price list and the price key (B).
5.  Select the option `Product` (C) and the product for which the discount shall be granted. The appropriate fields are accessible now.
6.  Go to field `Discount` and enter the value (E). The value will always be interpreted as a percentage.
7.  Tick the checkbox `Default discount` (D) if this discount shall be granted by default. You have filled in the mandatory fields now. All additional entries can be made later.

*(Fig. B-219: New discount shows the 'Customer discount' dialog with example data filled in.)*

8.  Select in the menu `Start > Save` to save the data. The data will be saved. The new discount appears on tab `Discount list`. You can add further data now, e.g. a graduation.

---

## Defining a Graduated Discount

Every discount can be graduated by a limit type. The limit types are the same as for graduated prices and surcharges.

### How to enter a graduated discount

1.  Go to menu `Master data > Partners > Customers > Customer discounts`. Dialog `Discount management` pops up.
2.  Enter a new discount or select the discount to be graduated. (See "Defining a discount" on page B-353)
3.  Go to tab `Graduated discount` to enter the steps for the graduation.

*(Fig. B-220: Define the graduation shows the 'Graduated discount' tab with the following fields marked.)*
-   **A**: Limit type for the graduation
-   **B**: Column header for discount levels

4.  Go to field `Quantity limit unit` (A) and choose the limit type, e.g. `pcs`. The setting appears in the column header (B).
5.  Use the `<Tab>` key to go to the next field and press `<Ins>`.

*(Fig. B-221: Fields for graduated discount are accessible shows the input fields for the graduation levels.)*
-   **A**: Value of the level (limit)
-   **B**: Amount of discount

6.  Enter the value (A) for the first level, e.g. 5 (pcs.).
7.  Enter the value (B) for the discount, e.g. 0 (%) if the discount shall be granted from 6 pcs. upwards.
8.  Press `<Ins>` and repeat steps 6 to 8 until all levels have been defined. You can define the discount graduation in the same way as the graduated vector price.
9.  Select in the menu `Start > Save` to save the data. The data will be saved. The new discount appears on tab `Discount list`.

*(Fig. B-222: Graduated discount - overview shows the discount list with a graduated discount and its levels displayed.)*

---

## Defining an Exchange Discount

Exchange discounts are granted for elements which are used in a BOM instead of the original element. If a surcharge is applied when a lite of an IG unit is exchanged, the resulting exchange price may be reduced by the exchange discount.

An exchange discount can refer to a single product or to a whole product group.

### How to enter an exchange discount

1.  Go to menu `Master data > Partners > Customers > Customer discounts`. Dialog `Discount management` pops up.
2.  Enter a new discount or select the discount to be edited. (See "Defining a discount" on page B-353)
3.  Go to tab `Exchange discounts` to enter the exchange product for which the discount shall be granted.

*(Fig. B-223: Define an exchange discount shows the 'Exchange discounts' tab with the following fields marked.)*
-   **A**: Product (or PGR) for which a different discount shall be granted for an exchange
-   **B**: Discount rate for the product
-   **C**: Accessible line
-   **D**: Product replacing the original one
-   **E**: Exchange discount for the product

The fields for the discount information (A, B) have been filled in when the discount was defined. The exchange discount for a product is entered as described below. The procedure is the same for a product group.

4.  Select the first line (C) in section `Products` and press `<Ins>`. You can repeat pressing the `<Tab>` key until the cursor is on section `Products`.
5.  Go to field `Product` (D) and choose the new product to be used. The product name appears on the list.
6.  Go to field `Discount` (E) and enter the percentage to be granted for the exchanged product.
7.  Select in the menu `Start > Save` to save the data.

The data will be saved. To enter further exchange discounts, select the last entry on the list and repeat steps 4 to 7.

---

## Defining a Diversion of Rates

Prices, discounts, and surcharges are always allocated to a rate (price list and key). When a product is entered in a document, price and surcharges are loaded from the allocated price list. You can define however that the prices and/or surcharges for certain customers shall be loaded from another rate, e.g. if an order refers to a project for which special rates have been defined.

### How to define the diversion to another rate

1.  Go to menu `Master data > Partners > Customers > Customer discounts`. Dialog `Discount management` pops up.
2.  Enter a new discount or select the discount to be edited. (See "Defining a discount" on page B-353)
3.  Go to tab `Divergences` to select other rates.

In this example, divergences are defined for a project if a certain product is entered in an order for this project. The procedure is the same for a product group.

*(Fig. B-224: Divergences to other rates shows the 'Divergences' tab with the following fields marked.)*
-   **A**: Product (or PGR) for which the divergences shall be valid.
-   **B**: Project for which the divergences shall be valid.
-   **C**: Different rate for prices
-   **D**: Different rate for group surcharges
-   **E**: Different rate for exchange and shape processing surcharges
-   **F**: Different discount

4.  Choose the project (B) for which the different rates shall be valid.
5.  Choose the product (A) for which the different rates shall be valid.
6.  Enter a different discount (F) for the product if required.
7.  Select the different rates:
    -   for the prices (C)
    -   for the price group-related surcharges (D)
    -   for the price group-independent surcharges (E).
    If no different rate is set, the standard rate will be used.
8.  Choose another Misc. surcharge for this customer is required. Another miscellaneous surcharge has to be selected only if this surcharge shall differ from the surcharge entered in the product definition.
9.  Select in the menu `Start > Save` to save the data. The data will be saved. The divergences for the rates have been defined.

---

## Copying and Changing Discounts

You can copy discounts, increasing or reducing them at the same time.

> **Prerequisite**
> If a discount for a new rate (price list, key) shall be copied, the new rate must be defined first. (See "Editing rates" on page B-227)

There are the following instructions on this subject.
-   "How to copy discounts" on page B-361
-   "How to change discounts in general" on page B-362

### How to copy discounts

1.  Go to menu `Master data > Partners > Customers > Customer discounts`. Dialog `Discount management` pops up.
2.  Go to menu `Functions > Copy discounts`.

*(Fig. B-225: Sources and target data for copying shows the 'Copy discounts' dialog with the following fields marked.)*
-   **A**: Select the group (Target)
-   **B**: Customer whose discounts will be copied (Source)
-   **C**: Rate (year, key)
-   **D**: Choose the product group
-   **E**: Action for target discounts

In this example, a customer's PGR discount is copied to a customer group.

3.  Choose the customer (B) whose PGR discount shall be copied. The customer name is loaded when you press `<Tab>` to continue.
4.  Tick the option `Group` (A) and select the customer group to which the discount shall be transferred.
5.  Tick the checkboxes for the rate (C). The fields `Price list` and `Key` for the source and the target are accessible.
6.  Select the price list and the key.
7.  Tick the checkbox `PGR` (D). The fields for selecting the product groups are accessible.
8.  Select the PGR or the series of product groups the discounts of which shall be copied. If you enter the same PGR in both fields, just this one will be copied.
9.  Tick the checkboxes (E) for the target discount:
    -   The existing discounts can be changed. If you do not tick the checkbox, the existing discounts will not be changed but completed by the new discounts.
    -   All copied discounts can get the default discount code. This code will be deleted for the existing discounts.
10. Click on `[OK]` to adopt the data.

*(Fig. B-226: Copy discounts shows the result after copying.)*

The discounts are copied and saved for the customer group. A message will tell you how many discounts were copied. In discount management you can view the discounts for the customer group and edit them if required.

### How to change discounts in general

1.  Go to menu `Master data > Partners > Customers > Customer discounts`. Dialog `Discount management` pops up.
2.  Go to menu `Functions > Change discounts`. Dialog `Copy discounts` appears with the tab `Change discounts`.

*(Fig. B-227: Change discounts shows the 'Change discounts' tab with the following fields marked.)*
-   **A**: Value of the change
-   **B**: Type of change (absolute, percentage, fixed)
-   **C**: Select all discounts
-   **D**: Select the customer or group (Source)
-   **E**: Rate (year, key) (Source)
-   **F**: Discounts to be changed (Main, Graduated, Exchange)
-   **G**: Target rate (price list, key) for copying

3.  Choose one of the following options from the fields in section `Source`:
    -   Tick the checkbox `all` (C) to change all discounts. Enter the price list and the key (E) to which the discounts have been allocated.
    -   Determine the discount by selecting the customer (D) or customer group, the price list, the key, the product group, and the product.
4.  In section `Change discount`, choose the option (B) for the change and enter the corresponding value (A):
    -   **Absolute** and a number, e.g. `5` or `-5` if the discounts are to be increased or reduced by 5 Euros.
    -   **Percentage** and a number, e.g. `2` or `-2` if the discounts are to be increased or reduced by 2%.
    -   **Fixed** if a fixed value shall be applied to the discounts, e.g. `12` to set all selected discounts to 12%.
5.  First choose the price list and the key (G) in which the changes shall be saved.
6.  Now tick the checkboxes (F) for the discounts to be changed.
7.  Click on `[OK]` to adopt the data.

The data will be saved.

---

## Exercises

-   Enter the following discounts for your training customer:
    -   Standard discount for colored float glass
    -   Graduated discount for laminated glass lites of 8 mm thickness
    -   Exchange discounts for the PGR IG
-   Copy these discounts to another rate and raise the discount rate by 5%.
-   Define a divergence of rates for your customer where the price group-independent exchange surcharges are diverted to PGR 2**.

### Additional Information

-   Software Reference, "Change/Copy Discounts" on page B-811
-   Software Reference, "Delete Discounts" on page B-815
-   Software Reference, “Company Data > Price Calculation" on page B-944

---

# Additional Information on the Company

Company-related settings can be made in various dialogs, e.g. to define access rights for A+W Business or for maintaining clients and subsidiaries. The major settings are explained in connection with this set of topics.

## Company-related Data

### Objectives
-   Getting an idea of the global settings.
-   Introducing clients and subsidiaries.
-   Entering one's own bank accounts.
-   Defining sales representatives and commissions.

### Benefit
-   General settings control the program behaviour, irrespective of customer, prices, and products.
-   These settings are valid for a client with its subsidiaries.
-   Commissions are paid to the sales representatives based on the turnover for product groups and/or territories.

### Note

-   **System settings**: Global settings apply to the client for whom they have been entered. They refer e.g. to pricing, interfaces, archiving.
-   **Database**: The current data are maintained in the main database. Invoiced documents are archived in separate databases. Documents can be copied from archives database to the main database.
-   **Financial accounting (FinAcc)**: There are different interfaces for exchanging data with financial accounting (FinAcc) programs. Various functions depend on the financial accounting program used, e.g. the external key, receivables reports.
-   **Data transfer**: Data transfer to other programs is usually controlled by a workflow task, e.g. transfer to financial accounting or archives.
-   **Clients**: Clients access the same server and the same database. They use the same master data, e.g. products, product groups, prices, terms.
-   **Subsidiaries**: Several subsidiaries can be defined for a client. They use the same customer and order data. Subsidiaries of clients can be billed separately.
-   **Sales territory**: A sales territory has the following functions:
    -   Calculation of commission (sales commission)
    -   Sorting criterion in A+W Business turnover statistics.
-   **Sales representative**: Sales representatives are entered as employees. To define an employee as a sales representative, he is assigned a sales territory.
-   **Commission**: Commission can refer to single sales persons, product groups, and/or rates.
-   **Commission splitting**: Commissions can be split proportionally to two sales persons. The actual splitting is defined in the order.

---

## System Settings

You can define the standard settings for your company in `Company data`. Apart from financial accounting and other interfaces, this includes price calculation, e.g. the currency to be used, and how discounts shall be applied.

A+W Business allows to manage several clients and their subsidiaries. For every client, you can define the default settings to match his business processes.

### Financial accounting (FinAcc)

By default, A+W Business is installed with interfaces to various financial accounting programs. This is why you have to choose the right interface for importing and exporting invoice data. Various functions depend on the financial accounting program used, e.g. the external key.

Depending on the interface, invoices are transferred to financial accounting automatically or manually. The status defines the minimum status an invoice has to have for this purpose. A lock status is defined to make sure it is not transferred to financial accounting a second time. (See Tutorial 2, "Lock status" on page B-423)

Cash sales invoices are excluded from transfer to financial accounting by giving them a special status.

If your financial accounting system allows to import customers and suppliers entered in A+W Business via interface, you do not have to keep your customers' and suppliers' data twice. The customer or supplier number is used to allocate and book orders and purchase orders.

Minor customers are invoiced as so-called **Miscellaneous customers**, for which a collective account in your financial accounting system is used. This saves you from having to create individual accounts for those customers.

The receivables report lists all unpaid invoices, stating the sum, reminder date, and reminder level. The credit limit and the credit limit snapshot complete the current state of accounts for the individual customer.

### Database

The main database includes all documents entered in A+W Business. To keep up the usual processing speed, old documents have to be archived and deleted from this database.

Documents are simultaneously transferred to archives and statistics, before being deleted from the main database by default. Generally, transfer to statistics is based on the month in which the document was issued while archiving is based on the year.

Upon transfer of the data to archives, the main database is re-initiated to restore the usual processing speed.

---

## Archiving

Completed business transactions will remain in the main database for a defined period after which they are automatically archived. This is based on the minimum status you have defined for archiving. All document data are saved as they are. Copies can be loaded from archives.

*(Fig. B-228: Settings for archiving shows the 'Archives' tab in company settings with the following sections highlighted.)*
-   **A**: Global settings for archiving
-   **B**: Document-related settings
-   **C**: Archiving year
-   **D**: Requirements for archiving

This example shows the settings that can be made in general (A) and those for the individual document types (B).

Archives form separate databases, each summing up a year (C). At the change of year, the system archives the documents in the corresponding archives, based on the invoice date.

Documents can be transferred to archives manually, by means of a number manager. Since archiving requires a lot of computer capacity, it is done automatically in the evenings.

## Statistics

The Statistics module in A+W Business offers a number of reports. Documents are transferred to statistics for analysis. For every document type, you can define whether and when the corresponding document is to be transferred.

Documents are simultaneously transferred to statistics and archives. For statistics, certain order data are saved in a special table in the main database.

## Day-end closing

Invoices can be transferred to financial accounting e.g. once a day, in a nightly batch. When transferred to financial accounting, documents are usually (automatically) transferred to archives and to statistics.

By means of the defined deadlines (storage days) the system checks how long these shall remain in the main database before they are automatically deleted.

All data older than the defined deadline will be deleted from the main database. You can define the deadline by document type.

> **Example**
> To create annual overviews, you should enter a long interval to have sufficient time for creating the analysis.
> Commission statistics are based on the rhythm in which commissions are calculated.

## Clients and Subsidiaries

Clients are used if several companies want to access the same server and database. Clients use the same master data, e.g. products, product groups, prices, terms. They maintain their own customer data however.

Your company can manage subsidiaries as well as clients with subsidiaries. The version you choose depends on how customer data and orders shall be managed:
-   Set up clients if your subsidiaries shall maintain their own customer data and orders.
-   Set up subsidiaries if the subsidiaries use the same customer data.

The financial accounts for each client can be maintained separately. Internal work or services can be invoiced among clients.

*(Fig. B-229: Company, client, subsidiaries - master data, customers, orders illustrates the database structure. A central `Company` with shared `Master data` (Products, Prices) can have multiple `Clients`. Each `Client` maintains its own `Customers` and `Orders` (with separate number ranges) but can share the company's master data.)*

This example shows that e.g. the number ranges for the customer numbers are defined per client. The document numbers are taken from separate number ranges.

The settings for documents and pricing are made by client. Among other things, this defines how items are entered and shown in the document. The parameters for pricing partly overrule the standard calculation defined in master data. Basically, the price and discount settings for individual customers or customer groups have top priority.

In case of subsidiaries, master data are only maintained by headquarters and are transferred to the subsidiaries (replication). If a product is deleted at headquarters, it will not be automatically deleted at the subsidiaries however. It has to be deleted manually in all subsidiaries. This way, the subsidiaries can delete a product from product management when it has been sold out.

Prerequisite for replication is that all subsidiaries are using A+W Business and that all databases have the same release.

---

## Definition of Clients

A+W Business allows to manage several clients with several subsidiaries each. Company settings are valid for a client with its subsidiaries. Clients cannot be deleted (referential integrity).

> **Maintaining the settings per client**
> Please note that new clients should be entered based on existing data. Afterwards you should check and amend the settings in all dialogs.

### How to enter a client

1.  Go to menu `Master data > Company > Company data`. Dialog `Company data` appears.
2.  Go to tab `Table` and select the client that matches the new client best.
3.  Go to the menu `Start > New` to switch to the input mode.

*(Fig. B-230: Fields for the new client are accessible shows the client definition screen with fields marked.)*
-   **A**: Number, internal company number
-   **B**: Address
-   **C**: Communication data

4.  Amend the client and company numbers. Once it has been saved, the client number cannot be changed.
5.  Enter a unique matchcode if required.
6.  Enter at least the address and communication data.
7.  Select in the menu `Start > Save` to save the data. The data will be saved.
8.  If necessary, amend further settings in dialog `Company data`.
9.  Select in the menu `Start > Save` to save the data. The data will be saved. You should now check which other amendments this client requires, e.g. number ranges, automatic surcharges.

## Enter the Bank Account

You can enter several accounts with different banks for your own company and for every client. If several bank accounts have been entered for a client, one of them must be marked as the main bank.

> **Prerequisite**
> A client's account number can be entered only if the bank data have been defined before. The IBAN can only be calculated automatically if all bank data have been entered. (See "Banks" on page B-89)

### How to enter bank accounts for a client

1.  Go to menu `Master data > Company > Banks`. Dialog `Banks` appears.
2.  Choose the client for which data shall be entered.
3.  Go to the menu `Start > New` to switch to the input mode. All fields will be deleted if no bank account has been entered for the selected client yet.

*(Fig. B-231: Fields for the new bank account are accessible shows the bank account entry screen with fields marked.)*
-   **A**: Select bank
-   **B**: Account number
-   **C**: Code for the main bank

4.  Click on the zoom icon to choose the bank (A). The bank data are loaded now. If no bank data have been entered yet you can use the directory icon to open the corresponding dialog and add the data.
5.  Enter the account number (B). The IBAN is automatically determined and displayed.
6.  If necessary, tick the checkbox `Main bank` (C). You can change this code later, after you have entered all bank accounts.
7.  Choose the client for which data shall be entered. You only need to select the client when you enter the first bank account. This step can be omitted when you enter further bank accounts for this client.
8.  Select in the menu `Start > Save` to save the data. The data will be saved.
