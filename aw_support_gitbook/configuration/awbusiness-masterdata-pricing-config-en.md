---
title: "EN_AWBusiness_Master_Data_9_10-3"
source: "EN_AWBusiness_Master_Data_9_10-3.pdf"
tags: ["A+W Business", "Master Data", "Software Reference", "Pricing", "Stock Management", "EDI", "Archiving", "System Configuration", "Company Data"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for A+W Business Master Data, covering company-level settings for pricing, stock management, EDI, data archiving, and system configurations."
long_description: "This comprehensive software reference guide details the configuration options available within the A+W Business Master Data module. It is divided into several key sections, providing administrators and advanced users with the necessary information to customize the software to their company's specific needs. The guide covers a wide range of topics, including detailed price calculation settings such as handling surcharges, French pricing rules, currency conversions, and CPIP creation. It also explains settings related to stock, purchasing, and EDI, including how purchase prices are calculated, how inventory is managed at the BOM level, and configurations for EDI interfaces and Dorma web services. Furthermore, the document outlines the procedures for data archiving, explaining how to set up global and document-specific archiving rules, manage statistics (turnover, sales commission), and configure automatic data deletion policies. Finally, it details system-level settings, such as units of measurement, date/time formats, lead day calculations, and integrations with other A+W modules like A+W CAD Designer. The guide uses screenshots, option descriptions, and cross-references to other parts of the documentation to provide a thorough understanding of each configuration parameter."
---

---
## Software Reference - Company

### Delete glass, gas, and airspace surcharges if price/unit is defined (not for French pricing)
Surcharges can be suppressed in case of manual price changes. The corresponding option is displayed at item entry.

-   This option is active at item entry by default.
-   This option is disabled at item entry.

⇨ "Options menu" on page C-412

### French Pricing
With French pricing, you can choose any option at item entry.

### Spacer does not get discount PGR of IG
If a special product group has been entered for discounts on IG units, you have to define whether this should be applied to all BOM elements.

-   Generally, the IG discount product group is applied to all BOM elements.
-   The discount product group for IG will not be used for spacers.

### Obey currency in price master data
Currencies can be taken into account in price lists and orders. You can even take into account a third currency.

-   By default, price lists are entered in national currency so that no special settings are required. An exchange rate is defined for conversions into foreign currency.
-   You have to choose this setting if orders are entered in foreign currency.
-   This function needs to be enabled if the price list is not entered in national currency and if orders are also entered in a third currency, or converted into a third currency. You also have to enter the exchange rate in this case.

⇨ Tutorial 2, "Currencies" on page B-456
⇨ "Currency" on page B-908
⇨ "Currency settings" on page B-921

### CPIP creation
Characteristic Performance Identification Paper (characteristics of features and of the performance). The CPIP code can be created automatically at order entry provided that the parameters have been defined in the CE code dialogs. This function is only required in France. It can be used only if the complete master data for CE codes have been entered.

-   No CPIP code will be created.
-   When documents are entered, the CPIP code will be determined, to be printed on the forms. The program also checks the defined restrictions and issues a message if they are not met.

⇨ "CE Code" on page B-1079

### Extended pricing (reference price, manual change)
Prices can usually be changed in the order. You have to define if customized price lists are still to be used in case of price changes.

-   If prices are changed by hand in an order, the price entered in customer master data will not be loaded.
-   If prices are changed by hand, the system checks if the price entered lies below the standard price defined for this customer. If so, an additional dialog appears where a reason for the new price has to be given.

The setting enables the **Mandatory reason for price change** checkbox.
⇨ "Customer Individual Products" on page B-818

### Mandatory reason for price change
For a manual price change in the order, the specification of a reason can be made mandatory.
The checkbox is only enabled if the **Ex. pricing (reference price, man. change)** checkbox is enabled.

-   The specification of a reason for a manual price change is not required.
-   In case of a manual price change, a reason must absolutely be specified.

### Check min. qty. mainly by price unit
Minimum quantities are usually calculated based on the quantity unit.

-   The quantity unit defined for the product will be applied by default when checking the minimum quantity.
-   The minimum quantity check is based on the price unit.

⇨ Tutorial 1, "Pricing Codes" on page B-168
⇨ Tutorial 1, "Limit Types for Graduations" on page B-249

### Calculate total order price for BOM
The amounts of the individual order items are multiplied by the quantity, provided that amounts should be displayed and printed at all.

### Total per PGR combination
The total quantity for the BOM can also be calculated by means of the PGR combination. This checkbox is accessible only if checkbox **Calculate total order price for BOM** has been checked.

-   The total quantity will not be calculated by PGR combination.
-   The total quantity will be calculated by PGR combination. This allows e.g. distinguishing total quantities with and without processing.

### Sort individual prices by price list
You can control the sorting of individual prices.

-   The program will first find the individual price the price list of which has the lowest ID, i.e. which has been entered first.
-   The program will find the price list with the highest ID first.

### Delete surcharges only if SP+PP are zero
The surcharge can be deleted if no price has been entered for an item.

-   The surcharge will be deleted if zero (0) is entered for the sales price.
-   The surcharge will be deleted only if zero has been entered for the sales and the purchase price.

### Calculate external PGR key as an inexact quantity limit
The quantity limit **140 Exact external PGR key** can be used as an exact quantity limit for the external PGR key.
If the quantity limit is **External PGR key**, item price and price list price will be calculated in different ways.

-   The quantity limit **140 Exact external PGR key** will not be treated as a system-wide quantity limit.
-   The quantity limit **140 Exact external PGR key** will be treated as a system-wide quantity limit.

⇨ Tutorial 1, "Price Calculation by PGR" on page B-262

### Enable pricing based on macro prices
The search for prices can also include macro prices.

-   No macro prices will be checked when searching for prices. This setting makes sense only if macro prices are not used at all.
-   Macro prices, e.g. for specific IG structures, will be checked when searching for prices. The price macro can be valid for a customer or in general. Macro prices will be shown in customer terms at item entry.

### SP relevance of customer's own glass
Glass supplied by the customer can be entered with or without a price. This depends on the supply type **Customer's own glass** or on document type **Customer's material**.

-   Glass supplied by the customer is entered without a price.
-   A sales price will be calculated for glass supplied by the customer.

### PP relevance of customer's own glass
Glass supplied by the customer can be entered with or without a price. This depends on the supply type **Customer's own glass** or on document type **Customer's material**.

-   Glass supplied by the customer is entered without a price.
-   A purchase price will be calculated for glass supplied by the customer.

### Apply misc. surcharges to price/PU in case of manual entries
A miscellaneous surcharge that is applied to the price/the price unit, will be added to the price. For prices entered by hand, you can define how the price should be displayed in connection with miscellaneous surcharges.

-   The increased value is shown in the price/price unit.
-   The miscellaneous surcharge is included in the gross price. If the gross price is not shown on the form, the price cannot be explained.

### Qty. limit on BOM level for French pricing (gas and spacers)
In connection with French pricing, the search for the quantity limit can be set to **Exact variant no.**

-   For French pricing, the quantity limits for the spacer and the gas will be defined on item data level. The program will not search for the exact spacer variant (color).
-   French pricing also takes into account a spacer with limit type **Exact variant no.**

### For French. price calc. calculate the min. price on BOM
For the French price calculation, the minimum price can refer to the BOM components.

-   The minimum price is calculated on the main product.
-   In the French price calculation, the BOM is incorporated if the setting **XX+PU** is activated in the item.

### Exact calculation of surface/circumference for surface treatment
Surface and circumference calculation can be based on rounded or actual sizes.

-   Surface and circumference will be calculated based on rounded sizes.
-   Surface and circumference will be calculated based on the exact (actual) sizes.

### Calculate delivery fee by delivery date instead of by shipping date
The delivery fee can be calculated by shipping date or by delivery date. These dates can differ e.g. if shipping is done via an intermediate store.

-   The delivery fee will be calculated by shipping date.
-   The delivery fee will be calculated by delivery date.

### Price relevance for Shaping+Nesting shape rectangle acc. to master data
Shape 0 that has been defined for creating a SN file can adopt the code **price-relevant** from master data, or can be set to **not price relevant**.

-   The code will be set to **not price relevant**.
-   The code is adopted from master data. This means that you can enter prices and costs for shape 0 that will not be changed when a SN sketch is created.

### Master data rounding Price per quantity unit Foreign currency
The prices per quantity unit can be rounded off for foreign currencies.

-   The prices per quantity unit are not rounded off using the settings in the master data of the foreign currency.
-   The prices per quantity unit in foreign currency are rounded off. The number of places after the decimal point is taken over from the management of the currencies.

⇨ "Currency" on page B-908

## Company Data – Stock/Purchasing/EDI
**Master Data > Company > Company Data > Stock/Purchasing/EDI tab**

This tab serves to define how the purchase price of inventory products is to be calculated, and how inventory P.O.s should be reserved. You can also enter details for the EDI interface.

### Purchasing

**Calculate purchase price**
Check this checkbox if the purchase price for stock products should be calculated automatically. This releases the option buttons. The following options are available for selection:

-   **Average PP:**
    The average purchase price will be recalculated in the following cases:
    -   Whenever the receipt of stock P.O.s is booked.
    -   With every invoice check.
    -   After reallocations (stock movements).
    -   After an inventory value adjustment.
    The updated average purchase price is saved in the standard price table of the product.
-   **Last PP:**
    The last purchase price booked on stock after receipt of goods or an invoice check, will be saved in the standard price table.
    ⇨ Inventory Management, "Stock Management - Prices" on page G-190

### Ignore combined stock articles without sizes
You can define that combined stock articles for which no sizes have been defined should be ignored when calculating the average purchase price. In this case, only the average cost of the stock sizes will be calculated.

-   Stock articles without sizes will not be ignored.
-   Check this checkbox if combined stock articles without sizes should be ignored when calculating the average purchase price. You should choose this setting if you are using production reports.
    ⇨ Inventory Management, "How should stock be managed" on page G-15

### Include spacers in grill orders
Whenever the BOM or the procurement type is changed, the system checks if the BOM includes grill that have to be ordered.

-   The procurement type for the spacer is loaded from product data. It can be changed in the order. Transfer to purchasing will only check the procurement type defined in the order.
-   If the BOM includes grill of supply type P.O., the spacer's supply type is set to P.O. as well. This setting is adopted for the second grid if the first grid has been copied to the second spacer.

> **Order spacers and grill from the same supplier**
> If the spacer is set to procurement type P.O. in the order, it will be listed as a separate item at transfer to purchasing. If a supplier for grill has been entered in the supplier file, this will be used for spacers too.
> In case of manual changes please make sure that spacers and grills are ordered from the same supplier.

### IG as a purchased article (processing can be done in-house)
Purchased articles are ordered according to their procurement type.

-   If the BOM of an IG unit includes processing of the procurement type **In-house production**, these will not be ordered.
-   The entire IG unit including processing will be ordered even if the BOM includes processing steps with procurement type **In-house production**.

### Show items w/o inventory code for stock P.O.s are receipt of goods
Goods received will be entered based on their stock code.

-   In stock P.O.s, items without stock code will not be marked at receipt of goods as a standard.
-   If items are entered at receipt of goods for which no stock code has been defined, these items will be shown in red letters.

### Purchasing suggestions for articles without sizes
Automatic creation of stock P.O.s can also take into account sqm stock articles (size 0 x 0 mm).

-   Stock articles without sizes will not be taken into account.
-   Stock articles without sizes will be taken into account when creating automatic purchasing suggestions for stock P.O.s.

### Weight in lbs
Via the OrderXML interface, by default, weights are transferred in the unit kilograms to production.

-   The weight is transferred in the measurement system in kilograms.
-   The weight is converted to imperial pounds (lbs.) during the transfer to production.

### In case of incomplete P.O., process complete BOM
Specification for how purchase orders are transferred to standard suppliers.

-   If for an order a standard supplier is entered for the whole order, the item must be set to **Purchase order (complete)** so that the BOM elements of an item to be ordered are also processed. If the item is only set to **Purchase order**, the BOM elements are not transferred to the purchase order.
-   This item is treated as if no standard supplier is entered. Thus the BOM elements to be ordered are transferred to the purchase order pool.

### Change PO and order if surplus/shortfall accepted
On receipt of goods of ordered order items, surplus/shortfall can be delivered.

-   Surpluses or shortfalls are not written back.
-   If on goods receipt a deviating quantity for an item is specified and accepted, the new quantities in the order are entered as surplus or shortfall.
    -   If the order is already in production, the quantity change is transferred to the production system.
    -   If the order is not yet in production, the over/excess quantity is reported to the production system with the production transfer.

### Stock control mode

**Update inventory in case of reservations**
Selection of whether the inventory should be updated in case of reservations.

-   **w/o:**
    When you enter an order, the quantity of the product entered will be reserved but not withdrawn from the stock on hand.
-   **with:**
    The reserved quantity is withdrawn from the stock on hand when the deliver note or invoice is printed.
    If no other storage place has been entered in the stock search, the order quantities are allocated to the standard storage place.
    The decision about the stock location from which the product is withdrawn is made with reports from the optimization by the bar code registration.

### Stock control on BOM level
Products can be kept on stock even if they are part of a BOM.

-   By default, products are only added and withdrawn on main product level in A+W Business.
-   Additions and withdrawals are also made on BOM element level.
    ⇨ Inventory Management, "Stock control on BOM level" on page G-58

### Execute stock booking before printing the document
The stock on hand is usually updated when a delivery note or invoice is issued; this is recorded in stock history. You can define that withdrawals should always be recorded.

-   Stock withdrawals are booked when the form is printed.
-   Stock withdrawals will be booked separately from the printing of forms.

### Delete articles with ID if there is no stock on hand
When boxes are received, they get an identification number (ID) that is usually deleted when the box is withdrawn from stock. If boxes are broken up internally it can happen that the box is still kept on stock with this ID.

-   Stock articles (boxes) with ID and stock = 0 have to be deleted by hand.
-   Stock articles with an ID and stock = 0 will be deleted automatically.

### Stock control even without document type Stock P.O.
Partial deliveries can be created for stock P.O.s.

-   An (independent) partial P.O. for stock articles cannot be issued. The quantity delivered for a stock P.O. will be adopted for the partial P.O. however if part of the goods received have been booked already.
-   A partial P.O. can be issued for partial receipt of goods if the P.O.'s document type is not Stock P.O.
-   A partial invoice can be booked for such a partial P.O. In the order, the costs will be updated based on the average costs from all partial P.O.s. The costs will be saved as unit costs.

### Consumption of BOM elements in production orders
For production orders, the consumption of BOM elements in stock can be booked.

-   The consumption of BOM elements is not withdrawn automatically from the stock.
-   In production orders, a stock-kept BOM element is withdrawn from stock automatically and the product for the main item is added to the stock.

> **Example**
> In a production order, an IGU with a TSG is entered. After reporting of the production order, the IGU is booked into the stock, the TSG is withdrawn from the stock.
> If for the same IGU with TSG a normal customer order is entered, only the IGU is withdrawn from the stock. The TSG is not kept in the stock since it has already been withdrawn from the stock by the production order.

### XTV feedback for stock sizes only (w.o. reservations)
Also for products with the stock-keeping mode size-dependent, automatic withdrawals can be made with feedback from the optimization.

-   Products with the stock-keeping mode size-dependent are not withdrawn automatically from stock with feedback from optimization.
-   Products with the stock-keeping mode size-dependent are withdrawn automatically from stock with feedback from optimization. The quantity entered is not marked as reserved in the qm record. Only the stock sizes from the optimization feedback are withdrawn.
    ⇨ "Stock control mode" on page B-958

### Always calculate area according to circumscribed rectangle
Size-dependent lites can be booked differently in stock.

-   By default, lites that are not kept in stock depending on size are always booked with the actual area or waste in stock.
-   The area of the circumscribing rectangle is booked.

### Include foot surcharges in the purchase price of boxes
Percentage costs can also be considered for boxes with ID, e.g. energy surcharges, transport costs.

-   The percentage costs are not calculated in the box PU.
-   For boxes with ident number, the percentage costs are calculated in the PU.

### Stock preview

**No. of workdays**
The stock preview shows the availability of products for a certain period in the future. The number of days represents the number of days to be shown in the preview. The display starts from the current date.

### Dorma web service
The data in this section have to be entered if BMECat is to be downloaded from the Dorma website. These data match those for automatic Dorma purchase orders.

**Address**
Internet address of the Dorma web service.

**[Globe]**
When you have entered or changed the Internet address you can use this icon to check whether the connection can be established.

**User, Password**
Registration data that entitles you to access the Dorma web service.

**Save costs in the order**
The actual costs of a purchase order can differ from the costs defined in supplier data.

-   The costs will not be saved. The P.O. still shows the costs defined in master data.
-   The actual cost of the ordered articles will be saved in the order.

**[A+W test login]**
This button can be used to change the access data to the A+W Software GmbH test login. This allows to check whether the connection can be correctly established based on these data.

### Confirm Dorma transmission by email
You can have a transmission confirmation issued automatically to make sure that your online P.O. has been sent.

**Server**
Name of the server controlling the transmission confirmation.

**Port**
Number of the port for the transmission confirmation.

**Sender's address, Recipient's address, cc:**
Email addresses to be used by default for the transmission confirmation.

**Authentication**
An authentication can be used for the transmission confirmation.

-   The transmission confirmation will not be sent without authentication.
-   The transmission confirmation requires authentication. The fields for entering the registration data are accessible.

**Use SSL encryption**
Secure Sockets Layer (SSL); encryption program for safe data transfer in the Internet.

-   The transmission confirmation will not be encoded.
-   The transmission confirmation will be encoded acc. to the SSL log.

**User, Password**
Registration data the sender uses for authentication.

### EDI interface
Documents can be exchanged electronically (as files); the data will be imported into another system right away. The following settings are important only if you are using EDI interfaces.

**Disable OEM/ANSI conversion**
For transfer, the interface converts the data into a format that can be read by all other programs.

-   The data of the file to be transferred are automatically converted to ANSI format by default, e.g. ä becomes ae.
-   In special cases, data conversion has to be switched off, e.g. in connection with certain interfaces.

### Disable automatic scheduling in capacity planning
This setting only applies to A+W Business capacity planning. It is necessary to transfer order data electronically. The data are usually transferred by means of a work flow task.

-   Generally, the data of the imported orders are automatically scheduled in capacity planning if automatic scheduling is active.
-   Automatic scheduling of imported orders is disabled. This permits to check imported orders before scheduling.

If you are using A+W Business capacity planning, the checkbox for automatic scheduling must be disabled.
⇨ "Automatic scheduling" on page B-939

### Use architect from header record for article reference
During EDI import, no article reference in the header record is used.

-   During EDI import, the article reference to the architect is entered in the header record.
-   The architect number used for import is transferred to the order with import in order to distinguish the eCommerce orders from the rest of the orders later on.

### Reg. point allocation

**Order produced at**
When an item has been registered at the selected registration point, its status will be set to **produced** in A+W Business. The corresponding batch number will be saved with the order item.
If AWBar or A+W Production reports are sent to the files of the types STSP, STSL, STSD, STSB, STSG, you have choose a registration point that is allocated to a status point. If such a registration point was not assigned, the report generates an error.
Order information shows this item on tab Produced. The production date is updated in the order header.
⇨ Statistics, "Order Information" on page F-10

**Goods receipt in/for**
Specification of registration point.

### Check the P.O. parts in purchasing
The goods receipt of purchase order parts can be checked from a registration point or in purchasing.

-   Goods receipts from partial delivery items are checked through the packaged quantity reported by STSG. The reported quantities are queried for the generation of partial deliveries. The parts delivery can only be created for the quantity reported.
-   The goods receipt of purchase order parts is checked in purchasing.

## Company Data > Archives
**Master Data > Company > Company Data > Archives tab**

This tab defines how data and documents should be archived.
⇨ Tutorial 1, "Database" on page B-369
⇨ Tutorial 1, "Statistics" on page B-371

### Global settings
The settings in this area refer to automatic archiving that can be enabled in section **Automatic options**.

**Archives database**
Name of the A+W Business archiving database. Usually, the customer code is used as the name. The name of the archives database is completed by the corresponding year. This allows to manage several years in one database.

> **Create new archives**
> Please remember to have A+W Software GmbH create new archives for the next year.

### Consider complaints for sales commission
Complaints can be taken into account when calculating the sales commission.

-   Complaints will not be considered as a standard. The commission will not be reduced.
-   Complaints will be considered in the salesman's turnover. The sales commission will not be diminished however.

### Complaints without quantities (pc., sqm., lin.m.) to turnover statistics
Complaints can be analyzed with regard to prices and quantities.

-   Apart from the amounts, quantities (piece, sqm, linear meter, etc.) are also transferred to turnover statistics. This can mean that the quantities from uninvoiced complaints will reduce the total result.
-   Only the price is transferred to turnover statistics by default.

### Export super statistics
This option refers to module Group statistics. Group statistics are designed for groups of companies who are using different servers with separate databases, but need comprehensive statistics for all companies of the group.

-   This checkbox must be disabled for the main company running the analysis.
-   The checkbox has to be active for the client supplying the statistical data.
    ⇨ Statistics, "Super Statistics" on page F-32

### Transfer to statistics w/o printing an invoice/credit note
Turnover and quantities can be analyzed before or after printout of invoices and credit notes.

-   The invoice number created at printout has to be available to release transfer to statistics.
-   Orders can be transferred to statistics even if no invoice or credit note is printed. Transfer is released by the defined minimum status.
    ⇨ Tutorial 2, "Lock status" on page B-423

### Transfer to statistics only after invoice check
This option only refers to module **Invoice check** in purchasing.

-   By default, purchase orders are transferred to purchase statistics without an invoice check.
-   Purchase orders can be transferred to statistics only after the invoice has been checked.

### Transfer BOM glass turnover to main product
The turnover from exchanged lites can be analyzed together with the main product, or separately.

-   By default, the replacement surcharge is included in the turnover of the new element.
-   The replacement surcharge is included in the main product's turnover. The checkbox for cost analysis is accessible.

### Transfer cost of BOM glass elements to main product
The cost of exchange glass can be evaluated in statistics separately or together with the main product.
This checkbox is accessible only if the checkbox for turnover evaluation has been checked.
-   By default, the costs of replaced lites are included in the costs of the replacing element.
-   The costs of the replaced lites should be included in the costs of the main product.

### Book transfer to statistics of box qty./surface to item
The size and quantity included in a box can be analyzed in statistics on BOM element level or on item level.

-   The contents of boxes is booked to statistics on BOM element level by default.
-   The contents of boxes should be booked to statistics on item level. With this setting, the analysis depth in statistics must refer to items only. The analysis depth **Item and BOM** would falsify the size on product group level otherwise because the size is calculated for the glass and the processing.

> **Statistics update**
> If you have chosen the setting **Book transfer to statistics of box qty./surface to item**, statistics must be drawn up anew via **Utilities > System > Statistics update**.

### Transfer to archives by input date
Documents are archived based on their input date.

-   Archiving is based on the invoice date by default.
-   The order input date is used as a basis for archiving.

### Delete documents without checking the reference
This setting only refers to documents created by transfer to purchasing.

-   Usually, a P.O. can be deleted only if the corresponding order has been archived, and deleted from the main database.
-   When deleting a document, the system does not check if there are reference documents. The archiving year does not depend on the order but on the P.O.

### Delete documents only if already archived
Documents can be deleted from the main database to keep its size at bay.

-   The document can be deleted without checking archives.
-   A document (order, P.O., etc.) can be deleted (by hand) only if it has been transferred to archives before. The system will search for the corresponding history entry.

### Multiple archiving
The document is archived when the order is completed, i.e. when the invoice has been transferred to financial accounting and statistics.

-   Every document can be archived just once.
-   Documents can be archived several times. This setting makes sense only if a document is fetched from archives to be amended. In this case, the original document will be deleted; only the amended one will be archived.

### Book complaint orders only in turnover statistics
Orders based on complaints can falsify turnover statistics.

-   By default, the turnover of orders and the corresponding complaint orders are booked in turnover statistics.
-   Orders based on complaints are only booked in turnover statistics. A reason for the complaint has to be entered for this purpose.

> **Example**
> A customer complains about an order. The operator enters a complaint order of the document type **Complaint** without a reason for the complaint. An invoice will be issued for the complaint order; it is booked in statistics like a standard order.
>
> If the complaint is justified, a complaint credit note will be issued as a third document (credit note of the document type **Complaint** and reason for complaint). This document corrects turnover statistics by the corresponding sales price (cost and surface remain unchanged); unlike the standard booking, positive amounts will be booked in complaint statistics.
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

### Document archiving without items
Documents can be archived even if they contain no items.

-   Documents without items will not be archived.
-   Documents without items will also be archived.

### Complaint statistics for credit notes

**Entry of complaint cause obligatory**
When a complaint is entered, both the place and complaint and the cause of complaint can be defined.

-   Generally, input of the complaint cause is optional.
-   The document cannot be saved if no cause of complaint has been entered.
    ⇨ Software Reference, "Complaint Cause" on page B-574

### Default complaint place
The place of complaint can be entered for statistical purposes. If there are several places of complaint, one of them can be used as a default.

-   Usually, no default place of complaint is set.
-   You can choose the most frequently stated place of complaint as default. This can be changed in the document.

### Document settings
The settings in this area are valid for the selected document type.

**Document type**
Choose the document type for which you are going to set automatic options in the following fields. The settings can differ for the individual document types.
⇨ Sales, "Transfer to Archives" on page C-684

### Automatic options
The settings in the following fields refer to the document type selected in field **Document type**. This means that you can enter different archiving settings for every document type.

Usually, documents are transferred to both statistics and archives at (automatic) archiving, and will then be deleted from the main database. Generally, transfer to statistics is based on the month in which the document was issued while archiving is based on the year.

> **Settings for transfer to archives**
> Document management allows to set the details for automatic transfer to archives.
> Documents can also be transferred to archives by hand.
> ⇨ Sales, "Transfer to Archives" on page C-684

**Transfer to commission statistics**
This checkbox refers to module **Sales commission**.

-   Data are not transferred to commission statistics.
-   Automatic archiving will also transfer the data to commission statistics.
    With this settings, you should also check the field **Process complaints in sales commission** in section **Global settings**.

**Transfer to turnover statistics**
This checkbox refers to the module **Turnover statistics**.

-   Data will not be transferred to turnover statistics.
-   Automatic archiving will also transfer the data to turnover statistics.
    With these settings, you should also check the field **Complaint w/o quantities ...** in section **Global settings**.

**Transfer to archives**
This checkbox refers to the module **Document archiving**. Archives are set up by year. At the change of year, the system archives the documents in the old or in the new archives, based on the invoice date.

-   Documents will not be archived automatically. Documents can be transferred to archives by hand however.
-   Documents will be archived automatically. Enter the archiving year as well.
    With this setting you should also check the checkbox **Delete document**.

**Delete document**
Documents should be deleted from the main database in regular intervals in order to keep its size at bay.

-   Documents will not be automatically deleted upon archiving.
-   Documents will be deleted from the main database after transfer to archives.

> **Relieve main database**
> Delete the archived documents from the main database. This will relieve your database and will improve its speed. Archived documents can be retrieved from archives any time.

### Archiving mode
The settings in the following fields refer to the document type selected in field **Document type**. You can enter different archiving settings for every document type. Choose an option to define the mode:

-   **Minimum status:**
    Status from which on documents should be archived automatically. Status **820-Auto. archiving** is selected by default for automatic archiving.
-   **Document older than x days:**
    If automatic archiving should depend on the document date, you can enter the number of days that have to elapse after the given date before the document can be archived.
-   **Status + document older than:**
    With these settings, both criteria must be fulfilled: The corresponding status must be reached and the document has to have reached the defined age.

### A+W Production

**Path for report file**
File in which the report file should be saved. It includes the list of orders archived in A+W Business. A+W Production uses this information for deleting the corresponding orders from its system.

**Order area for batch number**
The batch numbers are only analyzed for the defined order area. The batch number is selected from the corresponding number range in dialog **Number ranges** in field **Alcim archives batch number**.
⇨ "Number Ranges - Production" on page B-894

**Version**
If different versions have been defined for an order area, you can choose the current one.

## Company Data – Daily Closing
**Master Data > Company > Company Data > Daily Closing tab**

Enter the deadlines after which files are finally deleted from the main database.

### Storage days
The following fields serve to enter the number of days for which data should be saved in the main database for statistics and backup purposes before they are automatically deleted for good. This helps to keep the database small and fast.

All data older than the defined number of days will be deleted. This does not include the archived data.

**Statistics**
To create annual overviews you should enter more than 365 days to have ample time for creating the reports.
⇨ Statistics, "Purchasing Statistics" on page F-44
⇨ Statistics, "Turnover Purchase Statistics" on page F-44

**Commission statistics**
Long periods allow to analyze the commission for several years.
⇨ Statistics, "Commission Statistics" on page F-54

**Time management**
Long periods allow to analyze time management statistics for several years.
⇨ Capacity Planning, "Statistics" on page H-267

**EDI backup file**
Backup files for interfaces are practical until data processing has been successfully completed by the connected programs.
⇨ "Interface service" on page B-1027

**History entries**
Number of days for which a document history will be saved.

**Order information**
You should choose a longer saving time for analysis purposes.
⇨ Statistics, "Order Information" on page F-10

**Stock logbook**
Inventory history shows the goods received and withdrawn, purchase orders, etc. You can keep this list at bay by deleting the entries after a reasonable time.
⇨ Inventory Management, “Stock History" on page G-204

**Rack history**
You should choose a longer saving time for analysis purposes.

**Credit limit snapshots**
Credit limit snapshots can be used for analyzing the development of certain financial data for a customer within a defined period.
⇨ "Credit Limit Analysis" on page B-844

**OderXML data records**
You should choose a longer saving time for analysis purposes.

### System logbook

**Age of entries when deleted**
Number of days for which an entry should be saved in the logbook before it is automatically deleted for good.

**Archives path/name**
Directory and name of logbook archives.

## Company Data > System
**Master Data > Company > Company data > System tab**

This tab serves to adjust the measurement system, lead days for production, the transfer to A+W Production, and time management.

### Units of measurement
The measurement system does not have to be the same for the two areas.

**Database metric, imperial**
Unit of measurement to be used by default. You can enter your documents based on metric (=cm) or imperial measures (=Inch).

**Thickness metric, imperial**
Although you may usually enter sizes in inch, it may be necessary to enter the thickness in mm.

> **Choose measurement system by customer**
> You can change the predefined measurement system by customer. In this case, the measures will be converted in the customer-bound documents.

**Size precision = 1/**
If imperial measurements are activated for the database, enter **32, 64** or **128** in this field, depending on the factor to be used for calculation.
If you are using metric sizes, enter **1** in field **Size accuracy**.

**Metric digits after colon**
Number of places after the decimal point of the circumscribed rectangle for shapes if the measurement system is set to metric.

### Formats

**Date**
Display the date as:
-   dd.MM.yyy
-   MM.dd.yyyy
-   MM/dd/yyyy
-   yyyy-MM-dd
(d = day, M = month, y = year)

**Time**
Display the time as:
-   hh:mm
-   hh:mm AMPM (English 24 hour format)
-   hhhh/mm/ss
-   hhhh-mm-ss
(h = hour, m = minute, s = second)

**French keyboard support (. to ,)**
On keyboards with a French layout, the decimal separator on the number block is a dot. In the country settings for the operating system, however, the comma is entered as decimal separator.

-   The decimal separator matches the settings in the operating system (Windows country settings).
-   The decimal separator is converted:
    -   For countries using the colon as a decimal separator, dots will be changed into colons.
    -   For countries using the dot as a decimal separator, colons will be changed into dots.
When the Caps Lock key is active, the decimal separator of the numeric keypad is redirected to the dot.

### Customer version

**Producer, Trade**
Depending on the setting, the document header will show different fields for the dates. Calculation of dates is based on the settings in section **Lead days**.
Based on these options, you should fill in the fields **Start of production** and **Supplier's delivery** in section **Lead days** (see below).

**Code**
The customer code is used to check which parts will be enabled in this A+W Business installation.

> **Changing the customer code**
> If you change the customer code, you will lose access to the functions specially developed for your company.

**Edition**
If different editions of A+W Business are available, the version matching the customer code will be displayed. This is usually the standard edition however.

### Lead days
The fields in this area refer to the fields in section **Customer version**. The lead days can be changed at order entry.
The tutorial offers examples for scheduling of dates (customer's delivery date, shipping date, start of production, etc.) in the order header.
⇨ Tutorial 1, "Delivery Time" on page B-121

**Start of production**
Number of days to be deducted by default from the shipping date shown in the order header in order to determine the start of production.
This detail is required if you have selected the option **Producer** in section **Customer version**.
Start of production = shipping date - Start of production

**Production LG**
Number of days to be deducted by default from the shipping date shown in the order header in order to determine the start of production for laminated glass.
This field is displayed only if you have chosen **Producer** for the customer version.

**Delivery from supplier**
Number of days to be deducted by default from the start of production shown in the order header in order to determine the date for the supplier's delivery.
This field is displayed only if you have selected **Trade** for the customer version.
Supplier's delivery date = Start of production – Supplier's delivery

### Lead days for resubmission

**(Document)**
Selection whether quotations or orders are checked for resubmission.

**(Days)**
Enter the number of days after which the system should automatically remind you of following up a quotation.
When you enter a new quotation, the resubmission date is automatically determined based on the input date and the days defined here.

### Settings

**Use Windows registration for A+W Business login**
This setting is valid for all users. It cannot be linked with certain users.

-   A+W Business can be started only by separate registration.
-   After the Windows registration, A+W Business can be started without an additional registration (SSO: Single Sign On). User name and password have to be identical for this purpose.
A client-/server installation also requires input of the domain.

**Customizing activated**
This setting refers to customized amendments.

-   A+W Business can be used in the version installed.
-   Additional forms, variables, or fields can be used. If you do not need those, you should uncheck the checkbox to relieve your database.

**Enable Exchange Service for Workflow**
For the execution of workflows and the processing of production reports, the new A+W Commercial Exchange Service is now available. It replaces the A+W Business 6 Interface Service.

-   The A+W Commercial Exchange Service is not supported.
-   The A+W Commercial Exchange Service is used.

**openTrans Export in Thread**
Number of openTrans transfers per export process.

### A+W CAD Designer (Shapes)

**View**
View for the SN file:
-   **End product (sketch):** This is the standard setting if you are using the SN-Editor.
-   **Edgework (sketch):** With this setting, only the edgework will be shown.

**Color depth**
Color setting for displaying SN files:
-   **1 Bit:** This setting is used for line drawings. The display is monochrome.
-   **4 Bit:** This setting means that 16 colors or shades of grey can be displayed.
-   **8 Bit:** This is the standard setting. Up to 256 colors can be displayed with this setting.

**lite background**
This setting refers to the display of the sketch.
-   **Filled:** The lite appears as a colored area.
-   **Unfilled:** Only the outline of the lite is shown.

**Pattern size, segment text, sizes**
Size in which the SN file is displayed at item entry. Standard settings:
-   Pattern size: 12 px
-   Segment text: 14 px
-   Sizes: 16 px

**File path**
Storage place for the SN file. For the transfer to production, this directory must be known to A+W Production. To be on the safe side, always start the path with a double backslash and enter the complete address (IP).

**Only processings broken down in the production BOM**
The production BOM breakdown for processing steps can be adopted from the SN file. Production BOM breakdowns from macros will always be adopted.

-   The entire production BOM breakdown will be adopted.
-   Only the production BOM breakdown for processing steps will be adopted.

**In case of structural changes**
The SN files are regenerated after changes. This function only makes sense for structural changes.

-   With each change, a new SN file is generated. This also affects changes that are not production-relevant.
-   Only for structural changes is a new SN file generated, e.g. if the dimensions were changed.

**Edge processings and drillings on shape 99**
Edge processings and drillings can be applied to free shapes and imported SN files.

-   With the shape 99, no additional processings can be entered in the associated SN file.
-   The edge processings and drillings are saved in the SN drawing.

This function only refers to the dimension type **circumscribed rectangle** and to the program version 6 of A+W CAD Designer (Shapes).
With a free shape (shape 99), edge processings cannot be applied selectively, but rather only on all edges. Drillings can only be dimensioned with reference to the circumscribing rectangle.
If during import of the SN files into A+W Business there is a change to a standard shape, edge processings on individual edges can be entered if there is an edge numbering (1, 2, 3, 4) in the SN or DFXfile.

### URL for AWSOA services
Specification of the A+W SOA service. With this service, among other things, capacity overviews from A+W Capacity Planner (EL) can be imported, in order to view the free and occupied capacities.

### Customer logo
Path for the files containing the customer logos. The customer logo is defined in dialog **Logo position**.
⇨ "Logo" on page B-842

### Path for product images
Path for the directory containing the product images assigned to a product. These images will be used for the printing of forms.
⇨ "Article Sketch" on page B-595

### Replication
Replication means that master data are copied from the headquarters' database to the subsidiaries' databases.
The replication is started in module **Utilities > Replication management**.

**Replication recipient**
You will need this function only if you have several subsidiaries with separate databases.

-   This checkbox must not be checked at headquarters.
-   This checkbox must be checked in the subsidiaries. This will lock all master data fields that are maintained in the main database.

**Language**
Dialog **Replication** shows the descriptions in tables and fields in the selected language.

### Database parameters

**Isolation level**
The transaction mode of the database can be changed:
-   **RL:** Release Lock (restrictive transaction mode). This is the setting for the older versions of A+W Business.
-   **RC:** Read Committed (restrictive transaction mode). This setting increases the performance. It will be adopted for all terminals after the system is rebooted.

### A+W CAD Designer (Bars)

**Show clear field sizes**
For grill patterns, the clear sizes of the fields can be displayed.

-   The clear sizes of the fields will not be shown.
-   The sizes of the glass without the grill width (clear fields) will be displayed.

**Sum up grill quantities from macros**
Prices can be adopted from A+W CAD Designer (Bars) macros.

-   Prices will not be adopted.
-   The prices from A+W CAD Designer (Bars) will be adopted and added to the existing quantities. If e.g. a sun consisting of three fields is added, the extra fields will be added to number of fields.
