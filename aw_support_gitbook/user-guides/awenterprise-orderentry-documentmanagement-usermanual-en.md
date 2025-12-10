---
description: "EN-UM-AW_Enterprise-Sales_4_3"
---


---
## Order Entry – Miscellaneous
**Sales > Order Entry >Miscellaneous tab**

*Fig. D-33 Order Entry - Miscellaneous*

Use this tab to view complaint information, private fields, additional options, details regarding the delivery, and payment options. You can edit the entries.

### Header
The fields in the header area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

### Complaint Information
You can use this data to maintain complaint statistics. The **Reason**, **Place**, and **Type** of complaint must be created in the master data.

- **Reason**: Number of the complaint type. If you select a number, the name of the complaint type is displayed in plain text, e.g. glass break.
  - *Technical info: numeric field, DB field: kauf.reklamart*

- **Place**: Number of the complaint place. If you select a number, the name of the complaint place is displayed in plain text, e.g. unloading.
  - *Technical info: numeric field, DB field: kauf.reklamort*

- **Type**: Number of the complaint type. If you select a number, the name of the complaint type is displayed in plain text, e.g. incorrect color.
  - *Technical info: numeric field, DB field: kauf.reklamspec*

- **Date**: Complaint date in the format DD.MM.YYYY. By default, the current day is displayed. You can edit the complaint date.
  - *Technical info: date field, DB field: kauf.reklamdat*

### Payment Options

- **Curr. Rate**: Number and name of the currency and currency rate. The price is calculated customer-specifically in the currency specified. If you select a number, the currency name and currency rate are displayed in plain text. The Rate field is locked if Own Currency is selected.
  - *Technical info: mandatory field, numeric fields, DB fields: kauf.waehrung, kauf.kurs*

- **Calculate in**: This field is only enabled if Own Currency is not selected in the Currency field. You can specify whether the prices are calculated in own currency or in the market partner's foreign currency:
  - **Own Currency**: The prices are calculated by A+W Enterprise in own currency.
  - **Foreign Currency**: The prices are calculated in the currency that is assigned to the market partner in the Currency field.
  - *Technical info: toggle field, DB field: kauf.waerprs*

- **Print in**: Number for printing the market partner-specific documents in the calculated currency or foreign currency. If you select a number, the name of the print option is displayed in plain text. The appropriate report must be stored for the printing.
  - *Technical info: numeric field, DB field: kauf.waehrdru*

> **The fields Calculate in and Print in**
> The fields Calculate in and Print in are only accessible if the currency module is licensed.

- **Pay.Term**: Payment term in days, which has been agreed upon with the market partner.
  - *Technical info: numeric field, DB field: kauf.zahlziel*

- **Val.Date**: Period until the value date in days.
  - *Technical info: numeric field, DB field: kauf.valuta*
  > **Example:**
  > If an invoice is due on the 15th of a month, the entry of 2 days would result in the due date in Financial Accounting being extended by 2 days, i.e. until the 17th of the month. These days are taken into account for sending through the post, for example.

- **Cash D. 1, Cash D. 2, Cash D. 3**: Keys for the cash discount rates for the payment term. You can specify up to 3 different keys. This way, you can define scaled payment terms.
  - *Technical info: numeric fields, DB fields: kauf._skonto1, kauf._skonto2, kauf._skonto3*

- **Charact.**: Number of the form of payment, e.g. bank debit, bank booking. You store characteristics in the system master data as payment methods. If you specify a number, the name of the characteristic is displayed in plain text.
  - *Technical info: numeric field, DB field: kauf.zahlngmerk*

- **Payments**: Type and method of payment, e.g. upon delivery or by direct debit. The specifications for payment method are specified by the system.
  - *Technical info: toggle field, DB field: kauf.skontoart*

- **FIN. Key**: Key for transfer to financial accounting. The keys for financial accounting are entered by the system and sent to financial accounting.
  - *Technical info: alphanumeric field, DB field: kauf.fibukey*

- **FinAc Debitor**: Market partner's customer number, which is intended as invoice recipient. The field is pre-populated by default.
  - *Technical info: numeric field, DB field: kauf.stddebnr*

- **Bonus**: Bonus that a supplier grants its customer and that has been agreed for this document. The amount of the bonus is oriented according to the sales that are achieved with the customer within a specified period. The bonus is calculated as a percentage.
  - *Technical info: numeric field, DB field: kauf.bonusnr*

- **Commission**: Sales commission for this order. The commission is calculated as a percentage.
  - *Technical info: numeric field, DB field: kauf.provnr*

### Private Fields
The private fields are used customer-specifically for additional information. They can be configured at will. The field names are set via the environment variables. The two upper lines are numeric field; the two lower lines are free text fields.
- *Technical info: numeric fields, alphanumeric fields, DB fields: kauf.private_long1, kauf.private_long2, kauf.private_char1, kauf.private_char2*

### Additional options

- **Control**: Number of the employee who controls the document. If the field is filled, the documents will only be released after checking by the appropriate employee.
  - *Technical info: numeric field: DB field: kauf.kontrollmanr*

- **Wind Load**: Wind load in the installation location. Wind load (N/m²) is the pressure applied by direct winds onto the external surface of a building. The wind load can only be specified for glass with multiple lites.
  - *Technical info: numeric field, DB field: kauf.wlast*

> **Restriction check after input of wind load**
> If an appropriate entry is created for the wind load in the master data, the specified wind load is subjected to a restriction check. The system checks, e.g. whether the thickness group of the selected glass types suffice for the wind load defined. In case of violation of the restriction check, a message is displayed.

- **Facade Zone**: Specification of the facade zone in which the lites will be installed. E.g. tall buildings or buildings on the outskirts are loaded with increased wind load.
  - **1 Edge**: For buildings with increased wind load.
  - **2 Central**: For buildings without increased wind load.
  - *Technical info: numerical field, DB field: kauf.bereich*

- **min/max IG Tot.thickn.**: Minimum and maximum glass thickness for the entire IG article in millimeters. The glass thickness depends on the facade zone selected and the wind load.
  - *Technical info: numeric fields, DB fields: kauf.minszr, kauf.maxszr*

- **Tight Size**: Correction size in millimeters. The tight size added to the width and height of the items. For example, for a glass with the dimensions 1050 mm x 1250 mm and a tight size of 2 mm, the dimensions 1052 mm x 1252 mm are stored in the database. The value is transferred to production. If you are working with A+W Production, this value is generally ignored and the tight size is drawn from A+W Production.
  - *Technical info: numeric field, DB field: kauf.falzmass*

- **Text Formulas**: Number and description of the product labeling, e.g. spacer text. The text formulas must be created in the master data.
  - *Technical info: numeric field, DB field: kauf.artikennfrm*

- **Quot.Status**: Status of the quotation. This field is only shown for quotations. If referenced, this field content is transferred.
  - **open** = quotation has not yet been confirmed.
  - **confirmed** = quotation has been confirmed.
  - **rejected** = inquiry has been rejected.
  - **expired** = quotation is no longer valid.
  - *Technical info: toggle field, DB field: kauf.angbstatus*

### Shipping Details
These fields are pre-populated if the via site function is configured. With the via site function, deliveries to the customer via another site can be organized. For this, the internal site separation must also be active.

- **Arrival at Via Site**: Date on which the delivery will probably reach the site via which the delivery will be sent.
  - *Technical info: display field, DB field: kauf.ankunftvia*

- **Via Site**: Site number of the site via which the delivery will be sent. You can specify this target site in the header in the `Route` field with <F5>.
  - *Technical info: display field, DB field: kauf.vsvia*

- **Travel Time**: Estimated travel time to the target site. The travel time affects the delivery date.
  - *Technical info: display field, DB field: kauf.anfahrt*

- **Handl. Time**: Handling time to upload or unload the shipment.
  - *Technical info: display field, DB field: kauf.handlingvia*

- **Scheduled via**: Date of the planned delivery to the target site. The date specifies on which day the delivery will probably leave the target site.
  - *Technical info: display field, DB field: kauf.ltplanvia*

- **Route**: Route number. Delivery route to the customer. The route is different from the route in the starting site.
  - *Technical info: display field, DB field: kauf.endroutenr*

- **Arrival at Customer**: Date on which the delivery reaches the customer.
  - *Technical info: display field, DB field: kauf.ankunft*

- **Travel Time**: Estimated travel time to the customer's target site. The travel time affects the delivery date.
  - *Technical info: display field, DB field: kauf.anfahrtvia*

- **Goods Received on**: Date on which the delivery is received at goods receipt. The date is specified in the format DD.mm.YYYY.
  - *Technical info: date field, DB field: kauf.ptermin1*

### Footer
The fields and buttons in the footer area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85
You can only enter the fields if you have completed the order entry. Use `<End>` to change from the item level to the footer area.

## Order Entry - Totals
**Sales > Order Entry > Order footer > Discount Net Total fields > <F2>**

*Fig. D-34 Order Entry (Totals)*

On this dialog, you define discounts, rebates, and surcharges for the entire order and you can edit various payment options.
You can grant percentage, fixed discounts, and discounts per quantity unit and scale each discount according to quantity unit or order value. Depending on the discount type, the details will be calculated as price reduction or surcharge. If the system is configured appropriately, the discount will be drawn from the master data.
You must transmit the changes in the profit margin due to discounts to Financial Accounting. You can have the system automatically deliver the redistribution to Financial Accounting or deliver it manually. Manual delivery is described for the Discount Details tab.
⇨ "Order Entry - Detailed View Discounts" on page D-111

