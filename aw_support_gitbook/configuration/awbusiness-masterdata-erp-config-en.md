---
title: "EN_AWBusiness_Master_Data_9_10-4"
source: "EN_AWBusiness_Master_Data_9_10-4.pdf"
tags: ["A+W Business", "Master Data", "Software Reference", "ERP", "Production Management", "Capacity Planning", "Database Configuration", "Print Settings", "A+W Software"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A detailed software reference guide for the A+W Business Master Data module. It covers company-level configurations for printing, database transactions, cost calculations, production settings, capacity planning, and shipment management."
long_description: "This document serves as a comprehensive software reference manual for configuring the Company Master Data within the A+W Business software suite. It provides step-by-step instructions and explanations for various settings across different functional areas. The guide begins with configurations for construction printing (AWD20.INI) and database transactions for SQL Server. It then delves into the 'Calculation' tab, detailing how to set up surcharges for cost calculation, material overheads, and capacity areas. The 'Print' tab section explains settings for monthly invoices, print sketches, BOM (Bill of Materials) handling, print server connections, and integration with DMS (Document Management Systems). The 'Production' tab is extensively covered, with settings for transferring orders and quotes to production, profit center invoicing, automatic SN file creation, and integration with A+W Production via webservices. It also details configurations for the Production Manager, capacity planning feedback, and complaint order creation. The 'Shipment' tab focuses on rack management, number ranges, and route optimization with A+W Logistics Optimizer. The 'Capacity Planning' section explains how to configure automatic scheduling, error reporting, production scheduling modes, and feedback settings from A+W Production Capacity Planner. Finally, the 'Miscellaneous' tab covers settings for importing product data from suppliers using BMECat and linking contacts with MS Outlook. The document is structured with screenshots and detailed field descriptions, making it an essential resource for system administrators and power users."
---

---
## Company

### AWD20.INI for construction printing
The true-to-scale grill sketch can be printed according to the configuration for CAD Designer Bars.
- The grill sketch is printed according to the A+W Business standard.
- The configuration for CAD Designer Bars is used if in the order a true-to-size sketch for grills with the setting Output grill cutting list is printed.
- -> Sales, "Print Dimensioned Sketch" on page C-647

### Database

**Transactions**
The database support for SQL server also allows transactions. Thus, SQL commands that follow one another and change the data can be undone as long as the transaction has not been completed.
- Database transactions are only possible for the SQL Base database system.
- Database transactions are possible for SQL Server. This setting is important for the Microsoft SQL Server database system.
- For the SQL Base database system, the transaction logic is always active.

## Company Data > Calculation
**Master Data > Company > Company Data > Calculation tab**

This tab is used to enter the surcharges for cost calculation.
-> Tutorial 2, "Cost and Surcharge Calculation" on page B-539

### Cost and surcharge calculation
The costs calculated at document entry can be displayed at order and item entry.

### Material overheads

**Procurement type**
Supply types are preset by A+W Business.

**% surcharge**
Proportional surcharge to be used for the corresponding procurement type.

**Ancillary labour costs**
Proportional surcharge on ancillary labour costs.

**Sales overheads**
Proportional surcharge for the overhead cost of sales.

**Administrative overheads**
Proportional surcharge for the administrative overheads.

**Profit margin**
Proportional surcharge for the expected profit.

### Capacity areas

**Weekday, IG, LG, TG**
This table only refers to module Customer-based capacity information system. You can define total capacities for the three main product types (IG, toughened, laminated glass). Shares of those can be reserved for key customers. These shares are defined in customer master data.
-> "Partner Management - Production" on page B-784

Customers for whom no capacities have been defined, will be collected in a group to which the remaining capacity is allocated. At order entry, the function Capacity info by customer shows the remaining production capacity.
-> Sales, "Document - header data" on page C-415

### Default MI

**Minimum MI**
Percentage of marginal income that must be reached when an order is changed.

**Maximum MI**
Percentage of marginal income that must not be exceeded when an order is changed.

## Company Data - Print
**Master Data > Company > Company data > Printing tab**

This tab serves to define the settings for printing documents.

### Monthly invoices
The fields in this section refer to the module Monthly invoices. The checkbox Monthly invoice has to be checked in customer master data.
-> "Partner Management - Finances" on page B-773

All customer orders with the code Monthly invoice are automatically allocated the status point 73-Monthly invoice.
The corresponding user status in your A+W Business version depends on your own status organization. Based on this status, you can select the orders for each customer and invoice them together.
-> Tutorial 2, "Status Administration" on page B-418
-> Sales, "Monthly invoice" on page C-33

**Print point**
Print point for the printing of forms. Standard setting: 103-Invoices.

**Mail, Fax, Email**
For the print of monthly invoices you can define at which print point the invoice will be printed.
- The print point is not used.
- The print point is relevant for the print of monthly invoices. With the print, the status of the document is set. For this, the status point 73-Monthly invoice must be set.

**Status point**
Standard setting: 73-Monthly invoice. Orders for customers with monthly invoicing that are invoiced by mistake will be automatically set to status 73-Monthly invoice.

### Print sketches

**Extended grill sketch on printed forms**
Sketches can be printed schematically or true to scale. The setting can be changed in the order.
- By default, grills will be printed schematically.
- Grill sketches can be printed in detail. This requires that the sketch size is increased in management of forms for the detailed display. The function for true-to-scale printing must also be set in the order.
- -> Tutorial 2, "Printing sketches" on page B-479
- -> "Shape sketch, grill sketch" on page B-1059

### BOM

**Maximum quantity**
Number of BOM entries to be transferred to printing of forms. You should make sure that your BOMs can be actually processed.
- If an order has got a more extensive BOM, all entries exceeding the maximum number will not be printed.
- An input of 15-20 has proved sensible. A higher number will impede the processing speed considerably.

### Print server
This field refers to the module Print server.
-> "Print Jobs" on page B-1062

**Server name**
Enter the name of the server on which the print server has been installed.

### Printer list

**Check available printers via Windows API**
If you are using several printers, these can be offered for selection when forms are printed. Printing via print server requires the creation of print jobs.
- The forms will be sent to the standard printer.
- You can choose one of the available printers. This setting allows to decide whether a form is printed as a PDF file, as a fax, or as a hardcopy (on paper).

### Reprint for document archiving

**Printer**
Choose the standard printer. If an automatic reprint should e.g. be started for the DMS system ELO (electronic Leitz file), you have to select the ELO printer.

### DMS

**DMS archives path**
Path for saving the document files. All documents that can be archived in A+W Business will thus be archived in the document management system Saperion (DMS) at the same time.

### Primary form/report search
Clients may be using different forms for printing and for reports. Enter a path for the primary search for forms/reports. Printing of forms and printing of reports will search for the report and the form in this directory. If the forms cannot be found there, the program will fall back on the standard installation directory.

**Path**
Path in which the forms for the current client can be found. This path may also include amended standard reports. This field can be left blank if all clients are using the same forms or if just one client has been entered.

### Crystal Reports ODBC

**DSN**
Name of the domain server on which the application is installed.

**User, Password**
Login data for accessing Crystal Reports.

### Form printing

**Form printing via Crystal Reports**
As an alternative to the internal report forms, the reports can also be printed via Crystal Reports.
- Crystal Reports is not used.
- The forms are output via Crystal Reports.

**Path**
Path in which the forms can be found.

**Email**
Printer with which the reports will be output.

### Document management

**Enable archiving system**
If you are using a document management system (DMS), e.g. in Saperion, documents can be archived. An appropriate interface has to be installed.
- Documents will not be transferred to a document management system.
- The documents are transferred automatically to the connected DMS. For this, you have to activate the document archiving in the form management for each form.
- With this setting, e.g. when printing the invoice, the invoice is first sent automatically and then transferred to the document archive.
- -> "Archiving of documents" on page B-1054

**(Path)**
Specification of the archiving path.

## Company Data – Production
**Master Data > Company > Company Data > Production tab**

This tab serves to enter the settings for the transfer to production.

### Transfer to production

**[Settings for orders]**
Opens the dialog Settings – Transfer to production where various transfer parameters for orders can be set.
-> Production, "Settings for Transfer to Production" on page E-172

**[Settings for quotes]**
Opens the dialog Settings – Transfer to production where various transfer parameters for quotations can be set.
-> Production, "Settings for Transfer to Production" on page E-172
-> Production, "Optimization of Quotations" on page E-289

**Profit center invoicing active**
Profit center invoicing allows to invoice internal services between different clients or order areas.
- Profit center invoicing will not be used.
- When an order of the first client is transferred to production, a P.O. will be automatically issued for the corresponding client.

In product management, the corresponding procurement types have to be entered for every product, per client/OP area.
After that, the work performed by the corresponding client/order area will be invoiced.
-> "Product Codes" on page B-608

**Creation of follow-up orders enabled**
If your production areas (IG, laminated and toughened glass) are distributed to different clients or order areas, this module allows the automatic creation of follow-up orders for internal orders for the corresponding production area.
- No follow-up order will be issued for internal orders.
- At transfer to purchasing, all internal orders and follow-up orders for the corresponding client or order area will be created automatically.
-> "Product Management - Stock/Purchase" on page B-606

**Automatic creation of SN files (also at EDI import)**
SN files can be created automatically at transfer to production.
- SN files (Shaping+Nesting) will not be created automatically.
- At transfer to production or at EDI import, the system automatically creates a SN file for rectangles and standard shapes including the following processing steps for every item that includes e.g. single annealed or toughened glass: edgework, cut-off corners, rounded corners, notches, and drill holes. This procedure allows to print true-to-scale sketches on your production papers.
When a SN file is created, the user status SN file checked will be assigned so that the following transfer to production can use this user status as a minimum status.

**Shape 0 to be inserted automatically**
You can select the shape that should be inserted automatically for the creation of SN files for rectangular lites. If no item is selected here, the shape to be attached is determined as previously. The field is only enabled if the automatic generation of SN files is activated.

**Use Production Manager**
With this setting, you switch on the program variant A+W Business Pro.
If you are working with the Production Manager module, partial deliveries can be booked with fileless reporting.
- The production manager is not used.
- The production manager is activated. With this setting, stock residual lites are considered for batch optimizations in the production manager. The program does not establish a connection to A+W Production. Instead, production planning is available in the Production module.

**File path**
Path for saving the files.

### A+W Production connection

**PPS Webservice URL**
Address for the PPS Webservice. PPS Webservice is required for the following transfers:
- Production release after capacity transfer
- Goods received report to A+W Production
- Cancellation

**[Globe]**
Checks whether a connection can be established by means of the defined URL.

**Cancellation of production transfer via PPS WebService**
File-less transfer to production offers two ways of cancelling orders.
- Orders to be cancelled are transferred to production by hand, with a cancellation code.
- Orders to be cancelled are transferred to production via PPS Webservice. The quantities for the corresponding order items are manually set to 0 in the order.

**Cancellation of the production transfer only up to status ready for dispatch**
The cancellation and thus the decreasing of the status can be suppressed if the order has already been produced.
- Orders to be cancelled are transferred to production by hand, with a cancellation code.
- Orders can only be cancelled up to the status ready for dispatch. For this, the registration point for the status Order produced at must be defined.
- -> "Reg. point allocation" on page B-961
- At the registration points, a status assignment must be present for this registration point and the assigned status defined whether the order is produced if it is greater than or equal to.

**Message about P.O.**
Receipt of ordered goods can be directly reported to production so that the corresponding orders can be produced with the purchased articles.
- **None:** With this setting, receipt of goods will not be reported to the shop floor.
- **By AWPool transfer:** You should choose this setting if production data are saved in a file (AW-Pool or OrderXML).
- **By PPS Webservice:** You should choose this setting for file-less transfer of production data.

### ERP Webservice

**URL**
Address for the ERP Webservice. PPS Webservice is required for the following transfers:
- OrderXML production transfer
- Scheduling reports from A+W Capacity Planner
- File-less production reports
- AWPort connection

### Master data transfer and language A+W Production
Master data only have to be maintained in A+W Business and can be transferred to A+W Production.

**Server name**
Glass, processing, grills, fillings, articles, spacers, glass type groups, glass types, tables, jumbos, and jumbo/table allocations can be synchronized between A+W Business and A+W Production.
Enter the name of the A+W Production server (DNS name or IP address).
In product management, you also have to define which data will be transferred.
-> "Product Management - A+W Production" on page B-619

> **Complete the master data input**
> Enter the server name only after you have entered the corresponding master data. If this field is left blank you can e.g. enter products without transferring data.

**Diff. Diff. production language**
OrderXML can transfer product names and text from A+W Business in a language that differs from the language used in A+W Production, e.g. because different languages are used for order entry and for production. The field for selecting the target language is accessible only if this checkbox is checked.
- The language is the same in both programs.
- Product names and text from A+W Business will be transferred in a different language and should be translated into the target language. Text changed by hand at order entry will not be translated.

### Online production overview in
With the online production overview, it is possible to generate a report from the PPS Webservice. This production overview can be displayed for several orders at once if it is called from a Number Manager. For this, in the Report parameters field of the Crystal Report, specify the report that should be used for the production overview.
The online production overview draws the data directly from the PPS Webservice.

**Report parameter**
Specification of the report parameter in the following form:
Report=//awbawp60/Trans/Reports/BDE/
AUW_OrderList_Status.rpt&Unterteile_anzeigen=1&Auftrag=[OrderList]
For this, specify the rpt file to be used under report and link the report parameter with &. The text [OrderList] is replaced with the corresponding order numbers before transfer to the PPS Webservice.

### Production report

**[Settings]**
Opens the dialog Production reports (interface service) where various parameters for reports per file can be set.
-> "Interface service" on page B-1027

**Fileless production feedback**
The feedback is stored by A+W Production via the ERP Webservice and booked by A+W Commercial Exchange Service.
- Feedback from production is not imported online.
- Reports from production will be imported online. For this, no files are saved. On the tab Stock/PU/EDI, the control elements for management of the individual STS files are deactivated.
- -> Production, "Reports from Production" on page E-56

**Book feedback in partial deliveries**
The fileless feedback can also book production feedback in partial deliveries with partial invoices.
- Fileless feedback is not booked in partial deliveries.
- Fileless feedback is booked in partial deliveries. For feedback for an order, initially all partial deliveries are sought. The quantities reported are distributed accordingly across the documents found. Here, feedback is booked first to the documents whose delivery date is earliest. This means that the documents should have different delivery dates.

If the feedback of a registration point for a document is complete, it is booked to the following document. Breakage messages always apply only for the original order, excess quantities for the document with the latest delivery date.
Feedback already made is divided up according to the quantities selected when creating a partial delivery. Thus it is not relevant for the booking at what time of production a partial delivery is created.

**Production release for order if sub-order has been produced (STSP)**
This field is accessible only if production reports are imported.
Partial orders can be created for an order. If a production report refers to such a sub-order, the status of the whole order can be changed.
- An order is not automatically set to the Production release status.
- When the sub-orders are reported as produced, the status of the main order is automatically raised to Production release.

**Adopt batch no. from order header (STSP)**
This field is accessible only if production reports are imported.
If the defined registration point has no status allocated, the report is processed by A+W Business capacity planning, and the status is changed accordingly.
- The batch numbers of the items are updated separately from the batch number in the order header.
- After the order header has been updated, all items with an item status over/equal with the status of the registration point produced will get the order number's batch number.
- -> "Reg. point allocation" on page B-961

**Adopt production rack number for item (STSD)**
This field is accessible only in connection with the import of barcode reports.
If the barcode report includes rack numbers of items, these can be allocated to the items in A+W Business.
- Rack numbers will not be adopted for the item.
- The reported rack numbers will be saved in the order and allocated to the corresponding item.

**Update production list through registration point (STSG)**
The STSG report defines the rack that is allocated to the corresponding order item and the quantities produced. The rack number is printed on the delivery note.
In this field, choose the registration point used by the rack reports to raise the status. Based on the selected registration point, the production list in dialog List of status reports will be updated.
For this, the production status must be selected or defined via the folder symbol.
-> Sales, "Status Message Overview" on page C-574

**Quantity > Allow item quantity (STSB, STSD, STSG, STSL, STSP)**
This field is accessible only if production reports are imported. If the produced quantity is greater than the quantity of the order item, the produced quantity can be taken over.
- Produced surpluses are not taken over into the order.
- Produced quantities are taken over into the order item.

**Capacity planning feedback (STSD/STSB)**
STSD and STSB reports can be processed by capacity planning (time management).
- Capacity planning processes no data from STSD and STSB files.
- Capacity planning will process STSD and STSB files. So that the reporting of A+W Production can be processed correctly, on the Stock/PU/EDI tab, the registration point 700 must be selected.
- -> "Reg. point allocation" on page B-961

**Create complaint orders (STSB)**
This field is accessible only in connection with the import of breakage reports.
- Complaint orders will not be created automatically.
- A complaint order will be automatically created based on a breakage report. This function can be allocated a standard cause and a standard reason that can be changed for the individual complaint order.

**Cause**
This field is accessible only in connection with the automatic creation of complaint orders.
You can select a cause that is adopted for the automatically created complaint order. It will be loaded irrespective of the settings in Company Data > Archives tab.
-> "Default complaint place" on page B-966

**Reason**
This field is accessible only in connection with the automatic creation of complaint orders.
You can select a reason that is adopted for the automatically created complaint order.

**Order area**
This field is released only in connection with the automatic creation of complaint orders. You can select an order area: the order number will be taken from its number range.

**Target NM**
This field is released only in connection with the automatic creation of complaint orders. You can select a number manager to which the automatically created complaint order should be transferred.

**Free**
This checkbox is available only in connection with the automatic creation of complaint orders.
- Automatically created complaint orders are not free of charge as a standard.
- Automatically created complaint orders are free of charge by default. The setting can be changed in the complaint order.

## Company Data – Shipment
**Master Data > Company > Company data > Shipment tab**

This tab is used to define the settings for rack management and dispatch.

### Number areas

**Rack No. from, to**
First and last number of the number range for racks. The number range applies to the current client.
To lock racks for a client, enter 0 in both fields and 1 in field Current.

**Current**
Field actual shows the last number assigned by the system.

**Ident. no from, current, to**
These numbers define the IDs that can be assigned to racks, and the last assigned rack number.

### Rack load

**for packaging type**
Packaging type for which L rack numbers can be assigned. This field refers to module L racks.

### Rack Management
Choose an option to define the type of rack management you are using:
- **A+W Business:** This option enables the common rack management of A+W Business.
- **AWRack:** This option enables the Rack Manager rack management and gives access to the following fields.

**No back writing of remarks for pick up**
Pick-up information can be transmitted in STSK feedback.
- The pick-up information is written to the remark field for the rack. Thus, manual entries in this field are overwritten.
- Pick-up information is not written back.

**AWRack Webservice**
Complete Internet address for the Webservice Rack Manager.

**CommonBase client**
0 is entered here by default; this has to be changed only if you are using Rack Manager. The specified values are the IDs for the CommonBase interface.

**CommonBase company group**
0 is entered here by default; this has to be changed only if you are using Rack Manager.

**Default order area for invoices**
Select the order area for which rack invoices are issued on a regular basis. You can change this setting when issuing invoices in Rack Manager.

**Current client is the default client for invoices**
You can specify whether the client for which you are currently setting the company data should be stored in Rack Manager as default.
- The current client is not the default client.
- The current client is stored in Rack Manager as default. You can overwrite this setting when creating invoices in Rack Manager.

### Freight costs
If you are using imputed freight costs, you can enter a limit beyond which freight costs become unviable.

**Critical freight cost limit %**
Critical freight cost limit Critical freight cost limit in per cent. If the specified value is exceeded, the figures in dialog Imputed freight costs are shown in red.
-> Production, "Freight Costs" on page E-137

**Surcharges/freight revenues**
You can specify which surcharges form the freight revenues. This way, you also specify how freight revenues arise for the orders that are sent to the A+W Logistics Optimizer.

### Route optimization

**A+W Logistic Optimizer**
In order to work with the A+W route optimizing, you must activate this module.
- The A+W Logistic Optimizer is not used.
- The A+W Logistic Optimizer is enabled.

## Company Data - Capacity Planning
**Master Data > Company > Company data > Capacity Planning tab**

This tab serves to enter the details for capacity planning.

> **Automatic scheduling**
> To use capacity planning you have to switch off automatic scheduling. Go to tab Parameters and uncheck the checkbox Automatic scheduling.
> -> "Automatic scheduling" on page B-939

### Capacity planning

**Version**
For the selection of the program for capacity planning, you must pay attention to how you receive reports from production. You can choose from the following settings:
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

**Error report from automatic capacity planning**
With the selection of this option, you specify to whom error reports are sent.
- **To operator:** This setting means that error reports will be sent to the user who has entered the order in question. These error reports usually refer to dates that cannot be kept because of capacity bottlenecks. This is the default setting.
- **To employee:** This setting releases the field so that an employee can be selected. Select this option if only a single employee processes the orders that cannot be scheduled without problems.

### A+W Business Capacity Planner

**Number of shifts**
Number of shifts per day. You specify the shift times in the Capacity planning module on the Calendar dialog.
-> Capacity Planning, "Calendar" on page H-215

**Production scheduling mode**
You have to define whether you are going to use open or closed capacities.
- **Automatically normal capacity:** Orders are scheduled according to the shift times available. Overbooking is not possible. This is the default setting.
- **Automatic full days:** With this setting, the specifications on the calendar for the number of shifts and hours are ignored. Scheduling is based on a workday of 24 hours. However, this only applies for regular workdays, not for holidays.
- **Change machine only:** With utilized capacities, there should be an automatic search only for another machine. If it is also at capacity, the scheduling is interrupted and you must intervene manually.
- **Schedule without check:** This setting corresponds to the open shift. This means, for example, that despite the shift time of 8 hours, 16 hours can also be scheduled. Here no message is output if a day is fully utilized.

**Fill shift in case of item splitting**
Large items can be divided across several machines, shifts or days. Enter the percentage up to which the machine's shift(s) can be filled by split items in order to leave room for other orders.

**Machine alignment**
If you are using several machines that can perform the same work types, scheduling can consider these machines in different ways:
- **Automatic:** The program automatically searches for the most cost- and time-effective machine and schedules the orders on this machine. This is the default setting.
- **Semi-automatic:** The program offers the alternative machines for selection.
- **Manual:** Alternative machines can only be selected for manual scheduling or re-scheduling.

**Scheduling priority**
Priorities defined in the order can be taken into account for scheduling:
- **Standard:** The capacities of the required machines are checked and the orders are scheduled according to the priority entered.
- **Low priority:** By default, all orders are scheduled with low priority.
- **Apply changed priority in order:** If the priority is changed during scheduling, it should be written back to the order automatically.

**Max. shift for autom. delivery date calculation (days)**
You can specify how many days in the future the delivery date may be shifted automatically.

**Scheduling of P.O. items (only main products)**
With A+W Business Capacity Planning, PO articles can be scheduled.
- P.O. items are not scheduled.
- The P.O. items are scheduled. can report time costs.

**Scheduling of stock items (only main products)**
With the A+W Business Capacity Planning, you can schedule stock items. Thus the time costs can be determined for such items.
- Stock items are not scheduled.
- Stock items are scheduled. The time costs can be determined.

**Scheduling of manually entered service items (only main products)**
With A+W Business Capacity Planning, manually entered service items from the main item can be scheduled. The time costs for the items can be determined.
- Service items entered manually are not scheduled.
- Manually-entered service items are scheduled. The time costs can be determined.

**Fill history table for completion reports**
In the program variant A+W Business Pro, completion reports can be written to the history.
- Completion reports are not written into the history.
- The completion reports are written into the history. In addition, the work processes reported complete implicitly with a booking are logged, as well as STSD reports if there is no booking in the capacity planning. STSD reports are logged if no booking is made in the capacity planning.
The history can be evaluated in the Statistics module and printed out.

**Autom. delivery date search by route**
In case of bottlenecks, it is possible to search for a new delivery date automatically.
- The next possible date is chosen as delivery date no matter if this is a route day or not. This is the default setting.
- The program searches for a new delivery date based on the customer's route days. Automatic scheduling selects the new delivery date and saves it in the order.

**Do not split order**
Large orders have to be split into smaller portions if processing of the whole item cannot be completed in one day.
- The orders can be split for automatic scheduling. This is the default setting.
- The orders can only be split manually. Automatic scheduling of large orders triggers a message to that effect so that you can intervene.

**Reduced scheduling check if structure identical**
An order may contain items with the same BOM structure, which differ only according to the dimensions.
- The entire BOM structure is checked for each item.
- If the BOM structure is the same, scheduling is based on the previous item without checking the BOM again. This is the default setting.

**Schedule for delivery date**
Automatic scheduling generally schedules the orders for the delivery date. The searches for a new delivery date only if there is no free capacity.
- Orders are scheduled with delivery date search. This is the default setting.
- Orders are scheduled without searching for an alternative delivery date no matter whether or not there are free capacities.

**Automatic completion report for invoiced orders**
Orders can be automatically reported completed.
- Orders will not be automatically reported completed.
- Orders will be automatically reported completed if the invoices have already been issued. This setting makes only sense if transfer to production is triggered after the invoice has been issued.

**Transfer to production (OrderXML) incl. planning data**
At transfer to production, data can be transferred by OrderXML or Pool.asc.
- The data should not be saved in the OrderXML file.
- A+W Business capacity planning data should also be saved in the OrderXML file.

**Use change of shifts table**
A 'change of shifts' table can be used for the automatic changing of shifts.

**[Settings]**
Opens the dialog in order to define the shift change.
-> Capacity Planning, "Shift Settings" on page H-191

**Product classes without status change**
The raising of the item status (order status) can be prevented by completion reports for product classes. Just select the appropriate entries on the list.

**Order areas without scheduling**
You can define that certain order areas are excluded from automatic scheduling. This means that orders for the selected order areas can be scheduled manually only.

### Feedback settings regarding A+W Production Capacity Planner

**Update time costs**
A+W Capacity Planner can report time costs.
- Time costs will not be updated.
- Time costs will be updated.

**Check stock availability**
Capacity planning checks if enough of the materials required are available on stock.
- Availability of stock articles will not be checked.
- Availability of stock articles will be checked. If there is a shortage on stock, a task will be entered for the user.
Stock information will highlight any articles of which there is not enough stock and which might therefore endanger the scheduled delivery date.

**Barcode reports**
Fileless reporting of completion messages can be imported from A+W Business Pro and imported into the A+W Barcodescanner.
- Reports are not imported via barcode.
- Reports about the lites are imported via barcode. This settings must be activated both in the purchasing and supplying companies.
For this, barcodes in all participating operations must be identical. The barcode is transferred and also written back to the order in the Complete Scheduling report.

**Update production date**
If capacity planning realizes that the original production date cannot be kept, a new date will be reported.
- The production date will not be updated in the order.
- Based on the report, the dates for the start and end of production will be updated in the order header. The earliest date for all products of the order will be used as the start-of-production date. For the end of production, the program will use the latest date defined for any of the order items.

**Check replacement time for purchased products**
Capacity planning checks if there is sufficient time for replacing the necessary materials so that the order can be produced in time.
- The replacement time for stock articles will not be checked.
- The replacement time for stock articles will be checked.

**Don't check whether all items have been reported**
For the feedback for the scheduling in A+W Production it is possible to check in the ERP Webservice whether all necessary items have been reported back.
- The completeness of the feedback is not checked.
- The completeness of the feedback is checked. Here, partially-delivered items are also considered. The following items are not reported back:
  - Service or surcharge items
  - Items with numbers greater than or equal to 900
  - Article items if no item transfer is activated
The check also considers partially-delivered items.

**Del. date can be changed indep. from scheduling**
By default, the delivery date of scheduled orders can only be shifted to an earlier date if the status of the order was changed in advance.
- The delivery date can only be changed if the order status is reset.
- The delivery date can be changed after scheduling and production beginning.
  - Here it is not checked whether this is still possible in production. The order is not canceled automatically.
  - If the order has already been transferred to A+W Capacity Planner (EL), an entry is written to the order history.

**Direction of the delivery date update**
If the delivery date may be changed, you can specify whether an earlier or later delivery date is calculated automatically and written back to the order.

**Evaluate A+W Production document type in case of feedback from Capacity Planner**
Choose an option to define how documents should be transferred by A+W Business:
- **Search for quotation or order:** Both orders and quotations are transferred to production. With this setting, the two document types have to have separate number areas.
- **Always as order (must be active for capacity transfer):** You have to choose this setting if you are using OrderXML transfer and A+W Capacity Planner (EL).

## Company Data – Miscellaneous
**Master Data > Company > Company > Miscellaneous tab**

This tab is used for making the settings for importing products from the suppliers Dorma, KI-Megla, and Schlechtendahl. The settings are read by the module BMECat import.

You can also make the settings for the connection with MS Outlook.

Automatic purchase orders for Dorma and the export of invoices, delivery notifications, and order confirmations in openTrans format are exchanged via A+W Commercial Exchange Service.

> **Data import**
> Import of data is started via module BMECat. To import data from Dorma's website you have to enter the URL and access data on tab Stock/PCH/EDI.
> -> "Company Data – Stock/Purchasing/EDI" on page B-955

### Settings for BMECat import
The following settings can be made for the suppliers who provide their product catalogs in BMECat format.

**Template product**
Number of the product based on which the imported articles should be set up.

**Matchcode prefix for product**
Code for the supplier in question. The supplier codes must be different, e.g. D. for Dorma, M. for Megla, S. for Schlechtendahl.

**Product number from**
Product number from which on products should be imported.

**Price list, Price key**
Price list and key valid for the products of the supplier in question.

**Variants from table number**
Number of the price table for colors (variants).

**Import of short descriptions, product info, pictures**
You can import further product data from the corresponding suppliers.
- Short description, product info, and/or pictures will not be imported.
- Short description, product info, and/or pictures will be imported.

### Link to Outlook
Outlook contacts can be linked with A+W Business so that these data do not have to be entered again.

**Import customers, suppliers, partners**
You can import the Microsoft Outlook data from your business partners to make them available in A+W Business.
- Data will not be imported.
- Data can be imported.

**Exchange name and surname of market partners, employees**
You can exchange the names and surnames in the email addresses of your business partners or of their employees at data import in order to adjust the display.
- First and last names will not be exchanged.
- First and last names will be exchanged.

**No transfer of market partners if email address/phone number is missing**
You can prevent the export of partner data to Outlook if no email address and/or phone number has been entered for the contact.
- All data will be exported.
- Data will not be exported if there is no email address and/or phone number.
