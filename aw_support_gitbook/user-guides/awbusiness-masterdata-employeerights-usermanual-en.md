---
description: "EN-UM-AWBusiness_12"
---


# Company

---
## Input parameters

This list shows the document types. Click on a field to select the required user.

**Description** This column offers the following entries for selection:
- **Document type**:
    - User who should be allocated the corresponding document type.
    - ⇨ "Document Type" on page B-925
- **Order area**:
    - If you are using different order areas you can e. g. allocate an order area to the document input user.
    - When this user enters an order for example, the order will be allocated to the defined order area. The document number will be loaded from the corresponding number range.
    - ⇨ "Number Ranges" on page B-918

**General** Document type or order area allocated to the user. When you select an entry, the other fields in this line will be locked.
You can only select a user in the fields per document type if you have chosen the entry <disabled> in field General.

**Orders, P.O.s, Enquiries, Quotations, Credit notes** Document types or order areas allocated to the user. These fields are accessible only if the setting disabled> has been selected in column General.

### Copy settings from selected user

**Target** User to who the user settings or table properties should be copied.

**[User settings]** Transfers the settings of the current employee to another employee. The user settings refer to all settings in menu Options at order entry and to the last used number manager in module Documents.

**[Table characteristics]** Transfers the document settings from the current employee to another.

### User settings

**[Import...]** If A+W Business has been updated to a version in which the user settings are not saved in an INI file, you can import the old settings.

## Employee Groups

**Master Data > Company > Employee groups**

*Abb. B-604 Employee Groups*

This dialog is used for defining groups of employees in order to make the management of rights easier.
⇨ "Employee Rights" on page B-1037

Four groups of employees are predefined by default: Manager, Supervisor, User, Management. Further groups can be added. Every employee is allocated to a group in dialog Employees.
⇨ "Employees - Employees" on page B-1031

**Locked** A group of employees can be locked if it is no longer needed.
- The employee group can be allocated.
- The employee group is locked and cannot be allocated. If it has been allocated, it will still be displayed.

## Employee Rights

**Master Data > Company > Employee rights**

**To the dialog description:**
⇨ "Copy rights" on page B-1039

*Abb. B-605 Management of rights - Employees' rights*

This dialog serves for managing the access rights of employees or groups of employees.

Every employee automatically gets the rights of the group he is allocated to. In addition to that, an employee can be granted further rights, or certain rights can be withdrawn from him.
⇨Tutorial 1, "User Rights" on page B-456

### Menu Profiles

This menu can be used to allocate certain rights globally. Based on the option in section Identification, the entry is released for Group or Employee. The following entries are available:
- **All programs without rights**:
Records are created for all programs, the checkboxes Execute, Change, Insert, and Delete are unchecked.
- **All programs executable**:
Records will be created for all programs. Only the checkbox Execute will be activated. All other checkboxes are disabled.
- **All programs with all rights**:
In this case, all entries for the corresponding group will be deleted, i.e. no entry = all rights.

### Functions Menu

This menu can be used for copying or deleting rights.
- **Copy rights**:
Opens the dialog Copy right.
⇨ "Copy rights" on page B-1039
- **Delete rights**:
Deletes all rights defined for a group /user.
For a group, this means that it will be given all rights.
For a user, this means that he will get all rights defined for the group.

### Options Menu

This menu can be used to print the rights of individual employees or groups. If this option is disabled, all employees or groups will be printed.

### Identification, Program selection

Choose an option to define whether you want to edit the rights of a group, of an employee, or of a program item.
- **Group**:
The field for selecting the group can be accessed. If no criteria are selected, all products will be listed.
- **Employee**:
The field for selecting the employee is accessible. If no employee is selected, all employees and groups will be listed.
- **Program**:
The field for selecting the program is accessible. If no program is selected, all programs will be listed.

**Sub-rights** Shows the sub-program for which different rights have been granted or should be granted.

> **Example**
> An employee has the right to Change orders.
> He must not change Purchase prices and Discount/order. You can withdraw the right for these sub-programs.

### Rights

The following rights can be enabled and disabled:
- **Change**: Data can be edited.
- **Insert**: New records can be entered.
- **Delete**: Records can be deleted.
- **Execute/read**: Dialog can be opened.

> **Combine the right to change and the right to execute**
> If a user should be allowed to change data, he has to have the right to execute the corresponding dialog. Without the right to execute, he cannot open the dialog even if he is allowed to make changes and delete data.

### Overview

The list shows all rights that can be granted, matching the selection criteria.

## Copy rights

**Master Data > Company > Employees' rights > Functions menu**

*Abb. B-606 Copy employees' rights*

This dialog is used for transferring the rights of an employee or a group to an (other) employee or an (other) group.

**Source, Target**
Choose an option to define the source (record) from which the rights should be transferred, and the target of the transfer.

**Cancel existing rights for this target** The rights of the target can be overridden or completed.
- The rights of the target group of employee will be overridden by the source's rights, and completed by additional rights if applicable.
- The existing rights of the target group or employee will be deleted and replaced by the source's rights.

## Status Management per Employee (Group)

**Master Data > Company > Status management per Employee (Group)**

*Abb. B-607 Status management per employee (group)*

On this dialog, you define the status ranges for one of the document types quotation, order, credit note, inquiry or PO per employee or employee group. The settings are queried in case of a manual status change.

If the status of the current document is in one of the specified status ranges, the employee logged in may change the status.

### Identification

With the selection of the option, you specify for which employee group or for which employee the assignments should apply:
- **Group**: The settings apply for the employees of the selected employee group.
- **Employee**: The settings only apply for the selected employee.

### Document type

Document type to which the status ranges are assigned.

### Status range assignment

**Ranges 1, 2, 3, 4 (from - to)** Selection of the beginning and end status in which the status of the document can be changed manually.

### Overview

In the overview, all assignments are displayed that correspond to the current filter settings.

## Order Areas

**Master Data > Company > Order areas**

*Abb. B-608 Order Areas*

In this dialog you define the order areas and allocate to them the corresponding business types and document types. The details are shown in the documents and can be changed if required.

The order area also serves as a sorting criterion in A+W Business turnover statistics.

Employees can be allocated to the order areas. You can also set up special number ranges for the individual order areas.
⇨ "Number Ranges" on page B-918
⇨ "Employees > Settings" on page B-1034

### Overview

**Name** Name of the order area, e.g. IG production, toughened glass production.
**Business type** Business type of the order area that will be automatically used at order entry.
⇨ "Business Type" on page B-915

**Document type** Document type of the order area that will be automatically used at order entry.

**External key** External key for communicating with other programs. External key for communicating with other programs.

**Locked** An order area can be locked if it is no longer required.
- The order area can be allocated.
- The order area is locked and cannot be allocated. If it has been allocated before, it will still be displayed.

**Default storage location** Different storage place from which the corresponding order area gets the required materials by default.

## Field Services

**Master Data > Company > Field services**

*Abb. B-609 Field services*

This dialog serves to define the sales representative. Every sales representative can be allocated a territory, based on post codes or area codes.

The order area also serves as a sorting criterion in A+W Business turnover statistics.

**Sales rep.** Sales representative. All employees entered in dialog Employees will be offered for selection.
⇨ "Employee" on page B-1031

**Comment** Additional information, e.g. name of the territory.
**from post code, to post code** These fields can be used to specify the territory based on post codes.

**External key** External key for communicating with other programs, e.g. for the transfer to financial accounting or statistical analysis.

**Area codes** Area codes of the territories for which the sales representative is responsible.

> **Example**
> Entries: 400-440, 490-510, 750 – 760, 789, 865, 900 – 960
>
> When an order is entered, the appropriate salesman will be automatically selected if you enter a phone number in field Phone, separating the area code from the phone number by a blank or a hyphen.

**Type** Type used for commission splitting:
- **<n.e.>**: No type has been allocated to the employee.
- **Salesman 1, Salesman 2**: In case of commission splitting, the percentage for the selected type will be used.

## Commission

**Master Data > Company > Commission**

*Abb. B-610 Commission management*

This dialog serves to enter the details for the standard commission rates per salesman. You can choose from different commission types.
The commission can be analyzed in module Statistics.

### Functions Menu

This menu offers the following entries:
- **Copy commission rates**: Opens the dialog Sales representatives - Copy commission rates where the commission rates can be transferred to another salesman.
  ⇨ "Sales Representatives - Copy Commission Rates" on page B-1045
- **Delete all commission rates**: Deletes all commission rates.

### Select salesman / product group

**Price list, key** Different commission rates can be defined for the individual price list. If you select the entry <n.e.> in both fields, the commission rate is generally valid.

**Salesman** Salesman for whom the entries are valid. You have to enter a commission rate for every salesman and at least for every main product group (MPG).

**Valid until** Date up to which the commission rate is valid.

**Customer** The commission rate can be valid for all customers for just for a single customer:
- **0**: The sales commission applies to all customers.
- **1-9999999**: The sales commission is restricted to this customer.

**PGR** The commission rate can be valid for a certain product group (MPG, SPG, PGR). You should enter at least one rate per MPG and per salesman.

**Product** The commission rate can be valid for all products or just for a certain product:
- **0**: The sales commission applies to all products.
- **1-9999999**: The sales commission is restricted to this product.

### Commission type

Commission is applied to certain characteristics, e.g. to the turnover. Choose an option to define the basis for calculating the commission:
- **Discount %**: Discount in percent. This setting can e.g. be used in connection with a graduation where a salesman gets the more commission the lower the discount he grants.
- **Margin %**: Marginal income as a percentage (marginal income = sales turnover - primary costs). This setting can e.g. be used in connection with a graduation acc. to which a salesman will get the more commission the higher the marginal income.
- **Turnover**: Turnover (amount). This setting can be used best in connection with a fixed commission.
- **Contribution margin**: Contribution margin (amount). This setting can be used best in connection with a fixed commission.
- **Price/PU**: Price per price unit. This setting can be used best in connection with a fixed commission.

**Graduated qty.** Quantity by which the commission should be graduated.

> **Example**
>
> | Quantity | % Commission |
> | :--- | :--- |
> | 20 | 0,500 |
> | 100 | 0,750 |
> | 9999 | 1,250 |
>
> When you choose the commission type by turnover: 13-digit numerical field.

**Commission %** Percentage to be used for calculating the commission. 8-digit numerical field.
You can enter a negative value with up to four decimals. A negative entry would reduce the commission.