### Header

- **Order**: Display of the order number.
  - *Technical info: display field, DB field: kauf.auftrnr*
- **Customer**: Display of the customer number and name.
  - *Technical info: display field, DB field: kauf.kunr*
- **Sales**: Display of the total of the item prices.
  - *Technical info: display field, DB field: kauf.nettototal*
- **Costs**: Display of sum of the costs, e.g. purchase prices or production costs.
  - *Technical info: display field, DB field: kauf.ektotal*

### Detailed View Discounts
This area displays all order-specific discounts. You can check the surcharges and discounts, edit them, and grant new discounts for the order.

- **(Checkbox without name)**: Indicates whether discount is enabled:
  - ☑ The discount is calculated on the order price.
  - ☐ The discount will not be calculated.
  - *Technical info: checkbox, DB field: kaufrab.geloescht*
- **Name**: Name of the discount.
  - *Technical info: mandatory field, alphanumeric field, DB field: kaufrab.txt*
- **Seqnr**: Sequence number. The surcharges and discounts are calculated in the ascending order of the sequence numbers.
  - *Technical info: mandatory field, numeric field, DB field: kaufrab.seqnr*
- **Discount Value**: Specified calculation value of the discount. The calculation value depends on the discount selected.
  - *Technical info: numeric field, DB field: kaufrab.wert*
- **Type**: Specification of discount type. The discount type specifies whether the discount is a price reduction or surcharge:
  - **(-)**: The value is calculated as discount.
  - **(+)**: The value is calculated as surcharge.
  In the second field, you specify to what the discount applies:
  - **CU**: The discount is granted as fixed amount in the currency unit.
  - **%**: The discount is granted as a percentage of the total order value.
  - **CU/Pc**: The discount is granted as fixed amount in the currency unit per piece.
  - **CU/sqm**: The discount is granted per square meter of the total lite area in the currency unit.
  - **CU/kg**: The discount is granted per kilogram of the total weight in the currency unit.
  - **CU/km**: The discount is granted per kilometer of the total route in the currency unit.
  - *Technical info: toggle fields, DB fields: kaufrab.satzart, kaufrab.rabtyp*
- **Type**: Specification of the discount type. The discount type specifies to which price the discount refers:
  - **Sales**: The sales price is used to calculate the discount.
  - **Costs**: The total costs are used to calculate the discount.
  - *Technical info: toggle field, DB field: kaufrab.ekvkkz*
- **Prod. Group**: Identifier of the product group. If you specify an identifier, the discount is restricted to the corresponding product group.
  - *Technical info: alphanumeric field, DB field: kaufrab.wagrp*
- **Item**: Redistribution of the discount to the items.
  - ☑ The discount is redistributed to the individual items.
  - ☐ The discount is not redistributed.
  The redistribution is described in detail for the Discount Details tab:
  ⇨ "Order Entry - Detailed View Discounts" on page D-111
  - *Technical info: checkbox, DB field: kaufrab.verteil*
- **Sales**: Display of the discount in the selected line with the type Sales.
  - *Technical info: display field, DB field: kauf.nettototal*
- **Costs**: Display of the discount in the selected line with the type Costs.
  - *Technical info: display field, DB field: kauf.ektotal*

### Field descriptions
- **Margin, CU**: Display of the profit margin in currency unit and percent.
  - *Technical info: display fields, DB field: kauf.dbdm, kauf.dbvh*
- **Cash d.**: Number of the cash discount group. The cash discount group includes payment terms, e.g. the period in which the cash discount is granted and the cash discount rate. If you specify a number, the payment terms are displayed in plain text.
  - *Technical info: numeric field, DB field: kauf._skonto1*
- **VAT**: VAT rate. If several VAT rates have been defined for an order, the individual VAT rates are shown in % and as the currency unit. This is important for countries in which different VAT rates are being used. The fields are only displayed if the Multi checkbox is checked.
  - *Technical info: display field, DB fields: kauf.mwst, kauf.mwstbetrag, kauf.mwst1, kauf.mwstbetrag1, kauf.mwst2, kauf.mwstbetrag2, kauf.mwst3, kauf.mwstbetrag3, kauf.mwst4, kauf.mwstbetrag*
- **Min.inv.amount**: Minimum order value. If the net total value of the order is less than the minimum value, the minimum value is used as net total value. The difference is calculated as general surcharge.
  - *Technical info: numeric field, DB field: kauf._relimwert*
- **Print**: Selection for printing on the customer-specific forms.
  - **suppress**: No printing of discounts and rebates.
  - **only discounts**: Only the discounts are printed.
  - **only rebates**: Only the rebates are printed.
  - **Discount and rebate**: Discounts and rebates are printed.
  - **Minimum value**: The minimum value is printed. If the minimum value is used as net total value, this print option is selected. The option cannot be edited.
  - **free**: Currently not used.
  - *Technical info: toggle field, DB field: kauf.gesrnkz*
- **Mat. costs/Wage costs/Mach. costs**: Display of the total of costs of all order items.
  - *Technical info: display fields*

### (Calculation)
In this area, all discounts and surcharges are totalled with the prices and costs and the order amount is calculated. In the first field, the sales-side values are specified and in the second field, the cost-side values.

- **Total discount**: Display of the total of the discounts granted and surcharges.
  - *Technical info: display fields, DB fields: kauf.gesrab*
- **General discount**: Fixed amount that is deducted from the order total.
  - *Technical info: numeric fields, DB fields: kauf.gesrab, kauf.ekgesrab*
- **General surch.**: Fixed amount that is added to the order total, e.g. if the minimum order value is not yet reached or in case of special surcharges.
  - *Technical info: numeric fields, DB fields: kauf.sonderrab, kauf.eksonderrab*
- **Net total**: Total of all item prices, minus the discounts and plus the surcharges. You can edit the amount. The difference is displayed in the General Discount or General Surch. field.
  - *Technical info: numeric fields, DB fields: kauf.nettototal, kauf.ektotal*
- **Cash d.-able**: Total of the net amount and the VAT on which the cash discount is granted. The amount is calculated automatically and cannot be edited.
  - *Technical info: numeric field, DB field: kauf.skontierbar*
- **VAT**: Display of the VAT rate in percent and as amount. If several VAT rates are stored for an order, no percentage is displayed.
  - *Technical info: display fields, DB fields: kauf.mwstkz, kauf.mwstbetrag*
- **Cash d.**: Display of the cash discount rate and cash discount amount. The cash discount amount is calculated by the system.
  - *Technical info: display fields, DB fields: kauf.skvh1*
- **Gross**: Display of the gross total amount. The total amount is the sum of the net total amount and the VAT less the cash discount amount.
  - *Technical info: display field, DB field: kauf.gesbrutto*

### Footer
The fields and buttons in the footer area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

## Order Entry – Detailed View Discounts
**Sales > Order Entry > Order footer > Discount Net Total fields > <F2> > <F5> > <F5>**

*Fig. D-35 Detailed view Discounts*

Enter the details relating to the selected discount on this dialog. If the system is configured appropriately, the discount will be drawn from the master data. You can edit the entries order by order. The changes will not be taken over into the master data.

Some of the fields are described for the Order Entry (Totals) dialog:
⇨ "Order Entry - Totals" on page D-106

In addition, the following fields are displayed:

- **Active**: Specification whether the discount should be calculated.
  - ☑ The discount will be calculated.
  - ☐ The discount will not be considered.
  - *Technical info: checkbox, DB field: kaufrab.geloescht*

### Calculation
- **Sequen.**: Sequence number. The field corresponds to the Seqno. column on the Order Entry (Totals) dialog. The surcharges and discounts are calculated in the ascending order of the sequence numbers.
  - *Technical info: numeric field, DB field: kaufrab.seqnr*
- **Minimum value**: Minimum value of the discount. If the discount value is less than the minimum value, the minimum value is used for calculation.
  - *Technical info: numeric field, DB field: kaufrab.minbetrag*
- **Maximum value**: Maximum value of the discount. If the discount value is greater than the maximum value, the maximum value is used for calculation.
  - *Technical info: numeric field, DB field: kaufrab.maxbetrag*
- **Discount value**: Value of the discount and discount type. The field corresponds to the Discount Type column on the Order Entry (Totals) dialog. Use <F8> to calculate the values in the Amount (basic) field.
  - *Technical info: numeric field, toggle fields, DB fields: kaufrab.wert, kaufrab.satzart, kaufrab.rabtyp*
- **Method**: Display of the number of the discount method to which the discount value is assigned. The discount method is defined and assigned in the master data.
  - *Technical info: display field, DB field: kaufrab.methode*
- **Amount (basic)**: Display of the total discount amount. The basic value in parentheses specifies on which basic amount the discount is calculated. The fields depend on the discount type selected. Use <F8> to update the display, e.g. if you have changed the values in the Discount Value fields.
  - *Technical info: display fields, DB fields: kaufrab.betrag, kaufrab.grundwert*

