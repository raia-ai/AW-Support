---
description: "EN_AWBusiness_Production_2-4"
---


# Production

---
## Settings for Transfer to Production – Transfer Parameters

> **Path:** Production > Production > Transfer to Production > Functions menu > Settings > Transfer parameters tab

This tab defines the parameters that shall be written in the transfer file to be transferred to Production.

### Apply user-related settings
The settings are saved in the database and loaded when you start A+W Business. You can define user-related settings. This checkbox does not appear if you have opened the dialog via Company data > Production tab.

- The settings apply to all users who log into A+W Business.
- ✔ The settings only apply to users who are currently logged in in A+W Business.

### A+W Production
You can transfer the data in OrderXML format to A+W Production. You must not select this setting when using Pool.asc transfer.

- The data is not transferred to A+W Production. Choose this setting to transfer the data to A+W Standard Optimizer or ALFERT.
- ✔ The data is transferred directly to A+W Production. The path by which the transfer files are saved must be entered on the Interface tab for this purpose. (⇨ "Path/File name" on page E-174)

### Define job number
A+W Business can load the job number (transfer number) from the AWPool number area.

- The transfer job number is allocated on the shop floor.
- ✔ The transfer job number is loaded by A+W Business from the AW-Pool number area and saved in the interface file. (⇨ Master Data, "Nummernkreise - Produktion" on page B-905)

### Item splitting licensed
Pool.asc transfer only. If the production of large orders has to be distributed over several days, you can define whether the split is to be applied to the items as well. This setting is only valid for A+W Business capacity planning. This checkbox is only available if the module has been licensed.

- Items should always be scheduled in such a way that they can be produced in one day.
- ✔ Items can be produced on several days.

### Automatic transfer upon receipt of goods
If you have entered items with the code Production in an order which also includes elements to be purchased, these orders can only be produced after the ordered elements have been received, e.g. IG that includes a patterned glass which is not kept in stock. When the ordered elements arrive, information on receipt can be passed on to the shop floor. As a prerequisite, PPS Webservice must be installed and the URL must be entered in Company data > Production tab. (⇨ Master Data, "Firmendaten - Produktion" on page B-997)

- Receipt of P.O. items is not automatically transferred to production. It must be transferred to production manually after receipt has been booked.
- ✔ Receipt of P.O. items is automatically transferred to production. This function also has to be enabled in receipt of goods. (⇨ Purchasing, "Options menu" on page D-226)

### Transfer leaded designs
Pool.asc transfer only. Leaded designs can be transferred to production as Georgian bar records.

- Leaded designs are transferred to production not as processing steps, but as Georgian bar patterns.
- ✔ Leaded designs will be transferred to production as Georgian bar records. This information serves to organize the appropriate work flows. You should only use this setting after checking with A+W Software GmbH.

### Edgework per order
Pool.asc transfer only. Edgework requires the correction of the item sizes. This correction can automatically be made for all orders in order to add the edge protection.

- Edge work is only applied to orders for which it has been entered as a processing step. Size correction will be taken into account.
- ✔ Edge work is applied to all orders by default.

### Transfer article
This setting applies to all products of the product type Article. These are usually kept as stock articles, e.g. handles.

- Articles are not transferred to production by default.
- ✔ Articles are also transferred to production. See also settings in the product master data (A+W Production tab) and the company data (Production tab).

### Transfer (laminated glass) films
Pool.asc transfer only. If you produce laminated glass, you can define that the film is transferred to production too.

- Film is not transferred to production.
- ✔ Film will be transferred to production.

### Transfer cast resin fillings
Pool.asc transfer only. If you produce cast resin fillings, you can define whether these are to be transferred to production.

- Cast resin fillings will not be transferred to production.
- ✔ Cast resin fillings will be transferred to production.

### Transferring A+W Production-specific text
Pool.asc transfer only. This setting applies to the Pool.asc transfer files only. The files in these fields are limited. To be able to transfer certain text which is important for A+W Production, you can define text numbers for the appropriate supplementary information. These can be transferred. The text numbers are defined by the A+W Business- and A+W Production project teams.