**External key** External key for communicating with other programs, e.g. for transfer to financial accounting.

**Valid from** Date from which the commission rate should be valid.

### Overview

This table shows the fields with all entries that have been made to define the commission rate. Further details on the calculation of the commission have to be entered in the following columns.

## Sales Representatives - Copy Commission Rates

**Master Data > Company > Sales Commission > Functions menu > Copy commission rates**

*Abb. B-611 Copy commission rates*

This dialog can be used to transfer the commission rates from one salesman to another.

### Source, Target

**Salesman** If you select the same salesman in both fields you can copy his existing commission rates and save them together with other price lists, price keys, and a new validity before editing the quantity graduations and percentages.

**Price list, key** Source and target price lists.

**Customer** Customer for which the commission rates are valid.

**Validity, Set validity** Date from which the new commission should be valid. You can select a future date for the target.

**Change target** The target commission rates can be changed or completed.
- The commission rates defined for this salesman will be replaced by the source's commission rates and completed by additional commission rates if applicable.
- Existing commission rates for this salesman will be deleted and replaced by the commission rates from the source.

## Banks

**Master Data > Company > Banks**

*Abb. B-612 Banks*

You can use this dialog to enter your company's bank accounts. You can enter several accounts (with different banks) per client. You can enter only banks that have been defined before in dialog Banks.
⇨ "Banks" on page B-932

**Client** Client whose bank accounts are listed.

### Bank account

**Bank code/BIC** Bank code and BIC (Business Identifier Code). The zoom function can be used to search for the required bank.
Use the directory icon to enter further bank details or complete the existing entries.

**Name, Residence** Name and location of the bank will be shown automatically.

**Account** The client's account number.

**Main bank** If you have entered several accounts for a client you have to mark one of them as the main bank account.
- The currently displayed account has not been marked as the main bank account.
- The currently displayed account has been marked as the main bank account.

**IBAN** International Bank Account Number for the account in question.

### Banks

This list shows all bank accounts for the current client.

## Subsidiaries

**Master Data > Company > Subsidiaries**

*Abb. B-613 Subsidiaries*

This dialog is sued for maintaining your client's subsidiaries. The data serve for information only.

### Address

**Name** Name of the subsidiary as listed in the commercial register, or its official name.

**Street** The subsidiary's street address.

### Contact

**Phone 1-4, Fax, Email** Phone numbers, fax number, and email address of the subsidiary.

### Overview

This tab shows all subsidiaries of the selected client.

## Booking Periods

**Master Data > Company > Booking periods**

*Abb. B-614 Booking periods*

You can use this dialog to enter the booking periods. The entries will be checked at transfer to financial accounting.
To make sure that orders, P.O.s and credit notes are automatically transferred at the right time, you can define different booking periods. The transfer is triggered by the defined status.

Once the date defined e.g. for orders is reached, no further orders can be transferred to this booking period.

**Completed booking period** Date on which the booking period ends. Only the date closest to the current date is relevant for the document check.

**Order, Credit note, P.O.** The booking period only applies to the selected type.
- The booking period is invalid.
- The booking period is valid for this document type.

## Surcharge Product Assignment

**Master Data > Company > Surcharge Product Assignment**

*Abb. B-615 Product allocation surcharges*

> This dialog is used to handle special discounts and surcharges. In addition to the defined surcharges there are ten special discounts that can either be used as special discounts or surcharges, e. g. surcharges for transport/toll fees, L racks.

**Surcharge product**
Every surcharge or special discount that should be entered like a product, must be defined as a product.

### Assignment

**Client** Client for whom the surcharges should be valid.

**General, Customer** Choose an option to define whether the surcharge should be valid for a certain customer or for all customers. The corresponding input fields will be released.

**Surcharge** The defined surcharges and special discounts will be offered for selection.
⇨ Tutorial 1, "Available Surcharges/Special Discounts" on page B-397
⇨ Tutorial 1, "Defining an automatic surcharge" on page B-398

**Product** Product by which the surcharge or discount should be applied. The product name is Name 1 as defined in product management. It also appears in product and customer management in section Apply surcharges/discounts.

**Valid from - to** Space of time for which the discount or surcharge should be valid.

**Item in document** The item number defines the sequence in which the special discounts or surcharges will be added as an item in the document. It also defines the calculation sequence. The numbers can be assigned several times.
- **0**: Item-related special discounts or surcharges are defined as item 0, e.g. *Pattern inside*-surcharge, surcharge for exceeding the maximum surface.
- **950-999**: The special discounts or surcharges applied to all previous items or parts of the previous items, are defined by item numbers between 950 and 999.
- For the small quantity surcharge, all items with the same small quantity surcharge (product) will be checked; one surcharge item will be added for all of them together. The item number must be a number between zero (0) - referring to a single item - and 900 that is added at the end of the document.

> **Shipping fee for collection**
> To prevent the shipping fee from being automatically applied to the route Collection, the checkbox no shipping fee must be enabled in route management for this route.
> ⇨ "Routes” on page B-894

### Surcharge allocation

This list shows all surcharges for all clients.
When you select an entry you can change the input in the accessible fields.

## Formulas

**Master Data > Company > Formulas**

*Abb. B-616 Formula management*

> **Adding or editing a formula**
> If you need more formulas or a formula needs to be amended please contact A+W Software GmbH.

This dialog contains all formulas that can be used for automating certain tasks in A+W Business. Tab Formula shows the syntax of the formula selected on tab Table.

Via the selection in the Type field, you can restrict the display. This means that only particular formulas will be displayed in the rule entry of the iTOE. This increases clarify in the formula selection and make it easier for you to add the right formula to rules. It also prevents that a formula is executed and then it generates an error because it is executed in the wrong context. All formulas are initially set to Default; this way, no formulas are available in the rules. Here, there must first be a manual typification in the formula management.

### Options menu

This menu can be used to enable the formula check during input. You will be notified of any errors occurred when you save your entries.

## Interface service

**Master Data > Company > Interface Service**

Use this dialog to define the interfaces to be used for exchanging data between A+W Business and other programs.

Dialog Interface Service offers the following tabs:
- Interface Service – Settings for A+W Production Formats
- Interface Service - Settings for other formats
- Interface Service - Options

### Interface Service – Settings for A+W Production Formats

**Master Data > Company > Interface Service > Settings for A+W Production formats tab**

*Abb. B-617 Production reports - Settings for A+W Production formats*

This tab is used for selecting the reports you want to receive and import from A+W Production in file format.

If you are using STSP-, STSL-, STSD-, STSB-, STSG files for the reports you have to select a registration point in section Order produced at that is allocated to a status point. If such a registration point was not assigned, the report generates an error.

Registration points are entered in dialog Production registration points.
⇨ "Registration Points - Production" on page B-900

> **Locked fields**
> The fields are locked if the checkbox Import of production reports is active on the Settings of further formats tab. In this case, you cannot make any settings for A+W Production formats.

#### Identification

**Settings for** Employee to whom the settings should apply. If the settings are to be valid for all users, please select the entry Administrator. With this settings, you have to select the same registration point in section Order produced at as defined in Company data > tab Stock/PCH/EDI.

#### A+W Production formats

This is where you can select the reports to be loaded from A+W Production. The directory for the report file can be entered in the following field. The same directories have to be entered in A+W Production to make sure that the files are saved correctly. The files are imported by A+W Commercial Exchange Service.

**Import of production reports** STSP reports are mainly made by piece. For the registration point in question you can define whether the status should be raised with the first lite or only when all lites of the order have been reported.
- Report files from the shop floor will not be imported.
- The report from the shop floor is sent as a STSP file. The order status, production date, and the header or item number will be updated.

**Production release for order if sub-order has been produced** This field is accessible only if production reports are imported.
Partial orders can be created for an order. If a production report refers to such a sub-order, the status of the whole order can be changed.
- An order is not automatically set to the Production release status.
- When the sub-orders are reported as produced, the status of the main order is automatically raised to Production release.

**Adopt batch no. from order header** This field is accessible only if production reports are imported.
If the defined registration point has no status allocated, the report is processed by A+W Business capacity planning, and the status is changed accordingly.
- The batch numbers of the items are updated separately from the batch number in the order header.
- After the order header has been updated, all items with an item status over/equal with the status of the registration point produced will get the order number's batch number.
⇨ "Reg. point allocation" on page B-988

**Import scheduling reports** The STSL data of rough and detailed scheduling can be imported from production. If the defined registration point has no status allocated, the report is processed by capacity planning, and the status is changed accordingly.
- Reports from rough and detailed scheduling will not be imported.
- Reports from rough and detailed scheduling will be imported. The order status will be raised according to the defined registration point. The registration points for capacity planning (time management) have to be defined in section Options for this purpose.
⇨ "Registration Points - Production" on page B-900

**Import barcode reports** The STSD report from shop floor data collection (barcoding) serves for to update the order status, the production date, and the header and/or item number in A+W Business.
Reports are made mainly by piece. You can define whether the status should be raised with the first lite or only when all lites of the order have been reported.
If the defined registration point has no status allocated, the report is processed by capacity planning, and the status is changed accordingly. The registration points for capacity planning (time management) have to be defined in section Options for this purpose.
- Barcode reports will not be imported.
- Barcode reports will be sent as STSD files.

**Adopt production rack number for item** This field is accessible only in connection with the import of barcode reports.
If the barcode report includes rack numbers of items, these can be allocated to the items in A+W Business.
- Rack numbers will not be adopted for the item.
- The reported rack numbers will be saved in the order and allocated to the corresponding item.

**Import rack allocation reports** The STSG report defines the rack that is allocated to the corresponding order item and the quantities produced. The rack number is printed on the delivery note.
- Rack allocation reports will not be imported.
- The rack allocation report is sent as a STSG file.

> **Rack report for partial delivery**
> For partial deliveries, the quantity of the partial delivery item can be determined based on the quantity reported by the STSG file as having been packed. To do this you have to check the option Partial delivery qty. > Take rack report into account for partial deliveries when copying the order.
> The quantity of the partial delivery item is preset by the total quantity from the STSG reports for the corresponding order item in this case. It cannot be changed.

**Update production list through registration point** This field is accessible only in connection with the import of rack allocation reports.
In this field, choose the registration point used by the rack reports to raise the status. Based on the selected registration point, the production list in dialog List of status reports will be updated.
⇨ Sales, "Status message overview" on page C-1683