### Redistribution
- **Redistribute**: Redistribution of the discount to the items. The field corresponds to the checkbox in the Item field on the Order Entry (Totals) dialog.
  - ☑ The discount is redistributed across the individual items and transferred to the FinAc. The Stat. Product Group, Cost Center, and Account fields are locked. The Method (Redistribution) field is enabled if CU is selected as discount type in the Discount Value field.
  - ☐ The discount is not redistributed.
  - *Technical info: checkbox, DB field: kaufrab.verteil*
- **Method (Redistribution)**: The method for redistribution specifies how the discount is redistributed across the items. The field is only enabled if the redistribution of the discount is active and CU is selected as discount type in the Discount Value field:
  - **by %**: The discount is redistributed by percentage according to the item price.
  - **by kg**: The discount is redistributed according to weight of the items.
  If in the Discount Value field CU is not selected as discount type, the discount is always redistributed across the item prices.
  - *Technical info: toggle field, DB field: kaufrab.verteil*

The following three fields are only enabled if the redistribution of the discount is not active:

- **Stat. Product Group**: Identifier of the statistical product group. The product group must be specified for statistics bookings.
  - *Technical info: mandatory field, alphanumeric field, DB field: kaufrab.statwagrp*
- **Cost Center**: Identifier of the cost center. The discount is booked to the specified cost center.
  - *Technical info: mandatory field, alphanumeric field, DB field: kaufrab.kstelle*
- **Account**: Description of the discount cost center booking account. You enter the account number in the master data.
  - *Technical info: alphanumeric field, DB field: kaufrab.konto*

### Configuration
- **Discountable**: Specification whether another discount can be calculated on the discount or surcharge.
  - ☑ The discount or surcharge is discountable.
  - ☐ The discount or surcharge is excluded from further discount.
  - *Technical info: checkbox, DB field: kaufrab.rabattierbar*
- **Cash D.-able**: Specification whether a cash discount can be calculated on the discount or surcharge.
  - ☑ Cash discount applicable to this discount or surcharge.
  - ☐ The discount or surcharge is excluded from further cash discount.
  - *Technical info: checkbox, DB field: kaufrab.skonto*
- **Zero item**: Specification whether items with an item amount of 0 are considered for discounts. the checkbox is not considered for items with the discount type CU or CU/km.
  - ☑ The zero items are considered in the discounting. The discount is redistributed across all items.
  - ☐ The zero items are excluded from the discounting. The discount is only redistributed across items with a price > 0.
  - *Technical info: checkbox, DB field: kaufrab.nullpositionen*
- **Delivery surcharge**: Specification whether a delivery surcharge will be assessed.
  - ☑ The delivery surcharge is calculated per day and per delivery address.
  - ☐ The delivery surcharge is not calculated.
  - *Technical info: checkbox, DB field: kaufrab.lieferzuschlag*
- **Glazing**: Specification whether the discount refers to glazing work. The field is only enabled is the discount type % is selected in the Discount Value field.
  - ☑ The discount is only granted on glazing items.
  - ☐ The discount is granted on the entire glass price.
  - *Technical info: checkbox, DB field: kaufrab.verglkz*
- **SP call - Item**: Specification whether the discounts should be calculated via the stored procedure. The stored procedure can be configured customer-specifically in the system. For additional information about the stored procedure, contact your A+W Software GmbH contact person.
  - ☑ Stored-Procedure call of discounts per item is active.
  - ☐ Stored-Procedure call of discounts per item is not active.
  - *Technical info: checkbox, DB field: kaufrab.spaufrufkz*
- **SP call - Process**: Specification whether the discounts should be called up per document via the stored procedure.
  - ☑ Stored procedure call of discounts per document is active.
  - ☐ Stored procedure call of discounts per document is not active.
  - *Technical info: checkbox, DB field: kaufrab.spaufrufkzkauf*
- **Min. Amount for Zero**: Specification of whether for a zero amount of the discount value the minimum value of the discount is calculated.
  - ☑ The minimum value is used for zero amount.
  - ☐ The minimum value is not used for zero amount.
  - *Technical info: checkbox, DB field: kaufrab.minbeinullbetragkz*
- **in Credit Note**: Specification whether the discount should be calculated for a credit.
  - **Yes**: The discount is considered in credits.
  - **No**: The discount does not apply for credits.
  - **Question**: During the creation of the credit, a query is displayed, asking whether the discount should be considered in the credit.
  - *Technical info: toggle field, DB field: kaufrab.gutschrift*
- **Glass weight**: Specification of to which glass weight the discount refers. The field is only enabled if CU/kg is selected as discount type of by kg is selected as method of redistribution.
  - **Item weight**: The discount applies for the weight of the item.
  - **Only gls wgt**: The discount applies only for the weight of the glass.
  - **Glass Weight**: The discount applies for the weight of the glass. If the glass weight equals 0, the item weight will be used for discount calculation.
  - **Inv. Item Wt**: The discount applies for the invoiced item weight.
  - **Only inv. gls wt**: The discount applies only for the invoiced glass weight.
  - **Inv. gls wt**: The discount applies for the invoiced glass weight. If the invoiced glass weight equals 0, the invoiced item weight is used for discount calculation.
  - *Technical info: checkbox, DB field: kaufrab.glasgewicht*
- **VAT**: Number of the VAT rate that is calculated on the discount. You can assign one or several tax rates to the discount.
  - Open the list of VAT rates with <F9>.
  - Use the arrow keys to navigate among the tax rates.
  - Use <Toggle> to mark a VAT rate.
  - Use <End> to close the dialog and take over the selection.
  - *Technical info: selection field, DB field: kaufrab.verteil*
- **openTRANS - ID**: Identification number for internal settlement between the individual sites, e.g. for subsequent discounts.
  - *Technical info: alphanumeric field, DB field: kaufrab.otrabattid*

### Partial invoices
- **Article**: Article number for the partial invoice from the payment plan. The field is pre-populated automatically if a payment plan is active.
  - *Technical info: numeric field, DB field: kaufrab.artnr*
- **Invoice no.**: Invoice number of the partial invoice from the payment plan. The field is pre-populated automatically if a payment plan is active.
  - *Technical info: display field, DB field: kauf.rechnr*

## Order Items
**Sales > Order Entry > Items tab**

The Items area offers the following tabs:
- "Order Entry – General" on page D-116
- "Order Entry – Properties" on page D-129
- "Order Entry - Prices" on page D-134
- "Order Items – Status" on page D-137
- "Order Entry - Costs" on page D-139

In the Items area, you compile customer products, determine the product structure, and specify the quantities.

### Order Entry – General
**Sales > Order Entry > Items tab > General tab**

*Fig. D-36 Order Entry - General*

In this area, you enter and edit the items of an order. You can select the articles, the dimensions, quantity, and type and assign processings to the articles.

For orders already entered, the item status of the marked item is displayed at the top of the tab, e.g. Delivered Local – Correction. The symbol of the item status and if necessary the item code are displayed in front of the Itm field.
⇨ "Explanation of Symbols" on page D-79

Generally you enter order items on the General tab. On the other tabs in the Items area, you can view additional information about the item properties and prices.

The article structure of an item originates from the BOM description and is copied from the article master into the document. You can adjust the BOM to the customer requests correspondingly.
- ⇨ "BOM View" on page D-198
- Use `<Enter>` to change to the next field, `<Page Up>` to jump to the first item, `<Page Down>` to jump to the last item.
- Use `<End>` to switch to the footer and conclude the order entry.

### Header
The fields in the header area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

### Items tab (left area)
In the info area, various information about the marked item is displayed. The technical values can be edited.
⇨ "Items tab (Info area - graphic, technical values)" on page D-119

*Fig. D-37 Items tab (info area left, example of technical values)*

This area displays information about the marked item. The information about the header article is always displayed. All other information is only displayed if it exists. If no information exists, the corresponding position remains empty.
- Use `<F2>` to change to the Addresses, Properties or Miscellaneous tabs.
  - ⇨ "Order entry - Addresses" on page D-92
  - ⇨ "Order Entry - Properties" on page D-95
  - ⇨ "Order Entry - Miscellaneous" on page D-101
- Use `<Enter>` to change to the General tab that is on the Items tab.
  - ⇨ "Order Entry - General" on page D-116

- **Ref.**: Reference text for printing. The text can exceed the label length that is displayed. If you enter a new item, the reference text of the previous item is taken over automatically. You can also enter an individual reference text for each item, e.g. in order to assign the items in an order to two construction sites via the reference text.
  - Use `<F4> > References > New Reference` or `Change Reference` to create a new reference text via the supplementary menu or to change the existing reference text for the entire order.
  - Use `<Shift>+<F11>` to change from the item level to the text entry for the reference in order to create a reference text for the selected item.
  - *Technical info: alphanumeric field, DB field: komm.kommtxt*

> **Inheriting reference text**
> If you assign a reference text to an item with `<Shift>+<F11>`, the reference text can be taken over for all following order items. For this, you have to confirm the query whether the reference should be inherited downward with [Yes]. If you click [No], the reference text is only taken over for the current item. The query is only displayed if additional order items are entered after the current item.

- **DoP:**: Declaration of performance. Description of the declaration of performance that is assigned to the article. The field is only displayed if a declaration of performance is assigned to the current article.
  - *Technical info: display field, DB field: kposp.lbrefnr*