- Specific text will not be transferred.
- ✔ Text number for the specific text will be transferred.

| Text number | Text |
| :--- | :--- |
| 3100 plus x | BOM name of spacer |
| 3150 plus x | Short description of the spacer acc. to basic data |
| 3200 plus x | BOM name for UV edge seal, narrow edge seal |
| 3250 plus x | Short description for UV edge seal, narrow edge seal acc. to basic data |
| 3300 plus x | BOM color of spacer |
| 3400 plus x | BOM name of gas |
| 3450 plus x | Short description of gas acc. to basic data |
| x being a continuous counter, i.e. 0, 1, 2, 3 ... | |
| 3600 | Item cutback |
| 3700 | Element weight in grams for record type 8 |
| 4100 | CE code |

### Transfer route sequence
Pool.asc transfer only. The route sequence is loaded from customer master data. It may be important for the loading of lorries.

- The route sequence will not be transferred.
- ✔ The route sequence will be transferred.

### Do not transfer direct shipments
P.O. items can be directly sent from the supplier to the customer. The code is set in the order header on the tab Different addresses.

- All order items are transferred to production. The code for direct shipment will not be taken into account.
- ✔ Purchased items with the direct shipment code will not be transferred to production. The items are directly shipped from supplier to customer.

### OrderXML: Transfer short description instead of matchcode
With OrderXML transfer, the matchcode is transferred by default for products.

- The matchcode is transferred as the product name.
- ✔ The short description is transferred instead of the matchcode. If you have switched from pool transfer to OrderXML, you can choose this setting to go on transferring the short description.

### Supply type from production first
Pool.asc transfer only. The supply types for A+W Business and A+W Production are usually the same. In the case of differences, you can define the parameter that is the first to be analyzed. This setting is important for laminated glass, for example, which is both produced and cut. In the master data, the product is defined as 'cutting', for example. Laminated glass will be produced in connection with a certain order. For this purpose, you can define the supply type that should be analyzed first.

- The supply type from A+W Production is analyzed first. In this case, the above order will always be analyzed as Cutting.
- ✔ The supply type defined in the order will be analyzed first. In this case, the laminated glass will be analyzed as 'production' if the supply type Production is set for the order.

### Transfer the province with the address
Pool.asc transfer only. This setting only applies to countries in which the province is of importance.

- The province is not transferred to production.
- ✔ The province is transferred to production, and is added to the name of the place.

### Exchange quantity fields in the item record
Pool.asc transfer only. If you are using A+W Business capacity planning, you can adopt its quantity fields.

- The quantity fields are not adopted from capacity planning.
- ✔ The quantity fields will be adopted from capacity planning. The fields for the quantity (field 11) and for the item quantity (field 85) are exchanged. Field 11 now shows the subset created by capacity planning while field 85 shows the original quantity.

### Felt pad code in special text 1 in item record
Pool.asc transfer only. The code for felt pads can be transferred to production. This setting only applies to the Pool.asc interface in version 2.3.

- The felt pad code will not be transferred.
- ✔ The felt pad code for the first Georgian bar is transferred as special text 1 (in field 133) of the item record.

### Create order tags
Currently only used for specific customers.

### Laminated glass breakdown (Rel. 2.1)
Additional sets can be created in Pool.asc 2.1 for VSG (as a position or as a component in the BOM). This checkbox is locked if you have selected another format.

- Laminated glass breakdown will not create any additional records.
- ✔ Pseudo items will be created for laminated glass production. You should only use this setting after checking with A+W Software GmbH.

### Laminated glass (2.1) size allowance acc. to BOM
For laminated glass that includes glass elements with processing, the size allowances defined in the bills of material can be transferred by Pool.asc 2.1. This checkbox is locked if you have chosen another format.

- Size allowances for BOM elements are not taken into account.
- ✔ Size allowances for BOM elements are transferred.

### Inch values always in 1/256 inch
Pool.asc transfer only. In the company data in the System tab defines how the size precision is going to be calculated. This setting can be changed. (⇨ Master Data, "Maßsystem" on page B-984)