**Import rack receipt/exit reports** The STSK report specifies the rack status and the dates on which the rack was received/shipped.
- Reports on the receipt and shipping of racks will not be imported.
- Reports on racks received and shipped will be imported. After checking whether customer and rack do exist, shipment or return of the rack will be booked. If the rack does not exist in A+W Business yet, it will be entered as type <n.e>.

**Import breakage reports** The STSB report is used for reporting complaints and the lites broken on the shop floor. A+W Business can automatically turn these into complaint orders.
If the defined registration point has no status allocated, the report is processed by capacity planning, and the status is changed accordingly. The registration points for capacity planning (time management) have to be defined in section Options for this purpose.
- Breakage reports will not be imported.
- The breakage report is sent as STSB file.

**Create complaint orders** This field is accessible only in connection with the import of breakage reports.
- Complaint orders will not be created automatically.
- A complaint order will be automatically created based on a breakage report. This function can be allocated a standard cause and a standard reason which can be changed for the individual complaint order.

**Cause** This field is accessible only in connection with the automatic creation of complaint orders.
You can select a cause that is adopted for the automatically created complaint order. It will be loaded irrespective of the settings in Company Data > Archives tab.
⇨ "Default complaint place" on page B-992

**Reason** This field is accessible only in connection with the automatic creation of complaint orders.
You can select a reason that is adopted for the automatically created complaint order.

**Free** This checkbox is available only in connection with the automatic creation of complaint orders.
- Automatically created complaint orders are not free of charge as a standard.
- Automatically created complaint orders are free of charge by default. The setting can be changed in the complaint order.

**Order area** This field is released only in connection with the automatic creation of complaint orders. You can select an order area: the order number will be taken from its number range.

**Target NM** This field is released only in connection with the automatic creation of complaint orders. You can select a number manager to which the automatically created complaint order should be transferred.

**Import XTV reports** XTV reports serve to withdraw the stock sizes to be cut for an order. For articles with stock mode combined, the sqm reservations will be deleted from the orders.
- XTV reports will not be imported.
- The optimization report is sent as a PRODBDA* file.

#### Options

The fields in this section are available only if reports are imported for which further details can be entered.

**Allow qty. above item qty. in STSB, STSD, STSG, STSL, STSP** The shop floor can report larger quantities per item than stated in the order.
- Larger quantities per item are not permitted.
- Reports can be processed even for larger quantities.

**Capacity planning processes STSD and STSB** STSD and STSB reports can be processed by capacity planning (time management).
- Capacity planning processes no data from STSD and STSB files.
- Capacity planning will process STSD and STSB files.

**Registration point STSD** Registration point used to change the status if the STSD report is processed by capacity planning.

**Registration point STSB** Registration point used to change the status if the STSB report is processed by capacity planning.

#### Order produced at

To report an order completed, you have to enter a registration point for the reports.
If the settings should apply to all users you have to choose the same registration point as in dialog Company data.
⇨ "Company Data – Stock/Purchasing/EDI" on page B-981

**REGISTRATION POINT** Registration point that can trigger the following (additional) actions following a report:
- The production date and job number are raised in the order.
- For production orders, the receipt of goods on stock is booked.

### Interface Service – Settings for other formats

**Master Data > Company > Interface Service > Settings for other formats tab**

*Abb. B-618 Production reports - Settings for other formats*

From this tab choose the reports you want to receive and import from shop floor data collection (barcoding), from ALFERT, and from financial accounting.

#### Barcode and ALFERT formats

> **Locked fields**
> The fields in section Barcode and ALFERT formats are locked if the checkbox Import production reports is checked on tab Settings. You will not be able to make any settings for barcode formats in this case.

**Import of production reports** Reports are made mainly by piece. You can define in A+W Business whether the status should be raised with the first lite or only after reports on all lites of an order have been made.
- Report files from the shop floor will not be imported.
- Reports from production will be loaded from the AWB_STAT file.

**Adopt batch no. from order header** This field is accessible only if production reports are imported.
The batch number shown in the order header can be adopted for the items.
- The batch numbers of the items are updated separately from the batch number in the order header.
- After the order header has been updated, all items with an item status over/equal with the status of the registration point produced will get the order number's batch number.

**Import rack report files** The AH_GEST.DAT report specifies the rack status and the dates on which the rack was received/shipped.
- Reports on the receipt and shipping of racks will not be imported.
- Reports on the receipt and shipment of racks will be imported.

**Import AWPool files** The AWPool report updates the order status, production date, header and item number in A+W Business. Allocation of the AWPool status to an A+W Business status is predefined.
- AWPool reports will not be imported.
- AWPool reports are imported as POOL*.DAT files. Field Update production date from status is accessible.

**Update production date from status** This field is accessible only in connection with the import of AWPool reports.
- The production date will not be updated in the order.
- The production date will be updated in the order if one of the available statuses has been set.

#### Financial Accounting

You can use this section to make the settings for the reporting of receivables that are automatically imported by A+W Commercial Exchange Service.

**Import receivables reports** Receivables can be reported by the financial accounting program in file format. This only applies to the customer accounts.
- Receivables reports will not be imported.
- Receivables reports are imported in file format. The fields for the storage place, a backup, and a batch file are made accessible.

**Create backup file** This field is accessible only in connection with the import of receivables reports. You can save an additional backup file and enter the number of days for which it is going to be saved.
- No backup file will be saved for the receivables report.
- A backup file of the receivables reports (including a time stamp) will be saved elsewhere. The fields for selecting the directory and the storage days are made available.

**Storing days for backup files** This field is available only if a backup file is going to be saved. You can enter the number of days for which this file must remain unchanged.

**Batch file** Name of the batch file that is required for copying the files.

### Interface Service - Options

**Master Data > Company > Interface service > Options tab**

*Abb. B-619 Production reports - Options*

You can use this tab to define the intervals in which the program should search for new reports.

#### Interval

**Standard ... minute(s)** Interval for the A+W Commercial Exchange Service. If you enter 2, for example, the service will check whether there are new reports from Production every 2 minutes and, if so, import them.

**Receivables:Report** Interval for the receivables report. If you enter 120 for instance, new reports will be imported via batch every two hours.
Receivables reports can be imported only if the corresponding function is enabled on tab Settings for other formats.
The checkboxes for receivables reports must be checked in dialog Company data for this purpose.
⇨ "Company Data > Financial Accounting" on page B-947

#### Settings for automatic email dispatch

**Email dispatch** Emails from a specific sender can be automatically dispatched to a defined address.
- Emails will not be sent.
- Emails will be sent. The fields will be enabled.

**Server** Name of the server controlling the dispatch of emails.

**Port** Number of the port for email dispatch.

**Sender address, Recipient address** Email addresses to be used by default.

**Authentication** An authentication can be used for data transfer.
- The transmission confirmation will not be sent without authentication.
- The transmission confirmation requires authentication. The fields for entering the registration data are accessible.

**Use SSL encryption** Secure Sockets Layer (SSL); encryption program for safe data transfer in the Internet.
- The transmission confirmation will not be encoded.
- The transmission confirmation will be encoded acc. to the SSL log.

**User, Password** Registration data the sender uses for authentication.

## Customizing

**Master Data > Company > Customizing**

*Abb. B-620 Customizing*

This dialog is used for adjusting A+W Business and its functions to your company's requirements.
You will only be able to open this dialog if you have been logged in as an administrator, with the appropriate rights.

> **Customizing**
> Customizing may have far-reaching effects on the functions of A+W Business. To adjust A+W Business further to your company's needs please contact A+W Software GmbH to discuss and agree the required amendments.

## Data Container

**Master Data > Company > Data Container**

*Abb. B-621 Customizing data - Data container*

This dialog is used for managing data that is necessary for customizing in the A+W Business database. The names of the tabs and table columns can be configured as well.

# Text

**Master Data > Text**

This program section is used for managing text and text codes that are required for editing documents.

Menu Text offers the following entries:
- "Text Code" on page B-1063
- "Text" on page B-1064
- "System Text" on page B-1064
- "Reminder Text" on page B-1065
- "File Attachment Types" on page B-1065
- "File Attachment Remarks" on page B-1067
- "Technical Values" on page B-1067

## Text Code

**Master Data > Text > Text code**

*Abb. B-622 Text identifier*

This dialog is used for entering the text codes. Text codes serve for allocating text modules to subjects, e.g. P for production, D for delivery note, T for common text. Text codes can be used to define which text is to appear on the individual documents.
⇨Tutorial 2, "Text types" on page B-535

**Identifier** Text code, e.g. P for production text, D for postponed dates.

**Name** Name, e.g. Production for text to be transferred to production.

## Text

**Master Data > Text > Text**

*Abb. B-623 Multilingual text*

This dialog can be used for entering standard text that is frequently used, e.g. spacer text or text for postponements. The text can include wildcards which will be replaced by the actual values only when the document is printed.
⇨Tutorial 2, "Text codes and standard text" on page B-536

In case of multilingual operation, all text modules have to be entered in the corresponding language(s). Please make sure that the text numbers are not changed in the course of translation.
⇨ "Languages" on page B-636

**Language** Select the language in which the text should be printed.

**Number** Random number for the text. You should collect the text modules per text code in number ranges, e.g. 1-99 for invoices, 100-199 for quotations. If you are using module Multilingual operation, at least one text of number 0 must exist before you start entering text in a foreign language.

**Matchcode** Input of the matchcode is optional.

**Identifier** These text code is used for allocating the text for printing. By entering the code D for delivery note you can e. g. define in dialog Forms whether or not the text should be printed.

**Text type A+W Production** Item text will be transferred to production if the text code (P) for the transfer to production permits this. For those text modules you can enter the text type (external key) that is used in A+W Production for the text. If no text type has been entered, text type 1 will be transferred by default.

### Selection

This list shows all text matching the selection criteria.

### Edit text

**Buttons** You can change the font type and size and add hyperlinks, images and tables.
⇨Tutorial, "Enter text" on page C-1170

**(Input field)** Standard text or spacer text. You can use wildcards (variables) for spacer text and certain types of standard text.
⇨Tutorial 2, "Text input" on page B-543

## System Text

**Master Data > Text > System text**

*Abb. B-624 System Text*

This dialog is used for maintaining the system text. This text modules have fixed lines in the dialogs and in the forms. They can be changed (without falsifying the sense) e.g. for another language.
⇨Tutorial 2, "System text" on page B-535