- **(CAD identifier)**: Identifier that indicates whether a CAD file is assigned to the item. If a CAD file is attached, the CAD identifier is displayed. For S/N items, the S/N code is displayed in brackets next to the CAD identifier.
  - *Technical info: display field*
- **(Cost center)**: Designation of the cost center that is assigned to the item. If no cost center is assigned to the item, the market partner-specific cost center is used. If no cost center is assigned to the market partner, the main cost center will be used.
  - *Technical info: display field, DB field: kpos.kostenst*
- **(Muntin flag)**: Identifier that indicates whether muntins are entered in the item.
  - **S**: Muntins are entered in the item. The muntin structure was not edited.
  - **E**: Muntins are entered in the item. The muntin structure was edited in the editor.
  - **(no identifier)**: No muntins are entered in the item.
  - *Technical info: display field*
- **(Header, article)**: Description of the header article. With multiple glasses, in addition to the header article, the descriptions of the individual glasses are displayed.
  - *Technical info: display field, DB field: aufstrukt.artbez1*
- **(Exchange, additional article, quantity1/quantity2)**: Description of the exchange and additional articles and number of articles in the BOM. Exchange articles are displayed with an A, additional articles with a Z in front of the description. Next to the article description, it is indicated how frequently the value width and how often the value height must be calculated for the article.
  - *Technical info: display fields, DB fields: aufstrukt.artbez1, aufstrukt.anzahl1, aufstrukt.anzahl2*
- **(Muntin exchange, muntin additional article, quantity1/quantity2)**: Description of the muntin exchange and/or muntin additional article and number of muntins in the BOM. Muntin exchange articles are marked with an A, muntin additional articles with a Z in front of the description.
  - *Technical info: display fields, DB fields: aufstrukt.artbez1, aufstrukt.anzahl1, aufstrukt.anzahl2*

### Items tab (Info area - graphic, technical values)
On the right side of the Items tab, depending on the system configuration and the settings, some of the following information is displayed:
- product group and shape
- Technical values
- Hidden dimensions

The information is displayed for the marked item. Depending on the configuration, you can select which pieces of the information should be displayed.
- Use `<F4> > Product Details > Technical Details > Show Technical Details` to display the technical details in the area.
  - ⇨ "Technical details" on page D-122
- Use `<F4> > Product Details > Technical Details > Show Hidden Dimensions` to display the hidden dimensions in the area.
  - ⇨ "Hidden dimensions" on page D-123

*Fig. D-38 Items tab (info area)*

- A: product group
- B: Technical values declaration of performance
- C: Shape, product structure
- D: Technical values (display)

On the right, there is a schematic depiction of the product. If you have entered a shape and/or muntins in the item, a schematic product depiction is also displayed on the left.
⇨ "Graphic display of the item" on page D-124

- **(type)**: Description of the type. You select the type in the B.Art field. For the types Production, Stock Withdrawal or Included, a corresponding notice is displayed. For a PO, the supplier number is displayed.
  - Use `<Shift>+<F12>` to edit the supplier and delivery time of POs. If you specify a supplier for an item, the type for the item is automatically specified as PO.
  - *Technical info: display field, DB field: kpos.beschaffart*
- **Supplier**: Supplier number. The field is displayed if PO is selected as type of the item. If you specify a supplier number, the supplier's name is displayed in plain text on the next line.
  - Use `<Shift>+<F12>` to edit the supplier and delivery time of POs.
  - *Technical info: display field, DB field: kpos.liefnr*
- **Del. time**: Time for delivery in days. The field is only available if PO is selected as type of the item. The delivery time is drawn from the master data.
  - Use `<Shift>+<F12>` to edit the supplier and delivery time of POs.
  - *Technical info: display field, DB field: mp.liefzeit*
- **ProductGrp**: Product group number of the item. Articles are divided into product groups for product grouping and analysis in sales statistics. When you change the BOM of an item, the information for the product group is adjusted. The field is only available if Stock is selected as type of the item.
  - Use `<Ctrl>+<F9>` to change from the item level to the input field of the product group.
  - Use `<F9> > <F8>` to open the selection list for the product group. Alternatively, you can specify a product group number. A correction of the product group is possible, but only required in exceptional cases.
  - *Technical info: display field, DB field: kpos.wgrp*
- **Shape**: Shape number.
  - Use `<Ctrl>+<F12>` to change from the item level to the input field for the shape number.
  - Open the Shape Catalog with `<F2>`.
  - Open a selection of shape names with `<F9>`.
  Alternatively, you can enter the shape number directly in the field. After specifying a shape number, the shape entry begins. By default, the system is configured with the A+W shape catalog. For the configuration of a customer-specific shape catalog, contact your A+W Software GmbH contact person.
  ⇨ "Shape - Dimensions" on page D-180
  - *Technical info: display field, DB field: kpos.modnr*

### Technical details
- Use `<F4> > Product Details > Technical Details` to select one of the following entries on the additional menu:
  - **Show Technical Details**: Displays the technical details of the selected item. If the calculation of the technical values via A+W SLT in the system is configured, then the Calculate technical details tab opens.
    ⇨ "Order Entry - Calculated Technical Values" on page D-190
  - **Change technical details**: Changes to the input fields for the technical details of the selected item. You can edit the fields.
  - **Show hidden dimensions**: Displays the hidden dimensions of the selected item next to the graphic display of the item, e.g. the spacer deduction dimension. If you select Show hidden dimensions from the menu while these are displayed, then they are hidden again.
  - **Change hidden dimensions**: Opens the Item dimensions dialog where you can edit the various dimensions of the item.
    ⇨ "Article Dimensions" on page D-153

Depending on the item selected, various parameters are listed. Use [OK] or `<End>` to save the changes and close the dialog.

- **Pltm**: Item number of the selected item. The field is only displayed if you change the technical details.
  - *Technical info: display field, DB field: kpos.posnr*
- **Ug value DIN**: Heat transmission coefficient according to DIN standard. Central dimensional unit for determining the heat loss of a component. The measurement is W/m²K. The smaller the Ug value, the larger the heat insulation.
  - *Technical info: numeric field, DB field: ktechw.kwert*
- **Ug value**: Heat transmission coefficient.
  - *Technical info: numeric field, DB field: ktechw.kbazwert*
- **Transmiss.**: Light transmission for the percentage of rays that are allowed to pass through. The reference value of 100% is an unglazed hole in the wall.
  - *Technical info: numeric field, DB field: ktechw.trwert*
- **g value**: Energy transmission coefficient (total transmittance). The value is composed of the direct transmission of solar energy and of the secondary heat emission to the inside due to long wave radiation and convection.
  - *Technical info: numeric field, DB field: ktechw.gwert*
- **dB value**: Sound insulation value of the item in decibels.
  - *Technical info: numeric field, DB field: ktechw.dbwert*

If you edit the technical details, additional fields are displayed with `<F2>`.

- **Article Code**: Article code of the selected item. The field is only displayed if you change the technical details.
  - *Technical info: display field, DB field: ktechw.artnrgen*
- **Total thickn.**: Glass thickness for the total article of the item. The glass thickness depends on the facade zone and wind load selected. The entry is made in millimeters. The field is only displayed if you change the technical details.
  - *Technical info: numeric field, DB field: ktechw.dicke*
- **Wind load**: Wind load in the installation location. Wind load (N/m²) is the pressure applied by direct winds onto the external surface of a building. The system uses this value to perform a plausibility check to determine whether the thickness group of the selected glass types suffice for the wind load defined. The field is only displayed if you change the technical details.
  - *Technical info: numeric field, DB field: ktechw.wlast*
- **Section**: Specification of the facade zone in which the lites will be installed. E.g. tall buildings or buildings on the outskirts are loaded with increased wind load. The field is only displayed if you change the technical details.
  - **Edge**: For buildings with increased wind load.
  - **Central**: For buildings without increased wind load.
  - *Technical info: toggle field, DB field: ktechw.bereich*

### Hidden dimensions
- Use `<F4> > Product Details > Technical Details` to select one of the following entries on the additional menu:
  - **Show hidden dimensions**: Displays the hidden dimensions of the selected item next to the graphic display of the item, e.g. the spacer deduction dimension. If you select Show hidden dimensions from the menu while these are displayed, then they are hidden again.
  - **Change hidden dimensions**: Opens the Item dimensions dialog where you can edit the various dimensions of the item.

Depending on the item selected, various parameters are listed. Use [OK] or `<End>` to save the changes and close the dialog.

The fields are described in detail in connection with the Article-Dimensions dialog.
⇨ "Article Dimensions" on page D-153

### Graphic display of the item
Various previews are displayed for the item:

*Fig. D-39 Graphic display of the product (examples)*
(Image shows examples of Shape, Muntin pattern, Shape with muntin pattern, Shape with steps, IG with step)

- **Schematic product display**: Displays the shape, muntin pattern, and step for the item schematically. The schematic product display is only displayed if you have entered a shape and/or muntins in the item.
- **Schematic view**: Shows the lite structure as a cross-section. The sun marks the outside of the lite. The schematic structure of the item is always displayed.

### General tab
The fields on the General tab vary depending on the item that you select.