- Size precision is adopted from company data.
- ✔ Size precision shall be fixed to 1/256 for production purposes.

### Connection type as second digit
Pool.asc transfer only. If the BOM includes an article of the product groups UV edge seal or Narrow edge seal, digit 2 of the edge seal field (field 77 of the item record) can show code 1 (for UV edge seal) or 2 (for Narrow edge seal).

- No code will be transferred for these processing steps.
- ✔ The seal type of the spacer code is exported to digit 2 of the spacer code field (field 80).

### Customer logo based on customer address
Currently only used for specific customers.

### Transfer laminated glass steps on the BOM level
Pool.asc transfer only. Transfer of the step can be set separately for the production of laminated glass in an IG unit.

- The step is transferred on the main product level.
- ✔ The laminated glass step is transferred as a processing for stepped units.

> **IG with laminated glass**
> For the correct transfer of data to A+W Production, this code should be set whenever a stepped laminated sheet is included in an IG unit.

### Transfer BOM element steps
Pool.asc transfer only. Transfer of the steps for all items which do not include laminated glass, can be set in general.

- The step is transferred on the main product level.
- ✔ The step is transferred as a processing step for the corresponding sheets.

### Transfer external packing code
Pool.asc transfer only. A suitable packing type can be defined for every order. If external codes for packing types have been defined in the master data, these can be transferred to production.

- The external code will not be transferred.
- ✔ The external code is transferred to production as a default rack.

### Export articles in BOM
By default, only articles from the main product level are transferred to production. The transfer of the individual BOM articles can be set.

- Articles from the BOM are not transferred.
- ✔ The individual articles in the BOM are transferred.

### Miscellaneous

**Item limit per transfer file**
For Pool.asc transfer, the items of all orders of a number manager are saved in a transfer file. If very many orders and/or items are transferred on a regular basis, you can define the point from which a new (second) file shall be started, e.g. after 50 items.
If you are using OrderXML, a separate file will be created for every order. The entry in this field should be 0 (zero) in that case.

## Settings for Transfer to Production – Additional Interfaces

> **Path:** Production > Production > Transfer to Production > Functions menu > Settings > Special settings tab

Use this tab to define the data for additional interfaces.

### RONA / LIOPT
If you do not use A+W Production, you have to define the export and the path for additional transfer files for these interfaces. The LIOPT interface will not be available as from A+W Business release 2012.

**Export active**
Export of the additional transfer file must be enabled for the additional interface.
- The interface will not be used; no transfer file will be created.
- ✔ An additional transfer file for RONA or LIOPT shall be created in the path defined below.

**Path/File name**
If export is activated, you have to enter the path and file name.

### Backup copies
These settings only apply to the Pool.asc interface.

**Create**
If you are using the Pool.asc interface, you can create a backup copy of the transfer file.
- No backup copy will be created.
- ✔ A backup copy of every Pool.asc file will be saved automatically.

**Path/File name**
To save an automatic backup copy, enter the path and file name.

**Delete file after ... day(s)**
If you save an automatic backup copy, you can define the number of days after which it is to be deleted automatically. If you enter 0 (zero), the backup copies will not be deleted automatically. Files which are no longer required should be removed from this directory manually.

## Settings for Transfer to Production – Text/Attachments

> **Path:** Production > Production > Transfer to Production > Functions menu > Settings > Text/Attachments tab

Use this tab to define the text and file attachments that should be included in the transfer to production.

### Codes for text to be transferred
You can enter text for the entire order and/or for individual order items in the order. A text code allocates each text to a text type. You can check the checkbox of the text type that should be transferred to production. This is usually the code P. You can check several text codes.
- A Auftragstexte/Order text
- G Gutschriftstexte/Credit note text
- K Kommissionstexte/Reference text
- O Angebotstexte/Offer text
- ✔ P Produktionstexte/Production text
- R Rechnungstexte/Invoice text
- T Texte allgemein/General text

### Codes for file attachments to be transferred
You can attach files with additional information for the entire order and/or for individual items, e.g. the sketch of a shape or a Georgian bar pattern.
- No file attachments will be transferred to production.
- ✔ File attachments will be transferred to production. (A All, P Production)