> **Do not delete text**
> Logical changes can be made to the system text. System text cannot be deleted however, nor can you add new system text. Wildcards (variables) can be moved to another position in the text.

**Language** Select the language in which the text should be printed.

**Number** Shows the text number.

**Edit text** You can edit the system text, e.g. translate it into another language.

### Selection

The list shows the numbers of the system text modules.

## Reminder Text

**Master Data > Text > Reminder text**

*Abb. B-625 Reminder Text*

You can use this dialog to enter the text to be used for reminders. This text only serves for information.
⇨ Sales, "Reminding" on page C-1819

**Name** Name of the reminder text.

**External key** External key for communicating with other programs, e.g. for transfer to financial accounting.

**Locked** Reminder text can be locked for document input if it is no longer required.
- The reminder text can be allocated.
- The reminder text is locked and cannot be assigned. If it has been assigned before in a document, it will still be shown and printed however.

## File Attachment Types

**Master Data > Text > File attachment types**

*Abb. B-626 File attachment types*

Use this dialog for entering the codes for file attachments. By default, all attachments are marked as type A (all) and will always be transferred except at transfer to purchasing.

The codes can be used to control the transfer of the attached files (documents, images):
- **Transfer to production**:
File attachments for transfer in OrderXML, e. g. product information.
⇨ Production, "Settings for Transfer to Production - Text/Attachments" on page E-2255
- **Copy documents**:
Quotation to order, e. g. calculation information.
⇨ Sales, "Copy documents - text/attachments" on page C-1658
- **P.O. transfer**, e.g. product information.
⇨ Sales, "Further settings - general" on page C-1761

## File Attachment Remarks

**Master Data > Text > File attachment remarks**

*Abb. B-627 Remarks for file attachments*

On this dialog, you store standard remarks that are used very frequently. These standard remarks are offered for selection on the Order entry > Details tab.
⇨ Sales, "Header data - attachments" on page C-1560

## Technical Values

**Master Data > Text > Technical Values**

*Abb. B-628 Texts for the technical values for declarations of performance*

On this dialog, you store the technical values for the generation of declarations of performance.
The texts must be entered for each language so that declarations of performance can be generated with the appropriate translation of the characteristics into the appropriate language.
This information is not required if the user already has finished declarations of performance.

# Forms

**Master Data > Forms**

Forms can be printed or displayed on screen. Apart from documents, these can lists and reports.

Menu Forms offers the following entries:
- "Form Management” on page B-1068
- "Order Forms" on page B-1083
- "Print Jobs" on page B-1083
- "Crystal Reports" on page B-1089

## Form Management

**Master Data > Forms > Form Management**

Management of forms allows to edit the general settings for printing forms. The forms themselves can only be changed by A+W Software GmbH.

Dialog **Management of Forms** offers the following tabs:
- Form Management - Form
- Form Management - Headers/Footers
- Form Management – Text
- Form Management – Options 1
- Form Management – Options 2
- Form Management - Sketch Printing
- Form Management - Customizing

The settings are used for printing, e.g. order confirmations.
⇨ Sales, "Form/label printing" on page C-1738

> **Connection to the Algeier scanView DMS system**
> During the printing process, a PDF file can be created from the current document and transferred for DMS archiving to the Allgeier scanView system. This functionality can be used even across sites. Contact A+W Software GmbH if you want to use this functionality.

### Form Management - Form

**Master Data > Forms > Form Management > Form tab**

*Abb. B-629 Form Management - Form*

This tab serves to define the forms to be used for the individual print items. The print item is the status point used by the program internally.
⇨ "Status Allocation" on page B-915

#### Print points

Choose an option to define whether you want to view or change customer or supplier forms.
- **Standard**: The forms are generally valid.
- **Customers, Suppliers**: The forms are valid just for a customer or a supplier. The field for selecting the partner is accessible.

**Print point** Print point allocated to a form. A print point can be allocated to any number of forms.
Once a form has been entered and the print point allocated, the print point cannot be changed in the form.
If e.g. an order confirmation with print point 100-Print OC is printed, the order automatically gets the user status 21.

#### Form settings

**Name** (Internal) name of the form.

**Quantity** Number of copies to be printed. Each page of the form will be printed several times. The number of copies is entered on tab Options 1.

**Standard** If your company uses different forms for printing a document you have to define which of them will be used by default.
- The form will not be used by default.
- This form will be used by default when you start printing, e. g. an order confirmation for a certain customer.

**Language** Language allocated to the selected form. An appropriate form must be defined for every language. This function is active only if the multi-lingual version of A+W Business has been installed.
A language is assigned to every customer, and all related documents. When a document is printed, the system checks the language code and uses the appropriate form. The text will be printed in the correct language.