- **Itm**: Item number. Displayed in front of the Itm field, are the item status and if necessary the item code of the item in question. The item status is only displayed after saving the document. The status of the document is reported by production, the stock, and dispatch.
  - *Technical info: numeric field, DB field: kpos.Ifdpos*
- **Cu.Item**: Customer's item description. Specification of the item description from the customer's item list. The field is only enabled if the entry Itm is selected in the Cu.Item field of the header area. The item description can be printed on all customer and supplier-side documents.
  ⇨ "Order Entry - header, footer area" on page D-85
  Alternatively, you can enter the article name of an existing, fixed-size article. The system then pre-populates the fields with the article data.
  ⇨ "Article Details for Dimensioned Variants" on page D-164
  - *Technical info: numeric field, DB field: kpos.kuposnr*
- **Type**: Glass type of the item. The field is used customer-specifically and can be configured at will. The field is only displayed if in the Cust. Item field the entry Type is selected. The item designation can be printed on all customer and supplier-side documents.
  ⇨ "Order Entry - header, footer area" on page D-85
  - *Technical info: numeric field, DB field: kpos.kuposnr*
- **Article**: Article number. In the Article field you can enter a customer- or supplier-specific article number.
  - Use `<F9>` to open the article search.
  - Search for customer-specific articles with `<F10>`.
    ⇨ "Article Details for Dimensioned Variants" on page D-164
  - use `<Ctrl>+<L>` to open the Third-party data import dialog.
    ⇨ "External Data - Import" on page D-169
  - *Technical info: mandatory field, numeric field, DB field: kpos.artnr*

> **Letting BOM numbers be assigned**
> With the BMno, the system counts the various BOMs that are added to the order. Not the quantity of BOMs is counted, but how many BOMs there are with different structures. Each new item with a BOM structure that differs from the BOM structure in the already-entered items is assigned the next BMno numerically. If the same item is entered in different items, then these items have the same BMno since their BOM structure does not differ. If you add an article that is already entered in another item that has an identical BOM, you can also have it assigned a new BMno by the system:
> - With `<Shift>+<F5>` in the Article field, the article is assigned the next free BOM number by the system.
> - With `<F5>` in the Article field, you take over the article's original BOM. The BOM number is assigned by the system.

- **BMno**: BOM number of the article. The number is assigned by the system by default. The BOM includes all parts and processings required for manufacturing of the article. The BOM number depends on the BOM structure of the item in question. Items with the same BOM are assigned the same BOM number. The number is displayed in the SLNr field. If you change the BOM structure of an item, the BOM number is changed by the system if necessary. After the dimensions of the item were specified, you can use `<F5>` to display and edit the item's BOM.
  ⇨ "Item Processing" on page D-221
  - *Technical info: numeric field, DB field: kpos.poskonr*
- **Supplier**: Number of the box supplier. The field is only displayed if you have selected a box article.
  - *Technical info: mandatory field, numeric field, DB field: kposk.liliefnr*
- **Qty**: Item quantity. The item quantity depends on which article is entered, e.g. pieces, square meters. For articles with stored dimension, color or thickness variants, after entry of the quantity, a dialog opens for selection of the respective variant.
  ⇨ "Variant and Color/Thickness Selection" on page D-167
  If you enter a box article, you cannot specify a quantity. The system calculates the quantity and pre-populates the field if you specified the box and sheet number.
  With `<Ctrl>+<B>` the Properties tab opens and you can assign a CAD file to the selected item.
  ⇨ "CAD File" on page D-132
  - *Technical info: mandatory field, numeric field, DB field: kpos.menge*
- **Width, height**: Width and height of the item in millimeters. For variant articles, the system takes over the dimensions from the article master data. If you change the stock dimensions, the variant query appears: *Can the variant reference really be removed?*
  - Click on [No] to reset the entered sizes to the stock sizes.
  - Click [Yes] to change the stock sizes. This can cause problems in the warehouse and with pricing.
  - *Technical info: mandatory fields, numeric fields, DB fields: kpos.laenge, kpos.breite*
- **(Field without name)**: For length, time, and piece articles, instead of width, height, and AIR, the dimension and corresponding dimension unit that are assigned to the selected article are displayed. The dimension unit of the article is drawn from the master data and cannot be edited. For installation work, for example, the dimension unit hr (hours) is displayed, for gas fillings / (liters) and for adhesive tape m (meters). You can select the dimension at will.
  - *Technical info: mandatory field, numeric field, DB field: kpos.me*
- **AIR**: Airspace in millimeters.
  - *Technical info: mandatory field, numeric field, DB field: kpos.szr*

> **Calling up BOM of the item**
> Use `<F3>` or `<F5>` to open the BOM for the selected item. You can only open the BOM after you have specified the dimension. If you try to open the BOM before that, the system will notice this action and open the BOM automatically after specification of the dimension. In addition to the item, you will see a gray checkbox. A message with this information will also be displayed.

- **KA**: Box quantity. The system calculates the quantity from box quantity x number of sheets. The field is only displayed if you have selected a box article and the system is configured appropriately.
  - *Technical info: mandatory field, numeric field, DB field: kposk.kianz*
- **Sheet**: Number of sheets of glass per box. The system calculates the quantity from box quantity x number of sheets. The field is only displayed if you have selected a box article and the system is configured appropriately.
  - *Technical info: mandatory field, numeric field, DB field: kposk.blattanz*
- **VA**: Identifier for the packing type, e.g. 12 = box packing. The field is only displayed if you have selected a box article.
  - *Technical info: mandatory field, numeric field, DB field: kpos.verpackart*
- **Chamber thickness**: Thickness of the gel layer in the intermediate space for fire protection glass. The field is only displayed if you have selected a fire protection article, the information is stored in the master data and the system is configured appropriately.
  - *Technical info: numeric field, DB field: kpos.szr*
- **SN**: Indication of whether the item is assigned a SN file for the A+W CAD Designer (Shapes). For example, all processing activities that are executed fully automatically by the machine during the production process are defined in the SN file. In the CAD file field on the Properties tab, you can see the assigned files or assign a file manually.
  - ☑ A SN file is assigned to the item.
  - ☐ No SN file is assigned to the item.
  - *Technical info: checkbox, display field, DB field: kpos.brokefile*
- **Comm**: Commission with active representative commission calculation. You can specify the commission key granted for each item individually. With inactive or margin-oriented commission calculation, the field is locked and will not be considered.
  - *Technical info: numeric field, DB field: kpos.provnr*
- **SType**: The type determines how an article is supplied. By default, the types are taken over from the system from the article master data. The type that is assigned to the article in the master data at priority 1 is pre-populated in the document entry in the S.type field. Depending on the order, you can edit the field.
  - **Production**: The article will be produced.
  - **Included**: The article will be included by the customer, e.g. for further processing.
  - **not avail**: The article is not available.
  - **None**: No type, e.g. for services.
  - **P.O.**: Article has to be ordered from the supplier.
  - **Stock**: Article will be taken from stock.
  - *Technical info: Toggle field, database field: kpos.beschaffart*
- **Ibs/Pc, EUR/Qty**: Weight in pounds per piece, quantity unit in square meters per piece. If you change to the Price field, you can switch the display of the field Ibs/Pc, EUR/Qty with `<Ctrl>+<M>`.
  - *Technical info: display field, DB field: kpos.gewme*
- **Price field**: Net price per item. The field name varies depending on the own currency and configuration, e.g. Price/piece, Price/m2. The system calculates the total price of the item including the conditions in the selected currency. You determine the currency in the Currency/Rate field on the Miscellaneous tab.
  - Switch the display of the Price field using `<Shift> + <F11>`.
  - Mark the item as fixed dimension product using `<Shift>+<F8>`. If you save the order, the item is stored in the master data as fixed dimension product.
    ⇨ "Article Details for Dimensioned Variants" on page D-164
  - Use `<Ctrl>+<F9>` to determine the SA price with the item conditions and recalculate the price.
  - Use `<Shift>+<F9>` to open the Item Conditions dialog.
    ⇨ "Conditions for PCD Processing" on page D-283
  - Use `<Shift>+<F10>` to recalculate the item price.
  - Use `<F3>` to display an overview of the dimensions of the individual items.
    ⇨ "Dimensions of Individual BOM Elements" on page D-222
  - Use `<Ctrl>+<M>` to change the display of the field kg/St, ME/St.
  - *Technical info: numerical field, DB field: kpos.nstpreis*

The following fields display on the tab if you use `<F4> > Price info > Price check`:

- **aVK**: Pre-sales price code from the transferring site.
  - *Technical info: display field, DB field: kpos.vorvkpkz*
- **PCD**: Pre-sales price code from the transferring site.
  - *Technical info: display field, DB field: kpos.vorpkz*
- **nVK**: Newly determined sales price code.
  - *Technical info: display field, DB field: kpos.neuvkpkz*
- **aVF**: Pre-sales price code from the transferring site.
  - *Technical info: display field, DB field: kpos.vorvkfaktor*
- **Factor**: Percentage pre-sales factor from the transferring site.
  - *Technical info: display field, DB field: kpos.vorfaktor*
- **nVF**: Newly determined sales factor.
  - *Technical info: display field: DB field: kpos.neuvkfaktor*
- **aVK-Pr.**: Pre-sales price from the transferring site.
  - *Technical info: display field, DB field: kpos.vorpreis*
