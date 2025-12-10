---
title: "EN-CONFIG-AW_Enterprise_8"
source: "EN-CONFIG-AW_Enterprise_8.pdf"
tags: ["A+W Enterprise", "Pricing", "Price Maintenance", "Surcharges", "Configuration", "Environment Variables", "ERP", "Order Processing", "Delivery Notes", "Invoice"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical configuration guide for the A+W Enterprise ERP system, focusing on advanced pricing rules, order processing, delivery note generation, and goods receipt functionalities. It details various settings, master data configurations, and the use of environment variables to customize system behavior."
long_description: "This document provides an in-depth technical configuration guide for several key modules of the A+W Enterprise ERP system. It covers Chapter 53 on Pricing, Chapter 54 on Number Ranges, Chapter 55 on Product/Sash Sets, Chapter 56 on Delivery Note Creation, Chapter 57 on Background Processes, and Chapter 58 on Goods Receipt. The guide is intended for system administrators and technical users responsible for customizing the software. It details a wide range of pricing functions, including global price maintenance, processing prices, special pricing, minimum prices, and various surcharges (e.g., shape, size, AIR surcharges). A significant portion of the document explains how these features are controlled through master data settings, specific user actions in the interface, and a comprehensive list of environment variables. It provides detailed instructions on configuring complex pricing rules, managing invoice and credit note numbering, setting up product sets for simplified order entry, and automating background jobs for tasks like delivery note creation. The document also includes information on handling goods receipts, particularly for rack-related stock, and outlines the logic for multi-site environments. It contains specific variable names, menu paths, issue tracking numbers (AWDesk, AWD), and process flows for different scenarios within the software."
---

Similarly, the flag is not taken over into the order data. This means if for a processing the pricing type is changed manually, this flag is not applied.

The new function is not for:
- stock assessment,
- price calculation in the PO pool,
- rack invoices
- old pricing method "IGU matrices", "processing matrices"
- pricing method "PCd whole-glass systems"
- pricing method "PCd processings"
- pricing method "PCd color articles"
- Customer-specific material calculation customer 10
- Proportional prices (enf? KUARTPRS_GRUPPE)
- Fixed IGU structure (KONDITIONEN_FESTER_ISOAUFBAU)

---
## 53.3. Global price maintenance

Currently, global price maintenance is available on the following menus:
- Master data - Prices – IG Prices – Exchange TG/LAMI/Special
- Master data – Prices – PCD prices – All article price vectors
- Master data – Prices – PCD prices – Processing vectors
- Master data - Prices – PCD prices – LAMI articles – LAMI exchange / additional prices
- Master data – Prices - PCD prices - Colored articles
- Master data - Prices - PCD prices - Variant prices
- Master data - prices - Muntin prices - Muntin price categories
- Master Data - Prices - Surcharges - Shape surcharges
- Master data - Conditions - Special prices - Article prices (no copy function, only conversion item-specifically)
- QR09/2022: Master Data - Conditions - Special Prices - Processing Prices (no copy function, only conversion)

### 53.3.1. Functions in the global price maintenance

**Key F5: Copy values from first line.**

As soon as values for the increase have been entered in the first line (step 1), you can copy these values to all additional steps (lines). This way, you can easily increase all steps with the same values (e.g. % value) without having to enter it on each individual lines.

## 53.4. Processing prices

### 53.4.1. Calculating no processings

**AWDesk: 72311**

Normally you can only define yourself for the processing whether or not it should be calculated. However, there are constellations (e.g., use of AWBroke) where it is necessary not to calculate processings depending on the item article.

If the environment variable `SN_KEINE_BEARBPREISE` is active and for the item article in the master data the private field long1 (artikel.private_long1) is equal to 1, no processings will be calculated. Accessories are still calculated and cannot be switched off via this function.

The decision what a processing is made using the article type.

Within the price calculation, among other things, processing and accessories are distinguished. Which article types are price-relevant processings and which price-relevant accessories is defined permanently in the program (see "Price-relevant article types").

### 53.4.2. Price-relevant article types

Whether or not a price is drawn for an article in the BOM depends on several conditions.

a) There if a fixed definition of article types for which the processing prices or accessory prices are determined. See also the listing of the price-relevant article types and assignment to "processings" and "accessories" below.
b) Settings in the article master data - article dimensioning
c) Creation of prices and terms

**Price-relevant processings are the following article types:**

- 505-Cuttingt
- 512 - Bending
- 513 - Curving
- 515-Tempering
- 516-Partial tempering
- 540 - Other processing
- 545 - Packing
- 550 - Grinding
- 551- Mitering
- 552 - Groove grinding
- 553- Arissing
- 560 - Drilling
- 561-Countersunk hole
- 565-Rounded corners
- 566-Corner cut-off
- 580 - Speak-thru
- 584 - Color application
- 585 - Enameling
- 586 - Etching
- 587-Sand blasting
- 588 - Screen printing
- 589 - Coating
- 592 - Masking
- 593 - Edge stripping
- 595 - UV protection
- 596-Inside thread
- 597 - Edging
- 598 - Forming
- 599 - Gluing
- 235-Lead muntins
- 570-Corner cut-out
- 571 - Edge cut-outs
- 575-Handles
- 703 - Wood cutting
- 752 - LAMI foil cutting

**Price-relevant accessories are the following article types:**

- 210 - Spacer
- 211 - Colored spacer
- 220 - Spacer
- 260- Gases
- 270 - Edge protection
- 280 - Capillary inserts
- 300 - Foils
- 320 - Color layer
- 340 - Resin
- 590 - Enamel strips
- 591 - Stamp
- 594 - Pressure compensation
- 600 - Rails
- 610 - Tubes
- 700 - Heat soak
- 800 - Accessories
- 820-Bleche
- 830 - Fittings
- 840 - Locks
- 850- Handles
- 870-Alarm transmitters
- 999 - Other articles

**Article types that do not flow into price calculation**

534 - Muntin construction: The article type is not considered in the addition of the prices, even if a processing price is displayed on the processing dialog. The background is that muntins have their own calculation logic.

### 53.4.3. Edgework for shapes

For the calculation of edgework by the linear meter, for shapes it is not the real edge lengths that are calculated, but always the edge lengths of the circumscribing rectangle.

### 53.4.4. Processing factors

Under Master data - Conditions - Special prices - Processing prices, you can create individual prices and factors for processing items. Here, however, the effect of the entry of a factor != 0 or price = 0 is that no price is calculated. If you would like to enter a different factor here, you must also enter a price.

Otherwise, it applies that:

The processing factors can currently only be defined in A+W Enterprise with reference to the item or the price list. Currently, there is no possibility for defining separate factors for individual processing items (exception: see above).

Where can processing factors be defined:
- Daily conditions
- Daily product group conditions (product group of the item)
- General conditions of the market partner
- Product group conditions of the market partner (product group of the item)
- Item conditions of the market partner (item - not BOM item)
s.a. environment variable `KEIN_TZ_BEI_SPEZARTPRS`

### 53.4.5. Special processing prices

**alcib 13.04.11733 - Jan 2022**

If the environment variable `KUBEAPRS_VEKTOR` is active, then in the "Master data - Conditions - Special prices - Processing prices" you can store individual prices for processing vectors in addition to prices for processing articles.

If the variable is active, it is possible to store special processing prices for processing vectors. The price calculation then first searches for a special price for the article. If no price is found, a special price with the vector number assigned to the article is searched for next. Here, the "Starting with PLCd" logic is considered. If starting with PLCd 1 a price for the article is stored and starting with PLCd 5 a price for the vector, then the behavior is as follows:

- PLKZ in the item = 2: The price for the article is pulled
- PLKZ in the item = 6: The price for the vector is pulled

s.a. environment variable `KEIN_TZ_BEI_SPEZARTPRS`

### 53.4.6. Minimum processing prices

For processings in LAMI and TG items in the order, you can specify scaled minimum prices according to the square meter in Master Data - Prices - PCd Prices - Minimum Processing Prices. If the total of processings relevant for the comparison is smaller than the minimum price that applies for the rounded square meter of LAMI or TG item, then this will be used as total price for these processings.

For the comparison processing total/minimum price, only such processings are summed up in which item master data (F4 - Price Properties) the identifier Minimum price rel. is set to 'Y'. All other processing will continue to be calculated separately.

In the price calculation of the sale price, the minimum processing price is compared to the total of the processing prices of all minimum price-relevant processings in the BOM. If the total is smaller than the minimum processing price, then the minimum price is calculated and the difference amount is allocated proportionally to the individual processing prices and the revenue distribution.

**Note:** A comparison with the minimum price only happens if the item article is a LAMI or TG. There is no comparison for LAMI or TG in IG.

The function is switched on separately for TG and LAMI via the environment variables `ESG_MIN_BEAPREIS` or `VSG_MIN_BEAPREIS`

In the general daily conditions, you can specify whether the minimum processing price should be calculated generally (the field minimum processing price = e.g. "Y"). In the special general conditions, you can then override this setting for particular customers (minimum processing price = e.g. "N"). The evaluation of the minimum processing price is done only during the determination of the sales price. For this reason, this functionality is only available for sales in the general daily conditions and in the special general conditions for the customer, sales objects, and customer groups.

**Example:**
In LAMI, there are two minimum price-relevant countersunk holes, for which the prices 10.00DM and 30.00DM were determined from the master data. However, the minimum processing price for LAMI is 60.00DM.

First the total of the drillings is determined: 10+30=40.00DM,
then the difference between the minimum processing price and the total calculated:
60-40=20.00DM,
this difference amount is distributed proportionally across both drillings:
20.00 is added as 5.00 share for the first drilling and 15.00 share for the second drilling. Therefore: in the revenue calculation, 15.00DM is written for the first countersunk hole and 45.00DM for the second.

After the complete texting of all processings in the item, an additional text line is generated: "Minimum processing price: xxxxx Difference: xxxxx".
The line is then only generated if such a difference (between the total of all processing prices per item and the minimum processing price) exists.

**Prerequisite:** The system has been configured appropriately.
The flag Minimum price rel. in the item dimensioning of the processing must be set accordingly.

Menu: `SALES`⇒`Order Entry`, Price field, `<A12>`, then `<DETAIL>`, 3. Mode screen for processings and `<A55>`, Revenue distribution

Interpane, AWDesk 25137

### 53.4.7. Minimum calculation

Within the processing vectors and the special processing price, a minimum calculation can be specified in the basic quantity unit.

**Minimum calculation ... TQU Specification** of the processing quantity in basic quantity units, the minimum price that is calculated. The basic quantity unit is determined from the article master data. If the price-relevant processing quantity in the order is less than the defined minimum quantity, the price for this minimum quantity is charged.

For edgework, this means that the total of the edges to be processed is compared to the minimum calculation.

For the article type 550, this can be configured so that the minimum calculation is calculated per edge.

`MINBER_AUF_KANTE` (Client reference: No)

If this variable is set, the minimum calculation per edge is calculated when the processing prices for grindings (article category 550) are determined if the price category GR/TQ is maintained and the article has the basic unit of measure linear meter or millimeter.

`MINBER_AUF_KANTE` (Client reference: No)

If this variable is set, the same minimum calculation for processings is calculated as for the main articles to be processed.

### 53.4.8. Processing group surcharges

Master Data > Prices > Surcharges > Processing surcharges

On this dialog, you create surcharges for processing groups. These surcharges are added to the price of a processing or subpart if the processing group is assigned to the glass article in whose BOM the processing is included.

The assignment to the processing group is entered in the article master data on the "Prices" tab in the "Processing group" field.

Processing group surcharges are only considered if the processing price is determined from the master data. They are not calculated if a special price is stored in the conditions.

The processing group surcharge is only calculated for processing articles with one of the following pricing methods:
- 7 - Processing matrices
- 25 - PCd prices general
- 26- PCd Processings
- 31- PCd colored articles
- 60 - UV protection

**Processing group**
Specification of the processing group. The code consists of two alphanumeric characters. Upper and lower-case letters are distinguished, e.g. 5H and 5h. There is no master data table for this.

**Surcharge**
Specification of the surcharge. This surcharge is charged on the basic price of the processing. Depending on surcharge type, the value is interpreted as percentage or fixed amount.

