---
title: "EN_AWBusiness_Master_Data_9_9-4"
source: "EN_AWBusiness_Master_Data_9_9-4.pdf"
tags: ["A+W Business", "Master Data", "Software Reference", "Production", "Order Management", "Rounding", "Status Management", "Number Ranges", "ERP", "Configuration"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the A+W Business Master Data module, focusing on the configuration of Production and Order management settings. It details parameters for cutting processes, rounding rules, status management, and number ranges."
long_description: "This comprehensive software reference manual provides detailed instructions for configuring the Master Data within the A+W Business ERP system. The guide is divided into two main sections: Production and Order. The Production section covers settings related to manufacturing processes, such as defining the minimum and maximum distances between cuts on a stock plate, setting limits for maximum waste, and configuring cutting table capabilities like automatic breakout, auto-loading, and laminated glass cutting. The Order section details the setup for managing orders and documents. This includes creating rules for rounding values (amounts, surfaces, lengths), defining status points that a document passes through, and allocating statuses to internal business processes. It also explains the configuration of number ranges for various documents (orders, invoices, credit notes), business types, quantity limits for pricing, and document types for different business scenarios like stock P.O.s, complaints, and partial deliveries. The manual is intended for system administrators and technical users responsible for setting up and maintaining the A+W Business software."
---

---
## Production

### Distance between cuts

*Fig. B-204 XYZ cuts on the stock plate*

**Min. dist. Y-Y cuts**
The minimum distance between Y-Y cuts depends on the use of the automatic breakout line and on the distance of the Y cutting heads. For cutting tables with several Y cutting heads, the minimum distance matches the distance of the cutting wheels of two cutting heads moved together, e.g. Bystronic XYZVA = 300 mm.

**Min. dist. X-X cuts**
Minimum distance between X-X cuts in case of automatic breakout.

**Max. Dist. Y-Y cuts**
Maximum distance between Y-Y cuts in case of automatic breakout.

**Max. Dist. X-X cuts**
Maximum distance between X-X cuts in case of automatic breakout.

### Maximum waste

**X direction**
Maximum length of waste permitted for a stockplate. This is the distance in mm from outermost X cut to the edge.

**Y direction**
Maximum length of waste permitted for a subplate. This is the distance in mm from outermost Y cut to the edge.

**Z direction**
Maximum length of waste permitted on a Y strip. This is the distance in mm from outermost Z cut to the subplate.

### Settings

**Auto breakout**
The lites can be broken automatically if the cutting table is equipped with a breakout device.
- Cut lites will not be broken automatically.
- Cut lites should be broken automatically.

**Auto. loader**
The lites can be loaded automatically if the cutting table is equipped with an automatic loader.
- The lites will not be loaded automatically, e.g. in case of manual cutting.
- The lites will be loaded automatically. Every stockplate must be allocated a loader code in this case.
⇨ "Autom. loader code" on page B-873

**Shapes**
Shapes can only be cut on tables that are appropriately equipped, e.g. for manual cutting.
- ☐ Shapes are not to be cut on this table.
- Shapes can also be cut on this table.

**Max. subplate can be enlarged**
The maximum subplate width can be exceeded for some tables.
- The maximum subplate width must not be extended.
- The maximum subplate width can be extended on this table.

**LAMI**
Laminated glass can only be cut on tables that are equipped appropriately.
- Laminated glass cannot be cut on this table.
- The table can be used for laminated glass cutting.

**Edge deletion**
Edge deletion is only possible on suitably equipped tables.
- This table cannot handle edge deletion.
- This table can handle edge deletion.

**Manual cutting**
Manual cutting is possible on tables that are suitably equipped.
- This table cannot be used for manual cutting.
- This table can also be used for manual cutting.

**Table**
This list shows all cutting tables.

### Processes

**Master Data > Production > Processes**

*Fig. B-205 Work processes*

This dialog is used for compiling the processes to be transferred to production. The processing steps are loaded from module A+W Business Capacity Planner.

The dialog functions are released only for specified customers. If you want to use this dialog please contact A+W Software GmbH.

### Breakage Reasons

**Master Data > Production > Processes**

*Fig. B-206 Breakage reasons*

| Logistics Breakage Type | Reason | Free |
| :--- | :--- | :--- |
| 1 Produktion / Production | Produktionsfehler / Error in production | ☐ |
| 2 Fahrer / Driver | Bruch / Breakage | ☐ |

Use this dialog to assign the causes of complaints to the reasons for complaints. With this information, you can create evaluations for the different causes of breakage.
⇨ "Complaint Cause" on page B-574
⇨ "Complaint Reasons" on page B-575

## Order

**Master Data > Order**

This program section serves to enter the data that are necessary for managing orders and other documents.

Menu Order offers the following entries:
- "Rounding" on page B-880
- "Rounding Points" on page B-882
- "Rounding Allocation" on page B-883
- "Status Management" on page B-884
- "Status Points" on page B-885
- "Status Allocation" on page B-886
- "Business Type" on page B-887
- "Quantity Limits" on page B-888
- "Priority" on page B-889
- "Number Ranges" on page B-890
- "Lock Code" on page B-897
- "Document Type" on page B-899
- "Categories" on page B-901
- "Reasons for change of delivery date" on page B-902

### Rounding

**Master Data > Order > Rounding**

*Fig. B-207 Rounding*

Use this dialog for entering the roundings you require. These roundings will be used for all values that should be rounded, e.g. amounts, surfaces, lengths, etc.

| Number | Name | Rounding Digits | Rounding type |
| :--- | :--- | :--- | :--- |
| 1 | Standard-Rundung/Standard rounding | 1 | 2 Commercially |
| 5 | Rundung auf 0,05 / Round to 0.05 | 5 | 2 Commercially |
| 10 | Rundung auf 0,1 / Round to 0.1 | 10 | 2 Commercially |
| 50 | Rundung auf 0,5 / Round to 0.5 | 50 | 2 Commercially |
| 100 | Rundung auf nächste ganze Zahl/Round 1.0 | 100 | 2 Upwards |
| 500 | Rundung Endbetrag / Round totals | 1 | 2 Commercially |
| 1000 | Rundung HKK / Round MCC | 1 | 5 Commercially |
| 1001 | Rd. auf 0,01 nach oben / Round to 0. | 100 | 2 Upwards |
| 1002 | Rundung 3NK/Rounding 3 digits | 1 | 3 Commercially |
| 1003 | Rundung 4NK/Rounding 4 digits | 1 | 4 Upwards |

When you enter special roundings for individual partners or whole partner groups, these have to be allocated to the partner or to the group afterwards.
⇨ Tutorial 2, "Roundings" on page B-441
⇨ "Rounding (Customer, Supplier)" on page B-839
⇨ "Rounding for Customer/Supplier Groups" on page B-840

**Number**
ID of the rounding.

**Name**
Name of the rounding.

**Rounding value**
Value to which the figure(s) should be rounded.

**Digits**
Number of decimals to be rounded to.

> **Example**
>
> **Consider 1 digit:**
> For a value of 0.14, the 4 will be rounded, e. g. to 0.1.
>
> **Consider 2 digits:**
> For a value of 0.147, the 7 will be rounded, e. g. to 0.15.

**Rounding method**
Rounding type to be applied:
- **Commercially:** Amounts from 0 to 4 will be rounded downwards and amounts from 5 to 9, upwards.
- **Upwards, downwards:** All amounts will be rounded upwards or downwards as indicated.

Rounding types have to be allocated to the rounding points in dialog Rounding allocation.
⇨ "Rounding Allocation" on page B-883

### Rounding Points

**Master Data > Order > Rounding points**

*Fig. B-208 Rounding points*

This dialog is used for defining the rounding points. They describe the units in which the values should be rounded, i.e. amounts, surfaces, and lengths.
Rounding points have to be allocated to the appropriate roundings in dialog Rounding allocation.
⇨ Tutorial 2, "Roundings" on page B-441
⇨ "Rounding Allocation" on page B-883

| Number | Name |
| :--- | :--- |
| 1 | qm-Preis/ME Glasposition |
| 2 | qm-Preis/ME Zuschläge |
| 3 | qm-Preis/ME Bearbeitungen |
| 4 | Brutto/Stk. Glasposition |
| 5 | Brutto/Stk. Zuschläge |
| 6 | Brutto/Stk. Bearbeitungen |
| 7 | Brutto/Stk. Stück Glasposition |
| 8 | Brutto/Stk. Stück Zuschläge |
| 9 | Brutto/Stk. Stück Bearbeitungen |
| 10 | Netto/Stk. Glasposition |
| 11 | Netto/Stk. Zuschläge |
| 12 | Netto/Stk. Bearbeitungen |
| 13 | Gesamtpositions-Netto Glasposition |
| 14 | Gesamtpositions-Netto Zuschläge |
| 15 | Gesamtpositions-Netto Bearbeitungen |
| 16 | qm Fläche ISO |

### Rounding Allocation

**Master Data > Order > Rounding allocation**

*Fig. B-209 Rounding Allocation*

Use this dialog to allocate the rounding to the corresponding rounding points. These rounding allocations are generally applicable.
If you have defined customer- or supplier-specific roundings you have to allocate them to the partners.
⇨ "Rounding (Customer, Supplier)" on page B-839
⇨ "Rounding for Customer/Supplier Groups" on page B-840

**Client**
Client for whom the rounding allocation should be valid. If you are using several clients, the roundings have to be allocated to each of them.

**Rounding points**
Rounding point to which a rounding should be allocated.
⇨ Tutorial 2, "Roundings” on page B-441
⇨ "Rounding Points" on page B-882

**Prod.type/class**
Product type and product group for which the allocation should be valid. The entry `<n.e.>/<n.e.>` means that the rounding allocation should be generally applicable.
This way, you can allocate different rounding types per product type and product class to every rounding point.

**Price unit**
Price unit to which the rounding allocation refers, e.g. for different price rounding per meter and millimeter or for the energy surcharge which is calculated with three decimals.

**Net price flag**
In customer/supplier management, you can define whether or not net prices should be calculated. The setting can be changed in the order. To make sure that the correct rounding is applied, you have to allocate a rounding in both cases.
- The rounding allocation does not apply to net prices.
- The rounding allocation applies to net prices.

**Rounding table**
Rounding to be allocated to the rounding point. You can define further roundings.
⇨ Tutorial 2, "Roundings" on page B-441
⇨ "Rounding" on page B-880

**Table**
The table shows all allocations for the client in question.

### Status Management

**Master Data > Order > Status management**

*Fig. B-210 Status Administration*

This dialog serves to enter the processing points (user status) a document passes on its way through your company. Every user status can be assigned an A+W Business status point to make sure that the status is automatically changed according to your business processes.
⇨ Tutorial 2, "Status Administration" on page B-418
⇨ "Status Allocation" on page B-886

> **Change of user status**
> Please contact A+W Software GmbH before changing a user status according to your ideas or before entering a new one. This will help to avoid system errors or incompatibilities.

### Status Points

**Master Data > Order > Status points**

*Fig. B-211 Status Points*

In this dialog you can use the process numbers and names defined in A+W Business. These so-called status points are used for the automatic processing of documents. They signal the end of various, internal processes a document passes from input up to the printing of an invoice, including complaints or credit notes. The status points are fixed in the system and are used to define conditions for further processing, e.g. for printing invoices. Every status point can be assigned a user status per document.
⇨ Tutorial 2, "Roundings" on page B-441
⇨ "Status Allocation" on page B-886

> **Do not change status points**
> The status points must not be changed. New status points can only be added in agreement with A+W Software GmbH.

The different status points are always described in connection with the circumstances in which the processes occur, e.g. printing of forms.

**Identifier**
Status point (process) number. The numbering has nothing to do with the sequence of processes.

**Type**
The type indicates the document type to which the status point should apply:
- 0: all documents
- 1: quotation
- 2: order
- 3: credit note
- 4: purchase order request
- 5: Ρ.Ο.

**Name**
Internal name of the process.

### Status Allocation

**Master Data > Order > Status Allocation**

*Fig. B-212 Status Allocation*

This dialog is used to allocate the internal processes (status points) to your business processes (user status).

**Status allocation table**
This table lists all status points managed by A+W Business.
⇨ "Status Points" on page B-885

**Status allocation**

**Status point**
Status points managed by A+W Business. The status points appear in numerical sequence. The numbering has nothing to do with the sequence of processes.

**Document type**
Document type for which the allocation is valid. You can thus restrict the automatic status allocation so that e.g. an order can be transferred to the purchase pool while a quotation can not.

**User status**
Allocated user status. All entries defined in status management are presented for selection.
⇨ "Status Management" on page B-884

**Min. status**
Minimum status the document has to have to reach the selected status point.

**Lock status**
Status for which the corresponding document is locked, e.g. a P.O. should be not be changed after receipt of the ordered goods has been booked.

### Business Type

**Master Data > Order > Business type**

*Fig. B-213 Business types*

This dialog is used to define the different business types. These are used for differentiating proceeds accounts and for statistics.

Business types can be allocated in the following dialogs:
- **Proceeds accounts:** Allocation for financial accounting (FinAcc).
  ⇨ "Proceeds Accounts" on page B-909
- **Order areas:** Allocation for internal invoicing.
  ⇨ "Order Areas" on page B-1014
- **Order header:** Allocation for booking to proceeds accounts.
  ⇨ Sales, "Header data - Document" on page C-416
- **Turnover statistics:** Selection and sorting criterion.
  ⇨ Statistics, "Turnover Sales – Restrictions" on page F-28

**Name**
Name, e.g. trade or drop shipment.

**External key**
External key for communicating with other programs.

**Locked**
A business type can be locked for entry in partner management and in documents if it is no longer needed.
- The business type can be allocated.
- The business type is locked and cannot be allocated. If it has been allocated to products and in documents, it will still be shown however.

### Quantity Limits

**Master Data > Order > Quantity limits**

*Fig. B-214 Quantity Limits*

This dialog shows the defined quantity limits, e.g. square meters, units, linear meters, thickness, airspace.
Quantity limits are used for defining prices and surcharges.
⇨ Tutorial 1, "Defining a Graduated Price with Limits" on page B-256
⇨ "Prices" on page B-713
⇨ "Miscellaneous Surcharges" on page B-664

> **Dialog locked**
> Only the system administrator can access this dialog.
> Amendments have to be approved by A+W Software GmbH.

**Name**
Name of the quantity limit.

**Code**
Internal identification number.

**External key**
External key for communicating with other programs, e.g. for transfer to production or financial accounting.

**Locked**
A quantity limit can be locked for the definition of prices if it is no longer needed.
- The quantity limit can be used.
- The quantity limit is locked and cannot be used any more. If it has been allocated, it will still be displayed.

### Priority

**Master Data > Order > Priority**

*Fig. B-215 Priority*

This dialog serves to enter the priorities for controlling the transfer to production. The priority defined for the order is transferred to capacity planning.
The priorities are predefined by A+W Business. If you add more levels, these have to be defined in A+W Production as well.

Priorities can be allocated in the following dialogs:
- **Order:** The priority loaded from partner management can be changed.
- **Capacity planning:** Determination of production dates and times depending on the priority of the order.

**Name**
Name of the priority.

**Production priority**
The numbers are predefined by A+W Business and must not be changed.
- **0 - Urgent:** These orders will be produced with top priority.
- **1 - Common:** These orders will be fitted into the usual schedule.
- **4 - Extra:** This priority means that the order should be produced from residue (plates) left over from cutting other orders.
- **9 - On call:** Orders are produced on call.

**External key**
External key for communicating with other programs, e.g. for transfer to production.

**Locked**
A priority can be locked for allocation if it is no longer needed.
- The priority can be set.
- The priority is locked and cannot be set. If it has been allocated, it will still be displayed.

### Number Ranges

**Master Data > Order > Number Ranges**

Number ranges are logical organization units as well as a means to combine work processes triggered by a so-called number manager.

Dialog Number Ranges offers the following tabs:
- Number Ranges – Documents
- Number Ranges - Production
- Number Ranges - Financial Accounting
- Number Ranges - Table
⇨ Tutorial 2, "Number Areas" on page B-432

> **Do not reset the number range during operation**
> Resetting or changing the number ranges during operation can cause problems if old document numbers should exist in a new number range. This is why you should carefully check beforehand to make sure that all documents with old numbers have been archived.

**Functions menu**
Menu Functions permits to check whether the (newly) defined number ranges clash. If so, the system will issue a message to that effect.

#### Number Ranges – Documents

**Master Data > Order > Number Ranges > Documents tab**

*Fig. B-216 Number Ranges – Documents*

You can use this dialog for setting up the number ranges for allocating consecutive numbers. You can allocate 8-digit numbers.

**Client, Order area**
For every client, you can define special number ranges by order area. Use tab Table to choose the client and OM area the number areas of which you want to check or change.

> **Example**
> Different number ranges have been set up for the order areas for toughened and IG production. Based on the order number, the workers can see whether the order in question concerns toughened or IG production.

The number ranges of the different clients and order areas must not overlap.

**Employee**
For documents, you can define different number ranges by employee.
If you do not want to bother with this, just leave the entry at `<n.e.>`. In user management, every user can be allocated to the appropriate order area. The document number will be automatically loaded from the corresponding number range.

**From, Current, To**

**From, to**
First and last number of the number range. The document number ranges must not overlap.
To lock a document for an order area, enter 0 in both fields and 1 in field current.

**Current**
Last number allocated by the system.

**By period**
This field is filled by the Number ranges print program.
⇨ Sales, "Number Ranges" on page C-726

> **Example**
> Field by period shows the number 181 for orders. The current order number has meanwhile reached 218. If you start the print program, all orders from 182 to 218 on this list will be printed. After printing, the value in field by period will be set to 218.

> **Note**
> When entering new number ranges please make sure that number ranges do not overlap. This also applies to documents, e.g. quotations that can be entered in different order areas.

**Prefix**
A separate prefix can be used per document type, e.g. for clients or order areas.

**Quotations**
Quotations are independent documents. The system checks this number range at order entry.

**Orders**
Orders are independent documents. The system checks this number range at order entry. Partial deliveries as well as complaints belong to the document Order. For the latter, special number ranges are set up on tab Production. These number ranges must not clash.

**Purchase Orders**
Purchase orders are independent documents. The system checks this number range at P.O. entry.

**Supplier inquiries**
Inquiries are independent documents. The system checks this number range at order entry.

**Invoices**
An order gets an invoice number when the invoice is printed. This will be saved in the order. The invoice number is independent of the order number.

**Credit notes**
Credit notes are independent documents. The system checks this number range at credit note entry. Generally, the system expects different number ranges for invoices and credit notes. To use the invoice number range for credit notes you have to check the checkbox Cred.no. = Doc.no. in company data.
⇨ "Company Data > Documents" on page B-928

**Delivery notes**
The delivery note number is assigned when the delivery note is printed, and is saved in the order.

**Batch No. A+W Production archives**
When an order is archived, an STST file is created which - among others - includes this batch number. This transfer file is imported by A+W Production and triggers the archiving in A+W Production.
The batch number is analyzed only for the order area defined in **Company data > Archives** in field **Order area for batch number**.
This means that you set up this number range only for the client `<n.e.>` and for the order area selected in company data.
⇨ "Company Data > Archives" on page B-962

#### Number Ranges - Production

**Master Data > Order > Number Ranges > Production tab**

*Fig. B-217 Number Ranges - Production*

This tab is used to define the number ranges to be checked for data interchange with the shop floor.
The columns from, current, to and by period are described in connection with the tab Documents.
⇨ "Number Ranges - Documents" on page B-891

**AWPool batch no.**
Start and end numbers for the AWPool batch numbers. The system checks this number area at transfer to production.
⇨ Production, "Transfer to Production" on page E-168

**Partial delivery, Complaint, Complaint when breakage**
Start and end numbers for partial deliveries and complaints.

> **Partial delivery, Complaint**
> When editing number ranges, please note that partial deliveries and complaints belong to the document Order. These three number ranges must not clash.

**Rack number**
Currently not used.

**S+N File Number**
This number range is checked in the following cases:
- If shape processing is saved as a SN file at item entry.
  ⇨ Sales, "Items - Stepping" on page C-485
- When a SN file is automatically created at transfer to production.
  ⇨ Production, "Transfer to Production" on page E-168

#### Number Ranges - Financial Accounting

**Master Data > Order > Number Ranges > Financial accounting tab**

*Fig. B-218 Number range - financial accounting*

On tab FinAcc, enter the first batch number for transfer to financial accounting (FinAcc).
The columns from, current, to and by period are described in connection with the tab Documents.
⇨ "Number Ranges – Documents" on page B-891

#### Number Ranges – Table

**Master Data > Order > Number Ranges > Table tab**

*Fig. B-219 Number Ranges – Table*

This tab shows the order areas (per client) for which different number ranges have been defined. To edit the number ranges, select the required entry. The other tabs will show the appropriate number ranges.
⇨ "Number Ranges - Documents" on page B-891
⇨ "Order Areas" on page B-1014

### Lock Code

**Master Data > Order > Lock Codes**

*Fig. B-220 Lock Code*

This dialog serves to define the lock codes. Lock codes can be used to lock documents for certain actions while automatically raising their status. This means that the document cannot reach the locked status but is instead diverted to another status point (process).

> **Example: Partial delivery without invoicing**
> If partial deliveries must not be invoiced, the system has to be able to recognize a partial delivery as such. In this case, no partial invoice can be created for the partial delivery. The status of the partial delivery will instead be raised automatically. After the order is diverted to Transfer to archives, the partial delivery cannot be edited any further.

Lock codes for complaints and partial deliveries are preset in the company data.
⇨ "Company Data > Documents" on page B-928

> **Please discuss changes with A+W Software GmbH**
> Please discuss any changes of lock codes with A+W Software GmbH beforehand to avoid problems.

**Name**
(Descriptive) name of the code.

**Locked**
A lock code can be locked for further use if it is no longer needed.
- The lock code can be allocated.
- The lock code is locked and cannot be allocated. If it has been assigned in a document, it will still be shown however.

**Status**

**Status restriction**
Status that will be diverted to another status.

**Deviation to status point**
Status point to which the document should be diverted.

**External key**
External key for communicating with other programs, e.g. for transfer to production or financial accounting.

**Table**
This list shows all lock codes. Select an entry to change the settings in the fields.

### Document Type

**Master Data > Order > Document type**

*Fig. B-221 Document type*

Use this dialog to check which document types are used by A+W Business.

> **Additional document types**
> The document types are preset by A+W Business. Please discuss any changes or extensions with A+W Software GmbH.

**Name**
Document type:
- **Down payment:** This document type is automatically used for down payment invoices.
  ⇨ Sales, "Down Payments" on page C-671
- **In-house production:** Not used at present.
- **Claim:** This document type is used for issuing invoices for a blanket order.
  ⇨ "Claims Calculation" on page B-837
- **Release:** Not used at present.
- **Internal invoicing:** This document type is automatically used in connection with module Profit Center Invoicing.
- **Internal order:** This document type is used for P.O. transfer in connection with the module Internal orders (multi-stepped production).
  ⇨ Sales, "P.O. Transfer" on page C-652
- **Customer material:** This document type must be set by hand. As a result, all items will be automatically set to procurement type Customer's own glass.
- **Stock P.O.:** This document type is automatically used for creating a stock P.O. The code can also be set manually for a P.O.
  ⇨ Sales, "P.O. Transfer" on page C-652
  ⇨ Inventory Management, "Stock P.O." on page G-220
- **Work order:** This document type is used for filling up your own stock.
  ⇨ Production, “Production Orders" on page E-128
- **Blanket order:** This document type is used for creating blanket orders.
  ⇨ "Projects (Customer, Supplier)" on page B-821
- **Complaint:** This document type is used for entering complaints.
- **Serial order:** This document type is used for creating serial orders.
- **Partial delivery:** This document type is automatically set when partial deliveries are entered.
- **Shipping order:** Not used at present.
- **Value booking:** This document type is used for entering credit notes. Quantities like piece, square meter and linear meter are not transferred to statistics as a result.
  ⇨ Sales, "Credit Note (Document Management)" on page C-722

**Locked**
A document type can be locked for further use if it is no longer needed.
- The document type can be allocated.
- The document type is locked and cannot be assigned any more. If it has been assigned before in a document, it will still be shown however.

> **Locking a document type**
> Locking a document type has a massive effect on order entry. If you want to lock a document type please contact A+W Software GmbH. This helps to avoid unwanted negative effects on your work with A+W Business.
