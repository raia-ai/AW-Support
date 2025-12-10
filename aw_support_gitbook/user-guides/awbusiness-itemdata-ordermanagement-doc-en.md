---
title: "EN_AWBusiness_Sales_4_6-1"
source: "EN_AWBusiness_Sales_4_6-1.pdf"
tags: ["A+W Business Sales", "Software Reference", "Item Data", "Order Management", "Document Search", "CEKAL", "Complaint Management", "Technical Values"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for A+W Business Sales, focusing on item data management within orders. It covers functionalities such as handling complaints, product groups, spacers, technical values, attachments, and detailed item settings."
long_description: "This comprehensive software reference manual provides detailed instructions and explanations for managing 'Item Data' within the A+W Business Sales application. It begins by detailing fields like the CE flag for CPIP codes and the process for managing complaints, including causes, reasons, and sales prices for returned items. The guide then covers various item-specific settings, including cutbacks, miscellaneous options like alternative items and cash discountability, and manual settings for weight, quantity, and rounding. A significant portion is dedicated to the 'Further details' tab, explaining fields related to production, CEKAL-specific data (for the French market), shipping, costs, and printing sketches. It also describes how to add and manage text blocks, file attachments, and technical values for items, including declarations of performance. The document further explains how to use classifiers for products and provides a thorough breakdown of the 'Totals' tab, which summarizes technical parameters, costs, contribution margins, credit limits, and total order values. Finally, it provides an in-depth guide to the 'Search Document' functionality, detailing how to use order-related, item-related, BOM-related, and other criteria to find documents in the main database or archives."
---

---
## Item Data

> **i**
>
> **CE flag**: The search for the CPIP code and for restrictions is loaded from the product definition and can be disabled in the order.
> - The search for the CPIP code and for restrictions is disabled. It cannot be reactivated. To reactivate this function, enter the product in a new item and delete the old item.
> - The setting is loaded from product management. If no CPIP check has been defined for the product entered, this function cannot be executed.

### Complaint
These fields are only available if you have entered or are processing a complaint.
You can enter the cause, a reason, and the sales price for every item returned. These details can be analyzed in complaint statistics.

**Open the Complaints dialog**
To fill in the fields, open the Complaints dialog using the [Directory] button.
⇨ Tutorial, "Complaints" on page C-278
⇨ "Complaints" on page C-586

**Cause**: This cause can be used for statistical analysis. Input is optional.
**SA Sales price of the returned item**: In cases of goodwill, this can be lower than the actual price.
**Reason**: The reason can be used for the statistical analysis of complaints. Input is optional.

### Product groups
**Discounts, Statistics**: Product groups from the product master data and PGR combinations. The setting applies to the selected item.
⇨ Master Data, "Rules for PGR Combinations" on page B-144

### Spacer
**Text**: This field is only available for products of the product group IG. You can enter an alternative spacer text to be transferred to production.
If you are using CEKAL, the CEKAL details are loaded from the product definition.

### Cutback
The cutback that has to be taken into account when cutting the lite is shown in mm. It can be changed. The values are transferred to the corresponding fields in Cutback in the Grills tab.
⇨ "Items - Grills" on page C-488

### Miscellaneous
**Alternative for item**: This field is intended for quotations. With it, you can define for which item the selected item is offered as an alternative.
⇨ Tutorial, "Enter Alternative Items in a Quotation" on page C-327

**Cash discountable**: This setting is adopted from the product definition. It can be changed. The setting applies to the selected item.
- The selected item will not be considered for cash discount calculation.
- The selected item will be considered for cash discount calculation.

**Packing unit**: The packing unit is transferred to the P.O. and production and can be printed.

### Manual settings
**Weight p.pc.**: Weight per piece of the current item. This entry can be changed. This information is used to calculate the energy surcharge.
⇨ Master Data, "Do not calculate energy surcharge by item weight" on page B-950

**Partial del. qty**: The original order shows the quantity already shipped as a partial delivery for the current item. This field remains empty in all other documents.

**Min. qty.**: Specify the minimum quantity in case this differs from the customized or company-wide settings. The entry applies to the current item.

**Size rounding**: Specify the measurement rounding in case this differs from the customized or company-wide settings. The entry applies to the current item.
⇨ Master Data, "Commercial size rounding" on page B-948
⇨ Master Data, "Standard rounding" on page B-764

### Items
The fields are described in connection with the Item tab.
⇨ "Items" on page C-452

## Items - Further details

> Documents > Order > Select order > Items > Further details tab

*(Fig. C-260 Items - Further details shows the user interface for this tab.)*

Use this tab to enter more details on spacer text, stock management, dispatch, and the calculation of costs and commission. The settings apply to the selected item.

### Text
The fields in this section refer to the CEKAL details if the CEKAL function has been enabled (only in France).

**Items group**: Number of the selected item. If several items have been compiled in a group, this is the group number.

**Serial item**: The present item may belong to a series.
- The present item does not belong to a series.
- The present item belongs to a series.

**Item text 1-5**: The texts for the current item are adopted from the master data. They can be changed and completed for this order. The texts are then transferred to production.
The Item text 5 field shows the entry for the surcharge basis.
⇨ "Surcharge basis" on page C-505

**CEKAL label**: Text to be printed on the CEKAL label. It is adopted from the master data and can be changed if required.
⇨ Master Data, "Product Texts" on page B-1077

**CEKAL general**: General text for CEKAL orders. It is adopted from the master data and can be changed if required.

**CEKAL production**: Text to be transferred to production for CEKAL orders. It is adopted from the master data and can be changed if required.

### Production
**Production line**: Defines on which production line the item will be produced. This information can be transferred to production.

**Label logo**: Number of the logo from the customer master data. The setting can be changed for this order.
⇨ Master Data, "Production labels" on page B-785

**Autom. cutting**: Information from the product master data. It will be forwarded to A+W Production. The setting can be changed for this order.
- The lite will not be cut automatically. It must be cut manually.
- The lite will be cut automatically.
⇨ Master Data, "Product Codes" on page B-608

**Edge stripping**: Edge stripping is added as a processing step.
- The edges of these lites will not be stripped.
- The edges of these lites will be stripped.
⇨ "Edge stripping" on page C-475

### Differing quantities
**Surplus/shortfall**: Allowed surpluses and shortfalls from the product master data. These values can be changed for each order.
Surpluses from A+W Production can be accepted if feedback without files is received.
⇨ Master Data, "Product Management - Production" on page B-596
⇨ Production, "Surplus" on page E-76

### Rack
**Type / quantity**: Rack type and number of racks onto which the item will be packed.
⇨ Master Data, "Product Management - Production" on page B-596

### Surcharge
**Surcharge basis**: If an automatic surcharge is calculated for the current order, this field shows the value that is used as a calculation basis, e. g. the weight.
⇨ "Automatic Surcharges" on page B-324

### Costs
Cost type and cost centers are defined in the product master data. The data can be analyzed by means of external reports.
⇨ Master Data, "Cost Accounting" on page B-602

**Cost center**: Cost center to which the product is posted.
⇨ Master Data, "Cost Centers" on page B-913

**Cost type**: Cost type to which the product is posted.
⇨ Master Data, "Cost Mode" on page B-912

### Shipment
The details in this section can be printed on the delivery note. The selection in the fields is defined in the Production module.
⇨ "Consignment" on page E-228

**Unloading point**: Standard unloading point at the customer's location. It can be changed for the current order.

**Packing rule**: Standard packing rule for this customer. It can be changed for the current order.

**Group creation**: Standard rack group for this customer. It can be changed for the current order.

### Print sketches
By default, details for the printing of sketches are loaded from the master data of the products.
⇨ Tutorial, "Printing Sketches" on page C-192

> **i**
>
> **Settings for printing sketches**
> You can set the printing of sketches for each item in various dialogs. If you change the setting, all corresponding fields will be updated.
> The printout can be adapted by means of the S+N-Editor, e. g. if the sizes are not clearly legible.

**Shape / grill**: Setting that defines how the sketch will be printed on the forms:
- **No printout:** Sketches will not be printed on the forms.
- **True to scale:** True-to-scale sketches will be printed.
- **Schematic:** Standard sketches will be printed. They only show the scheme of the shape or grill pattern, not the sizes.

These settings will be analyzed based on the settings made for the printing of forms.
⇨ Master Data, "Form Management - Sketch Printing" on page B-1058

### Document references
**P.O. reference, Delivery order, Customer number / item**: You can enter a reference to the P.O., the order, and the customer for every item. This reference can be alpha-numerical, and can be completed by the item number from the reference document.

### Commission
Details for commission are adopted from the product master data. The settings in the company data define how the commission will be calculated.
⇨ Master Data, "Interactive sales commission" on page B-937

**Rate 1 / 2**: The defined commission rate is only displayed if interactive sales commission has been enabled in the company data.
You can enter two different commission rates per item. These will be allocated to salesman 1 and salesman 2 respectively.
⇨ Master Data, "Sales Commission" on page B-376

### Items
The fields are described in connection with the Item tab.
⇨ "Items" on page C-452

## Items - Text

> Documents > Order > Select order > Items > Text tab

*(Fig. C-261 Items - Text shows the user interface for this tab.)*

Use this tab to enter text for the individual order items.
The settings always apply to the selected item. You can use the navigation buttons to scroll through the items.
⇨ Tutorial, "Enter text" on page C-52

### Block overview
You can add text by selecting a stored standard text or entering new text.
- The `+` field is released by means of the button.
- Inserted text is completely removed by means of the `-` button.

**Number**: Text number of the standard text. If you add your own text, enter the number 0 (zero).
⇨ Master Data, "Text" on page B-1040

**Text code**: The text code defines the document type for which the text is valid. Text with text code P for example will only be printed on production papers. In Management of forms you can exclude text from being printed on certain forms.
⇨ Master Data, "Text Types" on page B-461
⇨ Master Data, "Form Management - Text" on page B-1050

**Before, After item, Product referenced**: Use this option to define where the text should be printed in the document. The settings always refer to the selected item.
In the case of several texts per item, the settings only apply to the text that has been selected in the overview of allocated texts.
The following information is printed:
- **Before item:** In front of the product name.
- **Product referenced:** In front of the item line with dimensions.
- **After item:** After the item line with dimensions.

The standard option can be set in the Options menu > Positioning of text.
⇨ "Options menu" on page C-441

**(Overview)**: The table shows all the texts to be printed in this document. The checkbox After shows the option that has been selected for adding the text.

### Text block
**Keep text**: This checkbox is only available if text is added.
- The text is only added to the current item.
- The text is added to all items entered after the current item. It can be removed from every single item.

**Manual change**: This checkbox shows which texts have been added or changed manually. These texts cannot be translated for printing of forms. This checkbox is not ticked for standard texts.
- The standard text has been adopted without any changes.
- The text has been created manually, or standard text has been changed.

**Buttons**: You can change the font type and size and add hyperlinks, images and tables.
⇨ Tutorial, "Enter text" on page C-52

**Text field**: Click on the 'add text' button to release the text field. You can write directly into the text field to enter or change the text.

### POSITION
The fields are described in connection with the Item tab.
⇨ "Items" on page C-452

## Items - Attachments

> Documents > Order > Select order > Items > Attachment tab

*(Fig. C-262 Items - Attachments shows the user interface for this tab.)*

Use this tab to attach files and check which attachments have been saved together with the document. Attached files can be opened by double-clicking.
The attachment always applies to the selected item.
⇨ Tutorial, "Attaching documents" on page C-55

### File attachment
The file name and path are shown. You can add a note describing the attachment with each attachment.
Where the attachments are saved is defined in the company data.
⇨ Master Data, "File attachments" on page B-932

### Items
The fields are described in connection with the Item tab.
⇨ "Items" on page C-452

## Items - technical values

> Documents > Order > Select order > Items > Technical Values tab

*(Fig. C-263 Items - technical values shows the user interface for this tab.)*

On this tab, you can specify the technical values of a product. If the A+W SLT Interface is configured, the values are determined via the A+W SLT Interface.

### Technical data
**[Buttons]**: The buttons can be used to add or delete entries.

> **i**
>
> **Declaration of performance**
> It is possible to specify in the master data per customer and product whether a declaration of performance must be specified.

**Declaration of performance**: Number of the declaration of performance that should be assigned to the order. The number can be entered or selected via the button [magnifying glass] or [folder].
The number is generated automatically if the A+W SLT Interface is configured and the product structure is generated for the first time.

**[Calculator]**: The button is only enabled customer and/or product-specifically. With the button, you can have technical values calculated for the declaration of performance.

### Items
The fields are described in connection with the Item tab.
⇨ "Items" on page C-452

## Items - Classifiers

> Documents > Order > Select order > Items > Classifiers tab

*(Fig. C-264 Items - Classifiers shows the user interface for this tab.)*

On this tab, you can check and edit the classifiers of the product entered. The classifiers are also displayed if the product is a BOM component.
In the form printing and the document view, the classifiers can be transferred to the report.

### Items
The fields are described in connection with the Item tab.
⇨ "Items" on page C-452

## Document - Totals

> Documents > Order > Select order > Totals tab

*(Fig. C-265 Document - Totals shows the user interface for this tab.)*

Check the costs and the credit limit in this tab. The totals of the order and of technical values are displayed for your information. In addition, you can enter a fixed price for the total order.

### Totals (technical parameters)
This section shows the totals for surfaces, circumference, weight. The fields are blank if an order has been created but no items entered yet. The fields show the actual and rounded totals.

**Quantity. (Total/IG units)**: Displays the total quantity and number of IG units.

**Total surface (real / inv.)**: Shows the total surface calculated from the width and height. (Inv. = invoiced)
- The first value shows the actual total surface.
- The second value shows the total considering the settings for invoicing. If pricing is based on the surrounding rectangle and/or minimum quantities, different figures may be shown.

**Total circumference (real / inv.)**: Shows the total edge length calculated from the width and height.
- The first value shows the actual total edge length.
- The second value shows the total considering the settings for invoicing. If pricing is based on the surrounding rectangle and/or minimum quantities, different figures may be shown.

**Total weight (real / tare)**: Shows the total weight of the order and the weight of the packing material. The Tare field remains blank if no entries have been made for the packing material.

**Total length grills (real / inv.)**: Total length of all grills entered for this order.
- The first value shows the actual total grill length.
- The second value shows the total considering the settings for invoicing. If pricing is based on minimum quantities, different figures may be shown.

**Additional information**
⇨ Master Data, "Size rounding width/height" on page B-604
⇨ Master Data, "Commercial size rounding" on page B-948
⇨ Master Data, "Company Data > Price Calculation" on page B-944
⇨ "Size rounding" on page C-426

### Cost/Contribution margin
The costs and contribution margin is particularly of interest if predefined prices have been changed manually. In this display, the difference between the sales price and purchase price is the contribution margin.
If you are using the cost calculation module, the contribution margin will be based on the product prices.
The fields are blank if no items have been entered yet.

**Material cost**: Shows the material cost included in this order.
**Time cost**: Shows the time cost included in this order. These costs are only shown if the order has been transferred to and booked in capacity planning.

**DB% 1, 2**: The contribution margins are determined for material, time and freight costs.
- The first value shows the absolute value of the calculated contribution margin for this order.
- The second value shows the percentage value of the calculated contribution margin for this order.

**Freight costs**: The freight costs are calculated from the entry in the Distance field and the price per kilometer defined in the route master data. The distance is defined in the customer master data or amended in the Different addresses tab for the current order.
Use the button to open the overview on the imputed freight costs.
⇨ "Imputed Freight Costs" on page C-569

**Freight costs %**: The percentage of the freight costs refers to the total order value.

**Total cost**: Shows the total cost for all items included in this order.

**Fixed costs**: You can define a value for the fixed costs (purchase costs) for the entire order.

### Credit limit
The credit limit is automatically updated even if no receivables are reported by the financial accounting system. Orders are taken into account up to transfer to Financial Accounting.
Limit 1 specifies the insured amount and Limit 2 the uninsured amount.
Calculation of the balance is based on the settings made in the customer data.
The balance is calculated as follows:
Limit 1/2 - Receivables (FinAcc) - Liabilities - Orders = Balance 1/2
The values in the fields for Balance 1/2 are shown in red if the credit limit is exceeded.
⇨ Master Data, "Partner Management – Balance" on page B-778
⇨ Tutorial, "Credit limit" on page C-45

### Total value
The two columns in this section show the amounts in the national currency and in the foreign currency. The totals are updated automatically when changes are saved.

**Currency**: Shows the currency defined in the Terms tab.
⇨ "Currency" on page C-428

**Order total**: Shows the current totals calculated from the prices entered for the individual items. If you have entered a fixed price or discount, the prices will be recalculated when you save the order.

**Fixed price**: You can enter a fixed price for the entire order. The prices of the entered items will be recalculated proportionally when you save the fixed price. The price unit for all items is set to Pcs.

**% discount**: You can enter a discount for the total order value. The discounts for the items will be set to zero in this case. The item prices will be converted to unit prices.

> **i**
>
> **Amounts in red**
> The amounts for Order total, Net and Gross are shown in red just to highlight them.

**= Net**: Shows the calculated net value for this order.

**Tax rate**: You can change the rate defined in the master data for this order. All tax rates entered in the master data will be offered for selection.
If you change the tax rate for this order, A+W Business will check if collective invoices have been agreed for this customer. If so, a message is displayed with which you can recalculate the tax.
⇨ Master Data, "Tax" on page B-903

**Tax basis**: Shows the amount with which the tax is calculated.

**= Gross**: Shows the gross order value resulting from the order value and tax.

**Cash discount**: Shows the amount that can be deducted as cash discount. The percentage value for the cash discount calculation is defined in the payment terms entered for this customer.
⇨ Master Data, "Due date calculation" on page B-774
⇨ Master Data, "Discount calculation" on page B-781
⇨ Master Data, "Payment Conditions" on page B-905

**Down payment amount**: Shows the down payments paid. This field only shows an entry if down payments have been paid.
Open the Payment Management dialog with this button in order to enter a down payment.
⇨ Tutorial, "Enter Down Payment" on page C-273
⇨ "Payment Management" on page C-575

## Overviews and References concerning Header Data

> Documents > Quotation, order, credit note, inquiry, P.O. > Quotation, order, credit note, inquiry, P.O.

The document management menus can be used to display different types of information without having to close the dialog. Dialogs are the same for all document types. We are going to describe it in connection with an Order in this manual.

This chapter provides information on the following subjects:
- "Search Document" on page C-518
- "Copy Documents" on page C-527
- "Document View" on page C-543
- "Customer Info" on page C-544
- "Capacity Overview" on page C-545
- "History" on page C-547
- "Status Change" on page C-549
- "NM Selection" on page C-550
- "Packing Stock Sizes in Boxes" on page C-551
- "Overview Partial Deliveries" on page C-553
- "Complaint Overview" on page C-555
- "List of Down Payments" on page C-556
- "Order/P.O. Info" on page C-557
- "Duplicates" on page C-559
- "Customer Information (Delivery Date Check)" on page C-560
- "Capacity Information by Customer" on page C-565
- "Check Receivables" on page C-567
- "Imputed Freight Costs" on page C-569
- "Cost and Surcharge Calculation" on page C-570
- "Status Message Overview" on page C-571
- "Delivery Date Calculation" on page C-573
- "Edit Delivery Date" on page C-574
- "Payment Management" on page C-575

## Search Document

> Documents > Order > Search
> Documents > Order > Order > [Magnifier] at field Number

You can use various criteria to search for documents. The selected criteria are saved when you close the dialog and reloaded when it is reopened.
Document search is the same for all document types. The dialog is described in connection with an Order in this manual.
This dialog offers the following tabs:
- "Search documents – Order-related" on page C-519
- "Search documents – Item-related" on page C-520
- "Search documents – BOM-related" on page C-521
- "Search documents – Table" on page C-522
- "Search documents – Options" on page C-524
- "Search Documents – Details View" on page C-526

### Search group
> Documents > Order > Search > Start menu > Search group

The search can relate to the main database or the archives. You can select the following entries:
- **Main (F2):** Starts the search in the main database. Alternatively, you can also use the <F2> key.
- **Archive (Shift+F2):** Starts the archive search. Alternatively, you can also use the <Shift>+<F2> keys.
- **Search all (F3):** Starts the search in the main and archive database. The button is only enabled if you have ticked the Archive checkbox in the Options tab and have selected at least one archive. Alternatively, you can also use the <F3> key.
- **Delete values:** Resets the search criteria.

## Search documents – Order-related

> Documents > Order > Search > Order-related tab

*(Fig. C-266 Search documents - Order-related shows the user interface for this tab.)*

Use this tab to define search criteria relating to the document header. In order to expand or restrict the search to the archive databases, you can select the requested archive in the Options tab.

### Criteria from, to
The selection lists shows only those entries that relate to information on the order header.
The first entry is automatically repeated in the second field. Any number of criteria can be used to restrict the search.

**Search criterion (first field)**: Selection of the search criterion, e. g. date entered. The second field is enabled.

**Operator (second field)**: The following restrictions can be entered as a sequence or an exact value:
- **From-To:** Define a sequence with this setting. The `from` and `to` fields are enabled.
- **=:** With this setting the search is restricted to an exact value. The `to` field is locked.

**Customer**: A search is carried out to search for documents for a certain customer. The name and city will be imported from the customer data.
**Projects**: The search is carried out to search for documents for a certain project. The name is imported from the master data.

## Search documents – Item-related

> Documents > Order > Search > Item-related tab

*(Fig. C-267 Search documents – Item-related shows the user interface for this tab.)*

Use this tab to define search criteria referring to order items. You can use a combination of product number and sizes to search for orders with identical items.

### Criteria from, to
The selection lists only show those entries that relate to entries on items.
The fields are used in the same way as in the Order-related tab.
⇨ "Search documents - Order-related" on page C-519

**Product number, Product description**: The search is restricted to documents in which a certain product has been entered.

**Product type**: The search is restricted to documents in which a certain product type has been entered.

**Product group**: The search can be restricted to documents addressing a certain product group for discounts or statistics. The following entries are available:
- **Comb. disc..:** Combination product group for discounts.
- **Comb. stat.:** Combination product group for statistics.
- **Discount:** Product group discounts.
- **Statistics:** Product group for statistics.

## Search documents – BOM-related

> Documents > Order > Search > BOM-related tab

*(Fig. C-268 Search documents - BOM-related shows the user interface for this tab.)*

Use this tab to define search criteria referring to entries in the BOM.

### Criteria from, to
The selection lists only show those entries that relate to entries in the BOM.
The fields are used in the same way as in the Item-related tab.
⇨ "Search documents - Order-related" on page C-519

## Search documents – Table

> Documents > Order > Search > Table tab

*(Fig. C-269 Search documents – table shows the user interface for this tab.)*

This tab shows a hit list of the search result. The search criteria from all tabs are displayed as columns of the table.

### Table
This tab shows a hit list of the search result. The search criteria from all tabs are displayed as columns of the table.
- **No.:** Number of the document
- **Cust. / Supplier:** Name of the market partner.
- **Archives:** Archive year of the document.
- **Status:** Status number of the document.
- **Input Date:** Input date of the document.
- **Del. Note Date:** Date of the delivery note generation.
- **Shipping Date:** Shipping date of the document.
- **Invoice No.:** Invoice number of the document.
- **Invoice Date:** Invoice date of the document.
- **Reference:** Customer reference defined by the customer.
- **Route:** Route that is driven by the forwarding agency.
- **Net Amount:** Net price of the document.
- **Net Amount (FC):** Net price of the document in foreign currency.
- **Marginal Income (%):** Percentage of the marginal income.
- **Prod. Start:** (Latest) date on which the production must start.
- **LG:** (Latest) date on which the shipment must arrive.
- **Prod. End:** Date on which the production is completed.
- **Delivery:** Date of the requested delivery date to the customer.
- **Purch. Text 1, Purch. Text 2:** Additional information on the purchase order.
- **Batch Number Transfer to Production:** Batch number of the transfer to production.
- **Batch Number Production Report:** Batch number(s) of the production report(s).
- **Total Quantity:** Total quantity.
- **Total Sqm:** Total square meters.
- **Supplier(s):** Name of the supplier.
- **OC Supplier:** Number of the supplier's order confirmation.
- **Delivery Address:** Delivery address of the market partner.
- **Tel, Fax:** Contact data of the market partner.
- **Invoicing:** Number of invoice.
- **Payment Mode:** Payment mode agreed with the customer, e.g. invoice, cheque, bank transfer, etc.
- **Payment Terms:** Payment terms agreed with the customer.

## Search documents – Options

> Documents > Order > Search > Options tab

*(Fig. C-270 Search documents – Options shows the user interface for this tab.)*

Use this tab to select the archives in which you would like to run the search.

### Find in
Select an option to define the document type to be searched for, e. g. quotations.

**(Archiving year)** The search for documents can incorporate documents in the archive. You can limit the search to one or several archive years. Archived documents are displayed in red on the hit list.
- The archiving year will not be searched.
- The archiving year will be searched.

**[All]** The button selects all archive years for the search.

**[None]** The button selects no archive years. The search only relates to the main database.

**Show locked entries**: Documents with locked entries of a criterion can be shown, e. g. to search for a route that has been locked (in the meantime).
- Documents with locked criteria will not be displayed.
- Documents with locked criteria will be displayed. The criteria can be selected for the search.

**Observe capitalization**: Upper and lower case can be taken into account for search criteria that relate to text.
- Upper and lower case will not be taken into account. You should choose this setting if the names of products, customers, etc. do not follow uniform rules.
- Upper and lower case will be taken into account for the search.

**Display Documents in Archive Colored**: In the document search, the entries for archive documents can automatically be marked in color.
- The archive documents are marked in color.
- The archive documents are marked in red.

**Document Entry via Double Click**: You can open documents from the document search with a double-click.
- The marked document cannot be opened with a double-click. The document entry can be called up via the context menu.
- The marked document can be opened with a double-click.

### Sorting sequence
Select an option to define the sorting of the hit list entries in the Table tab:
- Ascending order numbers
- Descending order numbers
- Ascending entry dates
- Descending entry dates