If you specify a fixed amount, the value has to fit the currency of the price list code (PLCD) to which these surcharges are assigned.

In the order, the processing price is displayed in the item conditions including surcharge.

**Price type**
Specification of to what the specified price refers:
- **CU/value:**
The surcharge is charged as fixed value on the processing price.
If the surcharge on the order is charged as a fixed amount, the currency of the PLCd determined for the header article applies. The currency is not converted.
- **Percent:** The surcharge is calculated and charged as a percentage of the processing price.

### 53.4.9. Size surcharges

See section "Prices - size surcharge" below.

### 53.4.10. Parameter-dependent processing prices (formulas)

**QR2406**

It is now possible to create the processing prices per glass type and according to the processing parameters (e.g., diameter for holes).

Therefore, the dialogs for maintenance of the processing vectors and processing prices have been reworked. The main views (table view) were expanded to include the fields "Glass type" and "Formula".

The detail view of a processing vector or of the processing prices were also reworked extensively. On the upper part of the dialog, the "Glass type" field was inserted. The selection field "Calculation type" has been expanded to include the value "Formula". On the lower part of the dialog, the two-column structure has been removed. The individual data records are now all lined up as in a table. This was necessary since a new field "Formula" for maintenance of the parameter-dependent prices was inserted.

**Master data maintenance**
- Master data - Prices - PCD prices - Processing vectors
- Master data - Prices - PCD prices - Spec. Processing vectors
- Master data - Conditions - Special prices - Processing prices

**"Glass type" field:**

In this field, you can maintain for which glass article type a processing price vector or processing price is valid. The following values are available:

- **All:** This data record is used for all glass article types
- **Basis:** This data record is used for the article types "Float FM (100)", "Float LM (180)", "Cast FM (110)", "Cast LM (181)", "PVC FM (120)", "PVC LM (185)", "Special glass FM (130)", "Special glass LM (182)" and "Artistic glazing (175)".
- **TGH:** This data record is used for the article types "TGH (150)".
- **LAMI:** This data record is used for the article types "LM FM (170)" and "LM FM (183)".
- **IGU:** This data record is used for the article types "IGU (200)".
- **Fire:** This data record is used for the article types "cast resin FM (140)", "cast resin LM (184), "fire protection glass FM (160)" und "fire protection glass LM (187).

If the price calculation does not find a special entry for a glass type, then the glass type "all" is used. That is, if there are entries for "All" and "LAMI", then, for example, the data record for "All" is used for "TGH". The hierarchy here is: "Product group, PLCD, glass type, quantity, thickness"

**"Calculation type" field:**

The "calculation type" field has been expanded to include the characteristic "Formula". If this calculation type has been selected, you can enter the "Formula" fields at the bottom of the dialog. In the "Formula" field, you can access the variables from the article master data. If you would like to scale the prices per diameter, for example, enter the formula "$W1 > <value>" in the field. The entry in this field is checked for syntax, however not for whether this parameter is available with the corresponding processing. This also means that this calculation type can only be applied for articles with A+W processing type. However, this restriction cannot be checked due to the complexity of the price and condition maintenance.

**Starting with alcib - 13.04.18658 (17.09.2024)**

Since QR 2406, it is possible to scale processing prices according to parameters. However, e.g., for drillings it was not possible to scale according to parameters and quantity. This is possible now. Within the formula, access to the item quantity is possible within the price calculation with "$PA". This is not the number of drillings in a lite, but the number of lites in the item. Thus, prices previously stored as calculation type "Pcs/Item" can now also be summarized with calculation type "formula".

For the sequence of the steps, you must pay attention that when using "greater than" or "less than" for example, that the order of the entries is correct.

| Step | Formula | from qty. | Price |
| :--- | :--- | :--- | :--- |
| 1 | | | 5.00 |
| 2 | $W1>5 | | 6.00 |
| 3 | $W1>15 | | 8.00 |
| 4 | $W1>50 | | 10.00 |
| 5 | | | |

**Replication:**

For this function, the tables "beavek" and "kubeapr" must each be expanded to include a new key column "glastyp". If these tables are replicated via key replication, the configuration for both of these tables must be expanded accordingly. The expansion is already possible BEFORE installation of QR2406. The table expansion has already been carried out with QR2306.

## 53.5. Minimum calculation

It generally applies that conditions have priority over prices. This also applies for the minimum calculation. This means that a minimum calculation, which is entered in the general product group conditions (Master data > Conditions > Daily conditions > Product group conditions) overrides the minimum calculation that is entered in the article vector (Master data > PCd prices > Article vectors)

In addition, the minimum calculation for processings can be set equal to that of the glass

`MINBER_WIE_GLAS` (client reference: no)

If this variable is set, the same minimum calculation for processings is calculated as for the main articles to be processed.

## 53.6. Min. price

### 53.6.1. Minimum price for child parts (accessories)

The minimum price that you define under MASTER DATA => PRICES => PCd PRICES => ARTICLE VECTORS and under MASTER DATA => CONDITIONS => SPECIAL PRICES => ARTICLE PRICES is evaluated for item articles and in particular cases also for accessory child parts.

The child part must have an accessory article type and must be calculated by pricing method 25 PCD "general prices". The item article in the process item has to have one of the following pricing methods: IG-current, PCD-basic glass, PCD-finishing, PCD-TG, PCD-LG, or PCD-glass doors. The minimum prices will be considered only for sales price calculation. The accessory price is first calculated with all surcharges and the factor, and then compared with the minimum price.

This function is not available if the environment variable `SPEZ_EINFACHGLAS` is active.

### 53.6.2. Minimum price for IGU

The minimum price is only done after the addition of the AIR surcharge.

## 53.7. Georgian bar

### 53.7.1. Prices for ordered muntins/grid patterns

Muntins are ordered as complete grid patterns. For this, in PU, a correct PU price calculation should be achieved in the PO. For this, you have to work with grid patterns. For this, the grid pattern must have the price method 23 "PCd basic glass". No price must be stored for the grid.

#238482 // #368937 // #393276 // #420510 // #434997

### 53.7.2. Calculation of the LM-K-R to be calculated

Prerequisite: `SPROSSENKREUZE_NEU_LOGIK` set

### 53.7.3. Calculation type 14 – "K or LM"

K or LM means - crossed or linear meters.

If the grill pattern does not include a cross, then calculation is done by linear meters. Otherwise, calculation is done as cross.

## 53.8. Exchange prices

### 53.8.1. Order article prices without exchange prices

**AWDesk document 441481: 25.11.2019:**

It happens that for a special article structure in an order, a fixed square meter price is awarded, on which no more exchange prices are to be calculated, but the processing. For this reason, the field "Without exchange" has been added to the dialog for entering order-related article prices (F4 - Price data - Order prices - Item prices). If this field is checked, no exchange or additional price will be calculated for the affected article within the price calculation for glasses and foils.
However, an exchange price can be entered manually in the item conditions dialog. This is then also taken into account in the price calculation.

It should be noted that exchange in the LAMI in IG is controlled via the indicator in the IG article.

### 53.8.2. Exchange prices by vector

### 53.8.3. IG

The IG exchange prices are currently always defined with regard to the article number of the glass in the master data. Now it is possible to configure the system in such a way that the exchange price for a glass can be stored for the vector assigned to this glass.

The logic is possible both in the general TG/LAMI/special exchange prices and in the individual IG exchange prices for market partners. The price calculation first checks whether IG exchange prices for individual market partners have been defined. In this case, the system first checks whether an exchange price has been defined for the item. The OC-PLCd logic must be observed. If no market partner-specific exchange price is defined for the article, the system determines which price vector is assigned to the article. The system then checks whether an IG exchange price has been defined for this price vector.

If no market partner individual IG exchange price is defined, the same 2-level search is carried out for the general TG/LAMI/special exchange prices.

This function is controlled via environment variable

`AUSTAUSCH_VEKTOR` ( client reference: No)

The variable controls that exchange prices can be stored in IG and LAMI for vectors. The price calculation then searches for exchange prices for the respective article. If none is defined, the system searches for the corresponding vector number for the article and checks whether a price has been defined for it.

The individual values define the range of conditions: IG Prices | LAMI Prices | IG Conditions | LAMI Conditions replaces `KUISOAUST_VEKTOR`.

### 53.8.4. LSG

The LAMI exchange prices are currently always defined with regard to the article number of the glass in the master data. Now it is possible to configure the system in such a way that the exchange price for a glass can be stored for the vector assigned to this glass.

The logic is possible both in the general LAMI exchange/additional prices and in the market partner individual LAMI exchange/additional prices. The price calculation first checks whether LAMI exchange prices for individual market partners have been defined. In this case, the system first checks whether an exchange price has been defined for the item. The OC-PLCd logic must be observed. If no market partner-specific exchange price is defined for the article, the system determines which master exchange list is defined and whether an exchange price is defined for this article. If no price is found there either, the system determines which price vector is assigned to the article. The system then checks whether an LAMI exchange price has been defined for this price vector. If no price is defined for the vector in the exchange list (the OC-PLCd logic must be observed), the following is checked with the vector in the master exchange list.

If no market partner-specific LAMI exchange price is defined, the same multilevel search is carried out for the general LAMI exchange/additional prices.

The function must be switched on via an environment variable.

`AUSTAUSCH_VEKTOR` (client reference: No)

The variable controls that exchange prices can be stored in IG and LAMI for vectors. The price calculation then searches for exchange prices for the respective article. If none is defined, the system searches for the corresponding vector number for the article and checks whether a price has been defined for it.

The individual values define the range of conditions:
IG prices | LAMI prices | IG conditions | LAMI conditions
replaces `KUISOAUST_VEKTOR`

### 53.8.5. Exchange price by matrix (size scaling)

To be able to create IG exchange prices size-scaled, the calculation type 'Matrix' was made configurable. According to the default logic, with the calculation type "Matrix", the exchange price is determined from the difference between the matrix of the exchange glass and the matrix of the header article. With the configurable new logic, the price is taken directly from the matrix of the exchange glass as exchange price; that is, the exchange price is independent of the price of the header article.

**Default:**

- IG basic price: 59.40
- Matrix exchange price: 10.95
- Calculation 50.40 + 10.95 =70.35 / 2 =35.17 - 59.40 = -24.22

Environment variable `ISOAUST_KEINE_MISCHMATRIX`

If you set the environment variable, 10.95 is used directly as exchange price.

### 53.8.6. Exchange factor

The exchange factor from the product group conditions is only used for the exchange directly in the item article. It is not used for exchange in the LAMI in IG. The special exchange list factors can be used for this. To be noted here is that the product group of the exchanged article is used by default and not that of the item article. To change this, the environment variable `SPEZATLFAKT_KOPFWAGRP` has to be activated.

**Pre-settings for the replacement factor in IG**
2011-08-05

According to the pricing standard logic, the factor defined for the main article will be used for glass and film layers to be exchanged or added to a LAMI in an IG. This is done only if no replacement/addition factor for laminated glass has been defined in the terms.

With the environment variables `DEFAULT_AUST_FAKTOR_VSG` it is possible to configure that in case of exchange/addition in the VSG in an IG article, not the factor of the header article but if present, the exchange factor of the VSGs in the IG is taken as exchange factor for glass and foils in the VSG.

### 53.8.7. LAMI exchange prices

**[AW-69695]**

Within the LAMI exchange prices (Master data - Prices - PCD prices - LAMI articles - LAMI exchange/additional prices and master data - Conditions - Special prices - LAMI exchange/additional prices), a new calculation type "total quantity per BOM header" is now available. In the course of introducing the new calculation type, the operation of the field has been changed from toggle to selo.

**AWD #89837: inheritance of manual LAMI exchange prices**
Product/Module: ALCIB / Prices /Terms (ALCIB 4.0) 28.11.2005:

By default, manually entered or changed LAMI exchange prices are not taken over into another article.

The system can now be configured so that manual exchange prices are inherited.

a) One possibility is the inheritance of the manual changes within a document entry. The LAMI exchange prices for a document item are displayed on the dialog, which can be reached as follows:

