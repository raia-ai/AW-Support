---
title: "EN-CONFIG-AW_Enterprise_3"
source: "EN-CONFIG-AW_Enterprise_3.pdf"
tags: ["A+W Enterprise", "configuration", "discounts", "invoicing", "order entry", "master data", "environment variables", "stored procedures", "payment schedule", "foreign currency"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical configuration guide for A+W Enterprise software, detailing settings related to discounts, invoicing, order processing, and master data management."
long_description: "This comprehensive technical manual provides detailed instructions for configuring various modules and features within the A+W Enterprise system. It covers a wide range of topics essential for system administrators and technical personnel. Key areas include the management and calculation of discounts, with sections on updating sales, costs, and purchasing discounts, and how to use stored procedures like 'rabattzuord' for custom calculations. The guide explains how to handle transactions in foreign currencies, including market partner-specific discounts and the rules for redrawing exchange rates. A significant portion of the document is dedicated to invoice generation, covering grouping criteria for collective invoices, and the setup and processing of payment schedules involving deposit and final invoices. It also details the data structures and master data tables involved, such as 'rabattmeth', 'rabstamm', and 'kaufrab', providing field-level descriptions. The document lists and explains numerous environment variables that control system behavior for features like recording documents with reference, small delivery surcharges, and automatic features in order entry like enamel and edge stripping. This guide is crucial for customizing A+W Enterprise to meet specific business requirements."
---

---
### Update sales
For the discounts of the methods that are defined in `RABATTMETHODEN_UPDATE` and already included in the order, the values are recalculated. Here, the current basic values are drawn from the master data. However, no new discounts are drawn from the master data.

### Update costs
For the discounts of the type cost that are already included in the order, the values are recalculated. Here, the current basic values are drawn from the master data. However, no new discounts are drawn from the master data.

### Update purchasing
For the discounts of the methods that are defined in `RABATTMETHODEN_UPDATE_EK` and already included in the order, the values are recalculated. Here, the current basic values are drawn from the master data. However, no new discounts are drawn from the master data.

### All new
All discounts are re-drawn from the master data and calculated.

### Basic values with/without SP RABATT_SP_PARAMETER (rabattzuord)
If the ID stored procedure (SP) is **not** set for a discount, then the discountable amounts will be calculated as the basis. The sequence of the discounts is crucial for the calculation of the basis.

If the ID stored procedure (SP) is set for a discount, then it is also considered that the SP is stored for the calculation. If this is not the case, the basis value is set equal to the PU price. The basis value across the amounts that can be discounted is not regarded.

**QR 11/2022**

In the master data and document, you can redirect the calculation of the discounts to the `rabattzuord` SP. If a discount is calculated via this SP, then the basis value is irrelevant because the amount is calculated via the SP. Unfortunately, you could also activate the calculation via this SP if no SP was stored. In this case, the basis value was set as irrelevant to the start value nevertheless and not to the ongoing discountable amount (considering the discountable discounts/surcharges). In order to avoid the negative side-effect, it is no longer possible to activate the SP evaluations if the corresponding SPs are not stored or not enabled. In the document, any active SP ID is also disabled if the configuration is lacking. If a SP is enabled and encounters an error, then the basis value is nevertheless set to the current discountable amount.

### Process
On the item level, the SP "rabattzuord" only collects the basic values for the calculation. It is decided by the SP to which items this discount is applied and to which it is not.

If you want to calculate the supplier costs already in the SA document, the discounts have to be stored globally as cost discounts. Via the SP, you can then decide whether the cost discount should be applied for a particular item. However, currently (as of 02/26/2024), no keys for access to item information, procurement types or supplier details are forwarded to the SP.

The SP that provides the value is controlled via `RABATT_SP_KAUF_PARAMETER` and is only called per document. Here there are only order-related parameters. A value can come from this SP. But no item-related parameters can be passed to this SP.

### Change of a discount criterion
If a discount criterion within an order changes (e.g. the kilometers due to a change of the delivery address), then there is a query as to whether the discounts of the relevant method should be recalculated.

**Query 14613:** "At least one discount criterion has changed. Redetermine discounts of the relevant methods (manual changes will be lost!)"

If this query is answered with "yes," the relevant method will be redetermined from the master data. If the answer is no, the method is not redetermined from the master data, but rather calculated on the basis of the existing definitions of the discount amount based on the new data.

This query is made only 1x per order. If a criterion changes again after the first answer, there is no additional query. The system retains the first answer.

### Currency

**QR11/2022 Discounts and foreign currency**
alcib - 13.04.14116 // [AW-128671]

Discounts for which the currency units (CU) are specified must generally be specified in own currency (environment variable `MODUL_WAEHRUNG`). This affects both the general and the customer-specific discounts.

If the market partner is on "Calculation in foreign currency", then discounts of the type "Sales" or "Purchasing" are recalculated in the corresponding currency in the document. Discounts of the type costs will not be recalculated.

If the currency, the conversion rate or the identifier "Calculation in" is changed in the document, then the discounts are recalculated accordingly. If the exchange rate is changed in a calculation or credit, there is no automatic adjustment of the discounts.

**QR 03/2024 [AW-166270]: Market partner-specific discounts in foreign currency**

If a market partner has a different currency than the client's own currency in the master data and if there is calculation in this foreign currency, now it is possible to calculate a market partner-specific value discount as discount in the foreign currency. This does not apply for the general discounts, which are still interpreted as discounts in the client's own currency and then converted. This way, you can maintain the market partner-specific discounts regardless of rate fluctuations.

Configuration is done via an environment variable and can be activated for all market partners, only for suppliers or only for customers. The rule for the customer applies for project-related discounts.

The evaluation whether or not a discount is converted is done on the basis of the document data (currency, calculation in foreign currency), which is drawn at the beginning from the market partner master data. If it is changed manually in the order, then it will also influence the discounts.

**Environment variable:**
`MP_DISCOUNT_OWN_CURRENCY` = ON - all
= `CUSTOMER` for customers, project in SA
= `SUPPLIER` for supplier in PU

## 14.5.8. Automatic cost rate for packaging
See Section "Rack planning"

## 14.5.9. Discount information on the item level

**QR 11/2022**

The discount values are currently not broken down by item. This can now be configured for special discount methods.

There are 3 environment variables in which the methods can be defined. In the environment variables `POSRABATT_VK_METHODEN`, `POSRABATT_EK_METHODEN`, `POSRABATT_KOSTEN_METHODEN`, up to 10 discount methods can be listed, separated by |. For these methods, the discounts calculated in the document are broken down to the item/piece level. Only the discounts with the direct item reference (CU/kg, CU/qm, CU/G*E) are considered. Furthermore, only max. 2 discounts from a method + type (sales, purchasing, costs) are considered.

In order to save the information, 4 main and 4 additional sets of configurable fields (`kposprvfld`) are provided on the item level. In the `kposprvfld.longval(X)` fields, the method number is saved, and in the `kposprvfld.decval<X>` fieldsSPn, the recalculated amount. The recalculated amount is an amount per piece of the item. The surcharges are saved as positive values and the discounts as negative values. As basis of the calculation, quantity (or delivered or calculated quantity, depending on the document) is used. Canceled items are not considered. There is also a rounding difference adjustment in the last active item with quantity>0. In the sets, the data is saved according to the sequence of the methods in the environment variables.

- **SET 17 (main set)** : Methods 1 - 5 from environment variables for SA/PU methods.
- **SET 18 (additional set)**: Methods 1 - 5 from environment variables for SA/PU methods (if 2nd discount of the same method is present).
- **SET 19 (main set)**: Methods 6 - 10 from environment variables for SA/PU methods.
- **SET 20 (additional set)** : Methods 6 - 10 from environment variables for SA/PU methods (if 2nd discount of the same method is present).
- **SET 21 (main set)**: Methods 1 - 5 from environment variables for cost methods.
- **SET 22 (additional set)** : Methods 1 - 5 from environment variables for cost methods (if 2nd discount of the same method is present).
- **SET 23 (main set)** : Methods 6 - 10 from environment variables for cost methods.
- **SET 24 (additional set)** : Methods 6 - 10 from environment variables for cost methods (if 2nd discount of the same method is present).

Sets 21 to 24 are only assigned for the SA documents; for the PU documents, these are left empty.

**Example:**
`POSRABATT_VK_METHODEN="300|100|500"`

In the order, for the method "300" there are two different surcharges; for method "100" there is just one surcharge, and method 500 has 3 different surcharges

**In set 17**
`longval1` = Method "300"
`decval1` = the associated discount amount of the first discount
`longval2` = Method "100"
`decval2` = the associated discount amount of the first discount
`longval3` = Method "500"
`decval3` = the associated discount amount of the first discount

**In set 18**
`longval1` = Method "300"
`decval1` = the associated discount amount of the second discount
`longval2` = 0 (since method 100 has no second discount)
`decval2` = 0
`longval3` = Method "500"
`decval3` = the associated discount amount of the second discount

The third discount of the method 500 is not calculated back in this new structure and saved. The normal recalculation to the item and incorporation into revenue is done regardless of this new function.

The recalculation is done during the determination of the gross amount of the document, directly when exiting the item level in the document footer.

If you would like to check the recalculated values in the order, you can go back from the document footer to the item and open the "configurable fields" there.

The calculation is also done during entry by reference. If a discount of the defined method is included in an order, the recalculation is also done if you answer the question about discount recalculation with "no." In this case, the existing value is used as starting point for the recalculation.

The recalculation is also done during the transfer from the dealer to the production site, when generating the delivery notes (manually or automatically), partial delivery notes, invoices, etc., as well as for PU invoices that were generated via the invoice check. If partial delivery notes or partial invoices are generated, then the records for the private fields are also not generated for the items not calculated. The evaluation of the data must always be done in connection with the item and the quantities booked there (delivered, calculated).

## 14.5.10. Tables and fields
The tables involved are described briefly below. For a detailed description of the individual fields, please use altab or read the appendix.

### Master Data
The new discount logic is based on three new master data tables and table for the language-dependent texts:
1.  **Rabattmeth**: This table includes basic information about a discount method such as the qualifier. The "method" field is the primary key.
2.  **Rabstamm**: This table describes actual discounts. The "rabattid" field is the primary key. Using the "method" field, the reference to the "rabattmeth" table is established.
3.  **Rabattstaf**: The scaling levels of the discounts are stored in this table. This table has no primary key. However, there is an index for the foreign key "rabattid."
4.  **Xsprbez**: The language-dependent names of the entries from the "rabstamm" table are stored in this table. The "rabattid" in the "id" field is used as a flag.

### Table `rabattmeth`
| Field | Type | Description |
| :--- | :--- | :--- |
| `methode` | smallint | Primary key. Some discount methods are pre-defined. New ones can also be defined by the customer. |
| `methodenname` | char(80) | Name of discount method. No language-dependent configuration possible. |
| `Seqnr` | smallint | Controls the sequence in which the discounts are applied. |
| `discountable` | smallint | 0=The amount of this discount is not considered for subsequent discounts. 1=The amount of this discount is considered for subsequent discounts. Subsequent discounts cannot present this effect. |
| `Step` | smallint | Controls on which hierarchy levels (object, customer, general) this method may be maintained: 1 General maintenance possible 2 Market partner-dependent maintenance 4 Object-specific maintenance. Ex: level = 6 -> object-specific and market partner-dependent maintenance possible. |
| `qualifier` | smallint | Specifies the dependency of the discount/surcharge (Criterion): 0 No qualifier, 1 Flag rush order, 2 Route, 3 Shipping type, 4 Packaging type, 5 Delivery type, 6 Destination, 7 Invoice country, 8 Online, 9 Special, 11 - EDI. |
| `glasgewicht` | smallint | 0 Discount refers to total weight. 1 Discount refers only to glass weight. 2 Discount refers to glass weight. If glass weight of all involved items 0, take total weight of items. (This flag is only evaluated for GR/kg discounts.) 3 Discount refers to the fact. item weight. 4 Discount refers only to the invoiced glass weight. 5 Discount refers to the invoiced glass weight. If the invoiced glass weight of all participating items is 0, then the invoiced item weight is used. 6 Discount refers to the physical sqm. 7 Discount refers to the invoiced sqm. |
| `gutschrift` | smallint | 0 Discount is not taken over in credits. 1 Question whether discount should be taken over in credits. 2 Take over discount automatically in credits. |
| `nullpositionen` | smallint | 0 For quantity calculation, items with item amount of zero are not considered. 1 Items with zero amount are also considered for quantity calculation. |
| `lieferzuschlag` | smallint | Starting with ALCIB 2011: Marks the discount method as a Delivery surcharge. See #152136. |

### Table `rabstamm`
| Field | Type | Description |
| :--- | :--- | :--- |
| `rabattid` | integer | Primary key, used for clear identification of the record. Is used as foreign key in rabattstaf and xsprbez. |
| `methode` | smallint | References record from "rabattmeth." |
| `qualifierwert` | char(10) | Value that the qualifier specified in "rabattmeth" must have in an order so that this record is drawn in this order. Records with value 0 are always drawn. |
| `Ekvkkz` | smallint | 0 Sales discount, 1 Cost discount, 2 Purchase discount. |
| `fremdsprachig` | smallint | Specifies whether for this record there is a language-dependent text in "xsprbez." 0 No record exists, 1 Record exists. |
| `rabatttext` | char(80) | Name of the discount, pre-populated with method name. |
| `Mpnr` | integer | References market partner or object from "mp." A "0" means general. |
| `kuliflag` | smallint | Market partner type: 0 Customer, 1 Supplier, 2 Other market partners, 3 Object. |
| `Wgrnr` | char(6) | Product group for which the discount is granted. Extended logic (`1*3***`)! |
| `staffelrabatt` | smallint | 0 No graduated discount, 1 Graduated discount. |
| `staffelbasis` | smallint | 0 No graduated discount, 1 Gradation basis square meter, 2 Gradation basis kilogram, 3 Gradation basis kilometer, 4 Gradation basis pieces. |
| `Value` | decimal | If "staffelbasis = 0" percentage or amount of the discount. |
| `rabattart` | smallint | 0 Fixed value (CU – currency unit), 1 Percentage value (%), 2 Value per piece (CU/pc), 3 Value per square meter glass (CU/sqm), 4 Value per kilogram glass (CU/kg), 5 Value per kilometer (CU/km), 6 Percent per sales value (%/SA), 7 Percent per cost value (%/Kst), 8 Value per kilogram glass and kilometer distance (CU/G*E). |
| `fixerabatte` | smallint | This flag describes the handling of fixed discounts for the generation of partial orders. Is only required for "rabattart=0." 0 Conversion into percentage discounts, 1 Take over complete amount in first partial order, 2 Duplicate complete amount in all partial orders. |
| `satzart` | smallint | 0 Discount, 1 Surcharge. |
| `minbetrag` | money(10,2) | Minimum amount of the discount. |
| `maxbetrag` | money(10,2) | Maximum amount of the discount. |
| `Verteil` | smallint | 0 Discount is not redistributed, 1 Discount is distributed to the items. |
| `Konto` | char(10) | If "verteil = 2," account to which booking should be done. |
| `Kstelle` | char(10) | If "verteil = 2," cost center to which booking should be done. |
| `Skonto` | smallint | If "verteil = 2": 0 discount not cash discount-capable, 1 cash discountable discount. |
| `statwgrnr` | char(6) | If "verteil = 2," statistical product group. References "wgrnr" from "wargrp." |
| `steuerzu` | char(4) | If "verteil = 2," value-added tax vector. Specifies which value-added taxes apply to this item. |
| `gueltigvon` | date | Date from which the discount record is valid. |
| `gueltigbis` | date | Date until the discount record is valid. |
| `verglkz` | smallint | 0 discount applies to everything. 1 discount only applies to glazing. Flag is only evaluated for percentage discounts. There, a total of kpos.vkverglas is used as basic amount. |
| `rabattidz` | smallint | For replication: rabattid from the central site. |
| `spaufrufkz` | smallint | Starting with ALCIB 2008: If in the orders the stored procedure "rabattzuord" should be called that is called for each item and decided whether this discount affects the current item. `RABATT_SP_PARAMETER` must be set. **Attention:** When creating stored procedures, you must make sure that if possible, no write operations are done on real tables since otherwise, due to the transaction logic in the document entry, there can be permanent blocks to the table. |
| `spaufrufkzkauf` | smallint | Starting with ALCIB 2009: Should the stored procedure "rabattanpassung" be called in the orders that allows adjustment of the discount. `RABATT_SP_KAUF_PARAMETER` must be set. |
| `otrabattid` | CHAR(30) | Starting with ALCIB 2011: This field allows the assignment of discounts from purchasing orders received from OpenTRANS. (#164543) |
| `glasgewicht` | smallint | Starting with ALCIB 2011: You can now configure per discount to which weight it should refer. This information overrides the information from the method master data, so that discounts of a method can now have different reference weights. |
| `minbeinullbetragkz` | smallint | Starting with ALCIB 2011: Flag whether the minimum amount should also be drawn for a calculated amount of 0.0 GR. |

### Table `rabattstaf`
| Field | Type | Description |
| :--- | :--- | :--- |
| `rabattid` | integer | Clearly references record from "rabstamm." |
| `minimum` | decimal | Minimum value of the gradation basis for this level. |
| `maximum` | decimal | Maximum value of the gradation basis for this level. |
| `Wert` | decimal | Percentage or amount. |

### Table `Kaufrab`
| Field | Type | Description |
| :--- | :--- | :--- |
| `Aufnr` | integer | Foreign key from "kauf". Handles the assignment to the order. |
| `Rabattid` | integer | Foreign key from "rabstamm". |
| `Methode` | smallint | Foreign key from "rabattmeth". |
| `Ekvkkz` | smallint | Flag for order type from "rabattmeth." |
| `Txt` | char(80) | Name of the discount from "rabstamm.rabattext." |
| `Qualifier` | smallint | Qualifier from "rabattmeth". |
| `Qualifierwert` | char(10) | Value of the qualifier from "rabstamm." |
| `Rabattierbar` | smallint | This field specifies whether subsequent discounts count the discount value of this discount in their basic amount. |
| `Seqnr` | smallint | Sequence number that produces the sequence in which the records are considered for the calculation. (`rabattmeth.seqnr` * 100 + addon) |
| `Verglkz` | smallint | Glazing flag from "rabattmeth". |
| `Gutschrift` | smallint | Credit note from "rabattmeth". |
| `Nullpositionen` | smallint | Consideration of items with amount of 0 from "rabattmeth." |
| `Wagrp` | char(6) | Product group from "rabstamm.wgrnr". |
| `Staffelrabatt` | smallint | Flag whether graduated discount from "rabstamm." |
| `Staffelbasis` | smallint | Basis for graduation from "rabstamm." |
| `Minimum` | decimal | Minimum value of the gradation basis for the currently-drawn level from "rabattstaf." |
| `Maximum` | decimal | Maximum value of the gradation basis for the currently-drawn level from "rabattstaf." |
| `Wert` | decimal | Value from "rabstamm". |
| `Satzart` | smallint | Surcharge or discount from "rabstamm." |
| `Rabtyp` | smallint | Discount type from "rabstamm.rabattart". |
| `Fixerabatte` | smallint | Handling of fixed discounts from "rabstamm.fixerabatte". |
| `Minbetrag` | money(10,2) | Minimum amount of the discount from "rabstamm." |
| `Maxbetrag` | money(10,2) | Maximum amount of the discount from "rabstamm." |
| `Verteil` | smallint | Redistribution from "rabstamm". |
| `Konto` | char(10) | see "rabstamm" |
| `Kstelle` | char(10) | see "rabstamm" |
| `Skonto` | smallint | see "rabstamm" |
| `Statwagrp` | char(6) | see "rabstamm.statwgrnr" |
| `Fremdsprachig` | smallint | See "rabstamm" |
| `Steuerzu` | char(4) | see "rabstamm" |
| `Grundwert` | decimal | Basic value that the discount affects: For "rabattart = 0" => unimportant, For "rabattart = 1" => monetary amount, For "rabattart = 2" => pieces, For "rabattart = 3" => square meter count glass, For "rabattart = 4" => kilogram glass, For "rabattart = 5" => number of kilometers, For "rabattart = 6" => discountable sales value, For "rabattart = 7" => discountable costs, For "rabattart = 8" => Glass weight and distance |
| `Betrag` | money(10,2) | Calculated discount amount |
| `Geloescht` | smallint | 0 Discount was deleted from order manually. 1 Discount enabled |
| `Manuell` | char(20) | Vector that is used to save the manually-changed fields. |
| `Ekwgrsum` | money(10,2) | Existing help field: purchasing total of specified product group. No longer used by new logic. |
| `Vkwgrsum` | money(10,2) | Existing help field: sales total of specified product group. No longer used by new logic. |
| `Artnr` | integer | Existing field for deposit invoices: item number of the discount/surcharge. No longer used by new logic. |
| `Rechnr` | integer | Existing field for deposit invoices: invoice number from the payment schedule. |
| `Bestellnr` | integer | Not used at present! |
| `Glasgewicht` | smallint | See table "rabattmeth" |

### Transaction data
The new discount logic uses the transaction table "kaufrab" of the old logic. This table was only expanded by a few fields.

## 14.5.11. Special functions

### Delivery surcharge (AWD #152136)
**ALCIB 2009 (February 2009)**

Since this version, it is possible to assign discounts per delivery. There is a new checkbox in the method master data for this that identifies these discount methods.

During delivery note generation, all discounts for the document are analyzed and for all records for whose method this flag is set, the following check is conducted. If for the delivery to which this delivery note applies there is already another delivery note that includes an active discount of this method, the discount is deactivated in the delivery note to be generated. If there is none and the discount is deactivated, it is reactivated again. This means that you cannot deactivate the delivery surcharge for individual orders (see also PF #[AW-165215]).

A delivery is identified via the customer, the route, the date, and the delivery address number.

If you use this logic, you must also set the environment variable `LS_EIGENE_AUFNR`. The effect of this is that when generating delivery notes, a new internal order number (`kauf.aufnr`) is always assigned. If you do not set this variable, there can be inconsistent totals in the orders. - Starting with A+W Enterprise 6, this is no longer required. Starting with this version, this is the default behavior.

**ALCIB 2011 / June 2010 (AWD #177072)**

This version offers an extended function "shipping surcharges". When generating the first delivery note for an order, it is now checked whether the delivery surcharge was deactivated according to the logic described above. If this is the case, the surcharge will be disabled in the order too.

This logic works only if the shipping surcharge is adopted only for the first partial document (flag 'partial document' in discount master data) and if this is a fixed discount (discount type WE). Because the shipping surcharge is disabled in the order now, it will also be disabled in invoices related to this order. Invoices will be entered with an order reference despite existing shipping notes, e.g. if the customer does not accept partial shipment.

## 15. Small delivery surcharge/shipping fee
ALCIB 2007 allows you to add surcharges for small shipments.

### 15.1. Data structures
The tables involved are described briefly below. For a detailed description of the individual fields, please use altab.

#### Master Data
- **`kleinliefkomm`**: This table shows the comments; please choose one of them if you do not want to add a small shipment surcharge.
- **`kleinliefnein`**: This table shows the partners for which no small shipment surcharge shall be applied.

#### Transaction data
- **`kleinlief`**: This table shows a record for every invoice issued for a small shipment. This needs to be edited. This means that first you have to decide whether a surcharge shall be applied at all. The corresponding invoice can be booked after that.

### 15.2. Stored Procedure
A stored procedure defines whether an invoice belongs to a small shipment, or to part of a small shipment. At present, an invoice is considered to belong to a small shipment if the invoice amount falls below a defined minimum.

The delivery value is the revenue for the item broken down across the quantities, which are planned for the route in question:
`kpos.erloes/kpos.menge * lapool.sollstk`

According to standard ALCIB logic, the revenue of the item also includes the discounts/surcharges charged back. General discounts will not be included in shipment value. The shipment value of a route includes all order items shipped on a certain date, on a certain route, to the recipient of the invoice (customer number on invoice/standard debtor for the order).

The stored procedure is called when booking sales invoices unless the market partner is stored in the table `kleinliefnein` or the invoice booking is called by the Intauf. If the SP shows that this is a small shipment, the program will refuse to book this invoice. The user is informed by a message. If the SP returns an error, the booking of the invoice is also canceled.

**Details regarding the functioning of the SP:**
- For small shipments, the SP makes an entry in table 'kleinlief'. If an entry in table `kleinlief` already exists, the SP checks whether the decision regarding surcharge calculation has already been made.
- Invoices the reference orders of which have a payment plan, will not be checked for small shipments. Shipment of an order with a payment plan contributes to the shipment value however.

An SP call will stop the booking in ALCIB if:
- this is a small shipment and the SP has created a record in `kleinlief`.
- this is a small shipment and `kleinlief` shows as yet unedited records for this invoice.

A SP call does not affect the booking if:
- the route is a pick-up route
- the route is a direct delivery route
- the reference document is neither an order nor an invoice
- the invoice refers to an order with a payment plan
- table `kleinlief` already shows an edited record
- the shipment value exceeds the value defined in `DELIVERY_SURGARGE_LIMIT`

The SP writes a log on the database server; the details depend on the help level set in ALCIB:
- `< 6`: Only invoice and result of the check will be recorded.
- `>= 6`: A detailed trace is written.

### 15.3. Dialog logic
Using `<Ctrl+K>` in the first field of the dialog for the automatic release of sales invoices brings you to the dialog for editing small shipments. When you open this, all records from table 'kleinlief' are loaded. The menu is protected by the right VOKZ.

This menu and the mode menu provide the following information on the invoices involved:
- Delivery date
- Customer number
- Route
- Invoice number and sub-number
- Invoice value
- Called quantity (MODE dialog)
- Default quantity (MODE dialog)
- Shipment value (MODE dialog)

Follows a checkbox with three options. It decides whether or not a surcharge shall be applied.
All checkboxes are empty when you open the dialog. For the records you want to edit, you can add a green checkmark or a red cross to the checkbox. The green checkmark means that this invoice will get a surcharge while the red cross means no surcharge. When you apply no surcharge, you have to select a reason for this in the last field of the dialog. This is selected by means of a selo from table `kleinliefkomm`.

When you start processing of the defined information by `<F3>`, the following database operations will be performed within a transaction:
- The surcharges for all defined invoices will be calculated from master data. For details on the calculation, please refer to paragraph 'Surcharge calculation'. These invoices will then be recalculated by means of Intaufs.
- All invoices that shall get a surcharge will be booked by means of Intauf.
- The changes are saved in table `kleinlief`.

### 15.4. Surcharge calculation
You can define three different surcharges. The actual surcharge to be applied to the invoice depends on the customer. Basically, the system will add the surcharge defined in `DELIVERY_SURCHARGE`. You can create a configurable partner field called `DELIVERY_SURCHARGE` however. If you enter for a customer 'A' or 'B' here, the system will the value defined in `DELIVERY_SURCHARGEA` or `DELIVERY_SURCHARGEB` instead of the value defined in `DELIVERY_SURCHARGE` for this customer.

### 15.5. Automatic processing of open invoices
To prevent small invoices from piling up and to avoid delays in booking of the invoices, you can have open invoices automatically processed. Every first invoice of a customer, route, and Itplan will get the surcharge. The remaining records will get no surcharge. This automation is enabled by the ALCIB start parameter "-kleinlief" and writes a log called "autokleinlief" while it is run.

### 15.6. Environment variables
- **`DELIVERY_SURCHARGE_LIMIT`**: This environment variable saves the limit to be reached by all shipments on a date and on a route to avoid the application of a surcharge.
- **`DELIVERY_SURCHARGE`**: This environment variable defines the general surcharge value. Furthermore, this variable is used in the program to check whether the logic is active.
- **`DELIVERY_SURCHARGEA`**: In this environment variable, the GR surcharge value is saved, which is used if an A was stored for the associated market partner in the configurable field `DELIVERY_SURCHARGE`.
- **`DELIVERY_SURCHARGEB`**: In this environment variable, the GR surcharge value is saved, which is used if a B was stored for the associated market partner in the configurable field `DELIVERY_SURCHARGE`.
- **`DELIVERY_SURCHARGE_SP`**: In this environment variable, the name of the stored procedure is specified that is called from A+W Enterprise and decides whether this is a "small delivery".
- **`DELIVERY_SURCHARGE_TRACEPATH`**: This environment variable defines the path for the SP log. If this variable is not set, `/tmp` will be used as a path.
- **`REP_FAKTURA`**: In this environment variable, form types are defined that can only be output if they have been invoiced or booked. The individual form types in the listing are separate by pipes.

### 15.7. Installation instructions
Starting with version 3.2:
- Create tables `kleinlief`, `kleinliefkomm` and `kleinliefnein` (scripts: `/develop/alcib/4/1/de/install/xsql/4/1/0/...`).
- You have to enter at least one record in `kleinliefkomm` because a record has to be selected if no surcharge is applied.
- Install SP (`\\\\srvalcib\\globusr\\matthias\\kleinlief\\cu_fillkleinlief.sql`).

AWDesk case: 120144

## 16. Configuration of the ICE environment
The description of the installation and configuration of the ICE environment is in the system configuration instructions (`DE-CONFIG A+W Enterprise System.pdf` or `EN-CONFIG A+W Enterprise System.pdf`).

## 17. Document search
If you enter an entry date in the document search, documents `AB` are searched for on this date (`kauf.edat >= <Eingabe>`). Only if you leave the field empty does the search go back only 365 days.