## Shape List

> **Path:** Production > Production > Shape list

This dialog serves to display orders for which a certain shape is to be delivered on a certain date. This gives you, for example, an overview of orders which include free shapes which have to be cut by hand. The result of this search can be printed as a report.

### Selection
- **Article number:** Entry of article number (product no.), not model number.
- **Delivery date:** Entry of delivery date at which the specified model is to be delivered.

### Articles
- **Description, Description 2:** The name of the selected product from the master data.

### Overview
This list shows all orders for which the selected shape should be delivered on the defined date.
- **Order number:** Number of the order which includes the required shape.
- **Item:** Order item number.
- **Customer:** Name of the customer for whom this order is produced.
- **Product number:** Number of the product.
- **Name 1, 2, 3:** Product descriptions.
- **Route:** Route by which the order shall be shipped.

## Rack Load

> **Path:** Production > Production > Rack load

This dialog serves to check the rack load for orders to be produced. The orders have to be allocated to racks already.

### Functions menu
Use this menu to open other dialogs without closing the current one. The following entries are displayed:
- **Create ASCII file:** The data is saved in an ASCII file.
- **Settings:** Opens dialog Settings dialog where you can define the settings for the ASCII file. (⇨ "Settings (check Rack Load)" on page E-189)

### Selection
- **Employee:** Name of the employee logged in to A+W Business.
- **Number Manager:** Choose the number manager the dialog should access.

### Sorting criteria
This option defines the sequence in which the orders should be listed:
- **By order + item no.:** The view is sorted by order number first, then by item number.
- **By P.O. text + customer item:** The view is sorted first by P.O. text 1, then by customer item.
- **All:** All orders of the selected number manager will be displayed.
- **Except TPS:** Orders that include TPS are excluded from the view.
- **Only TPS:** Only orders including TPS will be listed.

### Overview
The list shows the orders included in the selected number manager.
- **Number:** Serial number on the list.
- **Cust./Suppl. number, customer/supplier:** Customer or supplier name and number.
- **Status:** Order or item status.
- **P.O. text 1:** P.O. text 1 acc. to the order.
- **Rack/compartment no.:** Rack or slot number on the rack.
- **Sorting:** Sorting code.
- **Packing type:** Packing type, e.g. rack, box.
- **Prod. date IG, LG, TG:** Date on which the IG, laminated, or toughened glass is produced.
- **Job no. prod. IG, LG, TG:** Number of the job by which the IG, laminated, or toughened glass is produced.
- **Delivery date:** Delivery date defined in the order.
- **Delivery note:** Delivery note number.
- **Route:** Name of the delivery route.
- **Total weight:** Total weight of all order items.
- **Total quantity:** Total quantity of all order items.
- **Total sqm:** Total surface of all order items.
- **Total lin.m.:** Linear meters of all edges.
- **Input date:** Date on which the order was entered.

## Settings (check Rack Load)

> **Path:** Production > Production > Rack load > Functions menu > Settings

You can define additional settings for L racks. These settings are mainly important for TPS.
This dialog offers the following tabs:
- "Settings - Common” on page E-190
- "Settings - Customers" on page E-191

### Settings – Common

> **Path:** Production > Production > Rack load > Functions menu > Settings

This dialog serves to define the criteria for the transfer file. The rack load can be saved in an ASCII file.

- **ASCII file path:** Entry of path for ASCII file. A temporary directory will be saved on C:\ by default. The file name consists of customer number, day, and month.
- **Packaging type:** You can set the packaging type for orders the data of which shall be exported. The program will only offer the packaging types defined in the master data.
- **Printing:** This option defines how the data should be printed.
- **TPS L racks, L racks:** Enter the maximum number of slots for the racks. The maximum number for TPS is 22 and for the other L racks, 21. You can also enter the maximum sizes for the corresponding slots. The data will be checked before the ASCII file is created.

### Settings – Customers

> **Path:** Production > Production > Rack load > Functions menu > Settings > Customers