- **nVK-Pr.**: Newly determined sales price.
  - *Technical info: display field, DB field: kpos.neuvknstpreis*

### Footer
The fields and buttons in the footer area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

In addition, the following buttons are displayed:

- **Copy Item**: Copies the current item and inserts it behind the last item. You can edit the parameters for the copied item, e.g. quantity and dimensions.
- **BOM**: Opens the BOM dialog for the current item. Alternatively, you can open the dialog with `<F5>`.
  ⇨ "BOM View - Current BOM Level" on page D-205

## Order Entry – Properties
**Sales > Order Entry > Items tab > Properties tab**

*Fig. D-40 Order Entry – Properties*

On this tab, you can view and edit additional properties of the current item, e.g. warehouse assignment, packing type. In the upper area of the tab, the selected item is displayed, and in the lower area, the properties of this item.

- Use `<Page Up>` and `<Page Down>` to change to the previous and next item. In the lower area of the tab, the previous or next item is displayed according to its properties.
- Use `<F5>` to change from the current item to the Description field.

Generally you do not have to edit the details on the Properties tab.

If the status changes, an appropriate notice about the editing status of the marked item is displayed at the top of the tab, e.g. Delivered Local– Correction. In front of the Item field, the item status and if necessary the item code are displayed.
⇨ "Explanation of Symbols" on page D-79

### Header
The fields in the header area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

### Properties tab
Most fields are described for the General tab.
⇨ "General tab" on page D-124

In addition, the following fields are displayed:

- **Description**: Description of the header article. You can edit the description. The change is only taken over order-related.
  - *Technical info: alphanumeric field, DB field: kpos.artbez1*

> **Changes to the description**
> Once changed in this item, the article description will appear on all order-related documents and on all order-related dialogs for this document.

- **Cost Center**: Cost center name for statistical evaluations.
  - *Technical info: alphanumeric field, DB field: kauf.kostenst*
- **Stock**: Number of the default stock for stock articles. If you select a number, the description of the stock is displayed in plain text. If a default stock is assigned to the article in the master data, the field is pre-populated with this value. The field is only enabled if Stock is assigned to the article in the master data as type priority 1 or 2.
  - *Technical info: numeric field, DB field: kpos.Inr*
- **Stack**: Number of the stack stock for stock articles. If you select a number, the description of the stock is displayed in plain text. If a default stock is assigned to the article in the master data, the field is pre-populated with this value. The field is only enabled if Stock is assigned to the article in the master data as type priority 1 or 2 and the stack stock is selected as default stock.
  - *Technical info: numeric field, DB field: kpos.sfill1*
- **Product set**: Display of the description, number of the product set, and item number of the article in the product set. The fields are only pre-populated if you select an item with product set.
  - *Technical info: alphanumeric field, numeric fields, DB fields: kposex.sashcode, kposex.prodset, kposex.posnr*