In the price field of the document position, press <Shift+F9> to reach the terms dialog; from there, the dialog with the LAMI exchange prices can be reached with <Shift+F10>. On this dialog, any field you can enter can be changed. Every manual change is recorded internally. If an item with the same BOM structure (and same BOM number) is then entered anew, the changes recorded are taken over into the new item.

This possibility can be activated as entry help. Here it must be noted that the noting of manual changes is temporary: if the document is exited and loaded again later, the data noted is no longer available.

b) Another possibility is that after loading a document again, existing LAMI exchange price information is marked as "manual". If then another item with the same BOM number is added to the document, for the new item the system relies on the noted LAMI exchange price information. This possibility applies for re-loaded documents, that is, documents that are loaded into the entry screen and expanded again after saving. It does not apply for documents that are entered with reference.

In both cases, it applies that the LAMI exchange price information is noted per BOM number. If there are several items with the same BOM number but with different information in the document, the last manual change (or for re-loaded documents the last item) is inherited.

There is not only inheritance for newly created items; existing items with the same BOM number remain untouched by manual changes.

With a new price calculation incl. obtaining of terms (e.g., <CTRL+F9> in the price field or after specification of order prices) the manual information is overwritten. For additional items with the same BOM header number, the LAMI exchange prices will also be determined completely from the master data.

Both possibilities are switchable by activating the environment switch `VSGAUSTAUSCHPRS_VERERBEN`. This switch is specified with two parameters, separated by blank spaces.

If the first parameter is set to 1, the manual changes should be inherited during a document entry.

If the second parameter is set to 1, with renewed loading of a document, existing LAMI exchange price information should count as manual.

If only one of the possibilities should be activated, the parameter for the other possibility must have the value 0.

### 53.8.8. Patterned replacement

The patterned replacement is done differently than for float, TGH, and LAMI according to so-called pattern classes. Whether the exchange is determined via pattern classes or via the "normal" exchange depends on the article type of the glass replaced.

## 53.9. Step Surcharge

### 53.9.1. Extended options for LAMI step price calculation

Currently it is possible to define step surcharges according to "CU/unit" and "percent" in the LAMI price master data. This step surcharge currently effects the glass base price of the LAMI item.

These calculation types are now expanded by 4 calculation types.

In the master data dialog for LAMI base prices:

"Master data – prices - PKZ prices - LAMI base prices" and "master data - prices - PCD prices - special LAMI base prices" the step surcharge type is expanded by the characteristics "CU/piece net", "CU/piece gross", "CU/unit net" and "CU/unit gross". The existing characteristic "WE/piece" is renamed to "WE/piece/GME". The characteristic "percent" is renamed to "percent/GME". The two existing characteristics are only renamed, but not changed in their calculation manner.

The calculation of the surcharge of the characteristic "WE/piece net" occurs after application of price surcharge and the factor, however before minimum calculation, model surcharge and processing.

Number of steps * surcharge = step surcharge net

Price per piece after TZ and factor + step surcharge net

The calculation of the surcharge of the characteristic "WE/piece gross" occurs as follows:

Number of steps * surcharge = step surcharge gross

Price per piece after TZ and before factor + step surcharge gross

The calculation of the surcharge of the characteristic "WE/unit net" occurs after application of price surcharge and the factor, however before minimum calculation, model surcharge and processing.

Surcharge = step surcharge net

Price per piece after TZ and factor + step surcharge net

The calculation of the surcharge of the characteristic "WE/unit gross" occurs as follows:

Surcharge = step surcharge gross

Price per piece after TZ and before factor + step surcharge gross