For individual customers, you can define the number from which the counting of the required racks should start.

- **Customized settings**
- **Customer:** Number and name of the customer for whom the settings are made.
- **Surcharge articles:** Article number of the surcharge to be calculated.
- **Rack Type Number:** Starting number of the rack.
- **[New], [Delete]:** Activates a new line in overview, deletes the selected entry.

## Barcode Transfer

> **Path:** Production > Production > Transfer Barcode Prod.

Barcodes can be used for transferring individual order items to Production. This is done in the dialog Transfer to production (item orient.).

This chapter provides information on the following subjects:
- "Functions menu" on page E-192
- "Transfer Barcodeto Production" on page E-193

### Functions menu
> **Path:** Production > Production > Transfer Barcode Production

You can use this menu to open other dialogs without closing the transfer to Production.

**Production group**
- **Settings:** Opens the dialog of that name, in which you can define the settings for the transfer file. (⇨ "Settings for Transfer to Production" on page E-172)
- **Order overview:** Opens the Status report overview dialog in which you can display the status reported from Production for every order and item. (⇨ Sales, "Status Message Overview" on page C-574)
- **Delete runs:** Deletes the specified runs.

**Capacity planning group**
- **Processing:** Opens the Work types dialog in which you can display the use of capacity per work type. The corresponding data are only available if you are using A+W Business capacity planning. (⇨Capacity Planning, "Work Types" on page H-196)

## Transfer Barcodeto Production

> **Path:** Production > Production > Transfer Barcode Prod.

If you are using scanners, you can transfer the individual order items to Production via barcode.

This dialog offers the following tabs:
- "Transfer Barcode to Production - Overview" on page E-193
- "Transfer Barcode to Production – Details" on page E-194

### Transfer Barcode to Production – Overview

> **Path:** Production > Production > Transfer Barcode Production > Overview tab

You can use this tab to create jobs by work types. The job number is selected from the number area for AWPool. Clients and production preparations can be taken into account.

**Identification**
- **Client:** If there are different clients, these will be offered for selection.
- **Area:** If different production preparations have been defined, these will be offered for selection.
- **Comment:** You can enter comments for the users, e.g. to make them aware of peculiarities.

**Jobs**
The list shows all jobs which are to be, or have been transferred to Production. Jobs which have not been transferred yet come first, followed by those that have already been transferred. The number of jobs to be displayed can be restricted in the menu Functions > Number of jobs.
- **Number:** Job number
- **Status:** Current job status
- **Comment:** Text that was entered in the field Comment.

### Transfer Barcode to Production – Details

> **Path:** Production > Production > Transfer Barcode Production > Details tab

This tab can be used to add items by barcode or manually. The current job number from the Overview tab is displayed. Orders and items can be entered for this job only.

**Input**
- **Barcode:** Display of scanned barcode. If you enter the item manually, you can enter the work process, the order number and/or the group or item number, depending on the selected type. You can enter a maximum of 11 characters in the left field and a maximum of 3 in the right field.
- **Type:** This option defines the numbers you will be scanning or entering:
  - **Work process:** Choose this option to scan the work process.
  - **Ord.no.+Group.no.:** Use this option to scan the order number in the left field, and the group number in the right field.
  - **Ord.no.+Item no.:** Use this option to scan the order number in the left field, and the item number in the right field.
- Order or item data will not be processed further if they already exist in other jobs.

**Settings**
- **Number of jobs:** The maximum number of runs displayed. A new job can be entered even if this maximum number has been reached. If this is the case, the oldest (smallest) job number is deleted.
- **Registration point:** Specification of registration point.

**Codes**
You can enter a one-digit check code for the barcodes of work processes, group and order numbers, and/or order and item numbers in this section. The check digit can be a number or a letter. The check digits do not have to be sequential, e.g. the following entries are possible: 1, 2, 3 or 7, 4, 6 or G, 3, Z.
- **Work process:** Check digit for the barcode of the work process to be scanned.
- **Order/group number:** Check digit for the barcode of the group or of the order to be scanned.
- **Order/item number:** Check digit for the barcode of the orders or items to be scanned.