**Change document language** This setting can be used to change the language defined in field Language.
- The form is printed in the selected language (stan-dard setting).
- The selected language will be changed. Check the checkbox if a form is used as a production paper for instance. In this case, the production papers have to be printed in your national language (irrespective of the document's language code).

#### Report

**File Name** Allocate the form to a report file. Without this allocation, reports cannot be created.

Examples of allocations used by default in A+W Business:
- Quotation = ANGEB.QRP
- Order confirmation = AUFTRAG.QRP
- Delivery note = LIEFER.QRP
- Invoice = RECHN.QRP
- Credit note = GUTSCH.QRP
- PO request = ANFRAGE.QRP
- P.O. = BESTELL.QRP

**Print service report** Selection of the printer with which the report will be created.
For declarations of performance, for example, the value 006 - Declaration of Performance must be entered together with the appropriate language for the report. In addition, the transfer to the DMS system can be activated.
⇨ "Archiving of documents" on page B-1074

**Transfer to iQuote** Forms output can also be transferred to iQuote.
- The printed form is not transferred to iQuote.
- The printed form is transferred to iQuote.

#### Other form status

**Status point** Each form can be assigned a different status item. This is usually only necessary for cash sale forms. In this case, select the status point Cash sale.
A cash sale invoice is generally printed for cash sales. The customer pays in cash. No invoice must be issued for this kind of orders; the amount received must not be transferred to financial accounting.
If there is no status item for cash sale in your system, please create it only after checking with A+W Software GmbH.

#### Declaration of performance

**Send by email** You can specify when a declaration of performance should be dispatched.
- No declaration of performance will be dispatched when the selected form is printed.
- When the selected form is printed, a declaration of performance will be emailed automatically.

#### Forms

The list shows all forms matching the selection criteria.

### Form Management - Headers/Footers

**Master Data > Forms > Form management > Headers/footers tab**

*Abb. B-630 Form Management - Headers/Footers*

> **Prerequisite**
> The appropriate text must be entered in dialog Text.

This tab is used for selecting the text always to be printed on the form in question, e. g. if you want to appear information regarding your next company holidays on all your order confirmations.

The fields in the section Forms are explained in connection with tab Forms.
⇨ "Form Management - Form" on page B-1069

#### Text

Use the zoom icon to select one of the existing text modules for every header and footer.
⇨ "Text" on page B-1064

**Header** The selected text will appear on the form header.

**Footer** The selected text will appear on the form footer.

### Form Management – Text

**Master Data > Forms > Form Management > Text tab**

*Abb. B-631 Form Management – Text*

Enter all differences from standard printing.
The fields in the sections Print items and Forms are explained in connection with tab Forms.
⇨ "Form Management - Form" on page B-1069

**Text not to be printed** Codes of the text modules that should not appear on the selected form. An order confirmation e.g. should not include text with the text code D (delivery note) and P (production).
This setting always refers to all text modules of the selected text code. To exclude certain text modules from printing, enter them in field Variable Text.
⇨ "Text Code" on page B-1063

**Variable text** Up to ten variable text modules can be managed per form. This text can be used at random on forms, e.g. as an alternative header. The settings can be especially used for supplier- and customer-specific text. The text has to be defined in text management.

> **Example**
> Just one form is used for printing orders. The text modules Order confirmation (1) and Delivery note (2) have been entered as variable text.
> When order confirmations are printed, variable text 1 will be automatically selected and printed. For delivery notes, text 2 will be used.

### Form Management – Options 1

**Master Data > Forms > Form Management > Options 1 tab**

*Abb. B-632 Form management - Options 1*

This tab defines how the details on order items should be printed.
The fields in the sections Print items and Forms are explained in connection with tab Forms.
⇨ "Form Management - Form" on page B-1069

#### Change header

Choose an option to specify how product names should be printed:
- **Standard**: Name 1 and 2
- **Short name**: Short info
- **IG structure**: Glass names acc. to BOM
- **Always**: The item header is always output.
⇨ "Product Management" on page B-667

**Incl. shape sketch (see tab Sketch Printing)** For every form you can define whether or not a shape sketch should be printed. Size and position of the sketch are defined on tab Sketch printing.
- No shape sketch will be printed on the selected form. This setting cannot be changed in the order or in product master data.
- You can print a shape sketch for every shape item. The sketch will be printed only if the corresponding checkboxes are checked in the order or product master data.
  ⇨ Tutorial 2, "Printing sketches" on page B-552
  ⇨ "Shape sketch, grill sketch" on page B-676
  ⇨ "Shape sketch, grill sketch" on page B-1081

**Spacer in description** The product name can include the spacer. This may be important for production papers.
- The spacer name will not be printed.
- The spacer name is added to the product name.

**Print shape parameters in**
Choose an option to specify the unit for entering shape sizes.
- **mm/Inch**: Sizes are entered in millimeters.
- **cm/Inch**: Sizes are entered in centimeters.

Input in Inch is controlled via company data:
⇨ "Units of measurement" on page B-997
The size of the sketch is defined on tab Sketch printing.
⇨ "Form Management - Sketch Printing" on page B-1081

#### BOM printing

Choose an option to define how the bill of materials should be printed:
- **Standard**: Product names 1, 2 and 3 from product master data will be printed always.
- **Print BOM always**: The BOM will be printed always irrespective of the print code in product master data. The procurement type of the BOM elements will be printed as well.
- **Acc. to print code**: The print code of the individual BOM elements are checked for printing.
- **Production-relevant BOM**: Bills of material will be printed only if they are relevant for production.
The size of the sketch is defined on tab Sketch printing.
⇨ "Form Management - Sketch Printing" on page B-1081

#### Print prices

For every form you can define whether or not the item price should be printed:
- **0 - Standard**: The settings made in the order are adopted for printing. The code in the order is loaded from customer data and can be changed in the order.
- **1 - Print prices always**: Prices will be printed as a rule no matter of the settings made in the order. This setting is e.g. used for invoices.
- **2- Print prices always (totals)**: The settings made in the order will be used for printing.
⇨ Sales, "Price printing" on page C-1321
⇨ Sales, "Management of forms" on page C-1322

#### Items

**On different forms** Specifies whether order items should be printed on different forms.
- All order items are printed on the same form (default setting).
- Order items can be printed on different forms. When you start printing, another dialog appears that allows you to group different items. You can e.g. print IG items on the production papers for the IG line in this case. Items to be processed should be printed on production papers, e.g. grinding of edges on the work order for the grinding machine.

#### Archiving of documents

**Active** Define whether an archives file for a document management system (DMS) should be automatically created at printing.
- No archives file will be created when the form is printed (default setting).
- An archives file is automatically created when the form is printed.
This setting is useful if you are using a document management system, e.g. ELO. The printer has to be specified in company data.
⇨ "Document management" on page B-1008
⇨ "Reprint for document archiving" on page B-1007

**PDF template** For the AWSOA Reporting Service, the template name for PDF files can be saved.
During the printing process, the AWSOA Reporting Service reads the information about the document in question and creates the PDF file for the DMS archiving in the storage directory for the Allgeier scanView system.
Thus, declarations of performance can also be created in the Allgeier scanView system.

#### Copies

**Close printer per document** Define whether the printer should be closed after every document.
- The printer will not be closed after the form has been printed (default setting).
- The printer will be closed after a form has been printed. This is important e.g. if the printer includes an automatic stapler.

**Quantity** Number of copies to be printed. The document will be printed several times automatically. 0 means that just one copy will be printed. 1 means that an additional copy will be printed (i.e. two identical copies).

### Form Management – Options 2

**Master Data > Forms > Management of forms > Options 2 tab**

*Abb. B-633 Form management - Options 2*

This tab is used to make further settings for the printing of forms.
The fields in the sections Print items and Forms are explained in connection with tab Forms.
⇨ "Form Management - Form" on page B-1069

#### Further options

**Read customer data (bank)** The bank account can be printed on the selected form. The corresponding data have to be entered in customer master data, fields Post code/post box.
- The bank account will not be printed on the form. This makes sense for shipping notes and work orders for example.
- The bank account will be printed on the form. This is the case for invoices for instance.
⇨ "ZIP/P.O. box" on page B-811

**Print references** You can print the references on the selected form, e.g. the order number a P.O. belongs to.
- No references will be printed.
- References will be printed, e.g. the order and item number for purchase orders.

**Print prices explicitly** The implicit prices of the BOM element Processing can be printed on the selected form. Prices will be printed only if the options Standard printout or Always print BOM have been selected on tab Options 1.
- Prices of the BOM elements will not be printed.
- BOM prices will be printed on the form.
⇨ "BOM printing" on page B-1074
⇨ Sales: Tutorial, "Manual change of price" on page C-1259
⇨ Sales, "Print prices" on page C-1547

**Print rack data** Rack data to be printed on the selected form.
- Rack details will not be printed on the form.
- The racks allocated to this order will be printed on the form.

**Print customized products** Customized products can be printed on the selected form.
- Customized articles will not be printed on the form.
- Customized articles will be printed on the form.

**Print graduated due dates** Graduated due dates and the corresponding amounts stated in an order can be printed on the selected form.
- Graduated payment terms will not be printed on the form. This is the case for work orders for example.
- Graduated payment terms will be printed on the form. This is the case for invoices for instance.
⇨ Sales: Tutorial, "Due date calculation" on page C-1330

**Print shipped racks** Details on the shipped racks can be printed on the selected form.
- Rack details will not be printed on the form.
- Rack details will be printed on the form. This is e.g. useful for reminding a customer that there are racks he should return.

**Print picking for every item** You can enter a picking text for every order item. This text can be printed on the selected form.
- The picking text is printed only for the first item.
- The picking text will be printed for every item even if it repeats itself.
⇨ Sales, "Consignment" on page C-1582

**Do not repeat product text** A document can include several items with the same product. You can define if the product text should be printed for every item. Product text is defined in product master data.
- Product text will be printed always.
- If the product text of several consecutive items is the same, it will be printed just for the first of these items.

**Print CP data** The machines for producing the item and the BOM can be printed on the selected form. The data will be printed for glass only.
This setting only refers to module Capacity planning.
- Capacity planning data will not be printed.
- If an item includes capacity planning date, these will be printed on the form.

**Classifier query** Additional customer information from classifiers can be printed on the selected form. This information has to be entered in customer master data.
- Classifiers will not be checked.
- Classifiers will be printed on the form.
⇨ "Partner Management - Classifiers" on page B-821

**Read previous invoice totals** Invoice data can be checked before the document is printed on the selected form.

**Read product data** You can define whether product data should be imported again before printing.
- Product data will not be loaded again.
- Product data will be loaded again before printing.

### Management of forms - Options 3

**Master Data > Forms > Management of forms > Options 3 tab**

*Abb. B-634 Management of forms - Options 3*

This tab is used to make further settings for the printing of forms.
The fields in the sections Print points are explained in connection with tab Forms.
⇨ "Form Management - Form" on page B-1069

#### Options for print service

**Different sender for email dispatch** In this field, you set which sender address should be used for sending the forms via e-mail. This way, the sender can be changed to the e-mail address of the employee if it is entered. The address of the employee always takes precedence when the option is enabled.

**Mail subject**

**Mail body** In this field, you can enter one or several placeholders for the mail subject. These placeholders can be provided by the printing program with any text to give an opportunity to customize the e-mail. To do this, use the placeholders in the system text in the format <<text1>>, <<text2>> etc. Please note that each placeholder must be supplied with a text from the print program. Otherwise, an error message appears when starting the printout.
As soon as the form for the e-mail dispatch is selected in the printing program, the tab 4. Cover letter(mail) is activated and the required placeholders must be provided with texts. Predefined text modules can be created in the text management, which can be selected here and adapted if necessary.

**Sender of the employee** In this field, you can specify that the employee's e-mail address should be used as sender. This enables more direct communication between the end customer and the employee since the end customer can reply directly to the e-mail.

**Path for PDF file** In order to reroute the output of the form printing to a file, it is possible to store a path and file name in the form management. It is recommended to use a UNC path for the path, one to which the reporting service has access. The file name can be provided with placeholders to indicate the content of the file. The possible placeholders are displayed when clicking on the button in front of the file name and this way they can also be taken over immediately.
⇨Sales: Software Reference, "Parameter replacement" on page C-1692
So that the output goes to a file, the output in the form printing has to be set to File with the radio button Output to....
⇨Sales: Software Reference, "Output to" on page C-1741

**Check PDF file** If you enable this checkbox, you can still modify the file name before saving.

**Attachments (File1; File2;...)** If a printout is sent by e-mail, it is possible to send any file in addition to the PDF file with the actual printout. These files must be located in the Crystal Report forms folder. This folder is found in the company master data on tab 12.Print.
⇨ Software Reference, "Path" on page B-1007

**No copy to employee** You can specify whether or not the employee should also receive a copy of the e-mail.
- The employee does not receive a copy of the e-mail.
- The employee does receive a copy of the e-mail.

**Exclusive mode** This option ensures that corresponding forms are never printed more than once. This prevents, for example, that when printing individual invoices via a large number manager, the invoice numbers are always sequential. All forms for which this checkbox is enabled are executed exclusively.

### Form Management – Sketch Printing

**Master Data > Forms > Form Management > Sketch printing tab**

*Abb. B-635 Form Management - Sketch Printing*

> **Prerequisite**
> Printing of sketches requires A+W CAD Designer (Shapes) for A+W Business.
> Entries on this tab will be taken into account only if the checkbox with shape sketch has been checked on tab Options 1.
> A+W Business allows to print one page per shape item. You have to create the corresponding form with print item 544 shape sketch for this purpose.

This tab can be used to define the size of the shape sketch and the corresponding text to be printed. Use tab Options 1 to define whether shape and/or grill sketches should be printed.
The fields in the sections Print items and Forms are explained in connection with tab Forms.
⇨ "Form Management - Form" on page B-1069

#### Shape sketch, grill sketch

**Print mode (restrictions)** Selection of restrictions for printing sketches:
- **No printout**: No sketch will be printed on the selected form.
- **Shape (true to scale), grill (true to scale)**: True-to-scale sketches can be printed on the selected form. The sizes defined in the fields Height x width of sketch will be used for this purpose.
- **Shape (schematic), grill (schematic)**: Standard sketches will be printed on the selected form, neglecting the actual sizes. No true-to-scale sketches will be printed.

**Width x height of sketch** Max. width and height of the true-to-scale sketch. Printing of grill patterns must be enabled in company data.
⇨ "Print sketches" on page B-1005

**Size info** Text size for grills to make sure that these details are legible on the printout. Default is x 1.00. This means that text will be printed in its original size.

#### Text size of shape sketch

You can adapt the text size to the size of the shape sketch.

**Size info** Text size to make sure that the dimensions are legible on the printout. Default is 12 px (pixel).

**Segment text** Text size of the segment text to make sure that the text is legible on the printout. Default is 12 px.

**Deco text** Text size inside shapes to make sure that the text is legible on the printout. Default is 6 px.

### Form Management – Customizing

**Master Data > Forms > Form Management > Customizing tab**

*Abb. B-636 Form Management - Customizing*

> **Formula for the printing of forms**
> If you need formulas or a formula needs to be amended please contact A+W Software GmbH.

You can use this tab to define where a certain paragraph should start on the selected form. You have to enter the necessary forms first.
⇨ "Formulas" on page B-1051

The fields in the sections Print items and Forms are explained in connection with tab Forms.
⇨ "Form Management - Form" on page B-1069

## Order Forms

**Master Data > Forms > Order forms**

*Abb. B-637 Management of forms for direct printing*

This dialog serves to defined the forms for direct printing. These are listed in dialog Document management in menu Print > Direct printing.
⇨ Sales, "Start menu" on page C-1534

### Settings

**Name** Name by which direct printing appears in document management.

**Document type** Allocation of direct printing to the document type. This allocation can be made for all document types shown on the list:
- Quotation
- Order including order confirmation, delivery note, invoice, complaints, etc.
- Purchase order request
- Purchase order
- Credit Note

**Print point** Print point allocated by printing the selected form. This results in the user status for the document.
⇨ "Status Management" on page B-913

**Printer** Direct printing is usually allocated to a system printer. The selected printer must be available for all terminals from where printing can be started.

**Form** Form for direct printing.

**Check before printing** Direct printing can be started right away or after another check.
- Forms will be printed right away, without further checks.
- When you select the form for direct printing, the system will ask you if you want to print the form (Yes/no). The form will be printed if the answer is Yes.

## Print Jobs

**Master Data > Forms > Print jobs**

*Abb. B-638 Print Jobs*

This dialog serves for managing the print jobs. You can define several print jobs to be automatically processed by the print server, e.g.:
- Printing order confirmations for internal purposes.
- Repeated printing for a fax per customer.
- Repeated printing as an email to the salesman.

Depending on the performance of the print server you can also define the number of output processes started by different users that can be run at the same time.

> **Enter print jobs on the print server**
> If no local printer is used print jobs are best entered right at the server as the combo box Printers only shows the printers installed on your computer.

### Print Job

All settings in this area only apply to the selected print job.

**Name** Name of the print job, e.g. print OC twice.

**Document type** Document type for which the print jobs has been set up, e.g. for quotations.

### Number area

**Number from document order area** If you are working with clients and/or order areas, you can define that the document number for a print job will be adopted from the allocated number areas. This way, print jobs can be defined for certain clients and/or OM areas.
- With this setting you have to select the client and the order area that are relevant for allocating the invoice and delivery note number.
- The client and order area defined in the document will be used to allocate the invoice and shipping note number. The fields for selecting the client and order area will be locked.

**Client** Client from whose number range the document number should be taken. This combo box is released only if the checkbox Number from order area document is disabled.

**Area** The document number should be taken from the number range of this order area. This combo box is released only if the checkbox Number from order area document is disabled.

### Form selection

One or more documents can be allocated to a print job. The print server will process these print jobs in the sequence shown on the list.
You have to obey the status allocation sequence for sorting. You can use the cursor keys to change the positions of the print jobs.

Most of the following settings for printing via server cannot be changed while printing.
⇨ Sales, "Form/label printing" on page C-1738

> **Sequence acc. to status allocation**
> When allocating a form please stick to the sequence of status allocation: After each print job, the document status will be updated; lock and minimum status will be checked before printing.
> The delivery note for example can only be printed after an order confirmation has been printed.

**Form** This field serves for selecting the form. The available checkbox depends on the print point assigned in the form.
⇨ "Form Management" on page B-1068

**Printer** This field is used for selecting the output media for the documents, e.g. printer, fax.

**Overview** This list shows all print jobs included in the selected batch. The print jobs will be started in the defined sequence.
You have to obey the status allocation sequence for sorting. You can use the cursor keys to change the positions of the print jobs.

**[Add]** Adds an other form.

**[Delete]** Removes the selected form from the print job.

### Print mode

Choose an option to define how labels should be printed. The options are available when you choose a form for labels.
- **per unit**: One label will be printed per unit.
- **per item**: One label will be printed per item.
- **per order**: One label will be printed per order.
- **acc. to document settings**: The document settings should be used.

### Special printing

**Repeat printout** This checkbox cannot be checked by hand. It is automatically checked when you select a form for repeated printing.
- Repeated printing is inactive if you have e.g. selected a form for order confirmations to which print point 100 - Print OC has been assigned.
- Repeated printing is active if you have chosen a form for repeated printing that has e.g. been assigned print point 200 - RP order confirmation.

**Archiving of documents** If you are using a document management system (DMS), e.g. in Saperion, documents can be archived. An appropriate interface has to be installed.
- Documents will not be transferred to a document management system.
- With this print job, documents are automatically transferred to the connected DMS.
⇨ "Interface service" on page B-1051

**Collective printout** Invoices can be printed collectively if this option is enabled in customer master data. A collective invoice includes all orders from a customer for which the corresponding code has been set. Collective printing requires that the documents in the number manager are sorted by customer and selection criterion.
- No collective invoices will be printed in this print job. The combo box for criteria selection is locked.
- All documents of a customer for which the code Collective invoice is active, will be printed together. The combo box for criteria selection is released:
  - **Always**: This setting overrides the collective printout setting made in the master data.
  - **By P.O. text 1**: All documents for a customer are filtered by P.O. text 1 and combined. If there are 10 orders from a customer, for example, five of which have the same P.O. text 1, six order confirmations will be printed.
  - **By shipping address**: All documents with the same shipping address will be combined.
  - **Standard**: All documents for the same customer/supplier are combined if the code for collective printout has been set.
⇨ "Partner Management - Finances" on page B-822
⇨Sales: Tutorial, "Printing of collective invoices" on page C-1149
⇨ Sales, "Partial delivery, Partial invoice, Collective invoice" on page C-1552

**Restriction of amount** You can specify whether the amount should be checked before printing:
- **All documents**: All documents will be printed without checking the amount.
- **Amount other than 0**: Documents without an amount or with an amount = 0 will be skipped at printing. This includes documents with a negative value.
- **Amount over 0**: Only documents with an order total over zero will be printed, faxed, or emailed.

**Only regular mail** This print job applies only to documents that are sent by regular mail.
- All documents will be printed acc. to the defined form.
- The documents will be printed on paper so that they can be sent by regular mail.

**Fax dispatch** This checkbox is checked automatically when you select a fax form. Fax transmission has to be enabled in partner master data, and a fax number has to be entered.
An appropriate fax interface and fax software are prerequisite for the faxing of documents.
- The documents should not be faxed.
- The documents will be faxed automatically.
⇨ "Partner Management - Address" on page B-809
⇨ "Interface service" on page B-1051

**Fax to sales representative** This checkbox is only active when you select a fax form.
- The documents will not be faxed to the salesman.
- Documents will be faxed to the salesman. The fax number has to be entered in user data.
⇨ "Employee" on page B-1031

**Email** This checkbox cannot be checked by hand. An appropriate fax interface and fax software are prerequisite for the faxing of documents.
- The selected form cannot be emailed.
- The selected form can be emailed. The following options are available:
  - **to customer**: Use this option to send a document to the customer's email address. In customer master data, document dispatch by email has to be enabled, and an email address has to be entered.
  - **to salesman**: Use this option to send a document to the salesman's email address. The email address has to be entered in user data.
⇨ "Document dispatch" on page B-814
⇨ "Employee" on page B-1031
⇨ "Interface service" on page B-1051

**Check archiving year** You can define if the archiving year set for printing of forms, should be considered for the print job. This is useful at the end of the year when the documents should be automatically archived after printing.
- The archiving year will not be checked.
- The archiving year will be checked at printing.
⇨ Sales, "Archives" on page C-1651

**Check printing date** You can define if the (manually entered) print date should be considered for a print job. When invoices are printed via dialog Print forms, the invoice date can be changed in field Print date.
- The print date will not be checked.
- The print date will be checked. This is useful for printing invoices for example.
⇨ Sales, "Print date" on page C-1740

**Non-optimized glass** This checkbox is accessible when you choose a form for labels.
- No labels will be printed for items that include non-optimized glass.
- Labels will be printed even for items containing non-optimized glass.

### Print Jobs

The list shows all saved print jobs. Select an entry to edit its settings.

## Crystal Reports

**Master Data > Forms > Crystal Reports**

*Abb. B-639 Available reports*

This dialog is used for entering hyperlinks for Crystal Reports *.RPT files. You can also enter a description of each report and allocate a data source and users or user groups. The execution of reports can be prevented or permitted by defining the appropriate rights for certain users.
The printing of the Crystal Reports is generated in a separate module, which can be accessed via the A+W Business start menu.

### Allocation

**Master Data > Forms > Crystal Reports > Select report > Context menu (right mouse key) > Allocate user, group**

*Abb. B-640 Allocation*

This dialog allows allocating a report to a user or user group.

# CEKAL

**Master Data > CEKAL**

French companies use CEKAL certificates. To get this certificate, an IG unit has to match certain quality criteria. These criteria are defined in the dialogs of this menu.

> **Requirements**
> The dialogs for CEKAL certification are accessible only if the product code CEKAL classification has been selected in company data.
> ⇨ "Product ID" on page B-956

Menu CEKAL offers the following entries:
- "Classes" on page B-1092
- "Assignment" on page B-1093
- "Results" on page B-1094
- "Allocation" on page B-1094
- "Restrictions" on page B-1096
- "Product Texts" on page B-1097

## Classes

**Master Data > CEKAL > Categories**

*Abb. B-641 CEKAL categories*

You can use this dialog for entering the variables (wildcards) for the different CEKAL categories. These variables are used for the standard text modules. At document entry, they will be automatically replaced by the text resulting from the CEKAL rules.

> **Requirements**
> This dialog is accessible only if the product code CEKAL classification has been selected in company data.
> ⇨ "Product ID" on page B-956

### Table

**No.** Number of the category.

**Name** Name of the category.

**Variable** Self-defined variable (wildcard) for the category. Please note that some of the variables have a fixed meaning in A+W Business.
⇨ Tutorial 2, "Available variables (wildcards)" on page B-597

**Level** BOM level up to which the CEKAL check should be made. This field shows zero by default.
- **0** = check main product level
- **1** = check first BOM level

**External key** External key for communicating with other programs, e.g. for transfer to production.

## Assignment

**Master Data > CEKAL > Allocation**

*Abb. B-642 CEKAL allocation*

You can use this dialog to allocate a category to every single glass product to be fitted into an IG unit, and enter the corresponding value.

> **Requirements**
> This dialog is accessible only if the product code CEKAL classification has been selected in company data.
> ⇨ "Product ID" on page B-956

**Product** Product to which a category has been allocated.

**Category** Allocated class.

**Level** Side of the pattern for which the allocation is valid.

**Value** CEKAL value of the product. Several products can have the same CEKAL value. If it has been entered before, it can be selected from the combo box. The entries are offered for selection in dialog Results.

**Remark** Additional information.

## Results

**Master Data > CEKAL > Results**

*Abb. B-643 CEKAL results*

This dialog can be used to combine the CEKAL values that have been previously allocated to products in dialog Allocation. The different CEKAL results area based on these combinations.
The combination are queried at item entry. The CEKAL result valid for the item will be saved as item text in the document.

> **Requirements**
> This dialog is accessible only if the product code CEKAL classification has been selected in company data.
> ⇨ "Product ID" on page B-956

### Assignment

**Category** Class for which the result has been entered.

**Result** Description of the result. In dialog Text allocation, these results can be allocated to the text matching the classification.

**Remark** Notes on the allocation.

### Elements

**Elements 1-10** A maximum of ten different CEKAL values can be allocated per CEKAL result. The element values are defined in dialog Allocation.

## Allocation

**Master Data > CEKAL > Allocation**

*Abb. B-644 CEKAL text allocation*

This dialog is used for defining the text to be printed for the different results. You can only allocate text that has been entered in dialog Text.
⇨ "Text" on page B-1064

> **Requirements**
> This dialog is accessible only if the product code CEKAL classification has been selected in company data.
> ⇨ "Product ID" on page B-956

### Classes

This section shows fields for all categories that have been defined in dialog Categories.
⇨ "Classes" on page B-1092

**Class 1 to 10** Result for which text should be printed.
To enter a standard CEKAL text please leave all category fields blank. In the text fields, enter the numbers for the standard CEKAL text. This will be used whenever no results are found for the categories at document entry.

### Bender

**Number** Text number to be transferred to the bender. The bender text shown below will not be taken into account when you enter a text number.

### Text

**Number** of the text to be displayed.

**General** This text will be printed on the forms and can be up to 80 characters.

**Label** This text will be printed on the labels and has to be short enough.

**Production** This text is printed on the production papers (in A+W Business or production software). It serves for internal purposes.

**Bender** This text can be transferred to the spacer bender provided that the bender can import text. When a number has been entered in the Bender section in field Number, the text entered in field Bender will not be taken into account.

### Text allocation

This list shows the text allocations by category.

## Restrictions

**Master Data > CEKAL > Restrictions**

*Abb. B-645 CEKAL restrictions*

This dialog serves to enter the restrictions for the CEKAL check.
These restrictions can be used to check technical values, e.g. the lite size or the grill thickness. There will be no CEKAL classification if these values are not met.

> **Requirements**
> This dialog is accessible only if the product code CEKAL classification has been selected in company data.
> ⇨ "Product ID" on page B-956

### Restriction values

**Number** The numbers are defined by the system.

**Parameters 1-4** Values for the individual restriction parameters. The number of changeable parameters depends on the selected restriction.

**Remark** Shows the predefined text for the restriction.

### Text

**General** This text will be printed on the forms and can be up to 80 characters.

**Label** This text will be printed on the labels and has to be short enough.

**Production** This text is printed on the production papers (in A+W Business or production software). It serves for internal purposes.

**Bender** This text can be transferred to the spacer bender provided that the bender can import text. When a number has been entered in the Bender section in field Number, the text entered in field Bender will not be taken into account.

### Bender

**Number** Text number to be transferred to the bender. The bender text shown above will not be taken into account when you enter a text number.

### Restrictions

This list shows all restrictions that can be used for the check.

## Product Texts

**Master Data > CEKAL > Product Texts**

*Abb. B-646 CEKAL product text*

This dialog is used for entering CEKAL text for special products that refer to a certain structural level. If such a product is part of an IG unit, this CEKAL text has absolute priority over other CEKAL text.

> **Requirements**
> This dialog is accessible only if the product code CEKAL classification has been selected in company data.
> ⇨ "Product ID" on page B-956

### Product selection

**Product** Product that has been allocated a special product text.

**Level** Structural level to which the text applies.

**Remark** Brief explanation of the text.

### Text

**General** This text will be printed on the forms and can be up to 80 characters.

**Label** This text will be printed on the labels and has to be short enough.
**Production** This text is printed on the production papers (in A+W Business or production software). Used for internal purposes.

**Bender** This text can be transferred to the spacer bender provided that the bender can import text. When a number has been entered in the Bender section in field Number, the text entered in field Bender will not be taken into account.

### Bender

**Number** This text can be transferred to the spacer bender provided that the bender can import text. If you have entered a bender number in section Text, the bender text entered here will be ignored.

### Text allocation

This list shows the structure-related text allocations.

# CE Code

**Master Data > CE code**

IG units that are marked with this certificate have to meet fixed quality criteria.
The CPIP code (Characteristic Performance Identification Paper) is only required in France. It provides details on the characteristics and the performance.

Menu CE code offers the following entries:
- "CPIP Code” on page B-1098
- "Size Restrictions" on page B-1098
- "IG Search Data" on page B-1099
- "Restrictions" on page B-1096
- "Settings" on page B-1100

## CPIP Code

**Master Data > CE code > CPIP Code**

*Abb. B-647 CE code - CPIP code*

You can use this dialog for entering details regarding the CPIP code, e.g. its validity, whether it has been certified, and if it matches a CE standard.
The standards and rules for CPIP creation can be imported in dialog Settings.
⇨ "Settings" on page B-1100

> **CE code with CPIP code**
> The CPIP code (Characteristic Performance Identification Paper) is only required in France. It provides details on the characteristics and the performance.

The CPIP code has to be entered for the corresponding products in product management.

## Size Restrictions

**Master Data > CE code > Size Restrictions**

*Abb. B-648 CE code - size restrictions*

This dialog allows entering the size restrictions for CPIP codes.
At order entry, the program checks whether the current item exceeds CE-relevant size restrictions. A message will appear should a restriction be violated.

## IG Search Data

**Master Data > CE code > IG Search Data**

*Abb. B-649 IG Search Data*

This dialog serves for managing the CPIP code data for IG. These data control the behavior of order entry.

> **Entering a new record**
> When you enter a new record you have to define a default for grills.
> Values that are not preset for the IG unit will be preset by default values in order to determine the CPIP code in search data.

### Table

This tab lists all search data defined in the system.

## Settings

**Master Data > CE Code > Settings**

*Abb. B-650 Master Data > CE Code > Settings*

This dialog serves for importing the files with the necessary CPIP codes and other definitions. The interface files are separated by a ^ sign. The first line must show the column name.
Depending on the size of the file, import may take some time.

### Standard values for the IG search function

This is where the standard values for non-glass elements are kept.

### File update CPIP code

Some of the database tables in this section can be filled via interface files. Select a file and start the process by pressing the [Upload] button.

# B2B

**Master Data > B2B**

This is where interface data for data transfer are entered.

Menu B2B offers the following entries:
- "Products (Customer, Supplier)" on page B-1101
- "Copying of External Products" on page B-1108
- "Spacer (Customer, Supplier)" on page B-1109
- "Gas (Customer, Supplier)" on page B-1110
- "Routes (Customer, Supplier)" on page B-1111
- "Customer, Supplier" on page B-1112
- "Document Export" on page B-1118
- "SN File Rules" on page B-1121
- "Product Import" on page B-1122
- "Price Import" on page B-1123

## Products (Customer, Supplier)

**Master Data > B2B > Customer, Supplier > Product**

Orders can be imported by EDI, and purchase orders exported. The product data for this data transfer are kept separately for customers and suppliers. The dialogs structures are identical. In this document, they are described for customers.

This section provides information on the following subjects:
- "Functions Menu" on page B-1101
- "Products - Bill of Materials" on page B-1102
- "Products - Parameters" on page B-1103
- "Products - Table" on page B-1104
- "Products - Shapes/Processings" on page B-1105
- "Products - Grills" on page B-1106

### Functions Menu

**Master Data > B2B > Customer, Supplier > Product > Functions menu**

This menu is used for exporting data. The following entries are displayed:
- **Define Dorma reference**: Enter references for Dorma products. With this function, the matchcode will always include the product's external Dorma number. This function is available for suppliers only.
- **Copy article**: Opens the dialog Copy external articles for copying the current customer's articles.
  ⇨ "Copying of External Products" on page B-1108

### Products – Bill of Materials

**Master Data > B2B > Customer, Supplier > Product > Bill of materials tab**

*Abb. B-651 Products - Bill of Materials*

This tab is used for allocating your own glass products to the business partner's products.

#### External product

**Partner** Business partner for whom the allocation is valid.

**Valid from** Data from which the allocation is effective.

**Article number** Alpha-numerical article number used by the business partner.

**Name** Name used by the business partner.

#### Identification

**Article/MCode** Article (product) number acc. to A+W Business master data.

**Name** Name as defined in master data.
**Width/Height** Sizes valid for the business partner.

**Color** Color variant valid for the business partner.

**Prices / PU**
Price:
Price per price unit.

#### BOM product

The fields in this section are accessible only if a BOM element has been selected .

**Article/MCode** Article (product) number of the selected BOM element.

**Name** Name of the selected BOM element.

**Qty. / Width / Height** Details for boxes.

**Color** Color variant of the selected BOM element.

**Pattern level** Pattern level of the selected BOM element.

**Sense of pattern** Sense of pattern of the selected BOM element.

**Coating side** Coated side of the selected BOM element.

#### BOM

The list shows the bill of materials for the selected product. Select an element to view its details in section BOM.

### Products – Parameters

**Master Data > B2B > Customer, Supplier > Product > Parameters tab**

*Abb. B-652 Products - Parameters*

This tab serves to specify whether the corresponding product number should be searched and entered automatically when the invoice is checked.
If you are using the electronic invoice check via openTRANS you can have the references entered automatically.
You can also specify that the default behavior (takeover of the names from the EDI file) is overridden, so that the import uses the product name from the company's own master data.

### Products – Table

**Master Data > B2B > Customer, Supplier > Product > Table tab**

*Abb. B-653 Products - Table*

This tab lists all allocated products.

### Products – Shapes/Processings

**Master Data > B2B > Customer, Supplier > Product > Shapes/Processings tab**

*Abb. B-654 Products - Shapes/Processings*

This tab serves to enter the parameters for shapes and processing steps. The fields are described in detail in connection with product master data in section Sales.
⇨ "Product Management - Shapes/Processing" on page B-688

### Products – Grills

**Master Data > B2B > Customer, Supplier > Product > Grill tab**

*Abb. B-655 Products – Grills*

This tab is used for entering the parameters for grills (patterns). The fields are described in detail in connection with product master data in section Sales.
⇨ "Product Management - Grills" on page B-699

### Product - Attachments

**Master Data > B2B > Customer, Supplier > Product > Attachments tab**

*Abb. B-656 Product - Attachments*

In the definition of the references for B2B products, file attachments can now be stored. These attachments are transferred to the respective order items during import. Here, however, only the references to the files are transferred. No copy of the actual files to the folder structure is made. This behavior is depicted with a corresponding link symbol in the table in the item entry.

## Copying of External Products

**Master Data > B2B > Customer, Supplier > Product > Functions menu > Copy articles**

*Abb. B-657 B2B - Copy external products:*

This dialog can be used to copy one business partner's data and transfer them to another partner.

## Spacer (Customer, Supplier)

**Master Data > B2B > Customer, Supplier > Spacer**

*Abb. B-658 B2B - Spacer*

This dialog is used for allocating your own spacer products to the business partner's products.
The spacer data of customers and suppliers are kept separately for data transfer purposes. The dialogs structures are identical.
The fields are described in detail in connection with dialog Products.
⇨ “Products – Bill of Materials" on page B-1102

## Gas (Customer, Supplier)

**Master Data > B2B > Customer, Supplier > Gas**

*Abb. B-659 B2B - Gas*

This dialog is used for allocating your own gas products to the business partner's products.
The gas data of customers and suppliers are kept separately for data transfer purposes. The dialogs structures are identical.
The fields are described in detail in connection with dialog Products.
⇨ "Products – Bill of Materials" on page B-1102

## Routes (Customer, Supplier)

**Master Data > B2B > Customer, Supplier > Routes**

*Abb. B-660 B2B-Routes*

This dialog serves to allocate your own routes to the business partner's routes.
The route data of customers and suppliers are kept separately for data transfer purposes. The dialogs structures are identical.
The fields are described in detail in connection with dialog Products.
⇨ “Products – Bill of Materials" on page B-1102

## Customer, Supplier

**Master Data > B2B > Customer, Supplier > Customer, Supplier**

The settings for customers and suppliers are maintained separately for EDI data transfer. The dialogs structures are identical. In this document, they are described for customers.

This section provides information on the following subjects:
- "Functions Menu" on page B-1101
- "Customer, Supplier - Selection" on page B-1112
- "Customer, Supplier - Parameters" on page B-1114
- "Customer, Supplier - Table" on page B-1117

### Functions Menu

**Master Data > B2B > Customer, Supplier > Customer, Supplier > Functions menu**

This menu can be used for importing or exporting command scripts.

### Customer, Supplier - Selection

**Master Data > B2B > Customer, Supplier > Customer, Supplier > Selection tab**

*Abb. B-661 B2B-Partner selection*

This tab serves to enter the settings for the EDI interface for every business partner.

#### Partner

**Number** Number of the business partner with whom you want to exchange data by EDI.

**Plant number** Number of the market partner's subsidiary.

#### Different partner for article reference

**Number** Number of the business partner to whose articles should be used as references if no special references have been defined for the current business partner.

#### Interface

**Type** Interface version. If you also want to transfer order confirmations and invoices electronically (openTRANS-Format) you have to choose the version you have been using so far for transferring the data. The version is defined when A+W Business is installed.

#### Batch number of target file

**From, Current, To** First and last number of the number range to be allocated for the batch numbers for transfer.

#### Path name

**Source path, Source file** Directory and file name for the import/export file.

**One file per document** This checkbox only appears for suppliers.
- All of a supplier's POs are written to one file.
- During export, one file per PO is generated.

**Protocol path, Log file, Backup path** Directories and file names for the log and backup file.

#### Command script

This is where you can enter a script that can be used for modifying and copying EDI files.

### Customer, Supplier - Parameters

**Master Data > B2B > Customer, Supplier > Customer, Supplier > Parameters tab**

*Abb. B-662 B2B - Interface parameters*

This tab serves to enter the parameters for the data transfer by EDI
The fields in sections Partner to Batch number are described in connection with the Selection tab.
⇨ "Customer, Supplier - Selection" on page B-1112

#### Parameters

**Compulsory referencing** Usually, references for customer or supplier products are defined in full. You have to decide however what is going to happen should references be missing.
- The product number defined in master data is saved in the interface file. This is e.g. useful if the sending and the receiving system use the same product master data. You do not have to enter data in reference tables if this is the case.
- If an item without a reference is transferred to an (external) product, this item can be ignored. An error report will be made in the logbook in this case.

**Locking active and maximum lock time** It may put quite some stress on your system if several users are using the transferred data.
- The interface file will not be locked. This setting is useful if just one program accesses the file.
- Just one program can access an interface file at a time for the defined period. The field for entering the time is released.

**Definition of document number permitted** The document number can be imported or assigned by A+W Business.
- The document number can be imported or assigned by A+W Business.
- The document number can be imported from the EDI file if not number has been assigned yet. An error message appears if a number has been assigned already.

**Adopt whole BOM from interface file** The BOM can be created from the interface file or from product master data.
- The BOM is adopted from product master data.
- The interface is selected from the structure shown in the EDI reference.

**Unit of measurement** Choose an option to specify how sizes should be interpreted in the interface file.
The settings for the measurements are generally made in company data. This default setting can be changed per customer in master data and in the documents. You have to define which unit of measurement should be used for the import.

**Size precision = 1/** If imperial measurements are enabled for the interface file, enter 32, 64 or 128, depending on the factor to be used for calculation.
If you are using metric sizes, enter 1 in field Size accuracy.

**Do not create order in case of an error** The interface file may contain errors to which the system must react.
- The data from the interface file will always be turned into an order.
- No order will be created if there are errors in the interface file. An appropriate message will be displayed at the import.
You can use the log to search for the error and correct it. After that, the data can be imported again.

**Restriction exceeded - item rejected** The interface file may include items violating the restrictions in A+W Business.
- Items violating the restrictions will be adopted as they are. The orders have to be edited by hand afterwards.
- Items violating the restrictions will not be imported. You can use the log to search for the error and correct it.

**Exchange if restriction is not met** If the interface file contains items violating the restrictions in A+W Business, alternative products can be used automatically.
- Items violating the restrictions will be adopted as they are. The orders have to be edited by hand afterwards.
- If there are items violating the restrictions, the alternative products defined in A+W Business will be used automatically.

**Permit complaints** Complaints can be imported through the interface.
Complaints are usually not permitted but imported as "common" orders. After that, the system checks if the order is a complaint.
- Complaints are not permitted.
- Complaints are permitted.

**Change basic product if 2 elements are exchanged** If more than two elements of an item are exchanged, another A+W Business product can be used automatically.
- The items are adopted as they are.
- If two elements of an item are exchanged, the system will automatically use the basic product specified in product management.
⇨ "Basic product" on page B-679

**Delete inferior edge processing** Specification of whether for edge processings all processings should be executed if they differ only in the quality, e.g. seaming and polishing on the TG.
- All edge processings are executed as they are entered.
- Only the superior edge processing is executed. The inferior edge processing is ignored.
If an edge processing should therefore affect no edge, then the whole processing is deleted from the BOM.
See also the setting in the company data.
⇨ "Company Data – Parameters" on page B-958

**Check processing parameters** During EDI import, the processing parameters in the processing record can be checked.
- Processing parameters are not checked.
- Processing parameters are not checked. If parameters are not set or values are not permitted, they are corrected automatically.
For edge processings, for example, the number of marked edges are checked; that is, if there is no shape, logically a maximum of 4 edges can be processed.

**Import of market partner-specific texts** Specification whether individual texts of the market partner should be imported.
- These texts are not imported.
- These texts are imported.

**No shape recognition** Specification whether or not a shape detection should be conducted during the EDI import of a DXF file. If no model detection is conducted, the result is a shape 99 (free shape) with a corresponding *_C.SN file in its shape record.
- The shape detection is conducted.
- No shape detection is conducted.

#### Prices

**Permit import and export of prices** Defines whether or not prices should be imported or exported.

**Deactivate calculation of surcharges/discounts** Specification whether surcharges and discounts should be calculated.
- Surcharges and discounts are calculated. Thus, the price defined in the EDI file is taken over unchanged into the document.
- Surcharges and discounts are not calculated.

### Customer, Supplier - Table

**Master Data > B2B > Customer, Supplier > Customer, Supplier > Table tab**

*Abb. B-663 B2B - table for customers, suppliers*

This tab lists all defined customers or suppliers. The interface file path is shown for those business partners for whom data transfer for EDI has been set up.

## Document Export

**Master Data > B2B > Customer > Document export**

*Abb. B-664 Settings for openTrans export*

This dialog serves to make the settings for export in openTrans format per customer. This format can be used for transferring order confirmations, delivery notifications, and invoices.

The openTRANS files have the suffix *.awotdis, *.awotres oder *.awotinv.

### Customer

**Number** Number of the business partner who should get the documents in openTrans format.

### Interface

**Type** Interface version. If you also want to transfer order confirmations and invoices electronically (openTRANS-Format) you have to choose the version you have been using so far for transferring the data. The version is defined when A+W Business is installed.

**Export type** Documents can be dispatched as files or as email attachments:
- **Export to a file**: This setting means that the data will be saved in a file. The field for the target path is released. You can select a directory or enter the path manually.
- **Export via email**: This setting means that the data will be attached to an email. The checkbox for the email address is accessible.

**Export order confirmations, invoices, dispatch notification, credit notes** These document types can be exchanged in openTrans format.
- The corresponding document type will not be exported in openTrans format.
- This document type will be exported in openTrans format.

#### Settings

In this area, you can enter article numbers (e.g., 6530, 6600) that should not be considered during export in a comma-separated list. These article number are then not written to the openTRANS file. You can only make this setting for openTRANS 2.1. Furthermore, this does not apply for order confirmations.

#### Export in file

The field for the target path is accessible only if you have selected Export to file.

**Target path** You can select a directory or enter the path manually.

**File suffix** The following file extensions are available:
- 0 - Default
- 1 - XML file (*.XML).

### Export by email

**Use special email address for the export** This checkbox is accessible only if you have selected Export by email.
- Email transfer uses the addresses entered in master data. You have to check whether the email address has been defined correctly in the customer master data.
- Different email addresses should be used for the email transfer. The fields for the corresponding document type are released.

**For OCs, invoices, disp. notif.** You can enter a separate email address for every document type.

### Tab Table

This tab lists all specified customers.

## SN File Rules

**Master Data > B2B > Customer > SN file rules**

*Abb. B-665 Rules for creating a SN file*

This dialog serves to specify the product types/classes for which an SN file should be automatically created at transfer to production (OrderXML). This file is attached to the BOM. Manual creation per item is therefore unnecessary.

During the transfer to A+W Production, this SN file is usually created by A+W Production.