By setting the environment variables `KONDITIONEN_VSG_WAGRP` = `<VSG product group>` in the form `<nnnnnn>` to `<n*****>` it is possible to use the expanded step surcharge types also in the special product groups and special article conditions. ("master data - conditions - special conditions - product group conditions", "master data - conditions - special conditions - article conditions"

This expanded step surcharge calculation is controlled with the environment variable `KONDITIONEN_VSG_WAGRP` in versions ALCIB 2011 and AWE5.

**ATTENTION:** In version ALCIB 2011 it is necessary to update the program environment. The function shall be available in AWE5 as at version 5.3

### 53.9.2. Number of steps

`STUFE_KANTE_ALT` (client reference: no)

The number of steps is calculated per edge and per glass. In the calculation, for multiple glass (3-layer IG, LAMI), there were problems if several step records per item were written. The problem was eliminated, which caused changed price calculation.

If this environment variable is set, generally only one step record per item is evaluated.

## 53.10. AIR surcharge

**#455799/#454786**

### 53.10.1. Default calculation

**Surcharge type GR/piece**
- Only the first AIR is used to determine the AIR surcharge.
- No size surcharges are applied to the AIR surcharge
- The AIR surcharge is calculated AFTER exchange factor on every exchange, even if the exchange price=0. (`SZR_NUR_AUF_GRUNDPREIS`)
- The AIR surcharge is added to the glass price BEFORE the application of the glass factor

### 53.10.2. AIR surcharge on exchange

By default, the AIR surcharge is calculated on the base glass price and all exchange glass. The AIR surcharge GR/piece or GR/squ is then also calculated on the exchange if not exchange price is found.

With the activation of the environment variable `"SZR_NUR_AUF_GRUNDPREIS"` the AIR surcharge is not calculated on the exchange glass.

If this variable is active, it can happen, however, that no AIR surcharge is calculated. This is the case if the glass base price + AIR surcharge is less than the minimum calculation.

**Surcharge type GR/piece**

(glass unit price + AIR surcharge) * glass factor + exchange + shape surcharge on unit price

### 53.10.3. AIR surcharge for triple IG

The following description assumes that the environment variable `SZR_ZUSCHLAG_SZR2` is set.

When fetching the conditions for the IG current article, the system first checks whether a surcharge is found for AIR1. If the search was successful, an additional surcharge for AIR2 will be applied. The system now checks whether the surcharge categories of these two surcharges are the same. If this is the case, the surcharges are added together. Otherwise, the overhead must be converted to a uniform overhead category - CU/piece - before it is added. This only works if the surcharges are to be calculated on the net basic price, i.e. if the variables `SZR_NUR_AUF_GRUNDPREIS` and `SZRZUSCHLAG_NETTO` are set. If one of these variables is not set and the overhead types are still different, no unique conversion is possible. An error message is then displayed and only the surcharge for AIR1 is taken into account for the price calculation.

The added surcharges for AIR1 and AIR2 are displayed in the AIR surcharge field in the item conditions of the order.

If the environment variable `SZR_ZUSCHLAG_SZR2` is not set, the old logic still applies; that is, only the surcharge for AIR1 is calculated.

**AWDESK #17629**

### 53.10.4. Size surcharges also on AIR

By default, size surcharges are not added to the AIR surcharge. With the environment variable `GROSSZU_AUF_SZR = ON`, it can be achieved that size surcharges of the type "Percent" are applied to the AIR surcharge.

## 53.11. PCd glass doors

**alcib - 13.04.11780 Feb 2022**

For glass doors and all-glass doors, there is the price calculation method PCd glass doors. Within this pricing method, previously only the float glass (article type 100), TG (article type 150), LAMI (article type 170), and IGU (article type 200) were permitted.

Now additional types of glass have been added:

| Glass | Article type |
| :--- | :--- |
| Patterned | 110 |
| PVC | 120 |
| Special glass | 130 |
| Cast resin | 140 |
| Fire protection | 160 |

Furthermore, the glass had to be created with the pricing methods:
- IG current
- PCd TG
- PCd LAMI
- PCs Basic glass
- PCd Processed glass

New is now also the price calculation method "PCd prices general", which was added.

## 53.12. Shape Surch.

### 53.12.1. No shape surcharge for articles, with shape in article master data

If the article is already defined as shape in the article master data, no shape surcharge is calculated. In this case, it is assume that the list price already includes the shape surcharge.

### 53.12.2. Shape surcharge for sealants

Articles of the article type sealants (240) are not calculated as processing, but as accessories. In addition, a special price calculation applies for sealants within the IG price calculation (IG-current artikel.vkptype = 41), whereby no shape surcharge is considered. (#386510)

### 53.12.3. Shape surcharge per product group

Starting with A+W Enterprise 6

The shape surcharge can be entered per shape type or per product group. How the product group is entered and evaluated is controlled via the environment variable.

`ALLGEMEIN_WAGRP`

controls whether product groups in product group conditions can be selected freely or whether they must be specified according to the ALCIB convention (10****, 1010**, 101010).

The product groups "******" is only permissible with set environment variables and is only evaluated then. If the customer creates "******" with a designation in the product group master data, then the entry within the price master data is possible, but it is not found in the price calculation.

### 53.12.4. Shape surcharge/minimum shape surcharge

**Version 3.0**
MASTER DATA=>PRICES=>SURCHARGES=>SHAPE SURCHARGES
MASTER DATA=> CONDITIONS=>SPECIAL CONDITIONS=>SHAPE SURCHARGES

Previously, the minimum shape surcharge that you can maintain on the screens mentioned above is only evaluated for items with the pricing method IG-Swiss. In the current version, the price calculation has been expanded so that the minimum shape surcharge is also calculated for the pricing methods IG-current, PCd-basic glass, PCd-finished glass, PCd-TG, and PCd-LAMI.

The minimum shape surcharge is determined from the conditions or the price master data and displayed in the item conditions for the above-mentioned pricing methods next to the Shape Surcharge field. This minimum shape surcharge can be changed manually in the item. The minimum shape surcharge is considered both in the sales as well as in the purchasing price calculation, and also in the cost calculation for purchased glass, but not for the processings.

Depending on how the Shape Surcharge field is specified in the conditions, the minimum shape surcharge is calculated as follows.

- **Basic price**: The shape surcharge is only calculated on the basic glass price and then this value is compared to the minimum shape surcharge.
- **Glass price**: The shape surcharge is calculated on the basic glass price and on the exchange prices. In this case, the minimum shape surcharge is compared to each of these values.
- **Unit price**: The minimum shape surcharge is calculated on the unit price and then this value is compared to the minimum shape surcharge.

Environment variable `MINMODZU_NUR_AUF_GRUNDPREIS`
Client reference: no

If the variable is active and has the value ON, the shape surcharge for the current IG price method is calculated only on the base price and not on the exchanged lites. To determine whether the minimum shape surcharge should apply or not, the shape surcharge on the exchanged lites is calculated. This variable only applies if "Shape surcharge on glass price" is set in the condition master data.

This means that if the shape surcharge should be calculated on the glass price, the shape surcharge and the respective exchange glass is calculated first. This total is compared to the minimum shape surcharge. If the total of the shape surcharges is less than the minimum shape surcharge, no shape surcharge is calculated on the exchange glass.

## 53.13. Size surcharge

### 53.13.1. IG/replacement

With the term "size surcharges" used here, reference is made to the "Size surcharges" dialog, not to the surcharge matrix. If the surcharge matrix is used, the surcharge is not calculated on the exchange prices. With size surcharges, the environment variable `ISO_GROSSZU_AUF_AUSTAUSCH` can be activated.

If the steps for the size surcharges are not sufficient, the exchange can also be calculated according to matrix. Here, the variable `ISOAUST_KEINE_MISCHMATRIX` must be heeded.

### 53.13.2. Size surchargers for processing and accessories

**alcib 13.04.19502**

For accessories and processings, by default no aspect ratio and area surcharges from the size surcharges are applied. With the environment variable `BEARB_GROSSZU_ALL = ON`, it can be achieved that these surcharges are also applied.

If, however, the environment variable `SEITENVERH_AUF_STUECKPREIS` is active, no aspect surcharge is applied to processings or accessories since their price is already included in the unit price and otherwise the aspect surcharge will be calculated twice.

**alcib 13.04.19732**

For accessories and processings, size surcharges are applied additively; not for glass.

e.g.
Glass: glass base price * overlength surcharge = result 1
Glass base price * area surcharge = result 2
Glass base price + result 1 + result 2

Accessories: Base price * overlength surcharge = result 1
(Base price + Result1) * area surcharge = result 2

Furthermore, for accessories and processings, the priority flag is not evaluated in the surcharge matrix. The environment variable `ZUSCHLAGSMATRIX_MIT_PRIO` only affects the price method 41 - IG-current.

With the environment variable `BEARB_GROSSZU_WIE_GLAS`, it can be accomplished that the surcharges for accessories and processings are calculated as for glass; that is, the size surcharges are not calculated additively and the priority flag from the surcharge matrix is evaluated.

### 53.13.3. Aspect ratio surcharge

**Aspect ratio surcharge on the unit price**
**#120141**

In the current version, there is the configurable possibility to define an aspect ratio surcharge that is calculated on the unit price of the glass. This logic is available for header articles with the price methods IG-current, PCd-LAMI, PCd-TGH, PCd-basic glass or PCd-finishing in the sales price calculation.

The aspect ratio surcharge can be created under Master data > Prices > Surcharges > Size surcharges on the Shp screen and assigned to the glass articles in the IG basic prices or in the article vectors.

The size surcharges can also be assigned customer-specifically in the conditions (per product group or per article).

The new logic replaces the old logic for IG-current, with which the aspect ratio surcharge was calculated on the glass basic price.

In the display of the item conditions in the document entry (Shift+F9 in the item), the aspect ratio surcharge is not displayed with this configuration. At the same time, the "Special surcharge" field is not available. (Up to A+W Enterprise QR2503)

The logic is controlled by the environment variable `SEITENVERH_AUF_STUECKPREIS`.

**Starting with A+W Enterprise QR2503**

For accessories and processings, by default no aspect ratio and area surcharges from the size surcharges are applied. With the environment variable `BEARB_GROSSZU_ALL = ON`, it can be achieved that these surcharges are also applied.

If, however, the environment variable `SEITENVERH_AUF_STUECKPREIS` is active, no special aspect surcharge is applied to processings or accessories since their price is already included in the unit price and otherwise the aspect surcharge will be calculated twice.

**Starting with A+W Enterprise QR2506**

If the environment variable `SEITENVERH_AUF_STUECKPREIS` is active, you could not use the special surcharge in the order item. In addition, the aspect surcharge was calculated in the item conditions, but not displayed.

The program has now been changed, so that even with the price calculation method IG_CURRENT the aspect surcharge is displayed in the item conditions and the special surcharge can be used.

### 53.13.4. Size surcharges on AIR surcharge

See "Prices > AIR surcharge > Size surcharges on AIR"

## 53.14. Reference price

During the document entry, in the current version it is possible to calculate a reference unit price for each item.

This reference unit price is compared to the current unit price of the item. If the current unit price is less than the reference unit price by a configurable percentage deviation, the person entering the document is asked to enter a reason for this deviation. (`REFERENZ_ABWEICHUNG`)

The reasons are saved with the document and are available for later evaluations through reports. The checking of the deviation is always done when exiting the current item.

The reference price is a sale unit price that is calculated with the prices and condition master data of a reference customer. The reference customer can be specified system-wide in an environment variable or stored for each customer in a configurable MP field (the field must be created as [NUM] [REF_CUSTOMER]).

When calculating the reference price, the order conditions and order prices are not drawn; the conditions of any existing project are also ignored. It is recommended that you maintain the prices and condition master data for the reference customer completely so that no messages about prices not found will appear during the calculation of the reference price.

The reference price logic allows that a customer can be assigned himself as reference customer. This configuration would allow the logging of the deviations, which occur due to order price or manual changes in the item conditions.

In addition it must be noted: If the BOM does not change between 2 items, the conditions are not re-determined. Only special dimension-dependent values are recalculated. If thus for a customer different conditions are maintained than for the reference customer, this can mean that there is a price deviation between 2 identical items.

Cf.: #136027

Previously it was the case that for each item whose price differs sharply from the reference price, a reason had to be entered. If you now activate the environment variable `REFERENZ_PRUEFUNG_AUFTRAG`, you will no longer be asked to give a reason for each item.
Instead, when saving the order, the screen with the data for the first deviating item will open. The reason given there will be taken over into all other items of this order.

**Restrictions:**
- The currency of customer and reference customer must match. When calculating the deviation, no different currencies are considered.
- The reference customer may not be assigned prices/conditions with price types that refer to the order total quantities. The reference price is always calculated per item and the total order quantities would never be considered.

**Configuration:**
- The table `cu_sgg_price_comment` with the structure
  `commenttxt (char 30)`
  `sprkz smallint - local language from alsysinfo`
  must exist and data must be contained.
- `Kposprvlfd-Set 1` must exist
- Private field in the market partner master data: numeric – `REF_CUSTOMER`

`REFERENZ_ABWEICHUNG` (client reference: no)
This environment variable is only evaluated if `REFERENZ_KUNDE` is active. The content of the variable is interpreted as a deviation limit in percent of the reference price. If the item price has more than the variance to the reference price defined here, the creator is asked in a sales document to enter a comment as an explanation for this variance.

`REFERENZ_KUNDE` (client reference: no)
The environment variable activates the logic of the reference price calculation and contains a default customer to which reference prices and conditions are assigned.

`REFERENZ_PRUEFUNG_AUFTRAG` (client reference: no)
(case #136027): This variable is only evaluated if `REFERENZ_KUNDE` is active. If this variable is activated, the entry of a reason for break is not required for each item for which the price differs significantly from the reference price, but the entry dialog in which the reason for break must be entered is displayed once when the document is saved. This reason is then written back to all affected items.

## 53.15. Terms in the order

### 53.15.1. Wrong prices in the order

If the price is changed manually in the order for a position to be ordered, only the change of the basic glass price is recorded in the context of the item condition as a manual change and transferred to purchasing. However, if the exchange price or the exchange factor of a glass is changed in IG, this change is overwritten during the price calculation within the generation of a purchase order.
This system was changed to the effect that changes of the SA exchange lists, the SA exchange prices and the SA exchange factors as well as the purchase exchange lists, the purchase exchange prices and the purchase exchange factors are recognized as manual changes and are thus also transmitted to the subsequent programs.

Further fields within the IG price calculation will be incorporated into this function as at version AWE5.3.

The following fields cause the manual flag to be set in the terms:

**Price method "IGU current" (artikel.vkptyp1 = 41) (purchasing and sales respectively)**
- Manual changing of the PLCD (not for implcit changes due to changing of the PCd)
- Matrix or vector number
- Basic Glass Price
- Base price calculation type
- Exchange list 1-3
- Exchange factor 1-3
- Exchange price 1-3
- Step surcharge type (not the step surcharge value)
- AIR surcharge type
- Calculation type of the special surcharge
- Factor
- Size rounding

### 53.15.2. Do not mark IG conditions as manual

The function expanded with version AWE 5 for detecting manual conditions of the price calculation type IGU-current goes too far for individual customers. Therefore, the function was made more flexible with the setting of an environment variable.

In the variables `KONDITIONEN_ISO_NICHT_MANUELL` you can define those fields with whose change you would not like to have the manual identifier set automatically.

## 53.16. Printable prices

### 53.16.1. Requirements

**Market partner master data; kaufpreisdrkz**

The variable `kaufpreisdrkz` from the kauf-Memrel (table kauf) decides whether for the current market partner (customer or supplier) printable prices should be determined. This depends on the setting in the market partner master data. On the Printout tab, the screen field print Gross price must be toggled to Y so that the printable prices are even set.

**Item master data**

In the item master data of the header article, the field `poffen` is evaluated. It can be set on the Prices tab in the Price display field. The field is evaluated depending on how the variable `DRUCKBARE_PREISE` is set.

`DRUCKPREISUMGEBUNG` (client reference: no)
This environment variable is evaluated if the variable `DRUCKBARE_PREISE` is not set or not equal to 1, 2 or 3. It specifies by how much the printable prices may deviate. If the deviation is greater, the prices will not be set. Which values are compared is described in the section "Description; `DRUCKBARE_PREISE` not set".

If this variable is not set, **0.01** is allowed as standard deviation.

`DRUCKBARE_PREISE` (client reference: no)
The environment variable has the characteristics:
1. The price per quantity unit or gross unit price should be printed
2. Price per quantity unit of the glass incl. the processing should be printed
3. The base price, gross price or both will be printed
- **other:** If the variable is different or not set, the gross unit price and price per quantity unit are set, insofar as the deviation does not exceed a particular value.

`SPEZIAL_ME_PREIS` (client reference: no)
If this variable is set, the printable price per quantity unit is calculated by adding all price-relevant sqm prices. If a non-sqm price is found, the printable price per quantity unit is not filled. (only for user=25)

### 53.16.2. Factor

It is first set to the factor of the header article. Normally, this will also be the printable factor. If the factors for exchange prices and/or subelement prices and/or processing prices differ from the factor of the header article, however, the printable factor will be set to **0.00**.

Background: It must be possible to calculate price per quantity unit and unit price apart from one another via the factor. This only works if the factor is the same for all partial prices.

The printable factor is set regardless of which environment variables or settings are set in the item master data or market partner master data.

If the factor of the header article is changed manually, it can happen that the processing factors therefore deviate. The environment variable `MANUELLER_FAKTOR_AUF_BEARB` can be used for this.

### 53.16.3. Prices

The printable prices are determined under the prerequisite that this is permitted for the market partner in question (kaufpreisdrkz). Then the price determination depends on the environment variable `DRUCKBARE_PREISE`. The sales prices are set in the following description; this applies analogously for the purchase price fields.

**`DRUCKBARE_PREISE = 1` (BRUTTO_STUECK)**

Depending on the setting for the header article in the item master data, the following printable prices are determined:
1. The price per quantity unit is printed:
   `druck_vk_me_preis = vkmepreis` (as determined in the course of the price calculation)
2. Insofar as the **printable factor** is set, the gross unit price is printed:
   If `SPEZ_BRUTTO_STUECKPREIS` is set
   `druck_vk_brutto_stkpreis = vk brutto stkpreis`
   (as determined in the course of the price calculation)
   otherwise:
   `druck_vk_brutto_stkpreis = stkpreis/druckbaren Faktor`
   If the printable factor is 0, however, the printable gross unit price is not filled.
3. Both the price per quantity unit and the unit price should be printed. The setting of the fields is done precisely as described for 1 and 2.

Any other setting for `poffen` in the item master data causes the printable prices not to be set.

**`DRUCKBARE_PREISE = 2` (ME_GLAS_MIT_BEARB)**

Depending on the setting for the header article in the item master data, the following printable prices are determined:
1. The price per quantity unit is printed
   `druck_vk_me_preis = stkpreis / Glasfläche`
2. Insofar as the **printable factor** is set, the gross unit price is printed:
   `druck_vk_brutto_stkpreis = stkpreis/druckbarer Faktor`
   If the printable factor is 0, however, the printable gross unit price is not filled.
3. Both the price per quantity unit and the unit price should be printed. The setting of the fields is done precisely as described for 1 and 2.

Any other setting for `poffen` in the item master data causes the printable prices not to be set.

**`DRUCKBARE_PREISE = 3` (DRUCK_GRUND_BRUTTO_NETTO)**

Depending on the setting for the header article in the item master data, the following printable prices are determined:
1. The price per quantity unit is printed:
   `druck_vk_me_preis = grundpreis` (as determined in the course of the price calculation)
2. Insofar as the **printable factor** is set, the gross unit price is printed:
   `druck_vk_brutto_stkpreis = brutto_stueckpreis`
   (as determined in the price calculation)
   If the printable factor is 0, however, the printable gross unit price is not filled.
3. Both the price per quantity unit and the unit price should be printed. The setting of the fields is done precisely as described for 1 and 2.

Any other setting for `poffen` in the item master data causes the printable prices not to be set.

**`DRUCKBARE_PREISE` is not set**

If the variable `DRUCKBARE_PREISE` is not set or if it has a value other than 1, 2 or 3, the print price determination is done as described here.

In this case, the environment variable `DRUCKPREISUMGEBUNG` is relevant.

Regardless of `poffen` in the item master data, there is an essential attempt to set both the price per quantity unit and the unit price.

- **Price per qty.unit:**
  `druck_vk_me_preis = vk_me_preis` (as determined in the price calculation)
  Before setting, there is a check whether `vk_brutto_stkpreis` and `vk_me_preis * Fläche` no longer deviate from one another as defined via the variable `DRUCKPREISUMGEBUNG`.

- **Unit price:**
  `druck_vk_brutto_stkpreis = vk_brutto_stkpreis` (as determined in the price calculation)
  Before setting, it is checked whether `stkpreis` and `vk_brutto_stkpreis * druckbarer Faktor` no longer deviate from one another as defined via the variable `DRUCKPREISUMGEBUNG`.

**`SPEZIAL_ME_PREIS` is set**

If this environment variable is set, the price per unit quantity determines from the total of the prices per unit quantity of the header article, the exchange glass, and the processings/subelements.

If there is only one article for which a unit price is defined instead of a price per quantity unit, the special price per quantity unit (spez_mepreis) is not set.

- **Price per qty.unit:**
  `druck_vk_me_preis = spez_mepreis` (insofar as spez_mepreis is set)
- **Unit price:**
  If the printable factor is set:
  `vk_brutto_stkpreis = stkpreis / druckbarer Faktor`
  If the printable factor is 0, the gross unit price is not filled.

There is an essential attempt to set the printable unit price and the printable price per quantity unit, regardless of the settings in the item master data and the market partner master data and regardless of any other environment variables.

## 53.17. Environment variables

`AUSTAUSCH_VEKTOR` (client reference: no)
The variable controls that exchange prices can be stored in IG and LAMI for vectors. The price calculation then searches for exchange prices for the respective article. If none is defined, the system searches for the corresponding vector number for the article and checks whether a price has been defined for it.
The individual values define the range of conditions:
IG prices | LAMI prices | IG conditions | LAMI conditions
Example: 0|1|0|1 => for LAMI prices and LAMI conditions, vectors can also be entered; for IG not.
This variable replaces `KUISOAUST_VEKTOR`.

`BEARB_GROSSZU_ALL` (client reference: no)
For accessories and processings, by default no aspect ratio and area surcharges from the size surcharges are applied. If this variable is active, these are also calculated.

`BEARB_GROSSZU_WIE_GLASS` (client reference: no)
For accessories and processings, size surcharges are applied additively.
Base price * overlength surcharge = result 1
(Base price + Result1) * area surcharge = result 2
For glass, calculation is always on the base price
Glass base price * overlength surcharge = result 1
Glass base price * area surcharge = result 2
With the environment variable `BEARB_GROSSZU_WIE_GLASS`, it can be accomplished that the surcharges are not calculated additively

`BEARBMASSRUND_WIE_GLAS` (client reference no)
If this variable is set, the processing dimensions are rounded with the same dimension rounding as the article to be processed. If the variable is not set, the dimension rounding for the processings is retrieved from the `BEARBMASSRUNDUNG` variable.
VA side only.

`CUTOUT_PRICELM` (client reference: no)
Calculates for corner/edge/inner cut-outs and QU=LM the correct linear meters for the price calculation if the prices go according to LM (does not consider if the positioning wanders edge to corner cut-out or inner to edge cut-out, for example)

`DEFAULT_AUST_FAKTOR_VSG` (Client reference: No)
If the environment variable is set, then with exchange in the VSG in the IG, the exchange factor of the VSG in the IG is used instead of the item factor. (#218372)

`DRUCKBARE_PREISE` (client reference: no)
The environment variable has the characteristics:
- 4: The price per quantity unit or gross unit price should be printed
- 5: Price per quantity unit of the glass incl. the processing should be printed
- 6: The base price, gross price or both will be printed
- other: If the variable is different or not set, the gross unit price and price per quantity unit are set, insofar as the deviation does not exceed a particular value.

`ESG_MIN_BEAPREIS` (client reference: no)
The environment variable switches the maintenance and evaluation of the minimum processing prices for processings in TG. Only if one of these variables is set you can enter the menu item "Master data > Prices > PCd prices > Minimum processing prices".
See also: `VSG_MIN_BEAPREIS`.

`GROSSZU_AUF_SZR` (client reference: no)
By default, size surcharges are not added to the AIR surcharge. With the environment variable `GROSSZU_AUF_SZR = ON`, it can be achieved that size surcharges of the type "Percent" are applied to the AIR surcharge.

`ISOAUST_KEINE_MISCHMATRIX` (client reference: no)
If this environment variable is active with the value ON, then for an IG exchange price with the calculation type Matrix, the price is calculated from the specified matrix directly as exchange price.

`KEIN_TZ_BEI_SPEZARTPRS` (client reference: no)
If special article prices or processing prices are available and this variable is active, the inflation surcharges and discounts switched off (SC=0 and factor=100). The procedure applies to purchasing and sales.
**Attention:** This variable (hole_konditionen) overrides the variable `BEAFAKTOR_WIE_GLAS` during automatic price calculation!!

`KONDITIONEN_VSG_WAGRP` (client reference: no)
If this variable is active, expanded functions for the LAMI step price calculation according to Wagrp can be used. The LAMI product group can be stored as variable value.
Here, the entry of * is allowed. (Vg #237980)

`KUARTPRS_VEKTOR` (client reference: no)
If the variable is active, it is possible to store special article prices for article vectors. The price calculation then first searches for a special price for the article. If no price is found, a special price with the vector number assigned to the article is searched for next.
Evaluation during sales price calculation for objects (sales), customers, customer groups and during purchase price calculation for objects (purchasing) and suppliers. The logic only applies to header articles and not to accessory subparts

`KUBEAPRS_VEKTOR` (client reference: no)
If the variable is active, it is possible to store special processing prices for processing vectors. The price calculation then first searches for a special price for the article. If no price is found, a special price with the vector number assigned to the article is searched for next.

`LIEFERANTENPREISE` (client reference: no)
Purchase prices: If this variable is set, the supplier prices from tables artliefzu, artvarzu, and artfarbzu override the prices found based on supplier conditions.

`MANUELLER_FAKTOR_AUF_BEARB` (client reference: no)
If the variable is set to ON, manually changed glass factors are also applied to processing and accessories.

`MINBER_AUF_KANTE` (Client reference: No)
If this variable is set, the minimum calculation per edge is calculated when the processing prices for grindings (article category 550) are determined if the price category GR/TQ is maintained and the article has the basic unit of measure linear meter or millimeter.

`MINBER_WIE_GLAS` (client reference: no)
If this variable is set, the same minimum calculation for processings is calculated as for the main articles to be processed.

`MINMODZU_NUR_AUF_GRUNDPREIS` (Client reference: no)
If the variable is active and has the value ON, the shape surcharge for the current IG price method is calculated only on the base price and not on the exchanged lites. To determine whether the minimum shape surcharge should apply or not, the shape surcharge on the exchanged lites is calculated.
This variable only applies if "Shape surcharge on glass price" is set in the condition master data.

`NEUKALK_VKEK` (client reference: no)
For the environment variable active with the value ON, pressing <Ctrl+F9> or <Shift+F10> displays a query dialog on the price field in a position of a sales document, containing a toggle field where the user can select the following:
No recalculation | Sales and purchase prices | Sale prices | Purchase prices.
Accordingly, no price, a, only the sales price or only the purchase price will be recalculated.

`REFERENZ_ABWEICHUNG` (client reference: no)
This environment variable is only evaluated if `REFERENZ_KUNDE` is active. The content of the variable is interpreted as a deviation limit in percent of the reference price. If the item price has more than the variance to the reference price defined here, the creator is asked in a sales document to enter a comment as an explanation for this variance.

`REFERENZ_KUNDE` (client reference: no)
The environment variable activates the logic of the reference price calculation and contains a default customer to which reference prices and conditions are assigned.

`REFERENZ_PRUEFUNG_AUFTRAG` (client reference: no)
(case #136027): This variable is only evaluated if `REFERENZ_KUNDE` is active. If this variable is activated, the entry of a reason for break is not required for each item for which the price differs significantly from the reference price, but the entry dialog in which the reason for break must be entered is displayed once when the document is saved. This reason is then written back to all affected items.

`RUNDUNG_3NACHKOMMASTELLEN` (client separation: no)
If this variable is active, the price-relevant dimensions are rounded to three decimal places. By default, rounding is to 2 decimal places.
ON - Sales
SA+PU - Sales and purchasing including material costs
**Note:** This does not affect the physical quantity of the position. `RUNDUNG_PHYMESTK_3STELLIG` is responsible for this.

`SEITENVERH_AUF_STUECKPREIS` ( client reference: no)
If this environment variable with the value ON is active, then the aspect ratio surcharge from the size surcharges for all glass price methods is calculated on the unit price.

`SPEZATLFAKT_KOPFWAGRP` (Client reference: no)
If this variable is set, the product group that arises due to the product group logic for the header part after the exchange is used for the evaluation of the exchange list factors. If the variable is not set, the product group of the exchanged glass is used.

`SPEZIAL_ME_PREIS` (client reference: no)
If this variable is set, the printable price per quantity unit is calculated by adding all price-relevant sqm prices. If a non-sqm price is found, the printable price per quantity unit is not filled. (only for user=25)

`VSGAUSTAUSCHPRS VERERBEN` (client reference: no)
If the variable is active and set to 1, manually changed LAMI exchange prices are inherited in items with the same BOM header number.
The inheritance takes place when the item is newly entered; a subsequent price recalculation overwrites the manual values. The value can be specified in two parameters. If the first parameter is 1, only the manual changes during the current document entry are to be temporarily noted. If the second parameter is 1, the existing information is considered manual when the order is reloaded.

`VSG_MIN_BEAPREIS` (client reference: no)
The environment variable activates the maintenance and evaluation of the minimum processing prices for processing in LAMI. Only if one of these variables is set you can enter the menu item "Master data > Prices > PCd prices > Minimum processing prices".
See also: `ESG_MIN_BEAPREIS`.

## 54. NR server / number ranges

### 54.1. Allocation of invoice and credit note numbers via SPs

**(#112491)**
Increasingly, our customers are confronted with a situation where invoice numbers and the numbers of credits should be assigned from different number ranges. Here, the criteria according to which the number range is selected are different from case to case.

Now there is a logic with which the number range from which the number for a particular invoice or credit in sales or purchasing is assigned is selected via a SP.

Here, there are two possible parameters, which are optionally available to the SP for determination of the correct number range:
- Site number
- Market partner number

The logic is enabled by environment variable `RECH_NRKREISE_HNR`.
This variable is assigned with a bit vector (default "0000"). The number 1 means that for the corresponding transaction type, the selection of the number range is done via a SP.
- Point 1: number ranges for sales invoices will be assigned via SP "kaufGetRechkreis".
- Point 2: Number ranges for sales credits are assigned via SP "kaufGetGutskreis".
- Point 3: Number ranges for sales invoices are assigned via SP "kaufGetEKRechkreis".
- Point 4: Number ranges for purchasing credits are assigned via SP "kaufGetEKGutskreis".

The parameters that the respective SPs get when calling from Alcib are controlled by the environment variables
- `KAUFGETRECHKREIS_PARAMS`
- `KAUFGETRECHKREIS_PARAMS`
- `KAUFGETGUTSKREIS_PARAMS`
- `KAUFGETEKRECHKREIS_PARAMS`
- `KAUFGETEKGUTSKREIS_PARAMS`

The SPs must always deliver a valid number range.
See also "EN-CONFIG-A+W Enterprise Internal Client Separation"

### 54.2. Release locks #416415

In very rare cases it happened that a number lock got stuck in the number server, which could not be resolved without restarting the number server. This is particularly critical for large multisite systems with many sites, as the entire multisite had to be restarted.
So that this is no longer necessary in the future, it is now possible to release these locks manually. This must be done very conscientiously, otherwise several users will be able to process the same order, for example.

The procedure for lock release is as follows:
In a shell session to the corresponding site, enter the command "killserv info". From this, in the area NR_STATUS, the corresponding number range, the locked number, and the employee number of the user holding the lock are determined. In addition, the command "psgrep <Login of the user>" determines the PID of the process holding the lock. If this process no longer exists, the PID can also be determined from the area ZU_STATUS of the "killserv info" output.

The lock is then released via :
`alcib -nrexit <numberrange> <number> <manr> <pid>` (This output also appears if you enter only alcib -nrexit.)

After executing this command, the message appears:
Unlock numberrange `<numberrange>` number `<number>` manr `<manr>` pid `<PID>`
rc=`<ReturnCode>`

If successful, the return code -101 is output. In addition, by restarting the command "killserv info", you can check whether the deletion of the lock was really successful.

Please note: For order blocks, in addition to the external order number from the number range "Ip.kaufex.mfo", the internal order number from the number range "Ip.kauf.mfo" must also be released.

### 54.3. Re-use of invoice numbers without invoice document

**[AW-81443]** In extremely rare cases (program crash directly after the final invoice number has been assigned) it can happen that during the assignment of invoice numbers, there are gaps. Since these gaps can cause problems in controlling, a possibility has been created to re-use these numbers. For this, there is now a program setting with which the number server checks for a dedicated period in the past whether such numbers exist. These are then included in the number pool and re-assigned during the next invoice generation.

This logic can only be used if you are not working with site-specific invoice number ranges within a multi-site system.

In this context, the log `$PROTOPFAD/Rech<mmdd>` is expanded to include the entry "Action successfully completed".

**NRSERVER_CHECKNOTUSEDINVOICENO**
This variable switches on a check in the number server that ensures that gaps in the number range "rechex.mfo" are filled again. The value of the variables must contain the number of days in the past that the number server should check. If in this period for a number there is no Kauf record with document 7 present, the number is inserted into the pool and re-assigned on the next request. Caution: Here there are mismatches in the sequence of the assigned invoice numbers.

This variable must be set so that backdated invoices fall in any case within the time frame to be checked; otherwise they will be detected as not used and reassigned.

## 55. Product and sash size sets

### 55.1. Sash size sets

With case #147145 the customer-specific sash size sets were developed. This function was bracketed with environment variable `MODUL_SASCH`.

Version 2008 allows the storage of sash sets in Master data-> Keys-> Products-> Sash Size Sets. These consist of the quantity and the sizes (width and height) of up to ten items. These sash size sets can be used at document entry. A product code must be entered for each article to be generated. These items will then be generated automatically.

**Master Data > Keys > Products > Sash Size Sets > Manufacturer Code**
This menu item is used to create the manufacturers who work with these sash size sets. First enter a unique number, then the description (or manufacturer's name). The information is saved in database table 'xsashsizemakercode'.

**Master data->Keys->Products->Sash size set->Classification code**
The classification code serves to group the sash size sets. Since there are several million sash size sets, this additional level is quite useful. In the header of this dialog logic, you can restrict the records to be processed to those for a certain manufacturer. You can also enter the first few characters of the classification code, followed by an asterisk. This allows you to further restrict the records to be processed. If you enter neither the manufacturer nor the start of the classification code, all records will appear in the menu.

If you enter a manufacturer code in the header, you can change or enter only the classification code and description in the menu body. Otherwise, you can edit the classification codes of all manufacturers. The information is saved in database table 'xsashsizeclasscode'.

**Master Data > Keys > Products > Sash Size Sets > Sash Size Sets**
Use this dialog to generate or change sash size sets. In the header, enter a manufacturer code because without a restriction, you will get too many hits. In addition, you can restrict the number of hits by selecting a certain classification code or by entering the start of a classification code followed by an asterisk. You can further restrict the part codes to be processed by entering the start of a part code followed by an asterisk.

If you open the footer dialog, all part codes matching the information in the screen header will be loaded. These can be amended. You can enter new part codes as well. These have to match the restrictions defined in the header. The first mode dialog enables you to enter the part code and also amend the size. This will be used to adapt the glazing channel. The mode dialog now allows you to enter a name for this part code and the sizes and quantities for up to ten items. The information is saved in database table 'xsizemaster'. Since every manufacturer has its own sash size sets, a sash size set cannot be identified by its part code alone. You will always need a manufacturer code as well.

As there are many sash size sets, the master data tables for the customer are not filled via this dialog; instead, the data is loaded into the database via script. The dialog usually only serves to make minor adjustments.

**Document entry**
Solely due to the activation of the environment variable `MODUL_SASCH`, the entry of the sash size set in the order is not possible. (see Chapter 40.2)

In the product code field from document entry, press <Ctrl+F10> to apply the sash size sets. First select the part code you want to use, and enter a multiplier. The actual quantities for the individual items are calculated from the quantities defined in master data using this multiplier. This brings you to a screen listing all items belonging to this part code. Enter a product code for every item. The items will now be inserted into the order.

### 55.2. Product sets

In the master data, the so-called product sets can now be entered. Basically, such a set consists of several predefined items that can be consulted in order entry.

In the master data, it is possible not just to store completely new product sets, but also those with the reference. For the specification of the reference process, it must be heeded that only "customers' own" product sets can be used as reference cases. Under Master data -> Finished products -> Product sets, the product sets (with one or several items with defined structure and dimension) can be entered anew and existing product sets can be changed.

Currently, there are two possible function scopes:
- Entry depending on the manufacturer (Kauf.exbez2), `MODUL_PRODSET=0`
- Generally valid entry, which is relevant for KERMI interface, `MODUL_PRODSET=1`.

In the process, the number of the product set is assigned from an individual number range (nr_kreise.mfoname=sasche)

Thus, it is possible to enter the product sets either for a special customer (entry in the field Kunde) or you create a general "product set customer," whose product sets are generally valid.

If you also want to process the products sets via external EDI, the reference hierarchy must be heeded: Customer - A/Z debtor - Default product set customer, which is configured in the EDI.

For the use of product sets within the external EDI, additional restrictions have to be heeded, which are described in the configuration instructions "EN-CONFIG-A+W Enterprise EDI".

#### 55.2.1. MODUL_PRODSET=0

With case #145771, the first product set entry for manufacturers was developed. This development is customer-specific.

Entry of customer-specific sash size sets is only possible if the environment variable `MODUL_SASCH` is active. (see Chapter 40.1). The use of these sash size sets in order entry is associated with the environment variables `MODUL_PRODSET=0` and the database configuration `SASH_DB`.

To be noted here is that this logic was developed in 2008 especially for a customer, but it was not implemented. It is recommended that you not use this configuration.

#### 55.2.2. MODUL_PRODSET=1

For the setting `MODUL_PRODSET=1`, A+W Enterprise is configured for the entry of product sets. In addition, the `SASH_DB` must be activated. The database name for the creation and obtaining of the products sets is stored in these variables. This variable must absolutely be set if in Master data -> Finished Products -> Product sets you create and change the product sets.

For the order scheduling of the product sets used, `MODUL_PRODSET_DFUE` must be activated. All module variables are for-fee modules.

**Master data entry with reference**
Here it must be noted that the attached document is not copied to a new, order-specific or product-specific directory; instead, it remains in the old storage location. In the new product set, reference is made to the storage location from the original product set. This means that if the document is changed, it is changed in the original product set and in all orders generated via external EDI in which the product set was used.

**Document entry**
This product set can then be used in order entry. For this at item entry, just enter the set number instead of the product code or select it with <Ctrl+F9>. On the search dialog (<Ctrl><F9>), the hit quantity can be reduced by entering the manufacturer (customer in the product set master data) or an object, product type or product set name. Here, the entry is not required and the search can be started directly with <F3>.

With a double-click on the desired product set or by pressing the [OK] button, the product set is marked for transfer into order entry. The cursor activates the Quantity multiplier input field. Enter the desired multiplier. The complete product set will be added to the document. The item quantity is calculated from the quantity in product set times the multiplier.

In the order entry, product sets can also be entered in other customers' orders.

The set number is noted for all items and displayed in the order, item level, Properties tab. The order items entered this way can be changed. You can also delete elements of the set.

If a product set has been entered only with a global net price (no item prices) and you adopt the set, an additional price item will be added showing the net price for the entire set. Automatic creation of the total price requires amendment of master data. Please contact your project manager if you want to use this function.

**Additional possibility in the configuration: SASHPREISARTIKEL**
If the variable is activated, during the entry of a product set, an extra price item with the fixed price is attached to the transaction. As value, the variable must include the article number for this additional price item. If the switch is not set, the price is not taken over.

If the article is not defined in the master data, there will be problems during the entry: there is no takeover of the price.

**Restriction**
If product sets should be used within the external transaction interface, it is absolutely necessary that each product set consist of precisely one item. In addition, the product set name may not contain the following characters:
- ` ` (0x20) space (SPC)
- `\t` (0x09) horizontal tab (TAB)
- `\n` (0x0a) newline (LF)
- `\v` (0x0b) vertical tab (VT)
- `\f` (0x0c) feed (FF)
- `\r` (0x0d) carriage return (CR)

For the use of product sets within the external EDI, additional restrictions have to be heeded, which are described in the configuration instructions "EN-CONFIG-A+W Enterprise EDI".

**Document allocation**
If documents are attached to the product set via document link, the link is not taken over in the order during entry.
#410440: Starting with alcib – build 13.04.0655 (December 2017) the files are taken over into the order and copied into an order-specific directory.

**Article replication**
Product sets are not replicated. If they should be used in several locations, the use of a central product set database (SASH_DB) is recommended.

With A+W Enterprise 6 Build 01.02.2020, product sets can be transferred via internal EDI. For this, the product sets must be created in the master data and then entered into the table via individual scripts/procedures. Here it must be noted that the field intver must be = 3. See also "EN-CONFIG-A+W Enterprise EDI"

**External order interface**
The functionalities relating to the use of product sets within the external order interface are described in the special documents "EN-A+W-EDI Import" and "EN-CONFIG-A+W Enterprise EDI".

## 56. Delivery note creation from shipping

### 56.1. Error status

During delivery note generation in shipping, the following errors can occur, which are logged in the Lieffrei log.
- 772: The transaction X has a disused currency!
- 775: Delivery note X cannot be generated because a limit was exceeded.
- 778: Delivery note X cannot be generated due to a delivery stop.
- 779: Order X is a stock order. Delivery note cannot be generated.
- 780: Customer not in the database. Delivery note cannot be generated.
- 781: Delivery note for order X cannot be generated due to missing goods receipts.

### 56.2. Sending of delivery notes as e-mail on generation in dispatch

**[AW-166963]**
**Caution:** This function cannot be used together with "Delivery note printing in dispatch depends on a configurable field in the market partner master data".

If delivery notes are generated in dispatch, there is always a direct query for the corresponding printer. Now, over time, things have changed so that all delivery notes should not really be printed on paper; instead, they should be sent via e-mail.

Through configuration with the environment variables `LAPOOL_LS_EMAIL`, you can control from dispatch whether the delivery notes generated should be printed out or sent directly via e-mail.

For this, the form type of the form to be sent is entered in the environment variables. After generation of the delivery note in the dispatch control, with active logic, the dialog for sending the e-mail opens. This is the familiar dialog from the menu "Sales > Forms > E-mail". The e-mail recipient is determined and suggested by the existing function. It can be changed on this dialog. Similarly, you can use the code in the first column to determine whether or not the delivery not should be sent by mail.

If the delivery note is marked as "do not send" here, it will also not be printed. It will only be generated and can be printed later manually in Sales - Forms.

If this function is active and there is a partial delivery note for an order that was not yet sent via mail, then with generation of the following partial delivery note, it is offered again for mail dispatch. In the transition time, this can cause partial delivery notes that were already sent to the customer to be sent again via mail.

Therefore, we ask you to heed the following: Since especially in printing and in mail dispatch many customer-specific configurations and customizings are possible, the use of this function must be tested intensively at the customer's. A+W Enterprise can unfortunately not be tested in advance for all configuration and customizing variants.

### 56.3. Delivery note printing in dispatch depending on a configured field in market partner master data

**Caution:** This function cannot be used together with "Dispatch of delivery notes as e-mail during generation in dispatch" Similarly, this function cannot be used with the packing view of the dispatch control (`LAPOOLART = 3`).

The delivery note generation and the associated printing process in dispatch control were expanded, so that not all delivery notes generated must be printed.

**Installation:**
- A new private field in the market partner master data is required (Ifdnr=3001)
- A new set of configurable fields for the order header is required.
- The environment variable `LAPOOL_DNPRINT_VIA_MP = ON` must be set
- Binary lapool and alcib September 2024

The following installation scripts can be used for the system.
`/develop/globfiles/kflddef/mpprffld/set_VKLS.sql`
`/develop/globfiles/kflddef/kaufprvfld/set010.sql`

**IMPORTANT** As soon as the script "set_VKLS.sql" has been executed, you must enter the menu element "Master Data > Field Configuration > MP Field Configuration" and save. The question "Should the configured MP field be re-distributed to the market partners?" must be answered with "yes". Now the new field is generated for all market partners with the reserved Ifdnr=-3001 (DB table prvfld). The pre-population is done with 0 and printing is thus excluded for all market partners. Starting at this time, the logic is activated with regard to the assessment.

**CAUTION:** If you are working with market partner replication in this area, this may be done exclusively in the master.

The data in the order-related set is pre-populated during entry from the market partner master data. Here, both the data for customers as well as the data for a project entered is evaluated. If for the customer or project the new setting for printing the delivery notes from dispatch with = 1(YES), then the print=1(YES) is set automatically. However, it is not possible to overwrite the data directly in the order.

In dispatch on the route and order level, a new field was activated, which displays the data from the order.

On the route level, the field is active if at least one order is marked for delivery note printing. The flag is only displayed in dispatch and cannot be changed.

Due to limited space, the field "I(nformation)" was removed from the main overview. If on a route there is at least one order with dispatch information, it is displayed at the lower edge.

On the order level, the order information is abbreviated and displayed on the lower edge. The complete display is, as earlier, on the tab "DispatchInfo 1".
The determination is done first via order data. If the order was entered before creation of the new set, then the data from the customer/project is still evaluated. If the field is also not found in the market partner, then the logic applies as not active.

If you generate the delivery notes for a route via the menu "Delivery notes release+printing" and at least one order is on DN-print, then the data for the printer is queried. Then only the delivery notes are forwarded for printing that are on printing "yes". For the remaining orders, the delivery notes are only generated.

### 56.4. Plausibility check

During generation of delivery notes from dispatch, a plausibility check can be switched on by setting the environment variable `LIEFERSCHEIN_CHECKER`. This includes two aspects.
- For all ordered parts of the items to be delivered, it is checked whether goods receipt has been booked for a sufficient quantity.
- For all stock items, it is checked whether the number to be delivered is actually in the specified stock. The check is only done for header parts.

### 56.5. Configuration

`LAPOOL DNPRINT VIA MP` (client reference: no)
Controls the printing of delivery notes from dispatch via a configurable field in the market partner master data. If in the market partner master data you see "no printing"(=0; default), then the delivery notes are only generated in dispatch and not printed. Not possible together with `LAPOOL_LS_EMAIL`.

`LAPOOL LS EMAIL` (client reference: no)
In these environment variables, the form type is entered that should be used if the delivery notes from dispatch should not be printed, but rather sent as documents via e-mail. Not possible together with `LAPOOL_DNPRINT_VIA_MP`.

`DELIVERY NOTE CHECKER` (client reference: no)
AWD #125465
This environment variable activates a plausibility check for the delivery note generation (dispatch):
Ordered articles => Check for goods receipt...
Stock article => Check that there is no shortage.

## 57. Automatic delivery note creation in the background

This functionality was developed with Version 2008.2 and enhanced with Version 2012.

### 57.1. General process

Via a script, a file is generated in which the delivery notes to be generated are included. This file must absolutely be in `$ALDATPFAD`. Then, the program "lapool" starts with the parameters "AUTOLS" and the file name to be processed (relative to `$ALTDATPFAD`). ("lapool AUTOLS `<file>`").

#### 57.1.1. Log

The result of reading in each line of the interface file is logged in `$PROTOPFAD/AUTOLS<mmdd>`.

**AUTOLS_TEST:** With this environment variable, the FTEST for the background delivery note generation can be switched on. The value of the variables represents the test level.

#### 57.1.2. Processing of the transfer file

If the program lapool is started with the parameter "AUTOLS", the program searches in the directory `$ALDATPFAD` for a file that was transferred as 2nd parameter with the program call (Call: "lapool AUTOLS `<filename relative to $ALDATPFAD>`").

If this file cannot be read, the program ends with the error code 5555. At this time, no additional log was written. This error must be checked by the blanket script and logged.

Then there is a check whether the transfer file contains data. If this is not the case, then `$PROTOPFAC/AUTOLS<mmdd>` is logged and the program ends without error code.

The processing of the transfer file is done line by line. If a line of the transfer file can be read in successfully, this is logged in `$PROTOPFAD/AUTOLS<mmdd>`.

Then there is a check whether with the data transferred there is a data record in dispatch (table: lapool) that was not cancelled (storno=0) and there is an outgoing order (vmodus=0). If no data record was found, this is logged in `$PROTOPFAD/AUTOLS<mmdd>` and the system message 72 is sent to the employee `$AUTOLS_MANR`. Then the next line of the transfer file is processed.

If the order was found, then there is a check whether there is already a delivery note. If this is the case, this is logged in `$PROTOPFAD/AUTOLS<mmdd>` and the system message 72 is sent to the employee `$AUTOLS_MANR`. Then the next line of the transfer file is processed.

If there is no delivery note, there is a check whether the planned arrival date (lapool.ankunft) is within a completed period. This check only takes place if the environment variable `PERIODENPRUEFUNG` is enabled. If the arrival date is within a completed period, this is logged in `$PROTOPFAD/AUTOLS<mmdd>` and the system message 72 is sent to the employee `$AUTOLS_MANR`. Then the next line of the transfer file is processed.

If there is no delivery note and if the arrival date is outside of a completed period, then there is a check whether the order was already reported completely packed. If the order has not yet been booked completely packed, this is logged in `$PROTOPFAD/AUTOLS<mmdd>` and the system message 72 is sent to the employee `$AUTOLS_MANR`. Then the next line of the transfer file is processed.

If there is no delivery note and if the arrival date is outside of a completed period and if the order was booked completely packed, then there is a check whether the order is still being processed by the order completion (process: intauf) or by the booking process (process: rserv). If this is the case, this is logged in `$PROTOPFAD/AUTOLS<mmdd>` and the system message 72 is sent to the employee `$AUTOLS_MANR`. Then the next line of the transfer file is processed.

If there is no delivery note and if the arrival date is outside of a completed period, the order was booked completely packed and if the order is not in the processing of the background processes intauf and rserv, then there is a check whether the route for the order is a regular route to the customer. If the route is an internal route (routenkz=4), then this is logged in `$PROTOPFAD/AUTOLS<mmdd>` and the system message 72 is sent to the employee `$AUTOLS_MANR`. Then the next line of the transfer file is processed.

If the order has not yet been booked to transport and the environment variables `AUTOLS_WITH_TRANSPORT` and `FERTIGWARENLAGER_MIT_VLS` are set, then there is automatic booking to transport. If within this process an error occurs, this is logged in `$PROTOPFAD/AUTOLS<mmdd>` and the system message 72 is sent to the employee `$AUTOLS_MANR`. Then the next line of the transfer file is processed.

If in particular the variable `AUTOLS_WITH_TRANSPORT` is not set, it is assumed that the booking has already been made before the start of the automatic delivery note generation. This variable can be set within the script to start the automatic delivery note generation.

If the booking to transport was successful, then the actual delivery note generation is started. If within this process an error occurs, this is logged in `$PROTOPFAD/AUTOLS<mmdd>` and the system message 72 is sent to the employee `$AUTOLS_MANR`. Then the next line of the transfer file is processed.

**Summary of the checks**
1. Read transfer file in `$ALTDATPFAD`
2. Read line in transfer file
3. Non-cancelled order with transfer data from file exists as outgoing order
4. There is no delivery note yet
5. Arrival date is outside of completed period
6. Order is completely packed
7. Order is still before background process intauf
8. Order is still before background process rserv
9. If the order is not on an internal route (routenkz=4)
10. Booking to transport
11. Delivery note generation

### 57.2. Format of the transfer file

The program expects the following information in the transfer file:

| | | |
| :--- | :--- | :--- |
| Scheduled delivery date | lapool.ltplan | Char(10) |
| Order number | lapool.auftrnr | Long |
| Route number | lapool.routenr | Integer |
| Site number | lapool.hausnr | Integer |

The data is expected in a line separated by blank spaces. The delivery date is expected in `$DBDATE` format.

The result of reading in each line of the interface file is logged in `$PROTOPFAD/AUTOLS<mmdd>`.

### 57.3. Functions

#### 57.3.1. Locks

The process for automatic generation of the delivery notes may only be started once. For this, a lock logic outside of the program is required. This can be solved as follows:

`$IPCDIR/autoLS.<n>.log` is written by the blanket script `autols_batch.sh`.
The blanket script checks this log file and forbids a doubled start.

If the program lapool is started with the parameter `AUTOLS <filename>`, it first writes a lock file `$IPCDIR/autols.log`. This includes the PID of the lapool process. If this file cannot be written, the program ends with the error code 5555. At this time, no additional log was written. This error must be checked by the blanket script and logged.

### 57.4. Environment variables

- **`ALDATPFAD`**: Directory for the interface file. `$ALDATPFAD` is a global Unix environment variable.
- **`AUTOLS_MANR`** (client reference: no): Message recipient for the background delivery note generation. If the variable is not set, there is no e-mail notification by the program.
- **`AUTOLS_TEST`**: With this environment variable, the FTEST for the background delivery note generation can be switched on. The value of the variables represents the test level.
- **`AUTOLS_WITH_TRANSPORT`** (client reference: no): If this variable is active, the automatic generation of delivery notes assumes a previous transport booking.
- **`FERTIGWARENLAGER_MIT_VLS`** (client reference: no): The booking to the finished goods stock is made via the advance delivery note. At ADN goods are booked on "trucks" and only booked out of the site. But they are in FG stock with target site=-1. Only DN books out the records with destination site=-1. If no ADN is generated for the order, the data is output directly from house X for the DN. Source of error: Partially ADN and then completely LS not from shipping.
- **`LAPOOL_LS_PERIODENPRUEFUNG`** (client reference: no): If this variable is active, for the delivery note generation in dispatch it is checked whether the arrival date of the order lies within a completed period. If this is the case, the delivery note cannot be generated. `PERIODENPRUEFUNG` must be enabled for the actual period check.
- **`PERIODENPRUEFUNG`** (client reference: no): This activates the period end check for purchase invoices, goods receipts, and the mistaken quantity check in dispatch control. Purchase invoices, goods receipts, and mistaken quantity checks may be booked in an already-completed booking period.

## 58. Receipt of goods

### 58.1. Invoice transfer/automatic receipt of goods

For more information, see "EN-CONFIG-A+W Enterprise B2B Service ERP WS" and the documentation in Sharepoint:
[https://awsoftwaregmbh.sharepoint.com/:w:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/DE-A+W%20Enterprise%20Cust%20Auto%20Goods%20Receipt.docx?d=w10900c1fb5f645278125dda31105c10f&csf=1&web=1&e=eQMeMy](https://awsoftwaregmbh.sharepoint.com/:w:/r/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/DE-A+W%20Enterprise%20Cust%20Auto%20Goods%20Receipt.docx?d=w10900c1fb5f645278125dda31105c10f&csf=1&web=1&e=eQMeMy)

### 58.2. Check receipt of goods

#### 58.2.1. Automatic warehouse in / delivery note generation for direct delivery

This was implemented as default logic.
See AWDesk #334475.

Documentation in Sharepoint:
[https://awsoftwaregmbh.sharepoint.com/:w:/r/sites/AWClarityRD/Shared%20Documents/Configuration/EN-CONFIG-A+W%20Enterprise%20B2B%20Service%20ERP%20WS.docx?d=wfbedc124aae54176806873f8f37b36d7&csf=1&web=1&e=MSk9hm](https://awsoftwaregmbh.sharepoint.com/:w:/r/sites/AWClarityRD/Shared%20Documents/Configuration/EN-CONFIG-A+W%20Enterprise%20B2B%20Service%20ERP%20WS.docx?d=wfbedc124aae54176806873f8f37b36d7&csf=1&web=1&e=MSk9hm)

#### 58.2.2. Internal charging (customer-specific)

There is a possibility via a control pool to generate receipt of goods and purchase invoices based on the underlying PO and a received invoice.

This customer-specific solution is described in the following document:
[https://awsoftwaregmbh.sharepoint.com/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/DE-A+W%20Enterpprise%20%20Cust%20Auto%20Goods%20Receipt.docx?web=1](https://awsoftwaregmbh.sharepoint.com/sites/AWClarityRD/Shared%20Documents/Interfaces/Enterprise/B2B%20Interfaces/DE-A+W%20Enterpprise%20%20Cust%20Auto%20Goods%20Receipt.docx?web=1)

### 58.3. Rack-related incoming goods

(#335042) The rack-related incoming goods were expanded so that now a LieferID on the rack level can be entered. If the system is configured such that this LieferID must be entered, the rack number is left blank. In this case, the next free internal rack number is assigned by the system.
Furthermore, it is now possible, in addition to order-related purchase orders, to book stock-filling purchase orders via the rack-related incoming goods. Manual purchase orders cannot be booked here. Per rack, only one order type (order or stock) is allowed.

It is now possible using rack-related incoming goods to book stock orders to the rack stock. Here the registration point is used as slot and the Lieferid as external rack number. The rack number entered in incoming goods is used as internal rack number in the stock. However, it is not displayed in the stock module since here generally you are working with the external rack number. For the correct stock booking, it is important that in the purchase order a stock of the type rack stock was assigned to the order items; otherwise there can be no correct stock booking. To book the stock, first it is checked for a purchase order which items were already made ready in the stock forecast table wldispo. The booking of the incoming stock is based on the data of this table; however as booking quantity, the quantity that was entered in the rack-related incoming goods is used. The quantity of the table wldispo plays no role in this case. After the racks were booked in the stock, the stock booker ensures that the records of the table waeingestkopf and waeingestpos are backed up and deleted.

#### 58.3.1. Rack stock

The rack stock booking is subdivided into two areas, incoming rack stock and outgoing rack stock. Both dialogs initially display racks that are currently in the stock.

The incoming rack stock is used in order to book items to an existing rack or to enter an item on a new rack.

The outgoing rack stock is used to remove items from a rack, to rebook them to another rack or to book a rack into a different slot.

In the first step after entering the dialog, the filters are selected that limit the display of the racks in the stock. At the same time, the filters specify properties for racks that are newly booked into the stock.

The selection of the filters can occur in different combinations.
- **Article / Stock**
  Articles and stocks limit the display of the racks in the stock.
- **Article / Stock / Rack**
  After selection of article and stock, in the rack selection only racks are displayed that correspond to these criteria. After selection of the rack, only this rack is displayed.
- **Rack**
  The field 'G' for mixed is selected if there are different items or different variants of an item on a rack.

The list is sorted according to the time of the first rack loading booking.

#### 58.3.2. Booking of incoming rack stock

**Selection of the filters**
After the filters have been selected and the stock is displayed, the user can begin booking the new items into the stock.

**Review**
First there is a check of whether this is a new rack in the stock. If the rack is not in the stock, a new data record is created. If the rack is already in the stock, it must be checked whether the item in its variant is already on the rack. The system does not allow a new data record to be created for a variant that is already on the rack.

**Input**
If the item in its variant is already on the rack, the quantity that should be booked to the rack is entered in the 'Booking' field.

If the rack does not exist yet or if the current variant is not yet on the rack, the user creates a new data record at the end of the list.

In the first step, the user selects the variant using a selo.

The rack is entered in the second step. This can either happen via a direct input or the rack can be selected from the existing racks in a selo. In both cases, there is a check of the entry. If the variant is already on the rack, the selected rack is deleted and you either select a permissible rack or book the quantity to the existing data record.

In the third step, the slot is also entered directly or with a selo. The following check ensures that a rack cannot be booked into two different slots. If the rack is already assigned to another slot, then the slot found is selected automatically. In addition, the slot may only correspond to one of the specified registration points that are offered on the selo.

For permissible registration points, see the table `awc_alcimerfstellen`. As an additional limitation, there is a check whether the property `awc_alcimerfstellen.erftype` corresponds to the value of the environment variable `AWC_RACKSTOCK_REGPOINT_TYPE`.

Then the booking quantity and the price or price per unit are entered.

**Booking of outgoing rack stock**
In outgoing rack stock, items can be removed from a rack, whereby an order and an item can be specified. The procedure is different for header and child parts. Items can be rebooked to an existing or new rack and racks can be rebooked into another slot. The precise procedure is described in the following sections.

All upcoming bookings that are marked in yellow can be undone with the 'Reset' button.

**Removal of child parts in the rack stock**
The removal of child parts is done using production pick list via the menu element Stock > Booking > Outgoing rack stock. This dialog displays all associated racks for an item/stock combination, arranged according to the time of the first rack loading booking. For removal, you specify the quantity and the associated customer order item or stock filling order item.

The first field that you see when running through the data record is the order number. The order number can be entered or selected on a selo. The selection of the available order items on the selo is done based on the stock forecast for this item. In addition, the total quantity, the already-booked quantity and still-open quantity for the respective order item is displayed. If you exit the selo, the Item field is filled automatically with the selected order item. For a direct entry of the order number, the item must also be specified. The booking field is filled automatically with a selo selection. If there is a sufficient 'open quantity' available for the quantity on the rack, the booking field is filled automatically with the value in the quantity field. With a direct entry, the booking field is also checked and in the case that the value exceeds the 'open quantity,' it is lowered to the 'open quantity' value.

If you leave the data record, there is a splitting of the data record if the total quantity is not removed for this item/variant combination. That is, the value 'booking' is smaller than the value 'quantity.' The existing data record then contains the original 'booking' quantity in the 'quantity' and 'booking' fields and the selected order item. The first data record is now locked and as booking preparation, identified with a solid yellow dot.

The new data record is initialized with the remaining quantity ('quantity' - 'booking'). The view has now changed automatically from the order-related view to the 'rebooking' view. The user must book the remaining quantity to a new rack. For this data record only the fields rack and the associated slot can be selected; all other fields are locked. In addition, the data record is now marked as a half-filled data record with a half-filled yellow dot. If the rack and the slot are also selected, the data record is locked and the dot is filled out completely.

In order to reset a split booking, one of the two data records can be selected and then the 'Reset' button pressed.

For the removal of TGs, for example, the TG item must be set to stock change delivery note in the IG. Here the background process intauf ensures that for items with a rack stock, the table wldispo is booked as STD stock. This is necessary in order to be able to execute the removal with appropriate order reference in the outgoing rack stock.

The selection of the available order items and open quantity is determined by the table wldispo. With the limitation `b_status < 2` and `vorgang = 5` and `b_typ = -1` and the properties of the current data record, total (b_anz) booked (verbucht) and open (b_anz - verbucht) are determined. The program considers the quantities already assigned to another data record, corrects the 'booked' and 'open' quantities on the selo and in the check.

**Removal of header parts in the rack stock**
The removal of header parts with order reference is done analogously to the removal of the child parts. Here only the complete rack quantity can be removed and assigned to the order item. For this removal, the dispatch rack system is booked automatically. (tables gest and gestzu). If the order is still completely on a route, the rack "generated" in dispatch is also assigned directly to a route.

**Booking to a new or existing rack**
In the 'rebooking' view, an item can be booked to a new or existing rack.

As described in the incoming rack stock, the rack and slot selection are subject to limitations.

**Inventory in the rack stock**
The new dialog 'Inventory - rack stock' is used to correct the stocks in the rack stock. As in other stock types, the stocks for existing data records can be adjusted there. The 'target' column displays the current stock on a rack. The 'actual' column initially also displays the current stock, the new total quantity is entered. In the case that a rack should be booked to another slot, a new slot can be entered in the 'slot' column or selected in a selo. Only slots can be entered that are also specified in the selo. The available slots are determined as described in the 'incoming rack stock' section. The slot for other data records that contain the shifted rack is automatically changed too.

Data records can be deleted with F7. New data records are created when you call up the dialog for entering new data records with F6. In the first step, the item of the new data record is selected, then the variant and color. Racks can only be entered directly unless a selo can be called up since only new racks may be entered. In the end, for complete identification, the slot must be entered that is selected in a selo.

In order to enter the new data record completely, the stock fields must be filled and if necessary a remark can be added.

**Incoming stock via Barcoding rack bookings for stock filling orders**
For stock filling orders, the stock is first booked with the booking of a registration point that corresponds to a stock slot. In the rack stock, there is no incoming stock booking via completion report. The rack number used in A+W Production is taken over in the stock as external rack number. If this rack number is not yet known in the stock, a new internal rack number is determined for this via a number range. The registration point is used again as slot. After such a stock booking, currently no additional Barcoding bookings are possible. If nevertheless such a booking should be made, then an error e-mail will be sent to a configured user. This booking must then be made manually in the incoming/outgoing rack stock.

**Booking of the dispatch rack system for produced customer orders**
If customer orders are packed on racks in A+W Production and reported out of the house, a message for the appropriate rack is send to dispatch. Here, in turn, the dispatch rack system is booked (tables gest and gestzu). If the order should still be on a route, the route assignment of the rack is done at the same time. If this is not the case, then this rack assignment must be made manually in dispatch.

**Emptying the rack in the dispatch module**
If a rack that was previously reported outside the plant is booked back to "3 beginning," then the associated message to A+W Enterprise causes the emptying of the rack and the backing up of the associated rack data to the table gestzuprot.

**Incoming stock for stock filling orders**
The switch `WLDISPO_VARIABEL` may not be set, otherwise the fixed IGs in stock orders are booked to stock as variable variant.
#438795/02.2018: This restriction has been removed.

In ERP-WS, the booking is not initiated if:
- A registration point type defined IS `AWC_RACKSTOCK_REGPOINT_TYPE` and this variables the registration point type via which the slots can be grouped in AWP includes.
- In the AWP registration point an ERP tool is entered that correspond to the registration point number. Important: after creating new slots, these must be transferred via the A+W Enterprise Export Service into the ERP system. (insert into exportinfo (interface) values ("ERFSTELLENALCIM")) Here the table `awc_alciberfstellen` is filled.
- In the AWE table `awc_alcimerfstellen` for this registration point the type stored in `AWC_RACKSTOCK_REGPOINT_TYPE` was found.

When booking the rack-related incoming goods, first the structure `waeingestkopf` and `waeingestpos` are filled and after that the stock booker commissions the booking of the rack-related incoming goods analogously (b_status=133). The transferred rack number is used as lieferid (exgnr) and it is written negated by gestellnr. The stock booker thus recognizes that a new internal rack number must be assigned. Here there is a check whether the external rack number is already present in `waeingestkopf.lieferid` or in `waeingestkopfok.lieferid`. If this is currently, the stock booking is declined and a mail with the Meldid 52 is sent to the recipient from the variables `AWC_RACKSTOCK_MAIL_MANR`.

**Booking of gest and gestzu with order-related outgoing stock**
If there is a booking with order reference in the outgoing stock and the booking is about a header part that is removed from the stock, then gest and gestzu are booked. If the rack fits the route, it is then assigned to the route. This assumes that there are sufficient unpackaged quantities on the corresponding route.

Since the stock booker always generates a completion report when booking and if the variable `LA_LAPOOL` is set, a packaged report is also generated. This variable may not be activated.

**Rack-related incoming goods**
In rack-related incoming goods, the environment variable `WE_GEST_IDREQUIRED` controls whether the field "LieferID" or the rack number must be filled out.

- **Variable active:** LieferID must always be filled. In this case the rack number is assigned automatically if it is left empty.
- **Variable not active:** rack number must always be filled.

#### 58.3.3. Multi-site extension

**Adjustments in inward goods booking**
(#344831) Previously the rack-related inward goods (Purchasing – Receipt of goods – Rack-related receipt of goods) could not be started in a multi-site environment. This restriction was removed.

Prerequisite for the use of "Rack-related inward goods" in the multi-site environment is the presence of registration points for the company "0" or for the special company for which you are logged in (see "Determination/updating of the AWP registration points"). Registration points with the company number "0" are valid in the multi-site environment all companies.

For entry of the "Rack-related inward goods," the currently-valid company number is used. This is indicated in the title of the dialog. If there are still-unbooked inward goods present, the inward goods assigned to the current company are displayed on the dialog. If there are no unbooked inward goods present for the current company, the dialog remains empty.