- **Ibs/QU, Ibs/Piece, Ibs/Item, Ibs/GI**: Weight of the item. The details can be displayed in the following fields:
  - **Ibs/ME**: pounds per quantity unit
  - **Ibs/Piece** = pounds per piece
  - **lbs/Item** = pounds per item
  - **lbs/G/** = pounds per glass
  Only the field is enabled whose weight specification is assigned in the master data of the current article.
  - *Technical info: numeric fields, DB fields: kpos.gewme, kpos.gewst, kpos.gewicht, kpos.glasgew*
- **Actual QU/Qt**: Physical quantity in quantity unit per piece.
  - *Technical info: numeric field, DB field: kpos.phymestk*
- **Chargd. QU/Qt**: Calculated quantity in quantity unit per piece.
  - *Technical info: numeric field, DB field: kpos.qm*
- **QU/Item**: Total quantity in quantity unit per item. The value arises from the calculated quantity unit per piece x item quantity. For area articles, it applies, e.g. QU/Item = total area of the item x item quantity; for piece articles, it applies that QU/Item = total pieces of the item.
  - *Technical item: numeric field, DB field: kpos.geslief*
- **Bonus**: Number of the bonus process. If you select a number, the percentage of the item-related price discount is displayed in plain text.
  - *Technical info: numeric field, DB field: kpos.bonusnr*
- **CAD File**: Name of the CAD file that is attached to the item.
  - With `<Ctrl>+<F>` you can open the technical order entry (TOE). For this, you can enter and edit CAD files in A+W CAD Designer (Shapes).
    ⇨ Help Cards, "Enter item in CAD" on page D-22
  - Use `<F9>` to open a dialog for selecting the file type:
    - **SN**: All SN files are displayed for selection in the Explorer.
      ⇨ Help Cards, "Attach SN file" on page D-20
    - **DXF**: All DXF files are displayed for selection in the Explorer.
    If you select a file, the DXF Import dialog opens.
      ⇨ "DXF Import" on page D-175
  - Use `<Ctrl>+<F9>` to delete the CAD file that is attached to the item.
  - *Technical info: selection field, DB field: kpos.brokefile*

> **Special characters or blanks in file names**
> You may not use special characters or blanks for CAD file names.

- **CustArtNo**: Display of the customer article number for the item. The selected article must be assigned to the customer in the market partner master data.
  - *Technical info: numeric field, DB field: kpos.kuposnr*
- **Description**: Display of the customer article description.
  - *Technical info: alphanumeric field*
- **DOP Number**: Number of the declaration of performance. A declaration of performance can only be assigned to an article if in the master data for the corresponding article the Declaration of Performance checkbox is enabled. If the selected article is already assigned a declaration of performance in the master data, the field is pre-populated with this DOP number. Use `<Ctrl>+<T>` to open the Calculated technical details tab where you can enter a new declaration of performance. A declaration of performance can only be entered if the system is configured appropriately.
  ⇨ "Order Entry - Calculated Technical Values" on page D-190
  - *Technical info: alphanumeric field, DB field: kposp.lenr*
- **CE Code**: CE code. You can only specify a CE code if the system is configured appropriately.
  - *Technical info: alphanumeric field, DB field: kpos.cekz*
- **Print Sketch**: Type of sketch print, e.g. SNLive. You can specify the settings for the print service. When printing forms with Crystal Reports, in addition to the item details, various sketches can also be printed:
  - **SNLive**: sketch of the product structure including processings from the BOM
  - **AWBom**: sketch of the BOM structure
  - **AWDesign**: sketch of the muntin structure
  - **Prinzip**: principle sketch
  You can select none, one or several sketch types for printing.
  - Open the list of sketch types with `<F9>`.
  - Use the arrow keys to navigate between the sketch types.
  - Use `<Toggle>` to mark a sketch type. Marked sketches are highlighed in light blue.
  - Use `<End>` to close the dialog and take over the selection.
  - *Technical info: selection field, DB field: kpos.imagedrkz*
- **Pack. Type**: Number of the packing type, e.g. box. If you select a number, the description is displayed in plain text.
  - *Technical info: numeric field, DB field: kpos.verpackart*
- **Delivery**: Desired delivery type:
  - **Pickup**: Customer collects the goods.
  - **Third-party business transaction**: The producing plant will ship the goods directly to the customer. The type of the order item must be set in the article master data to purchased.
  - **No selection**: Goods will be delivered via the route that has been entered in the header.
  - *Technical info: toggle field, DB field: kauf.geschart*
- **Account**: Description of the cost center booking account.
  - *Technical info: alphanumeric field, DB field: kposp.mankonto*
- **Prod.Seq.**: Sequence of production that is specified to production for each item.
  - *Technical info: numeric field, DB field: kpos.ferts*
- **View**: Direction of the numbering sequence in the item structure of the entry view. This information is important, for example, for the item structure for glass with coatings.
  - **Outside**: Elements are numbered consecutively from the outside to the inside.
  - **Inside**: Elements are numbered consecutively from the inside to the outside.
  This field is not used at present.
  ⇨ "Product Structure" on page D-200
  - *Technical info: toggle field, DB field: kpos.ansicht*

### Footer
The fields and buttons in the footer area are described for the Order Items – General tab:
⇨ "Order Entry - General" on page D-116

## Order Entry – Prices
**Sales > Order Entry > Items tab > Prices tab**

*Fig. D-41 Order Entry - Prices*

This tab shows the calculation of the prices of the current item. The prices are displayed individually for each item.
- Use `<Page Up>` and `<Page Down>` to change to the previous and next item.
- Use `<F5>` to change from the current item to the Glazing/Pc. field.

If you want to edit the prices of the items, you have to edit the order and/or item conditions.
⇨ "Conditions for PCD Processing" on page D-283

If the status changes, an appropriate notice about the editing status of the marked item is displayed at the top of the tab, e.g. Delivered Local– Correction. In front of the Item field, the item status and if necessary the item code are displayed.
⇨ "Explanation of Symbols" on page D-79

### Header
The fields in the header area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

### Prices tab
The fields on item level on the Prices tab are described for the General tab.
⇨ "Order Entry - General" on page D-116

For some fields, several prices are specified:
- **SalesPrc**: The net sales price that is calculated from the conditions.
- **PrntSAPrice**: Net sales price that is printed on the documents.
- **Costs**: Cost portion of the sales price.

An individual column is displayed for each price. For the following fields, the prices are divided into three columns:

Use `<F4>` to open the supplementary menu. Use `Prices > Order conditions` to open the Order Conditions dialog where you can edit the order-related conditions for price calculation, such as price code, factor, minimum calculation areas, and processing surcharges.
⇨ "Conditions for PCD Processing" on page D-283

- **Price/QU**: Display of the price per quantity unit. The price is calculated from the glass price plus the surcharge.
  - *Technical info: display fields, DB fields: kpos.bmepreis, kpos.drbmepreis, kpos.ekbmepreis*
- **Gross Pieces**: Display of the gross piece price.
  - *Technical info: display fields, DB fields: kpos.bstpreis, kpos.drbstpreis, kpos.ekbstpreis*
- **Factor**: Display of the factor for the price surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
  - *Technical info: display fields, DB fields: kpos.faktor, kpos.drfaktor, kpos.ekfaktor*
- **Net Pieces**: Net price per piece.
  - *Technical info: display field, numeric field, DB fields: kpos.nstpreis, kpos.eknstpreis*
- **Glazing/Pc.**: Price per piece for glazing or installation work.
  - *Technical info: numeric fields, DB fields: kpos.vkverglas, kpos.ekverglas*
- **Total Price**: Display of the net total price of the item. The total price is calculated from piece price x quantity of the article.
  - *Technical info: display fields, DB fields: kpos.nstpreis, kpos.ekpospreis*
- **Minus**: Minus. Individually agreed upon discount for the item. You can specify the discount in the first field as percentage or in the second field as amount. The system calculates the value for the other fields.
  - *Technical info: numeric fields, display field, DB fields: kpos.rabatt, kpos.nachlass*
- **Item Price**: Item price. The item price is calculated from the total price less the discount from the Discount field. You can overwrite this value, e.g. if a flat fee has been agreed upon. If you change the item price, the discount in the Discount field is adjusted automatically.
  - *Technical info: numeric field, display field, DB field: kpos.npospreis*

For the following fields, only an amount is displayed:
- **EDI Price**: The EDI price is only important for companies with branch structure. In commercial undertakings, the purchase price is determined. This purchase price is then transferred to Production as the EDI price with openTRANS where it is treated as the preliminary sales price. Production can check the validity of this predefined sales price by recalculating the price.
  - *Technical info: numeric field, DB field: kpos.dfuenstpreis*
- **Margin**: Display of the retail margin in percent between price and costs.
  - *Technical info: display field, DB field: kpos.spanne*
- **Mat. Costs**: Display of the material costs for the item.
  - *Technical info: display field, DB field: kposp.komat*
- **Labor Cost**: Display of the labor costs for the item. The labor costs are only displayed if the order has been saved and transferred to production. The cost calculation in A+W Production calculates the costs and writes them back to the order. The costs are only displayed when you open the order again.
  - *Technical info: display field, DB field: kposp.kolohn*
- **Mach. Costs**: Display of the machine costs for the item.
  - *Technical info: display field, DB field: kposp.kobm*
- **Tax Rates**: Number of the VAT rate per item. Depending on the configuration, you can assign a VAT rate or several VAT rates per item.
  - Open the list of VAT rates with `<F9>`.
  - Use the arrow keys to navigate among the tax rates.
  - Use `<Toggle>` to mark a VAT rate.
  - Use `<End>` to close the dialog and take over the selection.
  - *Technical info: selection field, DB field: kpos.steuerzu*

### Footer
The fields and buttons in the footer area are described for the Order Items – General tab:
⇨ "Order Entry - General" on page D-116

## Order Items – Status
**Sales > Order Entry > Items tab > Status tab**

*Fig. D-42 Order Entry - Status*

On this tab, the item values are displayed according to the current status of the items, e.g. number of articles delivered and invoiced. As first item in the item overview, the item is displayed that is marked on the General tab. Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate in the item overview. Generally you do not have to edit the details on the Status tab.

If the status changes, an appropriate notice about the editing status of the marked item is displayed at the top of the tab, e.g. Delivered Local– Correction. In front of the Item field, the item status and if necessary the item code are displayed.
⇨ "Explanation of Symbols" on page D-79

### Header
The fields in the header area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

### Status tab
Most fields on the Status tab are described for the General tab.
⇨ "Order Entry - General" on page D-116

In addition, the following fields are displayed:
- **Complt**: Display of the units produced per item.
  - *Technical info: display field, DB field: kpos.lugesfert*
- **Packed**: Display of the units packed and prepared for transport per item.
  - *Technical info: display field, DB field: kpos.gespack*
- **Deliv.**: Display of the units delivered per item.
  - *Technical info: display field, DB field: kpos.geslief*
- **Invoice**: Display of the invoiced units per item.
  - *Technical info: display field, DB field: kpos.gesberech*
- **Cancel**: Display of the canceled units per item.
  - *Technical info: display field, DB field: kpos.gesstorno*

### Footer
The fields and buttons in the footer area are described for the Order Items – General tab:
⇨ "Order Entry - General" on page D-116

## Order Entry – Costs
**Sales > Order Entry > Items tab > Costs tab**

*Fig. D-43 Order Entry - Costs*

This tab displays the order costs of the items, e.g. material costs, labor costs. As first item in the item overview, the item is displayed that is marked on the General tab. Use the arrow keys and `<Page Up>`, `<Page Down>` to navigate in the item overview. Generally you do not have to edit the details on the Costs tab.

If the status changes, an appropriate notice about the editing status of the marked item is displayed at the top of the tab, e.g. Delivered Local– Correction. In front of the Item field, the item status and if necessary the item code are displayed.
⇨ "Explanation of Symbols" on page D-79

### Header
The fields in the header area are described for the Order Entry – Header, Footer tab:
⇨ "Order Entry - header, footer area" on page D-85

### Costs tab
Most fields on the Costs tab are described for the General tab.
⇨ "Order Entry - General" on page D-116

In addition, the following fields are displayed:
- **Mat. Costs**: Display of the material costs for the item.
  - *Technical info: display field, DB field: kposp.komat*

> **Display of the labor and machine costs**
> The labor and machine costs are only displayed if the order has been saved and transferred to production. The cost calculation in A+W Production calculates the costs and writes them back to the order. The costs are only displayed when you open the order again.

- **Labor costs**: Display of the labor costs for the item.
  - *Technical info: display field, DB field: kposp.kolohn*
- **Mach.Costs**: Display of the machine costs for the item.
  - *Technical info: display field, DB field: kposp.kobm*

### Footer
The fields and buttons in the footer area are described for the Order Items – General tab:
⇨ "Order Entry - General" on page D-116

## Site Change
**Sales > Order Entry > Header and Footer area <F4> > Change Site**

*Fig. D-44 Site change*

On this dialog, you change the site. The dialog is only enabled if the internal site separation is active, you have the required rights, and the system is configured appropriately.
Alternatively, you can open the Site Change dialog with `<F5>` in the Input field in the header area.

- **Site**: Site number to which you are changing.
  - Use `<F9>` to display the available sites.

> **Automatic site change**
> Depending on the configuration, another site can be assigned to the order automatically. For customer-specific adjustments, contact your A+W Software GmbH contact person.

## New Delivery Address
**Sales > Order Entry > Header and Footer area, Item level > <F4> > Addresses > New Delivery Address**

*Fig. D-45 New delivery address*

Use this dialog to enter a new delivery address.
- Use [OK] to save the new delivery address for the order.
- Use `<F3>` to save the new delivery address in the master data.

### Header
This area displays the current number of the address, the customer number, and the customer's main delivery address.

### Delivery address
- **Name, 1stname**: Customer's last name and first name.
  - *Technical info: mandatory field, alphanumeric fields, DB fields: adr.adrname, adr.adrvname*
- **Title**: Number of the customer's title. If you specify a number, the title is displayed in plain text.
  - *Technical info: numeric field, DB field: adr.anrede*
- **Attn.**: Name of the employee to receive the shipment.
  - *Technical info: alphanumeric field, DB field: adr.zhd*
- **Addition**: Additional information on the address.
  - *Technical info: alphanumeric field, DB field: adr.branche*
- **Street**: Street address of the delivery address.
  - *Technical info: alphanumeric field, DB field: adr.str*
- **PCd. POB**: Postal code and P.O. box number.
  - *Technical info: alphanumeric fields, DB field: adr.pfplz, adr.postfach*
- **PBoxCity**: City name for the PO box.
  - *Technical info: alphanumeric field, DB field: adr.pfort*
- **PCd.City**: Postal code and city of the delivery address.
  - *Technical info: mandatory fields, alphanumeric fields, DB fields: adr.plz, adr.ort*
- **DispatchRegion**: Dispatch region. The dispatch region is stored in the system master data and is determined via the postal code.
  - *Technical info: display field*
- **Country**: International country code for vehicles in the destination country. If you specify a code, the country name is displayed in plain text.
  - *Technical info: alphanumeric field, DB field: adr.Ifzcode*
- **Distance**: Distance to the customer in kilometers.
  - *Technical info: numeric field, DB field: adr.kilometer*
- **TravelTime**: Travel time to the customer in days.
  - *Technical info: numeric field, DB field: adr.fahrtzeit*
- **Tel**: Customer's phone number.
  - *Technical info: alphanumeric field, DB field: adr.orgtel*
- **Fax**: Customer's fax number.
  - *Technical info: alphanumeric field, DB field: adr.faxnr*
- **E-mail**: Customer's e-mail address.
  - *Technical info: alphanumeric field, DB field: adr.email*
- **Std. Route**: Number of the customer's standard route. If you specify a number, the name of the route is displayed in plain text.
  - *Technical info: mandatory field, numeric field, DB field: kauf.routenr*
- **Load.Seq.**: Number of the desired loading sequence. The loading sequence specifies in which sequence a truck is loaded. It serves to inform the logistics employee during loading of the truck and can, depending on the configuration, be printed on the delivery note. By default, the loading sequence is specified in shipping control. If you specify a number, it is transferred to shipping control.
  - *Technical info: numeric field, DB field: adr.routeposnr*
- **Remark**: Text area for additional information.
  - *Technical info: alphanumeric fields, DB fields: adr.text1, adr.text2, adr.text3*

## End customer address
**Sales > Order Entry > Header and Footer area, Item level > <F4> > Addresses > End Customer Address**

*Fig. D-46 End customer address*

Use this dialog to enter an end customer address. If the goods are picked up by the customer, you must enter a pick-up address in Purchasing.

- **Name, 1stName**: End customer's last and first name.
  - *Technical info: mandatory field, alphanumeric field, DB fields: adr.adrname, adr.vname*
- **Title**: Number of the end customer's title. If you specify a number, the title is displayed in plain text.
  - *Technical info: numeric field, DB field: adr.anrede*
- **Attn.**: Name of the employee to receive the shipment.
  - *Technical info: alphanumeric field, DB field: adr.zhd*
- **Industry**: Employee's industry.
  - *Technical info: alphanumeric field, DB field: adr.branche*
- **Street**: End customer's street address.
  - *Technical info: alphanumeric field, DB field: adr.str*
- **Reg. Num.**: Postal code and city of the P.O. box.
  - *Technical info: alphanumeric fields, DB fields: adr.pfplz, adr.postfach*
- **PBoxCity**: City name for the PO box.
  - *Technical info: alphanumeric field, DB field: adr.pfort*
- **PostCode, City**: Postal code and city of the end customer's delivery address.
  - *Technical info: alphanumeric fields, DB fields: adr.plz, adr.ort*
- **CCd Country**: International country code for vehicles in the destination country. If you specify a code, the country name is displayed in plain text.
  - *Technical info: alphanumeric fields, DB field: adr.kfzcode, adr.land*
- **Distance**: Distance to the end customer in kilometers.
  - *Technical info: numeric field, DB field: adr.kilometer*
- **Travel Time**: Projected travel time to the end customer. The travel time affects the delivery date.
  - *Technical info: numeric field, DB field: adr.fahrtzeit*
- **Handling Time**: Time for loading and unloading the shipment.
  - *Technical info: numeric field, DB field: adr.handlingszeit*
- **Arrival Time**: Requested arrival time at the customer's in the format hh:mm.
  - *Technical info: alphanumeric field, DB field: adr.ankunftszeit*
- **Unloading Point**: More precise description of the delivery point, e.g. gate A.
  - *Technical info: alphanumeric field, DB field: adr.anlieferstelle*
- **Fax No.**: End customer's fax number.
  - *Technical info: alphanumeric field, DB field: adr.fax*
- **Route**: Number of the route.
  - *Technical info: numeric field, DB field: adr.routenr*
- **Load.Seq.**: Number of the desired loading sequence. The loading sequence specifies in which sequence a truck is loaded. It serves to inform the logistics employee during loading of the truck and can, depending on the configuration, be printed on the delivery note. By default, the loading sequence is specified in shipping control. If you specify a number, it is transferred to shipping control.
  - *Technical info: numeric field, DB field: adr.routeposnr*
- **Remark**: Text fields for additional information.
  - *Technical info: alphanumeric fields, DB fields: adr.text1, adr.text2, adr.text3*

## Market Partner Info
**Sales > Order Entry > Header and Footer area, Item level > <Shift> + <F4> > Market Partner Information**

*Fig. D-47 Market partner info*

This dialog displays information about the selected market partner from the master data.

### Header
- **Cust**: Name and customer number. By default, the customer from the current document is selected. You can overwrite the number and select another customer. If you specify a number, the customer name is displayed in plain text.
  - *Technical info: mandatory field, DB field: limits.kunr*
- **Site**: Name and description of the site. By default, the site is selected from the current document. You can overwrite the number and select another site. If you specify a number, the description of the site is displayed in plain text. The field is only displayed if you are working with internal site separation.
  - *Technical info: numeric field, DB field: kauf.hausnr*

### Open Itm. FINAC
This area displays the open items from the financial accounting (FINAC).

- **Unpaid Invoices**: Display of the items for invoices that have not yet been transferred to the FINAC.
  - *Technical info: display field, DB field: limits.op*
- **Cred. limit**: Display of the defined credit limit that the unpaid invoices may not exceed.
  - *Technical info: display field, DB field: limits.sglimit*
- **Orders in Work**: Display of the orders that have not yet been delivered and/or invoiced.
  - *Technical info: display field, DB field: limits.oa*
- **Assu. Limit**: Display of the insured credit limit.
  - *Technical info: display field, DB field: limits.akvlimit*

### Table
The table displays information about the last quotation, the last order, and the last invoice of the selected customer:
- **Date**: Entry or change data of the document.
- **Number**: Document number.
- **Site**: Site number that is assigned to the document.
- **Amount**: Net end amount of the document.
  - *Technical info: display fields, DB fields: kauf.auftrnr*

### Footer
This area displays the total turnover of the selected customer in the current year.

## Contacts
**Sales > Order Entry > Header and Footer area > <F4> > Contacts**

*Fig. D-48 Main Contact*

On this dialog, you enter a contact person for the selected market partner or you assign a contact person from the master data to the market partner.
- Use `<Page Up>` and `<Page Down>` to display the contacts that are stored for the market partner.
- Use `<F6>` to enter a new contact.

### Header
This area displays the current number of the contact, the customer number, and the main contact.

> **Specify main contact**
> If several contacts are stored for a market partner, you can specify a main contact in the market partner master data.

### Contact
In this area, you enter or edit a contact's data.

- **Last name, 1stName**: Contact's last name and first name.
  - *Technical info: mandatory field, alphanumeric fields, DB fields: anspr.apname, anspr.apvname*
- **Title**: Number of contact's title. If you specify a number, the description is displayed in plain text.
  - *Technical info: numeric field, DB field: anspr.anrede*
- **Departm.**: Department in which the contact works.
  - *Technical info: alphanumeric field, DB field: anspr.abteilung*
- **Position**: Contact's position at the company.
  - *Technical info: alphanumeric field, DB field: anspr.position*
- **Birthday**: Contact's birthday in the format DD.MM.YYYY.
  - *Technical info: date field, DB field: anspr.gebdat*
- **Phone**: Contact's telephone number.
  - *Technical info: alphanumeric field, DB field: anspr.telefon*
- **Fax**: Contact's fax number.
  - *Technical info: alphanumeric field, DB field: anspr.telefax*
- **Mobile**: Contact's mobile phone number.
  - *Technical info: alphanumeric field, DB field: anspr.telex*
- **E-mail**: Contact's e-mail address.
  - *Technical info: alphanumeric field, DB field: anspr.email*
- **Fields without names**: Additional remark about the contact.
  - *Technical info: alphanumeric fields, DB fields: anspr.text1, anspr.text2, anspr.text3*

## Cancel
**Sales > Order Entry > Header and Footer area, Item level > <F4> > Cancel**

*Fig. D-49 Cancellation*

This dialog is used for canceling an order. You can also specify additional information about the cancellation.
If you want to cancel an order, first a query is displayed that you must confirm with [Yes].

- **Canc. Inform.**: Additional information about the cancellation, e.g. reason for the cancellation. This information is displayed if a canceled order is called up. Specification of this information is optional.
  - *Technical info: alphanumeric field, DB field: kauf.exbez2*
- **OK**: Cancels the current order.
- **Cancel**: Cancels the cancellation.

## Staff Allocation – Special
**Sales > Order Entry > Date field > <Ctrl> + <F8>**

*Fig. D-50 Staff allocation*

Use this dialog so specify employees for various areas. Alternative, you can assign the employees to the individual areas in the order entry on the Properties tab. The dialog is only enabled customer-specifically.
The fields are described in detail for the Order Entry – Properties tab:
⇨ "Order Entry – Properties" on page D-95
For customer-specific adjustments, contact your contact person at A+W Software GmbH.

## Configurable Fields
**Sales > Order Entry > Header and Footer area, Item level > <F4> > Configurable Fields**

*Fig. D-51 Configurable fields*

Use this dialog to display the configurable fields for the document.
The fields that are displayed on this dialog can be enabled customer-specifically. The dialog differs depending on the configuration.
The set-up of configurable fields always requires development work that has to be done by a A+W employee.
For customer-specific adjustments, contact your contact person at A+W Software GmbH.

## Overview
**Sales > Order Entry > Date field > <Shift> + <F11>**

*Fig. D-52 Overview*

This dialog displays an overview of the documents for an order.
The columns are described in detail for the Find Document - Overview tab:
⇨ "Search Document - Overview" on page D-388