**Work process**
> **Select work processes**
> You can select the work processes defined for production in the master data. These work processes can be scanned.

- If you have chosen the option **Work process**, you can select the desired work process from the combo box.
- **Contained processings:** This field shows all processing steps that are part of the selected work process.
- **[Delete all]:** Deletes all entries from the run. To remove just a single entry from the job, check it and go to the menu Start > Delete.

**Batch**
This list shows all order items that were added to the current job.
- **Order no.:** Order number
- **Item no.:** Number of the order item
- **Description:** Product name
- **Qty:** Item or group quantity
- **SQM:** Total surface area of the item or group
- **Weight:** Total weight of the item or group
- **Work process:** Work process in which the item is produced.
- **Total:** Total amounts of all listed items

## Production Data

> **Path:** Production > Production > Production data

Orders of the type Production order are used to produce products for your own stock. The raw material used and all production-relevant data are entered in production orders.
An additional option is to enter the production data and use the ensuing booking to withdraw the necessary raw material from stock, and add the items of the production order to stock.

### Production Data (Dialog)

> **Path:** Production > Production > Production data

This dialog can be used to enter and book all data that are necessary for production.
This dialog offers the following tabs:
- "Production Data – Order" on page E-198
- "Production Data – Table" on page E-200
- "Production Data – Booking" on page E-201

### Production Data – Order

> **Path:** Production > Production > Production data > Order tab

This dialog can be used to enter and book all data that are necessary for production. Please note that all fields must be filled in except the reason for downtimes.

**General**
- **Date:** Production date. If you enter the data for booking the addition to stock, this is the date on which the production order shall be or has been produced.
- **Machine:** Select the machine which is used to produce the production order.
- **Layer, shift:** Shifts are not taken into account for production orders. This field can be left blank.
- **Person in charge:** Name of the employee in charge

**Production details**
- **Set-up time/run time (minutes):** Enter the setup time and the production time in minutes.
- **No. of persons:** Number of persons required to produce the work order.
- **Downtime (minutes):** Enter the downtime in minutes.
- **Reason of failure:** If you have entered a downtime, you can also define the reason for this. Once defined, the reasons for failure will be kept in the combo box and can be selected again if required.

**Production order data**
- **Order:** Production order number
- **Item/quantity:** Number and quantity of the order item

**Finished product**
- **Articles:** Product number of the produced units acc. to the product master data. This number is used to book the finished product to stock.
- **Width/height:** When you enter the number, descriptions, sizes, and weight defined in the master data will be displayed automatically.
- **No. of units:** Number of units produced for the current item.
- **Automatically create ID no.:** Box IDs can be allocated automatically at booking.
  - Boxes will not be booked.
  - ✔ The production order includes boxes that should be automatically assigned IDs at booking. This allows you to enter different contents. If the product is a box with a complex BOM, but in which the glass is not the first BOM element, the contents cannot be changed.
- **Lites per unit:** IG unites can consist of 2, 3, or even 4 lites. Most units consist of two lites.
- **Lites completed:** Number of cut lites.

**Raw material**
- **Articles:** Product number of the glass (or of the stock plate) to be cut.
- **Width/height:** Sizes of the raw material.
- **Breakage:** This is where you can enter the breakage of raw material.
- **Machine breakage:** This field is filled by the report from A+W Production.
- **Supplier:** Supplier of raw material.
- **Stock sizes in job:** Number of stockplates cut for this job.
- **Stock sheets per stock size:** Enter the number of stock sheets cut from the stockplate.
- **Waste:** Waste (in sqm), i.e. the remainder resulting from the cutting of the stock sheets of a stockplate.

> **Example**
>
> | | |
> |:---|:---|
> |Stockplate 3210 x 5000 mm| = 16.05 sqm|
> |Cut: 2 pcs. of float 4: 2000 x 3210 mm = 6.42 sqm/pc.| = 12.84 sqm|
> |Waste| = 3.21 sqm|

### Production Data – Table

> **Path:** Production > Production > Production data > Table tab

This tab shows the items of a production order for which you have entered production data.
