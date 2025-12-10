---
title: "EN-UM-AWEnterprise_3"
source: "EN-UM-AWEnterprise_3.pdf"
tags: ["A+W Enterprise", "Software Reference", "Master Data", "Market Partner Keys", "System Keys", "Product Keys", "ERP Configuration", "Technical Manual", "Discount Methods", "Complaint Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a detailed software reference guide for the A+W Enterprise system, focusing on the configuration of Master Data. It provides comprehensive instructions on setting up 'Market Partner Keys,' 'System Keys,' and 'Product Keys.' Key areas covered include calendar settings, country and language management, quality assessment scales, complaint reasons, and discount method definitions. This guide is intended for system administrators and technical users responsible for configuring and maintaining the core data structures of the A+W Enterprise software."
long_description: "This document serves as an in-depth technical manual for the A+W Enterprise software, specifically detailing the setup and management of various 'Keys' within the Master Data module. It is structured into three main parts: Market Partner Keys, System Keys, and Product Keys. The 'Market Partner Keys' section explains how to configure calendars (business days, production days), financial accounting clients, country codes, economic areas, and quality scales for assessing suppliers on metrics like dates, prices, and quantities. It also covers the setup for reasons for complaint and various discount methods, including detailed field descriptions for criteria, calculation, and application rules. The 'System Keys' section provides a comprehensive overview of system-wide settings, such as job titles, ZIP codes, language management, document types, quantity units, shape descriptions for manufacturing, and dispatch configurations (packing types, routes, vehicles, customs). The 'Product Keys' section details the configuration of product-specific attributes like color variants, dimension variants, size variants, and technical value groups for properties like sound protection and thermal transmission. This guide is essential for administrators and power users, offering technical information, database field names, and step-by-step instructions for ensuring the foundational data of the A+W Enterprise system is correctly configured."
---

# Market Partner Keys

---
### Monthly view

#### Descriptions of fields

- **Date**: Each individual date is displayed here.
- **Day**: Each individual day is displayed here.
- **CW**: The calendar week is displayed here.
- **H**: Here you can see whether or not this day is a business day for the main client. The main client-specific business days are maintained in System > Keys > Market Partner > Calendar and cannot be changed here.
- **PD**: Here you can see whether or not this day is a production day for the main client. The main client-specific production days are maintained in System > Keys > Market Partner > Calendar and cannot be changed here.
- **T-CL**: Selection of whether this is a business day.
  - **Technical info**: toggle field, DB field: alkal.htag
- **P CL**: Selection of whether this is a production day.
  - **Technical info**: toggle field, DB field: alkal.ptag
- **Remark**: You can store an appropriate remark in this field.
  - **Technical info**: alphanumeric field, DB field: alkal.bem

#### Additional information

⇨ "Calendar" on page B-194

## FinAc clients

**Master Data > Keys > Market Partner > FinAc Clients**

You specify the FinAc clients on this dialog. For additional information, please contact a service employee of A+W Software GmbH.

**Fig. B-68 FinAc clients**

| No | Area | Booking Range | Site Area | Notes |
| :--- | :--- | :--- | :--- | :--- |
| 1 | 11 | 20 | 6 Hessen | |
| 2 | 22 | 23 | 10 Saarland | |

## Countries

**Master Data > Keys > Market Partner > Countries > Countries**
**Master Data > Keys > Market Partner > Countries > Individual Descriptions**
**Master Data > Keys > Market Partner > Countries > All Descriptions**

This dialog contains the different countries that can occur when entering market partners, in the relevant languages.

**Fig. B-69 Countries**

### Descriptions of fields

- **CCd**: Country codes, e.g. A (Austria). To create a new country, enter the appropriate code.
  - **Technical info**: <F9>, DB field: xsprbez.cid
  - **View**: xland.kfz
- **IG**: Country code according to ISO standard, e.g. AT (Austria).
  - **Technical info**: alphanumeric field, DB field: xxland.iso
- **Country**: Description of the country, e.g. Belgium.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xland.atxt
- **FinAc**: This field contains the appropriate country code for financial accounting.
  - **Technical info**: alphanumeric field, DB field: xxland.fib
- **Intracode**: This field contains the appropriate specification of the Federal Statistical Office for intra-commercial statistics.
  - **Technical info**: alphanumeric field, DB field: xxland.fib
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz

## Economic area descriptions

**Master Data > Keys > Market Partner > Economic Areas > Individual Descriptions**
**Master Data > Keys > Market Partner > Economic Areas > All Descriptions**

The free division of the country into economic areas grants the later assignment of market partners to an economic area, regardless of the federal state.
This dialog contains the different economic areas that can occur when entering market partners, in the relevant languages.

**Fig. B-70 Economic areas**

### Descriptions of fields

- **Number/No**: Key number. To create a new economic area, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
  - **View**: xwrtraum.wrtnr
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description of the economic area, e.g. middle.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xwrtraum.wrtraum

## Areas/Counties

**Master Data > Keys > Market Partner > Areas/Counties > Individual Descriptions**
**Master Data > Keys > Market Partner > Areas/Counties > All Descriptions**

The areas entered here can be assigned to customers and suppliers in the market partner master data. The assignment of the key number should be done for the intra-trade statistics according to the appropriate specification of the Federal Statistical Office.
This dialog contains the different areas and counties, in the relevant languages.

**Fig. B-71 Areas/Counties**

### Descriptions of fields

- **Number/No**: Key number. To create a new region, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
  - **View**: xregion.regnr
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Area/County**: Description of the region, e.g. middle.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xregion.region

## General quality scale

**Master Data > Keys > Market Partners > Quality Scale > General > Quality Scales**
**Master Data > Keys > Market Partners > Quality Scale > General > Individual Descriptions**
**Master Data > Keys > Market Partners > Quality Scale > General > All Descriptions**

On these dialogs, you create the general quality characteristics with priorities and in different languages. These keys serve to assess the market partner and are used for all assessment criteria.

**Fig. B-72 Quality scale**

### Descriptions of fields

- **No**: Key number. To create a new quality, enter the next free number.
  - **Technical info**: numeric field, DB field: xxqual.qualkz
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description, e.g. very good quality
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
- **Rank**: The rank that the assessment occupies within the assessment scale.
  - **Technical info**: alphanumeric field, DB field: xxqual.rang

## Quality scale dates

**Master Data > Keys > Market Partners > Quality scale > Dates > Quality Scale Dates**
**Master Data > Keys > Market Partners > Quality Scale > Dates > Individual Descriptions**
**Master Data > Keys > Market Partners > Quality Scale > Dates > All Descriptions**

To assess the suppliers with regard to adherence to dates, free descriptions are created and scaled with a ranking.
The dialog shows you the keys created, which are available for manual assessment of the suppliers in the market partner master data.

**Fig. B-73 Quality scale dates**

### Descriptions of fields

- **No**: Key number To create a new key number, enter the next free number.
  - **Technical info**: numeric field, DB field: xsprbez.id
  - **View**: xtermin.terminkz
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Key description, e.g. on-time.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xtermin.atxt
- **Rank**: The rank that the assessment occupies within the assessment scale.
  - **Technical info**: alphanumeric field, DB field: xxtermin.rang

## Quality scale prices

**Master Data > Keys > Market Partners > Quality Scale > Prices > Qual. Scale Prices**
**Master Data > Keys > Market Partners > Quality Scale > Prices > Individual Descriptions**
**Master Data > Keys > Market Partners > Quality Scale > Prices > All Descriptions**

To assess the suppliers with regard to prices, free descriptions can also be created and scaled with a ranking.
The dialog shows you the keys created, which are available for manual assessment of the suppliers in the market partner master data.

**Fig. B-74 Quality scale prices**

### Descriptions of fields

- **No**: Key number To create a new key number, enter the next free number.
  - **Technical info**: numeric field, DB field: xsprbez.id
  - **View**: xpreis.preiskz
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Key description, e.g. cheap.
  - **Technical info**: alphanumeric field, DB field: xxpreis.atxt
- **Rank**: The rank that the assessment occupies within the assessment scale.
  - **Technical info**: alphanumeric field, DB field: xxpreis.rang
  - **View**: xpreis.atxt

## Quality scale quantities

**Master Data > Keys > Market Partners > Quality Scale > Quantity > Qual. Scale Qties.**
**Master Data > Keys > Market Partners > Quality Scale > Quantity > Individual Descriptions**
**Master Data > Keys > Market Partners > Quality Scale > Quantity > All Descriptions**

To assess individual suppliers' quantities supplied, free descriptions can also be created and scaled with a ranking.
The dialog shows you the keys created, which are available.

**Fig. B-75 Quality scale quantities**

### Descriptions of fields

- **No**: Key number To create a new key number, enter the next free number.
  - **Technical info**: numeric field, DB field: xsprbez.id
  - **View**: xmenge.mengekz
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Key description, e.g. good stock.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xmenge.atxt
- **Rank**: The rank that the assessment occupies within the assessment scale.
  - **Technical info**: alphanumeric field, DB field: xxmenge.rang

## Quality scale special

**Master Data > Keys > Market Partners > Quality Scale > Special > Qual. Scale Special**
**Master Data > Keys > Market Partners > Quality Scale > Special > Individual Descriptions**

The Special quality scale offers an additional possibility to assess suppliers using freely-definable descriptions to which a rank is assigned.
The dialog shows you the keys created, which are available.

**Fig. B-76 Quality scale special**

### Descriptions of fields

- **Number**: Key number. To create a new quantity level, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
  - **View**: xspec.speckz
- **Rank**: The rank that the assessment occupies within the assessment scale.
  - **Technical info**: alphanumeric field, DB field: xxspec.rang
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description of the quantity level, e.g. good stock.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xspec.atxt

## Reasons for complaint

**Master Data > Keys > Market Partners > Complaint > Reasons > Reasons for Complaint**
**Master Data > Keys > Market Partners > Complaint > Reasons > Individual Descriptions**
**Master Data > Keys > Market Partners > Complaint > Reasons > All Descriptions**

The complaint types are stored as text here and provided with a freely-selectable key. They are needed for recording and assessing complaints.
In addition, the codes of the business type for the intra-trade statistics are maintained in this table.

**Fig. B-77 Reasons for complaint**

### Descriptions of fields

- **No**: Key number To create a new key number, enter the next free number.
  - **Technical info**: numeric field, DB field: xxrart.reklamart
- **Reason for complaint**: Key description, e.g. defective packaging.
  - **Technical info**: alphanumeric field, DB field: xxrart.bez
- **Intrastat**: The code according to the specifications of the Federal Statistical Office.
  - **Technical info**: alphanumeric field, DB field: xxrart.intrageschart
- **No headings**: You can define both columns without headings individually using environment variables.
  - **Technical info**: alphanumeric field, DB field: xxrart.private_long1/2
- **C**: Closed ID.
  - **Technical info**: toggle field, DB field: xxrart.lustill
- **Number**: Selection of the key number. To create a new key number, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
  - **View**: rart.reklamart
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Reason for complaint**: Description of the reason for complaint, e.g. defective packaging.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: rart.atxt

## Places of complaint

**Master Data > Keys > Market Partners > Complaint > Places > Reason for Complaint**
**Master Data > Keys > Market Partners > Complaint > Places > Individual Descriptions**
**Master Data > Keys > Market Partners > Complaint > Places > All Descriptions**

The text specifications for the complaint place can be defined freely. They are significant for the complaint processing and statistics.

**Fig. B-78 Places of complaint**

### Descriptions of fields

- **Number**: Key number. To create a new place, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
  - **View**: rort.reklamort
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Reason for complaint**: Key description, e.g. production.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: rort.atxt
- **C**: Closed ID.
  - **Technical info**: toggle field, DB field: xxrart.still

## Types of complaint

**Master Data > Keys > Market Partners > Complaint > Types > Types for Complaint**
**Master Data > Keys > Market Partners > Complaint > Types > Individual Descriptions**
**Master Data > Keys > Market Partners > Complaint > Types > All Descriptions**

The complaint types are stored as text on these dialogs and provided with a freely-selectable key. They are needed for recording and assessing complaints.

**Fig. B-79 Types of complaint**

### Descriptions of fields

- **Number/No**: Type number. Enter the description in the next field. To create a new key number, enter the next free number.
  - **Technical info**: numeric field, DB field: xsprbez.id
  - **View**: xxrspec.reklamspec
- **Description/Type of Complaint**: Description of the type, e.g. breakage.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xspec.atxt
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **No headings**: You can define both columns without headings individually using environment variables.
  - **Technical info**: alphanumeric field, DB field: xxrspec.private_long1/2
- **C**: Closed ID.
  - **Technical info**: toggle field, DB field: xxrspec.still

## Discount methods

**Master Data > Keys > Market Partners > Process Discounts > Discount Methods > Discount Methods**
**Master Data > Keys > Market Partners > Process Discounts > Discount Methods > Individual Descriptions**
**Master Data > Keys > Market Partners > Process Discounts > Discount Methods > All Descriptions**

This dialog serves to define valid discount methods that are described with different characteristics and then defined as document and market partner-specific discounts. Information is stored in the discount method that is valid for the entire method.

**Fig. B-80 Discount methods**

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Discount methods.

### Description of the fields

- **Method**: Method number. To create a new method, select the next free number.
  - **Technical info**: numeric field, DB field: rabattmeth.methode
- **Name**: Name of the discount method, e.g. energy surcharge.
  - **Technical info**: alphanumeric field, DB field: rabattmeth.methodenname
- **Sequen.**: In case of several simultaneous discounts, controls the sequence in which the discounts are applied.
  - **Technical info**: numeric field, DB field: rabattmeth.seqnr
- **Criterion**: In this field, you specify which document criterion has to be fulfilled so that the discount of this method is effective:
  - 0: No dependency
  - 1: Rush order
  - 2: Route
  - 3. Disp.type
  - 4: Packing type
  - 5: Incoterm
  - 6: Destination
  - 7: Invoice country
  - 8: Online
  - 9: Special
  - 10: EDI
  - **Technical info**: numeric field, DB field: rabattmeth.qualfier
- **Cre.note**: With this field, you control how the discount is treated for credits:
  - **Yes**: The discount is taken over automatically in credits.
  - **No**: The discount is not taken over automatically in credits.
  - **Query**: You will be asked whether the discount should be taken over into the credit.
  - **Technical info**: toggle field, DB field: rabattmeth.gutschrift
- **Weight**: With this field you control how the discount is handled for credit notes.
  - Only inv. gls wt: The discount applies only for the invoiced glass weight.
  - Inv. gls wt: The discount applies for the invoiced glass weight.
  - Itm wgt: The discount refers to the item weight.
  - Only itm wgt: The discount refers only to the item weight.
  - Gls wt: The discount applies for the glass weight. If this is zero, the item weight is used.
  - Inv. itm wgt: The discountapplies to the invoiced item weight.
  - **Technical info**: toggle field, DB field: rabattmeth.glasgewicht
- **Shs**: With this checkbox, you can mark a discount method so that this method deactivates discounts for delivery note generation if there is already a delivery note within this delivery.
  - **Technical info**: toggle field, DB field: rabattmeth.lieferzuschlag
- **Rab**: With this field, you control whether later discounts apply to the discount of this discount:
  - **Yes**: The amount of this discount is considered in the basic amount for subsequent discounts.
  - **No**: The amount is not considered.
  - **Technical info**: toggle field, DB field: rabattmeth.rabattierbar
- **Nul**: With this field, you control whether for quantity calculations items with a zero amount are considered.
  - **Yes**: Items with zero amount are considered.
  - **No**: Items with zero amount are not considered.
  - **Technical info**: toggle field, DB field: rabattmeth.nullpositionen
- **Gen**: With this field, you control whether this discount method can be maintained on a general level.
  - **Yes**: This method can be maintained on a general level.
  - **No**: This method cannot be maintained on a general level.
  - **Technical info**: toggle field, DB field: rabattmeth.allgemein
- **P.**: With this field, you control whether this discount method can be maintained on a market partner level.
  - **Yes**: This method can be maintained on a market partner level.
  - **No**: This method cannot be maintained on a market partner level.
  - **Technical info**: toggle field, DB field: rabattmeth.marktpartner
- **Prj**: With this field, you control whether this discount method can be maintained on a project level.
  - **Yes**: This method can be maintained on a project level.
  - **No**: This method cannot be maintained on a project level.
  - **Technical info**: toggle field, DB field: rabattmeth.objekt
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz

## Discounts

**Master Data > Keys > Market Partners > Process Discounts > Discount Methods > Discounts**

In the discount methods, information is stored that is valid for the entire method. These discounts should not be understood as concrete discount, but rather as a particular grouping of discounts such as energy surcharge or rush surcharge. In the following, no distinction is made between the terms surcharge and discount. The term more comprehensible in the respective context will be used. You define the specific discounts that are generally valid or valid for market partners here:

⇨ "Discounts" on page B-149

The dialog consists of the tabs:
- General
- Details

### Descriptions of fields

- **Method**: Selection of the discount method. The appropriate codes can be assigned via the Discount Methods (Codes > Market Partner > Process Discounts) menu.
  - **Technical info**: <F9>, DB field: rabstamm.methode
- **Name**: Name of discount method. This entry can be overwritten here.
  - **Technical info**: alphanumeric field, DB field: rabstamm.rabatttext
- **Criterion**: The criterion stored for the method is displayed here.
  - **Technical info**: <F9>, DB field: rabstamm.qualifierwert
- **Type**: Type of discount method:
  - **Sales**: Sales-related discount.
  - **Costs**: Cost-related discount.
  - **Purchasing**: Purchasing-related discount (only in the Purchasing menu).
  - **Technical info**: toggle field, DB field: rabstamm.ekvkkz
- **Prdgrp**: Product group of the discount method. The discount method only affects the products in this product group in the order.
  - **Technical info**: <F9>, DB field: rabstamm.wgrnr
- **Value**: The value specified is interpreted differently depending on the discount type and is used for calculation of the discount amount.
  - **Technical info**: numeric field, DB field: rabstamm.wert
- **Record type (column without header)**: The value specified is interpreted differently depending on the discount type and is used for calculation of the discount amount. Possible values are:
  - **+**: Surcharge
  - **-**: Discount
  - **Technical info**: numeric field, DB field: rabstamm.satzart
- **DiscTpe**: Via the discount type, you specify according to what the discount amount should be calculated.
  - **GR**: Fixed value
  - **%**: Percentage
  - **GR/unit**: Value per unit
  - **GR/sqm**: Value per sqm of glass
  - **GR/kg**: Value per kilogram of glass
  - **%SA**: Cost discount based on the sales amount. This discount is calculated with the basis value of the sales order
  - **%Cst**: Sales discount based on the costs. This discount is calculated with the basis value of the cost amount.
  - **GR/W*D**: Value per weight in kg multiplied by the distance in km. This discount is only applied if the distance was stored in the addresses or the market partner.
  - **Technical info**: numeric field, DB field: rabstamm.rabattart
- **Itm**: With this checkbox, you control whether or not the discount entered is redistributed across the individual items.
  - The discount is redistributed to the individual items.
  - The discount is not redistributed.
  - **Technical info**: toggle field, DB field: rabstamm.verteil

### Discounts - details

**Master Data > Keys > Market Partners > Process Discounts > Discounts > Details <F2>**

**Fig. B-82 Discounts, Details tab**

#### Descriptions of fields

- **Method**: Selection of the discount method. The appropriate codes can be assigned via the Discount Methods (Codes > Market Partner > Process Discounts) menu.
  - **Technical info**: <F9>, DB field: rabstamm.methode
- **Name**: Name of discount method. This entry can be overwritten.
  - **Technical info**: alphanumeric field, DB field: rabstamm.rabatttext
- **Criterion**: The criterion stored for the method is displayed here.
  - **Technical info**: <F9>, DB field: rabstamm.qualifierwert
- **Type**: Type of discount method:
  - **Sales**: Sales-related discount.
  - **Costs**: Cost-related discount.
  - **Purchasing**: Purchasing-related discount (only in the Purchasing menu).
  - **Technical info**: toggle field, DB field: rabstamm.ekvkkz
- **Prod. group**: Product group of the discount method. The discount method only affects the products in this product group in the order.
  - **Technical info**: <F9>, DB field: rabstamm.wgrnr
- **Discount value**: The value specified is interpreted differently depending on the discount type and is used for calculation of the discount amount.
  - **Technical info**: numeric field, DB field: rabstamm.wert
- **Scaling basis**: Selection of the scaling basis. If you specify a scaling basis, you must then apply the scaling levels with <F5>:
  - qm - square meters of glass
  - kg - kilograms of glass
  - km - kilometers
  - Pc. - pieces
  - GR - value
  - **Technical info**: <F9>, DB field: rabstamm.staffelbasis
- **Minimum value**: Minimum discount total.
  - **Technical info**: numeric field, DB field: rabstamm.minbetrag
- **Maximum value**: Maximum discount total.
  - **Technical info**: numeric field, DB field: rabstamm.maxbetrag

> **Minimum or maximum amount only in 1st partial document**
> If surcharges are calculated on the basis of Qm/kg/Stück/%, and for this a minimum or maximum amount is specified, it is recommended that you have the surcharges calculated only as "in 1st partial document". Since due to limiting amounts there can be differences between the confirmed surcharge in the order and the total of the surcharges from the individual partial delivery notes, the surcharge should be defined and calculated as "only in the 1st partial document" and thus no longer considered in all remaining partial documents.
> ⇨ "Partial document" on page B-232

- **Redistribute**: Redistribution of the discount to the items. By means of redistribution, the discounts are distributed to the respective item and automatically transmitted to FinAc by the program. If you do not use redistribution, you must manually transmit the discounts to FinAc. For this purpose, you must transmit the information from the Stat. product group and Cost center fields to FinAc.
  - The discount is redistributed to the individual items.
  - The discount is not redistributed.
  - **Technical info**: toggle field, DB field: rabstamm.verteil
- **Stat. product group**: This field is only active if the current record is not marked as redistributable. Then a statistical product group must be specified for statistics bookings.
  - **Technical info**: <F9>, DB field: rabstamm.statwgrnr
- **Cost center**: This field is only active if the current record is not marked as re-distributable. Then a cost center must be specified to which the booking should be made.
  - **Technical info**: <F9>, DB field: rabstamm.kstelle
- **Account**: This field is only active if the current record is not marked as redistributable. Then an account must be specified to which the booking should be made.
  - **Technical info**: <F9>, DB field: rabstamm.konto
- **Discount valid from**: Date from which the discount should be used.
  - **Technical info**: numeric field, DB field: rabstamm.gueltigvon
- **Discount valid to**: Date until which the discount should be used. With appropriate system configuration, you can activate the validity check during order entry. The configuration permits the following possibilities:
  - There is a check whether discounts expired in the last X days (the number of days can also be configured).
  - There is a check whether the discounts expired in the past and a message is also output about whether there are also discounts that expire today.
  - It is only reported if discounts are determined that expire today.
  - **Technical info**: numeric field, DB field: rabstamm.gueltigbis
- **Partial document**: For discounts of the type GR, it must be decided how the program proceeds for the generation of partial delivery notes or partial invoices. The discount is either taken over into the first partial document, taken over in all partial documents or transformed into a percentage discount. Possible values are:
  - **in 1. Pd**: Discount is taken over into the first partial document.
  - **in all Pd**: Discount is taken over into all partial document.
  - **proportion**: There is a transformation into a proportional discount.
  - **Technical info**: numeric field, DB field: rabstamm.fixerabatte
- **VAT**: Selection of the VAT rate. This field is only active if the current record is not marked as redistributable. The assignment to the value added tax rates only has an effect if the logic is activated for several value added taxes in the system.
  - **Technical info**: <F9>, DB field: rabstamm.steuerzu
- **Cash D.-able**: The checkbox is only active if discounts are not redistributable. The flag does not affect discounts of the type Costs.
  - The discount is cash discountable.
  - The discount is not cash discountable.
  - **Technical info**: toggle field, DB field: rabstamm.skonto
- **openTRANS - Id**: This field allows the assignment of discounts from purchasing orders that were received from OpenTRANS.
  - **Technical info**: numeric field, DB field: rabstamm.otrabattid
- **Glazing**: The glazing flag is only evaluated for percentage discounts. There, the total of the glazing amounts of the items is used as basic value. On the cost side, glazing discounts always have an amount of 0.
  - The discount only applies to glazing.
  - The discount applies to everything.
  - **Technical info**: toggle field, DB field: rabstamm.verglkz
- **Glass weight**: With this field, you can control to which weight the discount should refer. This information overrides the information from the method master data, so that discounts of a method can now have different reference weights. The glass weight influences the basic value of the discount type GR/ kg and the drawing of the scaling level within the processes.
  - **Itm wgt**: Item weight.
  - **Only glass wt.**: Only glass weight.
  - **Glass wt.**: Glass weight
  - **Inv. itm wgt.**: Invoiced item weight.
  - **Only inv. gls wt**: Only invoiced glass weight.
  - **Inv. glass wt.**: Invoiced glass weight.
  - **Technical info**: toggle field, DB field: rabstamm.glasgewicht
- **Min. amount for zero**: With this checkbox, you can decide that the minimum amount is also drawn if the calculated amount is 0.0 GR.
  - The discount is redistributed to the individual items.
  - The discount is not redistributed to the individual items.
  - **Technical info**: toggle field, DB field: rabstamm.minbeinullbetragk
- **SP call**: Flag that indicates whether the stored procedure rabattanpassung must be called, which adjusts the discount for each individual process.
  - The SP must be called.
  - The SP is not called.
  - **Technical info**: toggle field, DB field: rabstamm.spaufrufkzkauf
- **Item**: Flag that indicates whether the stored procedure rabattzuord should be called, which then decides which process items are considered by this discount and which are not.
  - The SP is called.
  - The SP is not called.
  - **Technical info**: toggle field, DB field: rabstamm.spaufrufkz
- **Discount - Id center**: This variable controls the replication of the data from the central office to the corresponding site.
  - **Technical info**: toggle field, DB field: rabstamm.rabattidz
- **Discount-Id**: Unique assignment to the discount rate.
  - **Technical info**: numeric field, DB field: rabstamm.rabattid

## Site specific master data

**Master Data > Keys > Market Partners > Site Specific Details**

On this dialog, you can store the site-specific details for market partners. The dialog is only active if you are working with the multi-site system.

**Fig. B-83 Site specific master data**

### Descriptions of fields

- **Partn.type**: Selection of the partner type.
  - **Technical info**: toggle field, DB field: mpmdzu.kuliflag
- **Partners**: Selection of the market partner.
  - **Technical info**: <F9>, DB field: mpmdzu.mpnr
- **Site**: Selection of the site number. The name is displayed in the next field.
  - **Technical info**: <F9>, DB field: mpmdzu.hnr
- **Sales rep.**: Selection of the relevant sales representative. The respective commission rates for the representative entered here can be booked and they are ready for invoicing. The name is displayed in the next field.
  - **Technical info**: <F9>, DB field: mpmdzu.lager
- **Debtor conditions**: Selection of the customer number whose conditions should apply for the documents entered.
  - **Technical info**: <F9>, DB field: mpmdzu.konddebnr

# System Keys

**Master Data > Keys > System**

Values for various areas are defined here; these will be available for selection later on.
For example, the licensed language is entered, which is required for report generation in various languages.
You have access to the following areas:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a a/b | Item | ⇨ "Job titles" on page B-238 |
| b | Zip Codes | ⇨ "Zip codes" on page B-239 |
| C | Languages | ⇨ "Languages" on page B-241 |
| d a/b | Text additions | ⇨ "Text additions" on page B-244 |
| e | Document Types | ⇨ "Document types" on page B-245 |
| f a/b | Quantity units | ⇨ "Quantity units" on page B-247 |
| g a | Shapes - edge allocation | ⇨ "Edge allocation" on page B-249 |
| g b/c | Shapes | ⇨ "Shape descriptions" on page B-251 |
| h | Production area | ⇨ "Production area" on page B-253 |
| i a | Dispatch - packing type | ⇨ "Packing type" on page B-254 |
| i b | Dispatch - rack packing types | ⇨ "Rack packing types" on page B-255 |
| i c | Dispatch - dispatch type | ⇨ "Dispatch type" on page B-256 |
| i d | Dispatch - supply types | ⇨ "Incoterms" on page B-258 |
| i e a | Dispatch - routes | ⇨ "Routes" on page B-259 |
| i e b | Dispatch - route plan | ⇨ "Route plan" on page B-263 |
| i f a/b | Dispatch - dispatch regions | ⇨ "Dispatch areas-descriptions" on page B-264 |
| i g | Dispatch - vehicles | ⇨ "Vehicles" on page B-265 |
| i h | Dispatch - customs exit | ⇨ "Customs exit" on page B-266 |
| i i | Dispatch - destin. customs | ⇨ "Customs destination office" on page B-268 |
| i j | Dispatch - dispatch groups | ⇨ "Dispatch groups" on page B-269 |
| j a/b | Rack status | ⇨ "Rack status descriptions" on page B-270 |
| k a a/b | PMO - rack groups | ⇨ "Rack groups descriptions" on page B-271 |
| k a a/b | PMO - packing methods | ⇨ "Packing methods descriptions" on page B-272 |
| k c | PMO - rack Packing Allocation | ⇨ "Rack packing allocation" on page B-273 |
| l | Currency | ⇨ "Currency" on page B-274 |
| m a | Taxes - tax types | ⇨ "Tax types" on page B-277 |
| m b | Taxes - tax rates | ⇨ "Tax rates" on page B-279 |
| n | Payment terms | ⇨ "Payment type descriptions" on page B-280 |
| o a | Cash discount groups | ⇨ "Cash discount groups" on page B-282 |
| o b/c | Cash discount group names | ⇨ "Cash discount groups" on page B-284 |
| p | End of period | ⇨ "End of period" on page B-285 |
| q a/b | Adhocsql groups | ⇨ "Adhoc SQL group descriptions" on page B-286 |
| r | Report texts | ⇨ "Report texts" on page B-287 |
| s a | Companies/Corporations | ⇨ "Companies" on page B-289 |
| s b | Companies/corporations - company assignment | ⇨ "Company allocation" on page B-290 |

## Job titles

**Master Data > Keys > System > Job Tittle > Individual Descriptions**
**Master Data > Keys > System > Job Tittle > All Descriptions**

On this dialog, you define the positions of the employees at the company. They serve later for the master data entry as specification of the employee's position.

**Fig. B-84 Job titles**

### Descriptions of fields

- **Number/No**: Key number. To create a new position, enter the next free number.
  - **Technical info**: numeric field, DB field: xsprbez.id
  - **View**: xpos.posnr
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Name of the position, e.g. Managing Director.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xpos.atxt

## Zip codes

**Master Data > Keys > System > ZIP Codes**

On this dialog, you can store all zip codes that you need later during order entry. The zip codes stored here make entering addresses easier.
In the Select fields area, you can enter search criteria and thus limit the number of hits. Without a search quantity, all zip codes will be displayed. * stands for all entries.
In the lower area you can correct the details or add new entries.

**Fig. B-85 Zip codes**

### Descriptions of fields for selection

- **ZIP code**: Selection and entry of the zip code as search value. You can enter the whole zip code or only part of it. * stands for all.
  - **Technical info**: <F9>, DB field: xplzk.plz
- **City**: Selection and new specification of the city as search value. You can enter the whole city or only part of it. * stands for all.
  - **Technical info**: <F9>, DB field: xplzk.ort
- **Country**: Entry of the country as search value. You can enter the whole country or only part of it. * stands for all.
  - **Technical info**: <F9>, DB field: xplzk.kfz
- **Dispatch region**: Selection of the dispatch region as search value. You can enter the dispatch region or select it with <F9>. Dispatch regions are in the menu element by the same name Master Data > Keys > System > Dispatch. -1 stands for no selection.
  - **Technical info**: <F9>, DB field: xplzk.vsregion

### Descriptions of fields for the hit quantity

- **PostCod**: ZIP code. To create a new zip code, insert a new line.
  - **Technical info**: numeric field, DB field: xplz.plz
- **City**: The city that belongs to the zip code.
  - **Technical info**: alphanumeric field, DB field: xplz.ort
- **CCd**: The country code that belongs to the zip code.
  - **Technical info**: alphabetic field, DB field: xplz.kfz
- **Dispatch region**: Selection of the dispatch region with <F9>. The dispatch region is displayed in the next field. Dispatch regions are in the menu element by the same name Master Data > Keys > System > Dispatch.
  - **Technical info**: numeric field, DB field: xplz.vsregion

## Languages

**Master Data > Keys > System > Languages**

This dialog is used to manage the licensed languages. The languages are defined with a language ID. It serves to print out customer reports in the local language and to be able to assign each market partner its own languages.
The number can be assigned freely. However, in a corporate group with several databases, the number assignment has to be uniform.

The following example should make this clearer:
A corporate group headquartered in France has branches in Germany, England, and Italy. Both the central office and the branches have customers in other countries in Europe.

| Branch | has customer in |
| :--- | :--- |
| Central office: France | France<br>Germany<br>Italy |
| Branch: Germany | Denmark<br>Germany<br>Netherlands |
| Branch: England | England |
| Branch: Italy | Germany<br>Greece<br>Italy<br>Slovenia |

> **Inter-country order transfer**
> So that an inter-country order transfer is possible within a corporate group, the ID number of a licensed language has to be the same company-wide. The report language number depends on the design of the report and has to be selected accordingly.

The following table shows how the languages can be created in the central office and the branches:

| A+W Enterprise database | has customers in | Licensed languages | No | Language |
| :--- | :--- | :--- | :--- | :--- |
| Central office: France | France | French | 1 | 1 |
| | Germany | German | 2 | 2 |
| | Italy | Italian | 3 | 3 |
| | Spain | Spanish | 4 | 4 |
| | | Danish | 5 | |
| | | English | 6 | |
| | | Greek | 7 | |
| | | Slovenian | 8 | |
| | | Dutch | 9 | |
| Branch: Germany | Denmark | Danish | 5 | 1 |
| | Germany | German | 2 | 2 |
| | Netherlands | Dutch | 9 | 3 |
| Branch: England | England | English | 6 | 1 |
| Branch: Italy | Germany | German | 2 | 1 |
| | Greece | Greek | 7 | 2 |
| | Italy | Italian | 3 | 3 |
| | Slovenia | Slovenian | 8 | 4 |

### Descriptions of fields

- **No**: Language ID. To create a new language ID, select the next free number.
  - **Technical info**: numeric field, DB field: xplz.sprkz
- **Language**: Name of the language, e.g. German.
  - **Technical info**: alphabetic field, DB field: xsprzu.atxt
- **Report lang.**: Selection of the language in which the report should be output.
  - **Technical info**: numeric field, DB field: xsprzu.repsprkz
- **AWE language**: Selection of the language in which the program is displayed. The language ID appears in the next field.
  - **Technical info**: numeric field, DB field: xsprzu.alenvsprkz

## Text additions

**Master Data > Keys > System > Text Additions > Individual Descriptions**
**Master Data > Keys > System > Text Additions > All Descriptions**

The text additions serve to provide text for articles and products during order entry and the generation of reports. For more information about the precise use of these text additions, see the A+W Enterprise configuration instructions.

**Fig. B-88 Text additions**

### Descriptions of fields

- **Number**: Key number. To create a new text, enter the next free number.
  - **Technical info**: <F9>, DB field: xzustxt.txtnr
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xzustxt.txtnr
- **Text constant**: Description of the text, e.g. horizontal.
  - **Technical info**: alphanumeric field, DB field: xzustxt.zustxt

## Document types

**Master Data > Keys > System > Document Types**

On this dialog, you can store various document types and the type of output. For declaration(s) of performance, the document type Declaration of performance has been fixed which is firmly linked with Document type 1.
The Output Type defines whether or not a market partner should receive the selected type via e-mail. The e-mail sending requires additional system-wide settings and configuration.

**Fig. B-89 Document types**

### Descriptions of fields

- **Tpe**: Key number To create a new key number, select the next free number.
  - **Technical info**: numeric field, DB field: xdokutype.dokuart
- **Description**: Description of the document type, e.g. declaration of performance.
  - **Technical info**: alphabetic field, DB field: xdokutype.dokubez
- **Document type**: Assignment to a document type.
  - **Technical info**: alphabetic field, DB field: xdokutype.dokutyp
- **Output type**: Use this field to control the output type. For the declaration of performance, this field is pre-populated with e-mail:
  - **none**: The market partner receives no declaration of performance.
  - **via e-mail**: The market partner receives the declaration of performance via e-mail.
  - **Technical info**: toggle field, DB field: xdokutype.ausgabeart
- **CF**: With this field, you control whether the data in the document should be taken over:
  - The data should be taken over.
  - The data should not be taken over.
  - **Technical info**: toggle field, DB field: xdokutype.vorgangflag
- **Prod**: With this field, you control whether the data should be transferred to production:
  - The data should be taken over.
  - The data should not be taken over.
  - **Technical info**: toggle field, DB field: xdokutype.prodflag

## Quantity units

**Master Data > Keys > System > Quantity Units > Individual Descriptions**
**Master Data > Keys > System > Quantity Units > All Descriptions**

You define the quantity units on this dialog.

**Fig. B-90 Quantity units**

### Descriptions of fields

- **Number/No**: Selection of the key number. To create a new quantity unit, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
  - **View**: xme.symb
- **Lng**: Selection of the language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Abbr**: Abbreviation of the quantity unit, e.g. mtr.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xme.kurzbez
- **Description**: Description of the quantity unit, e.g. meters.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez2
  - **View**: xme.atxt
- **Dimension**: Dimension of the quantity unit, e.g. linear meters (LM)
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez3
  - **View**: xme.dim

## Edge allocation

**Master Data > Keys > System > Shapes > Edge Allocation**

On this dialog, you specify how the shape edges are interpreted for circumscribing rectangles. For shape 7 (figure above), e.g., the diagonal edge is treated as the height.

**Fig. B-91 Edge allocation**

### Descriptions of fields

- **Shape**: Selection of the shape number for which the price-relevant edge should be defined. The description is displayed in the next field.
  - **Technical info**: <F9>, DB field: modkparam.modnr
- **Edge**: For this edge, it should be defined whether it should be entered in the price calculation as height or width.
  - **Technical info**: numeric field, DB field: modkparam.kante
- **Calculat.**: Defines how the edge goes into the price calculation:
  - 0: no calculation
  - 1: as height
  - 2: as width
  - 3: as height + width
  - 4: 2x height + width
  - 5: height + 2x width
  - 6: 2x height + 2x width
  - **Technical info**: toggle field, DB field: modkparam.berechnung
- **SE**: With this field, you control whether the edge to be processed is a shape edge.
  - This edge is a shape edge.
  - This edge is not a shape edge.
  - **Technical info**: alphanumeric field, DB field: modkparam.modellkante

## Shape descriptions

**Master Data > Keys > System > Shapes > Individual Descriptions**
**Master Data > Keys > System > Shapes > All Descriptions**

On this dialog, you store the designations for the shapes to be processed. The texts stored here for the shapes are required both in order entry and for customers papers and the creation of the lite labels.

> **Available shapes**
> Which shapes are available here depends on the Catalog type system setting.

**Fig. B-92 Individual shape descriptions/shape catalog**

### Descriptions of fields

- **No**: Selection of the shape number. The shape number corresponds to the shapes in the A+W shape catalog or the shape catalog that was set up during installation.
  - **Technical info**: <F9>, DB field: modkparam.modnr
- **Language**: Selection of the language ID.
  - **Technical info**: <F9>, DB field: modelle.sprkz
- **Description**: The shape description corresponds to the shapes in the A+W shape catalog or the shape catalog that was set up during installation.
  - **Technical info**: alphanumeric field, DB field: modelle.bez
- **Print descript.**: The print description can be changed if necessary.
  - **Technical info**: alphanumeric field, DB field: modelle.drubez
- **Inp**: With this field, you control whether or not the shape can be entered. It can happen that you are working with the A+W shape catalog, but the shapes are not cut at your company.
  - **Y**: The shape number can be entered.
  - **N**: The shape number cannot be entered.
  - **Technical info**: toggle field, DB field: modelle.erfassbar
- **Online**: This field is relevant for online entries. With it, you control whether or not the shape can be entered online.
  - **Y**: The shape number can be entered online.
  - **N**: The shape number cannot be entered online.
  - **Technical info**: toggle field, DB field: modelle.online
- **Edges**: Number of edges.
  - **Technical info**: numeric field, DB field: modelle.kantanz

## Production area

**Master Data > Keys > System > Production Area**

This dialog serves to define individual production areas that can be assigned in order entry.

**Fig. B-93 Production area**

### Descriptions of fields

- **No**: Number of the production area.
  - **Technical info**: numeric field, DB field: xpbbereich.bereich
- **Area description**: Description of the production area, e.g. screen printing.
  - **Technical info**: alphanumeric field, DB field: xpbbereich.bez

## Packing type

**Master Data > Keys > System > Dispatch > Packing Type**

On this dialog, you specify the packing types in the respective languages. This way, they can be output in the local language on customer papers.

**Fig. B-94 Packing types**

### Descriptions of fields

- **No**: The key number can be assigned freely. The same number should be assigned several times if the packing type is created in several languages. In this case, the number remains the same; the Language ID and Description change.
  - **Technical info**: numeric field, DB field: xverpack.verpnr
- **Description**: Description of the packing type.
  - **Technical info**: alphanumeric field, DB field: xverpack.atxt
- **mm**: Depending on the configuration, enter the thickness (in mm) of the packing material between two lites here. This entry is optional.
  - **Technical info**: numeric field, DB field: xverpack.vdick
- **Language**: Selection of the language. The selected language is displayed in the next field.
  - **Technical info**: <F9>, DB field: xverpack.sprkz

## Rack packing types

**Master Data > Keys > System > Dispatch > Rack Packing Types**

On this dialog, you can assign different packing types to a dispatch type (e.g. forwarding agency) depending on the destination country. The use of this function can be configured specially. For additional information, please contact a A+W Software GmbH employee.

**Fig. B-95 Rack packing types**

### Descriptions of fields

- **Disp. type**: Selection of the dispatch type, e.g. forwarding agency. The name is displayed in the next field. The appropriate codes can be assigned via the Dispatch Type (Master Data > Keys > System > Dispatch) menu.
  - **Technical info**: numeric field, DB field: gverpack.versnr
- **CCd**: Selection of the country code, e.g. D. The name is displayed in the next field. The appropriate codes can be assigned via the Countries (Master Data > Keys > Market Partner > Countries) menu.
  - **Technical info**: alphabetic field, DB field: gverpack.kfz
- **Packing type**: Selection of the packing type, e.g. L rack. The name is displayed in the next field. The appropriate codes can be assigned via the Dispatch Type (Master Data > Keys > System > Dispatch) menu.
  - **Technical info**: numeric field, DB field: gverpack.verpnr

### Additional information

- ⇨ "Countries" on page B-203
- ⇨ "Packing type" on page B-254
- ⇨ "Dispatch type" on page B-256

## Dispatch type

**Master Data > Keys > System > Dispatch > Dispatch Type**

On this dialog, you specify the dispatch types in the respective languages. This way, the dispatch type can be output in the local language on customer papers.

**Fig. B-96 Dispatch types**

### Descriptions of fields

- **No**: The key number can be assigned freely. The same number can be assigned several times if the packing type should be created in several languages. In this case, the number remains the same; the Language ID and Description change.
  - **Technical info**: numeric field, DB field: xversand.versnr
- **Description**: Description of the packing type in the respective language.
  - **Technical info**: alphanumeric field, DB field: xversand.atxt
- **Route**: The selection of a route is optional. The route is displayed in the next field.
  - **Technical info**: <F9>, DB field: xversand.routenr
- **TrMo**: Selection of the code for the transport branch according to the specifications of the Federal Statistitical Office. The description is displayed in the next field.
  - **Technical info**: <F9>, DB field: xversand.intraverkehr
- **Transp. surcharge**: The transport surcharge in percent is an estimated value that is required for the correction of the statistical value.
  - **Technical info**: numeric field, DB field: xversand.intrasatz
- **Language**: Selection of the language. The selected language is displayed in plain text in the next field.
  - **Technical info**: <F9>, DB field: xversand.sprkz

## Incoterms

**Master Data > Keys > System > Dispatch > Incoterms > Individual Descriptions**
**Master Data > Keys > System > Dispatch > Incoterms > All Descriptions**

This dialog shows you the defined incoterms in the respective languages. This way, they can be output in the local language on customer papers.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Incoterms.

**Fig. B-97 Incoterms**

### Descriptions of fields

- **No/Incoterm**: The key number can be assigned freely. The same number can be assigned several times if the packing type should be created in several languages. In this case, the number remains the same; the Language ID and Description change.
  - **Technical info**: numeric field, DB field: xlart.lanr
- **Description**: Description of the incoterm in the respective language.
  - **Technical info**: alphanumeric field, DB field: xlart.labez
- **Lng**: Selection of the language (language ID).
  - **Technical info**: <F9>, DB field: xsprbez.sprkz

## Routes

**Master Data > Keys > System > Dispatch > Routes > Routes > Route Details I**
**Master Data > Keys > System > Dispatch > Routes > Routes > Individual Descriptions**
**Master Data > Keys > System > Dispatch > Routes > Routes > All Descriptions**

The delivery paths are described in the route management. This way, a delivery route can be assigned and considered during calculation of the delivery date.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Routes.

**Fig. B-98 Routes**

### Descriptions of fields

- **Route**: Unique route number.
  - **Technical info**: numeric field, DB field: route.routenr
- **Route description**: The description of the route.
  - **Technical info**: alphanumeric field, DB field: route.routename
- **Abbrev.**: Abbreviation of the route.
  - **Technical info**: alphanumeric field, DB field: route.kurzbez
- **Travel days**: Selection of the travel days (Mo-Su).
  - **Technical info**: <F9>, DB field: route.routentag
- **Depart.**: Departure time for the route.
  - **Technical info**: numeric field, DB field: route.abfahrt
- **AIRte**: The alternative route refers to another line of the same table in which an alternative to the current route is located. It is used with locking of this route.
  - **Technical info**: numeric field, DB field: route.aroutenr
- **Reas.**: Selection of the route type:
  - **Route**: Route with several delivery points.
  - **Direct**: Goods are delivered directly by the pre-supplier.
  - **Pick-up**: Goods will be picked up by the customer.
  - **Backlog**: Goods are on backlog (planning route).
  - **Internal**: Route between two affiliated companies (viaPlant).
  - **Special**:
  - **Opti**: Optimization route that is created if you are using the A+W Logistics Optimizer.
  - **VWB direct**: Route type for the extended workbench
  - **Clarification**: This route type is used in A+W Enterprise Experience Dispatch.
  - **Technical info**: <F9>, DB field: route.routenkz
- **Site**: Selection of the site number to which the route belongs. The field has the following meaning:
  - In an A+W Enterprise instance where several sites are managed, the Site-no. specifies from which site a route is driven.
  - If an order with direct delivery is transferred between two affiliated A+W Enterprise instances, where in the receiving site the route is compared to the own route master. The direct route is selected whose site no. matches the site number of the sending site. In this case, the Siteno. specifies for which site a direct delivery should occur.
  - If for a route the field is empty and the system is configured for global routes, then this route is designated as global. Global routes can be used at all sites, e.g., in case of postponement. However, no new orders can be entered on such routes.
  - **Technical info**: <F9>, DB field: route.hausnr
- **Reg/Site**: Selection of the region to which the route belongs. The appropriate codes can be assigned via the Dispatch Regions (Master Data > Keys > System > Dispatch) menu.
  - **Technical info**: <F9>, DB field: route.region
- **Prio**: Entry of the priority within a region for via plant.
  - **Technical info**: numeric field, DB field: route.prio
- **TT**: Entry of the travel time in hours.
  - **Technical info**: numeric field, DB field: route.fahrtzeit
- **Cal**: With this field, you control whether or not the calendar should be evaluated.
  - The calendar is evaluated.
  - The calendar is not evaluated.
  - **Technical info**: toggle field, DB field: route.mitkalender
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz

### Additional information

⇨ "Route details II" on page B-262

## Route details II

**Master Data > Keys > System > Dispatch > Routes > Routes > F2**

The fields on this dialog are identical to the fields of the Route Details I dialog, with the exception of the Dispatch Type field.

> **Route Details II**
> By default, the Route Details II tab is hidden. It can be released by an A+W Software GmbH employee.

**Fig. B-99 Route Details**

### Descriptions of fields

- **Dispatch type**: Selection of the dispatch type. The appropriate codes can be assigned via the Dispatch Type (Master Data > Keys > System > Dispatch) menu. The description of the dispatch type is displayed in plain text in the next field.
  - **Technical info**: <F9>, DB field: route.versnr

### Additional information

⇨ "Routes” on page B-259

## Route plan

**Master Data > Keys > System > Dispatch > Routes > Route Plan**

On this dialog, you create the precise departure times for the individual routes. Thus you can define the different departure times for a route that is driven twice a day, for example. You can assign the customer order to the route plan accordingly.

**Fig. B-100 Route plan**

### Descriptions of fields

- **Route**: Selection of the route number. The selected route is displayed in the next field.
  - **Technical info**: <F9>, DB field: tourplan.routenr
- **Date**: Date on which the tour is driven.
  - **Technical info**: alphanumeric field, DB field: tourplan.tourdate
- **Depart**: Departure time for the route.
  - **Technical info**: alphanumeric field, DB field: tourplan.tourdate

## Dispatch areas-descriptions

**Master Data > Keys > System > Dispatch > Dispatch Area > Individual Descriptions**
**Master Data > Keys > System > Dispatch > Dispatch Area > All Descriptions**

On this dialog, you define the individual dispatch regions in the different languages.

**Fig. B-101 Dispatch areas-descriptions**

### Descriptions of fields

- **Number**: Key number. To create a new dispatch region, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
- **Language**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description of the dispatch region, e.g. Bavaria.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1

## Vehicles

**Master Data > Keys > System > Dispatch > Vehicles**

On this dialog, you store all vehicles that are available for delivery of the goods.

**Fig. B-102 Vehicles**

### Descriptions of fields

- **Vehicle**: Key number of the vehicle. To create a new key number, select the next free number.
  - **Technical info**: numeric field, DB field: Ikw.lkwnr
- **Veh. code**: Official license plate of the vehicle.
  - **Technical info**: alphanumeric field, DB field: Ikw.kennz
- **Vehicle type**: Selection of the vehicle type:
  - Truck
  - Semitrailer
  - Trailer
  - **Technical info**: toggle field, DB field: Ikw.art
- **Description**: This is a free-form name used at the company for the vehicle. It appears in the dispatch control.
  - **Technical info**: alphanumeric field, DB field: Ikw.bezeichnung
- **Tonnage**: The tonnage of the vehicle is entered here. It serves only informational purposes and is not evaluated.
  - **Technical info**: numeric field, DB field: Ikw.tonnage

## Customs exit

**Master Data > Keys > System > Dispatch > Customs Exit**

On this dialog, you store the customs exit offices at the foreign borders. The use of the outgoing/destination customs function requires configuration. For additional information, please contact a service employee of A+W Software GmbH.

**Fig. B-103 Customs exit office**

### Descriptions of fields

- **No.**: Key number of the customs office. To create a new key number, select the next free number.
  - **Technical info**: numeric field, DB field: xazstelle.azsnr
- **Customs exit office**: Description of the customs exit office according to the customs details.
  - **Technical info**: alphabetic field, DB field: xazstelle.bez
- **DesCoun**: Selection of the destination country. The description is displayed in the next field.
  - **Technical info**: <F9>, DB field: xazstelle.beland
- **CustomsTyре**: Selection of the customs type. The description is displayed in the next field:
  - **MCO**: Main customs office
  - **GCO**: German customs office
  - **CO**: Customs office
  - **DispOff**: Dispatch office
  - **Technical info**: <F9>, DB field: xazstelle.zaart
- **TranspMode**: Selection of the mode of transport. The description is displayed in the next field:
  - 1 - Sea transport
  - 2 - Railway
  - 3 - Highway
  - 4 - Air transport
  - 5 - Via post
  - 7 - permanently installed
  - 8 - domestic ship transport
  - 9 - own company
  - 99 - other
  - **Technical info**: <F9>, DB field: xazstelle.vkzweig

## Customs destination office

**Master Data > Keys > System > Dispatch > Destin. Customs**

On this dialog, you store the destinations customs offices at the foreign borders. The use of the destination customs function requires configuration. For additional information, please contact a service employee of A+W Software GmbH.

**Fig. B-104 Customs destination office**

### Descriptions of fields

- **No.**: Key number of the customs office. To create a new key number, select the next free number.
  - **Technical info**: numeric field, DB field: xbzstelle.bzsnr
- **CCd**: Selection of the country in which the customs office is located. The description is displayed in the next field
  - **Technical info**: <F9>, DB field: xbzstelle.kfz
- **Customs Office of destination**: Customs office of destination according to customs details.
  - **Technical info**: alphabetic field, DB field: xazstelle.bez

## Dispatch groups

**Master Data > Keys > System > Dispatch > Dispatch Groups**

You can define dispatch groups on this dialog. They are evaluated in the dispatch control and serve the purpose of data selection.

**Fig. B-105 Dispatch groups**

### Descriptions of fields

- **Dispatch group**: Key number of the dispatch group. To create a new key number, select the next free number.
  - **Technical info**: numeric field, DB field: xvsgruppe.vsgruppenr
- **Description**: The description of the dispatch group, e.g. IG group.
  - **Technical info**: alphanumeric field, DB field: xvsgruppe.bez
- **Standard group**: In this field, you define whether the dispatch group is a standard group. With the start of dispatch control, the appropriate field is populated with this value.
  - This group is a standard group.
  - This dispatch group is not a standard group.
  - **Technical info**: alphabetic field, DB field: xvsgruppe.stdgruppe

## Rack status descriptions

**Master Data > Keys > System > Rack Status > Individual Descriptions**
**Master Data > Keys > System > Rack Status > All Descriptions**

On this dialog, you define the status for racks in various languages. The rack status is required in the rack management.

**Fig. B-106 Rack status descriptions**

### Descriptions of fields

- **No**: Key number. To create a new rack status, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
- **Language**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description of the rack status, e.g. sold.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1

## Rack groups descriptions

**Master Data > Keys > System > PMO > Rack Groups > Individual Descriptions**
**Master Data > Keys > System > PMO > Rack Groups > All Descriptions**

On this dialog, you define main groups for racks in different languages. That is, you can combine rack types into rack main groups.

**Fig. B-107 Rack groups descriptions**

### Descriptions of fields

- **No**: Key number. To create a new rack group, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
  - **View**: xghgr.ghgrnr
- **Language**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Short name**: The short name of the rack main group, e.g. GG.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1
  - **View**: xghgr.kurzbez
- **Description**: The description of the rack main group, e.g. large rack.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez2
  - **View**: xghgr.bez

## Packing methods descriptions

**Master Data > Keys > System > PMO > Packing Methods > Individual Descriptions**
**Master Data > Keys > System > PMO > Packing Methods > All Descriptions**

On this dialog, you define the packing methods in different languages.

**Fig. B-108 Packing methods descriptions**

### Descriptions of fields

- **No**: Key number. To create a new packing method, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
- **Language**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description of the packing method, e.g. PMO1.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1

## Rack packing allocation

**Menu: access right for menu Master Data > Keys > System > PMO > Rack Packing Allocation**

Permissible combinations of rack groups and packing methods can be stored on this dialog.

**Fig. B-109 Rack packing allocation**

### Descriptions of fields

- **No**: Selection of the rack group. The rack group is displayed in the next field.
  - **Technical info**: <F9>, DB field: pmogestverp.pmogestgrpid
- **No**: Selection of the packing method. The packing method is displayed in the next field.
  - **Technical info**: <F9>, DB field: pmogestverp.pmoverpackid
- **Parameters**: In this field, you store the PMO parameters for this key combination. A pair of keys can exist just once.
  - **Technical info**: alphanumeric field, DB field: pmogestverp.pmoparameter

## Currency

**Master Data > Keys > System > Currency > Currency**
**Master Data > Keys > System > Currency > Individual Descriptions**
**Master Data > Keys > System > Currency > All Descriptions**

On this dialog, you maintain the currencies and conversion factors in which the prices are displayed. You assign the currency to the market partner in the Master Data > Payment tab.

> **Requirements**
> You can only work with different currencies if the for-fee module for multi-currency capability is configured. For additional information, please contact a service employee of A+W Software GmbH.

**Fig. B-110 Currency**

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Currency.

### Descriptions of fields

- **No**: The currency key is needed for the definition of price lists (PLCD) as well as for customer and supplier entry in order to be able to display and calculate order values in the customer's currency. To create a new currency key, enter the next free number.
  - **Technical info**: numeric field, DB field: xwaehr.wnr
- **Abbrev.**: Abbreviation of the currency can be assigned freely, e.g. KRW. However, it is recommended that you use the international identifier for the currency.
  - **Technical info**: alphanumeric field, DB field: xwaehr.kurzbez
- **Description**: Description of the currency can be assigned freely, e.g. Korean Won.
  - **Technical info**: alphabetic field, DB field: xwaehr.bezeichn
- **Rate**: Rate at which amounts of the local currency are converted to the foreign currency.
  - **Technical info**: alphabetic field, DB field: xwaehr.kurs
- **Factor**: The rate multiplied by the factor provides the actual rate. The field can be used to exchange information with FinAc.
  - **Technical info**: numeric field, DB field: xwaehr.faktor
- **Min. CU**: Smallest currency unit, e.g. 0.01 EUR.
  - **Technical info**: numeric field, DB field: xwaehr.min_we
- **Rounding**: Rounding type:
  - **None**: There is no rounding.
  - **Comm**: The number will be rounded commercially.
  - **Up**: The number will be rounded up.
  - **Down**: The number will be rounded down.
  - **Technical info**: toggle field, DB field: xwaehr.we_rund
- **Euro fact.**: Conversion rate for the EURO.
  - **Technical info**: numeric field, DB field: xwaehr.eurokurs
- **Disc.**: Currency is discontinued. A discontinued currency can no longer be selected in the market partner. The currency may remain in orders and on invoices, however. If a document is processed again, you will then be asked to change the discontinued currency.
  - **Yes**: The currency is discontinued, e.g. Italian Lire.
  - **No**: The currency still exists.
  - **Technical info**: numeric field, DB field: xwaehr.stillkz
- **FIN. key**: The field can be used to exchange information with FinAc.
  - **Technical info**: numeric field, DB field: xwaehr.fibuschl
- **VAT acct.**: VAT account. The field can be used to exchange information with FinAc.
  - **Technical info**: numeric field, DB field: xwaehr.mwstkto
- **Proc. acc.**: Revenue account. The field can be used to exchange information with FinAc.
  - **Technical info**: numeric field, DB field: xwaehr.erloeskto
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz

## Tax types

**Master Data > Keys > System > Taxes > Tax Types > Tax Types**
**Master Data > Keys > System > Taxes > Tax Types > Individual Descriptions**
**Master Data > Keys > System > Taxes > Tax Types > All Descriptions**

On this dialog, you store the tax types that are required for the entry of the market partners and document generation.

> **Multilingual names**
> Since QR2209, you can also store multilingual names in A+W Enterprise for Tax Types.

**Fig. B-111 Tax types**

### Descriptions of fields

- **Number**: Number of the tax type. To create a new tax key, select the next free number.
  - **Technical info**: numeric field, DB field: xkukz.kukz
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description of the tax type can be assigned freely, e.g. foreign (EC).
  - **Technical info**: alphanumeric field, DB field: xkukz.bez

## Tax rates

**Master Data > Keys > System > Taxes > Tax Rates**

On this dialog, you assign the appropriate tax rates to the individual tax types.

**Fig. B-112 Tax rates**

### Descriptions of fields

- **Number**: Selection of the tax type. The tax type is displayed in the next field.
  - **Technical info**: <F9>, DB field: xmwst.kukz
- **Tax rate**: Here you store the appropriate tax rate for the tax type in percent. If you need several tax rates, you can use the Tax Rates 1-3 fields.
  - **Technical info**: numeric field, DB field: xmwst.satz, satz1-3
- **Valid from**: Here you store starting when the tax rate is valid for the tax type.
  - **Technical info**: numeric field, DB field: xmwst.giltab
- **VAT acct.**: VAT account. The field can be used to exchange information with FinAc.
  - **Technical info**: numeric field, DB field: xmwst.mwstkto
- **Input tax account**: Input tax account. The field can be used to exchange information with FinAc.
  - **Technical info**: numeric field, DB field: xmwst.vstkto

## Payment type descriptions

**Master Data > Keys > System > Payment Type > Payment Type**
**Master Data > Keys > System > Payment Type > Individual Descriptions**
**Master Data > Keys > System > Payment Type > All Descriptions**

On these dialogs, you store the individual payment types that can be used at your company.

**Fig. B-113 Payment type descriptions**

### Descriptions of fields

- **No**: Key number. To create a new payment type, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
  - **View**: xzahlm.zmnr
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description of the payment type, e.g. prepayment.
  - **Technical info**: alphabetic field, DB field: xsprbez.bez1
  - **View**: xzahlm.atxt
- **FinAc**: Abbreviation for financial accounting.
  - **Technical info**: alphabetic field, DB field: xxzahlm.fib

## Cash discount groups

**Master Data > Keys > System > Cash Discount Groups > Cash Discount Groups**

You create the cash discount groups to which you can assign market partners on this dialog. The groups are available in sales and purchasing and can be changed there.

**Fig. B-114 Cash discount groups**

### Descriptions of fields

- **Payment condition**: Display of the key number. To create a new cash discount group, enter the next free number.
  - **Technical info**: numeric field, DB field: xxxskonto.zahlbed
- **Tpe**: Description of the cash discount type. Any text can be entered here.
  - **Technical info**: alphanumeric field, DB field: xxxskonto.art
- **Month**: With this field, you control how many (full) months are added to the invoice date or to the due date.
  - **Technical info**: numeric field, DB field: xxxskonto.monat
- **Deadline 1**: If necessary, an additional deadline can be added. Example: invoice date 02/14, month = 1, deadline = 15 days:
  02/14 + 1 month = 03/14
  03/14 + 15 days = 03/29
  - **Technical info**: numeric field, DB field: xxxskonto.frist1
- **Creation date 1-3/Deadline 2**: The creation dates (Creation date 1 - Creation date 3) and Deadline 2 enable an extension of the validity period for the cash discount. These fields do not always have to be filled in. The creation date 30 corresponds to the last day of the month.
  Example:
  Invoice date 02/10, month = 1, deadline = 10 days, creation date 1 = 15, creation date 2 = 30:
  02/10 + 1 month = 03/10
  03/10 + 10 days = 03/20
  The list of possible invoice creation days refers to 03/31 since starting from 03/20, the next possible creation date is determined.
  03/31 + 5 days = 04/05
  This means that the cash discount must be claimed by 04/04.
  - **Technical info**: alphanumeric field, DB field: xxxskonto.rechlegtag1-3, frist2
- **Cash disc. rate**: Amount of the cash discount granted in percent.
  - **Technical info**: numeric field, DB field: xxxskonto.satz
- **Description**: Defined payment term in words, e.g. 10 days, 2% cash discount.
  - **Technical info**: alphanumeric field
- **Next condition**: The next condition refers to the key for an additional cash discount agreement, which goes into force for the first cash discount agreement after the deadline has passed.
  - **Technical info**: <F9>, DB field: xxxskonto.folgezahlbed

## Cash discount groups (Language Descriptions)

**Master Data > Keys > System > Cash Discount Groups > Individual Descriptions**
**Master Data > Keys > System > Cash Discount Groups > All Descriptions**

These dialogs include the cash discount groups in the respective languages.

**Fig. B-115 Cash discount groups**

### Descriptions of fields

- **Number**: Selection of the key number. To create a new group, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
- **Lng**: Selection of the language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description of the group, e.g. 30 days net.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1

## End of period

**Master Data > Keys > System > End of Period**

The end of period serves in the FinAc as delimitation of the booking period.

**Fig. B-116 End of period**

### Descriptions of fields

- **End of period**: Date on which the current booking period ends. Depending on the configuration, the SA period end, PU period end or both can be entered here.
  - **Technical info**: numeric field, DB field: periode.ek_periode, vk_periode
- **Modified**: Date of the change. The field is filled automatically with today's date.
  - **Technical info**: numeric field, DB field: periode.aenderdat
- **Frm**: Name of the person who made the change. The field is filled automatically with the name of the person logged in.
  - **Technical info**: alphanumeric field, DB field: periode.aendermanr

## Adhoc SQL group descriptions

**Master Data > Keys > System > Adhoc SQL Groups > Individual Descriptions**
**Master Data > Keys > System > Adhoc SQL Groups > All Descriptions**

On these dialogs, you create new Adhocsql groups or make changes. For these groups, you can store your own queries in the system menu <Ctrl> + <F4>.

**Fig. B-117 Adhoc SQL Group Descriptions**

### Descriptions of fields

- **Number/No**: Key number. To create a new group, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Description of the group, e.g. 30 days net.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1

## Report texts

**Master Data > Keys > System > Report Texts**

This dialog shows you all defined texts for the reports in the respective languages.

**Fig. B-118 Report texts**

### Descriptions of fields

- **Type**: Selection field for the text type in order to restrict the hit quantity (optional).
  - **Technical info**: alphanumeric field, DB field: cr_repstrings.type
- **Language**: Selection field for the language in order to restrict the hit quantity (optional).
  - **Technical info**: numeric field, DB field: cr_repstrings.sprkz
- **Type**: Key description of the text. This is used in the report for reference.
  - **Technical info**: numeric field, DB field: cr_repstrings.type
- **Language**: Language ID.
  - **Technical info**: numeric field, DB field: cr_repstrings.sprkz
- **Description**: Name of the language, e.g. English.
  - **Technical info**: numeric field, DB field: cr_repstrings.sprkz
- **Text**: Name of the report.
  - **Technical info**: alphanumeric field, DB field: cr_repstrings.text
- **A+W-Flag**: Flag that specifies whether or not the text is specified by A+W.
  - The text is specified by A+W.
  - The text is not specified by A+W.
  - **Technical info**: alphanumeric field, DB field: cr_repstrings.awflag

## Companies

**Master Data > Keys > System > Companies/Corporations > Companies/Corporations**

This dialog shows you all defined companies and corporations in the respective languages. The dialog is only available if you are using the multi-site function. For additional information, please contact a service employee of A+W Software GmbH.

**Fig. B-119 Companies/Corporations**

### Descriptions of fields

- **Company**: Company ID. To create a new company, enter the next free number.
  - **Technical info**: numeric field, DB field: xcompany.compid
- **Name**: Name of the company.
  - **Technical info**: alphanumeric field, DB field: xcompany.name
- **Partners**: Selection of the market partner. Here only the Other market partners are suggested whose mp.private_long1 is.
  - **Technical info**: <F9>, DB field: xcompany.mpnr

## Company allocation

**Master Data > Keys > System > Companies/Corporations > Company Allocation**

Here you can assign a company to the individual sites (table xhaus). The data is then evaluated in all areas (document entry, SA, production) in order to guarantee the correct site assignment. On this dialog, it is not possible to enter new sites; it is only possible to make an assignment for existing sites. Please note that a site without company assignment counts as non-existent.
The dialog is only available if you are using the multi-site function. For additional information, please contact a service employee of A+W Software GmbH.

> **Changing the assignment**
> Since a change of the assignment can have massive consequences for the document handling in the entire system, there is a security query for each change, asking whether you really want to do this.

**Fig. B-120 Company allocation**

### Descriptions of fields

- **No**: Site number. The name is displayed in the next field.
  - **Technical info**: display field, DB field: xhaus.name
- **Site**: Site number. The name is displayed in the next field.
  - **Technical info**: display field, DB field: site2comp.hausnr
- **Company**: Selection of the company that should be assigned to the site. The appropriate keys are assigned via the Companies/Corporations menu (Master Data > Keys > System > Companies/Corporations).
  - **Technical info**: <F9>, DB field: site2comp.compid
- **Customer/Supplier**: Display of the customer and supplier number. These count as internal market partners. Internal market partners must absolutely be maintained in the master data. When opening the dialog for this market partner in the Master Data > Market Partner menu, the title changes to Internal Market Partner. For internal market partners, it is also possible to store a deviating FINAC debtor. However, stricter restrictions apply here: permissible are only internal market partners that belong to the same company/corporate group. If for an internal market partner a deviating FINAC debtor has been entered, then starting from this point, there is also increased checking of the change of the company assignment. The company assignment of an internal market partner cannot be changed if the market partner is also assigned to other internal market partners as FINAC debtor. In this case, the dependency must first be resolved (that is, the FINAC debtor of the affected other internal market partners changed) before a new company assignment can take place.
  - **Technical info**: display field, DB field: xhaus.kunr/linr
- **Host**: Host name.
  - **Technical info**: display field, DB field: xhaus.xhaus.host

# Product Keys

**Master Data > Keys > Products**

All permissible colors and dimension variants are stored here. It is also possible to form general exchange rules that change the product structure generally.
For IGUs, the determination of the technicalk values is controlled via the product keys.
You have access to the following areas:

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a a a | Variants - Colors | ⇨ "Color variants" on page B-296 |
| a a b/c | Variants - color descriptions | ⇨ "Color names" on page B-298 |
| a b a | Dimensions - dimensions | ⇨ "Dimension variants" on page B-299 |
| a b b/c | Dimensions - dimension descriptions | ⇨ "Variants" on page B-301 |
| a c a | Sizes - size variants | ⇨ "Size variants" on page B-302 |
| a c b/c | Sizes - size descriptions | ⇨ "Size variants" on page B-303 |
| b | Exchange/additional rules | "Exchange/additional rules" on page B-304 |
| c a | Technical values - groups | ⇨ "Submenu technical values > groups" on page B-294 |
| c b | Technical values - vectors | ⇨ "Submenu technical values > vectors" on page B-294 |
| c | Technical values - notification bodies | ⇨ "Notification bodies" on page B-330 |
| d | Technical values - product standards | ⇨ "Product standards" on page B-331 |
| e | Technical values - priorities | ⇨ "Priorities" on page B-333 |
| f | Technical values - product code | ⇨ "Product information (CEKAL)" on page B-334 |
| g | Technical values - CE code | ⇨ "CE code (CPIP)" on page B-336 |
| h | Technical value - declaration of performance | ⇨ "Declaration of Performance" on page B-336 |
| i | Technical values - product encryption | "Product encoding" on page B-338 |
| j | Technical values - product purposes | ⇨ "Product purposes" on page B-341 |
| k | Technical values - parameter description | ⇨ "Parameter description" on page B-343 |
| l | Technical values - declaration of performance | ⇨ "Declar. of Perform. (entry)" on page B-344 |
| d a/b | Analysis groups | ⇨ "Descriptions for analysis groups" on page B-345 |
| e a/b/c | Fitting types | ⇨ "Descriptions for fitting types" on page B-346 |
| f a/b | Foil types | ⇨ "Description for foil types" on page B-348 |
| g | Production types | ⇨ "Production types" on page B-349 |
| h a/b/c | Spacer types | ⇨ "Description for spacer types" on page B-350 |
| i a/b | Sealing types | ⇨ "Descriptions for sealing types" on page B-352 |
| j | Motifs | ⇨ "Motif assignment" on page B-353 |
| k | Stack | This is a customer-specific function that is not a component of this manual. |
| l a/b | Box signature | ⇨ "Descriptions for box signature" on page B-355 |
| m | Shaping/Nesting product | ⇨ "Shaping/Nesting article" on page B-357 |
| n | Template parameters | ⇨ "Template parameter" on page B-358 |
| o | ITOE exchange rules | ⇨ “iTOE exchange rules" on page B-359 |
| p | Sash size set | This is a customer-specific function that is not a component of this manual. |
| q | Customer products | ⇨ "Customer products" on page B-362 |
| r | Ordered processings | ⇨ "Ordered processings" on page B-364 |
| s | Site-specific details | ⇨ "Site-specific details" on page B-366 |
| t | LAMI/CR inheritance | ⇨ "LAMI/CR inheritance" on page B-367 |
| u | A+W iQuote - specific details | ⇨ "Submenu A+W iQuote-specific details" on page B-295 |

## Submenu technical values > groups

**Keys > Products > Technical Values > Groups**

With this menu, you create groups that are required for the description of technical values.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Sound protection | ⇨ "dB groups" on page B-312 |
| b | Thermal properties | ⇨ "U groups" on page B-313 |
| c | Total energy transmission | ⇨ "g groups" on page B-314 |
| d | Transmission | ⇨ "Transmission groups" on page B-315 |
| e | Size restrictions | ⇨ "Size restriction groups" on page B-316 |
| f | Thicknesses | ⇨ "Thickness groups" on page B-317 |
| g | Bending strength | ⇨ "Bending strength groups" on page B-318 |

## Submenu technical values > vectors

**Keys > Products > Technical Values > Vectors**

With this menu, you create vectors that are required for the description of technical values.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Sound protection | ⇨ "Vectors for sound protection (dB)" on page B-319 |
| b | Thermal properties | ⇨ "Vectors for thermal properties (U)" on page B-321 |
| c | Total energy transmission | ⇨ "Vectors for total energy transmission (g)" on page B-323 |
| d | Transmission | ⇨ "Transmission vectors" on page B-325 |
| e | Size restrictions | ⇨ "Dimension restriction vectors" on page B-327 |
| f | Wind load | ⇨ "Wind load vectors" on page B-329 |

## Submenu A+W iQuote-specific details

**Keys > Products > A+W iQuote-specific details**

With this menu, you maintain master data that is required for working with A+W iQuote. If you need information about this product, please contact an A+W Software GmbH employee.

| Shortcut | Entry | Description |
| :--- | :--- | :--- |
| a | Product groups | ⇨ "Article groups-descriptions" on page B-368 |
| b | Processing assignment | ⇨ "Processing assignment" on page B-369 |
| c | Processing for shape edges | ⇨ "Processings for shape edges" on page B-372 |
| d | Exchange groups | "Exchange group descriptions" on page B-374 |
| dc | Group allocation (products) | ⇨ "Group allocation (products)" on page B-375 |
| dd | Group allocation (spacers) | ⇨ "Group allocation (spacers)" on page B-376 |

## Color variants

**Master Data > Keys > Products > Variants > Colors > Colors**

All colors that are required in the article master data and later in the order entry must be created here.

**Fig. B-121 Colors**

### Descriptions of fields

- **Number**: Number of the color.
  - **Technical info**: numeric field, DB field: xxfarbe.farbnr
- **Description**: Description of the color.
  - **Technical info**: alphanumeric field, DB field: xcompany.name
- **Color no.**: RAL number of the color.
  - **Technical info**: numeric field, DB field: xxfarbe.ralnr
- **AWDesign ColorCode**: A+W color code that is required in the CAD Designer (Bars).
  - **Technical info**: alphanumeric field, DB field: xxfarbe.awfarbcode
- **RGB name**: RGB color name.
  - **Technical info**: alphanumeric field, DB field: xxfarbe.rgbname
- **red**: Share of red for RGB color definition.
  - **Technical info**: numeric field, DB field: xxfarbe.farbe_r
- **green**: Share of green for RGB color definition.
  - **Technical info**: numeric field, DB field: xxfarbe.farbe_g
- **blue**: Share of blue for RGB color definition.
  - **Technical info**: numeric field, DB field: xxfarbe.farbe_b

### Additional information

⇨ "Color names" on page B-298

## Color names

**Master Data > Keys > Products > Variants > Colors > Individual Descriptions**
**Master Data > Keys > Products > Variants > Colors > All Descriptions**

On this dialog, you define the individual colors in the different languages.

**Fig. B-122 Individual colors**

### Descriptions of fields

- **Number**: Key number. To create a new color, enter the next free number.
  - **Technical info**: <F9>, DB field: xsprbez.id
- **Lng**: Language ID.
  - **Technical info**: <F9>, DB field: xsprbez.sprkz
- **Description**: Color description, e.g. white.
  - **Technical info**: alphanumeric field, DB field: xsprbez.bez1

## Dimension variants

**Master Data > Keys > Products > Variants > Dims > Dims**

All dimension variants are maintained on this dialog, depending on the quantity unit. These dimension variants are then assigned in the article master data. The dimension variants are also the basis for the stock management.

**Fig. B-123 Dimensions**

### Descriptions of fields

- **No**: The variant no. is the unique key within the respective quantity unit (QU). It is used both in the article master data as well as in the course of order entry for identification of the desired variant.
  - **Technical info**: numeric field, DB field: xxvar.bitnr
- **QU**: Selection of the quantity unit. The codes are stored on the Quantity Units menu (Codes > System).
  - **Technical info**: <Selo>, DB field: xxvar.meh
- **Description**: The description of the dimension variant can be selected at will.
  - **Technical info**: alphanumeric field
- **Stock descr**: The description of a piece in stock can be selected at will.
  - **Technical info**: alphanumeric field
- **Part.dims 1-3**: Length, width, and height are specified in the smallest sensible unit. They are shown automatically during order entry.
  - **Technical info**: numeric field, DB field: xxvar.mas1, mas2, mas3
- **Total dims**: The total dimension provides the total dimension of the variant in the respective system basic unit. In the order entry, the total dimension is calculated using the conversion factor entered here.
  - **Technical info**: numeric field, DB field: xxvar.faktor

### Additional information

⇨ "Quantity units" on page B-247
