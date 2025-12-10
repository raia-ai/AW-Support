---
title: "EN-UM-AW_Enterprise-Sales_4_7"
source: "EN-UM-AW_Enterprise-Sales_4_7.pdf"
tags: ["A+W Enterprise Sales", "Software Reference", "Pricing", "Order Entry", "Conditions", "Delivery Notes", "Invoicing", "Cost Calculation", "Release Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the A+W Enterprise Sales module, detailing functionalities related to prices, conditions, order management, delivery, and invoicing. It provides descriptions of user interface dialogs, fields, and processes."
long_description: "This is a detailed software reference manual for the A+W Enterprise Sales application, version 4.00/03-2020. The guide covers a wide range of functionalities within the sales process, starting with the configuration of 'Prices and Conditions'. It explains how to manage various pricing methods, including those for basic glass, processing, manual prices, and specific items like LAMI articles and glass doors. It delves into the technical details of each field, providing database field names and data types. The manual also covers 'Production Cost Calculation', outlining how material, machine, and personnel costs are determined and displayed. A significant section is dedicated to 'Order Release', explaining the process of authorizing and releasing blocked orders for further processing. The 'Delivery' section details the creation of delivery plans, management of partial deliveries, and the generation of both automatic and manual delivery notes. Finally, the 'Invoices' section describes the procedures for creating, booking, and managing various types of invoices, including automatic, manual, partial, and final invoices, as well as cash transactions. The document is intended for users and administrators of the A+W Enterprise Sales software, providing the necessary information to configure and operate the sales and invoicing modules effectively."
---

# Prices and Conditions

If additional processing are included in the item's BOM, then the Processing Prices (SA), (PU) tabs are enabled:
⇨ "Item Conditions - Processing Prices (Sls), (Purch), Detail View" on page D-309

---
### Header

**SA PCD** Price code for the pre-defined price list for sales.
*Technical info: mandatory field, numeric field, DB field: pokokon.pkz*

**PU PCD** Price code for the pre-defined price list for purchasing.
*Technical info: mandatory field, numeric field, DB field: pokokon.ekpkz*

**Vector** Number of the vector from which the price should be drawn.
*Technical info: mandatory field, numeric field, DB field: pokokon.matnr*

### Conditions tab

Most fields are described for the Conditions for PCD BASIC GLASS, PCD Processing dialog:
⇨ "Conditions for PCD, PCD BASIC GLASS Processing" on page D-284

In addition, the following fields are displayed:

**Basic price** Basic price of the article. The price type determines to what the price refers:
- **CU/piece:** The price applies per piece.
- **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
*Technical info: toggle field, DB field: pokokon.flag2*

**Minim. Calculat.** Minimum number of quantity units for which the price is calculated. If the quantity in the order item is smaller than the minimum quantity, the price for this minimum quantity is charged.
*Technical info: numeric field, DB field: pokokon.zu6, pokokon.zuk6*

### Footer

This area displays the description of the article and the code for the article's product group.

## Conditions for PCD GLASS DOORS

**Sales > Order Entry > Items tab > Price field of item article with price method PCD glass doors > <Shift> + <F9>**

This dialog displays the price conditions for an item article to which the price method PCD Glass Doors is assigned. You can edit the price conditions.

The Sales and Purchasing areas display mainly the same fields. In the Sales area, you specify the sales prices; in the Purchasing area the purchasing prices.

### Header

**SA PCD** Price code for the pre-defined price list for sales.
*Technical info: mandatory field, numeric field, DB field: pokokon.pkz*

**PU PCD** Price code for the pre-defined price list for purchasing.
*Technical info: mandatory field, numeric field, DB field: pokokon.ekpkz*

### (Area without description)

**Lite 1, 2, ... 7** Area of the lites in the glass door system. In the adjacent fields in the Sales and Purchasing areas, the square meter price for the lite in question is displayed.
*Technical info: numeric fields, DB fields: pokokon.zu5, pokokon.zu7, pokokon.zu9, pokokon.zu11, pokokon.zu13, pokokon.zu15, pokokon.zu17*

### Sales and purchasing

**Scal. Level** Price level from which the price is used. The field is only evaluated by the price calculation if the price type 2 - Scaling Level is specified for the relevant article price vector.
*Technical info: numeric fields, DB fields: pokokon.flag1, pokokon.ekflag1*

**SC** Surcharge in percent. The surcharge is charged on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is charged.
*Technical info: numeric fields, DB fields: pokokon.zu3, pokokon.zuk3*

**Factor** Factor of the surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
*Technical info: numeric fields, DB fields: pokokon.zu4, pokokon.zuk4*

**Lite €/sqm** Price per square meter for the lite in question.
- **Sales:** Price per square meter for the adjacent lite.
  *Technical info: numeric fields, DB fields: pokokon.zu6, pokokon.zu8, pokokon.zu10, pokokon.zu12, pokokon.zu14, pokokon.zu16, pokokon.zu18*
- **Purchasing:** Purchase price per square meter for the adjacent lite.
  *Technical info: numeric fields, DB fields: pokokon.zuk6, pokokon.zuk8, pokokon.zuk10, pokokon.zuk12, pokokon.zuk14, pokokon.zuk16, pokokon.zuk18*

**Surcharge** Surcharge that is charged on the price. You specify the surcharge type in the second field. The surcharge type specifies to what the surcharge refers:
- **CU/unit:** The surcharge is charged as fixed amount on the unit price of the item.
- **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
- **Percentage:** The surcharge is calculated as a percentage of the basic glass price.
This field is only displayed in the Sales area.
*Technical info: numeric field, toggle field, DB fields: plkokon.zu19*

**SA Edge Processings/SC** Surcharge for edge processings on the sales price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
*Technical info: numeric field, DB field: pokokon.zu20*

**SA Edge Processings/Factor** Factor for edge processings on the sales price in percent. Generally a discount is granted with a factor.
*Technical info: numeric field, DB field: pokokon.zuk20*

**SA Corner Processings/SC** Surcharge for corner processings on the sales price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
*Technische Info: nnumeric field, DB field: pokokon.zu21*

**SA Corner Processings/Factor** Factor for corner processings on the sales price in percent. Generally a discount is granted with a factor.
*Technical info: numeric field, DB field: pokokon.zuk21*

**SA Surface Processings/SC** Surcharge for surface processings on the sales price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
*Technical info: numeric field, DB field: pokokon.zu22*

**SA Surface Processings/Factor** Factor for surface processings on the sales price in percent. Generally a discount is granted with a factor.
*Technical info: numeric field, DB field: pokokon.zuk22*

**PU All Processings/SC** Surcharge for all processings on the purchasing price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
*Technical info: numeric field, DB field: pokokon.zu23*

**PU All Processings/Factor** Factor for all processings on the purchasing price in percent. Generally a discount is granted with a factor.
*Technical info: numeric field, DB field: pokokon.zuk23*

**Accessory/SC** Surcharge for accessory articles on the purchasing and/or sales price in percent. If you enter the value 0 or a value <0, no surcharge is charged.
*Technical info: numeric fields, DB fields: pokokon.zu24, pokokon.zuk24*

**Accessory/Factor** Factor for accessory articles on the purchasing and/or sales price in percent. Generally a discount is granted with a factor.
*Technical info: numeric fields, DB fields: pokokon.zu25, pokokon.zuk25*

### Footer

This area displays the description of the article and the code for the article's product group.

## Conditions for Manual Prices

**Sales > Order Entry > Items tab > Price field of item article with price method Manual Prices > <Shift> + <F9>**

This dialog displays the price conditions for an item article to which the price method Manual Prices is assigned in the master data. You can edit the price conditions.

> **Automatic price method change**
> You can also specify a price manually for item articles with a different price method. The price method for this item article is then changed automatically to manual prices.

**Price Type** Specification of to what the price refers.
- **CU/piece:** The price applies per piece.
- **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
*Technical info: toggle field, DB field: pokokon.flag2*

You enter the following values for sales and purchasing prices separately.

**Price** Basic price of a glass lite. The price type is drawn from the previous field.
*Technical info: numeric fields, DB fields: pokokonzu1, pokokon.zuk1*

**SC** Surcharge in percent. The surcharge is charged on the quantity unit price.
*Technical info: numeric fields, DB fields: pokokonzu2, pokokon.zuk2*

**Factor** Factor of the surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
*Technical info: numeric fields, DB fields: pokokonzu3, pokokon.zuk3*

**Round Size** Specification of the dimension rounding in millimeters for price calculation of the article. The edge lengths in the order item will be rounded to the next higher value in millimeters that is divisible by the specified dimension rounding for the price calculation. This information is not considered in production.
*Technical info: numeric fields, DB fields: pokokonzu5, pokokon.zuk5*

**Minim. Calculat.** If the value in the order item is smaller than the minimum calculation quantity, the price for this value is charged. For an article that is specified as area, the minimum area in square meters is specified as minimum calculation value.
*Technical info: numeric fields, DB fields: pokokon.zu5, pokokon.zuk5*

## LAMI Exchange/Additional Prices

**Sales > Order Entry > Items tab > Price field of LAMI article > <Shift> + <F9> > <Shift> + <F10>**

This dialog displays the conditions for the exchange and additional prices for the individual lites in a LAMI article. You can edit the price conditions.

The values for sales, purchasing, and the detail view of the exchange and additional prices are each displayed in their own view.
- Use `<F2>` to change between the views for sales, purchasing, and the detail view.

The dialog is only enabled if LAMI articles are included in the selected item.

### Sales and purchasing

- **Article:** Article number.
  *Technical info: display field, numeric field, DB field: pokoaust.artnr*
- **Exchange/Additional List, Description:** Number of the exchange list. If a number is specified, the description is displayed in plain text.
  *Technical info: numeric field, display field, DB fields: pokoaust.vkatlnr, pokoaust.ekatinr, xatl.bez*
- **Min.calc.:** Minimum calculation. Specification of the minimum area in square meters for which the price is calculated. If the area of the exchange glass in the order item is smaller than the minimum calculation area, the price for this minimum calculation area is used.
  *Technical info: numeric field, display field, DB fields: pokoaust.vkminber, pokoaust.ekminber*
- **Factor:** Factor of the surcharge in percent.
  *Technical info: numeric field, display field, DB fields: pokoaust.vkfaktor, pokoaust.ekfaktor*
- **SA price, PU price:** Sales or purchasing price of the exchange glass.
  *Technical info: numeric field, DB field: pokoaust.vkmepreis, pokoaust.ekmepreis*
- **Type:** Specification of to what the price refers.
  - **CU/m2:** The price applies per square meter.
  - **Percentage:** The surcharge is calculated as a percentage of the basic glass price.
  *Technical info: toggle field, DB field: pokoaust.vkpreistyp, pokoaust.ekpreistyp*

### Detailed view

The fields in the detail view correspond to columns in sales and purchasing. In addition, the fields for the size surcharges for sales and purchasing are displayed. The surcharge type specifies to what the surcharge refers:
- **CU Value:** The surcharge or discount is calculated as fixed amount on the sales/purchasing price.
- **Percent:** The surcharge is calculated as a percentage of the sales/purchasing price.

**Small Glass Surcharge** Price surcharge for small glass if the area of the glass is smaller than the specified limit value. You select the surcharge type in the second field.
*Technical info: numeric field, toggle field, DB fields: pokoaust.vkklzuschlag, pokoaust.vkklzutyp, pokoaust.ekklzuschlag, pokoaust.ekklzutyp*

**Overlength Surcharge** Price surcharge for overlengths if an edge length is longer than the specified limit value. You select the surcharge type in the second field.
*Technical info: numeric field, toggle field, DB fields: pokoaust.vkuebzuschlag, pokoaust.vkuebzutyp, pokoaust.ekuebzuschlag, pokoaust.ekuebzutyp*

**Oversize Surcharge** Surcharge for oversizes if both glass edges exceed a specified length. In the second field, you select the surcharge type.
*Technical info: numeric field, toggle field, DB fields: pokoaust.vkuebzuschlag, pokoaust.vkuebgrzutyp, pokoaust.ekuebgrzuschlag, pokoaust.ekuebgrzutyp*

## Item Conditions – Processing Prices (Sls), (Purch), Detail View

**Sales > Order Entry > Items tab > Select price field of item article including additional processing steps > <Shift> + <F9>**

These tabs display the price conditions for a price-relevant processing depending on whether it is included in the item BOM. You can edit the price conditions.

The processing prices are divided into Sales and Purchasing. Furthermore, there is a detail view that is the same for both tabs. The detail view displays more values of the processing prices for the individual processing.

- Switch to the Detail view using `<F5>`.

The tabs are only enabled if additional processings are entered in the selected item. The Processing Prices (Sls) tab is only enabled if the type PO or Included is selected for the item.

### Processing Prices (SIS) tab

- **Article:** Description of the processing.
  *Technical info: display field, DB field: aufstrukt.artnr*
- **Wd., Hgh:** Number of processed widths and heights of the lite.
  *Technical info: numeric fields, DB fields: poszu.panz1, poszu.panz2*
- **Price Type:** Specification of to what the price refers.
  - **CU/piece:** The price applies per piece.
  - **CU/TQU:** The price is calculated per basic quantity unit, e.g. per square meter.
  - **Percent:** The price is calculated as a percentage from the base price of the head article.
  - **CU/m2:** The price applies per square meter.
  - **CU/linm:** The price applies per linear meter.
  *Technical info: toggle field, DB field: poszu.part*
- **Qty:** Quantity of the processing per basic quantity unit.
  *Technical info: numeric field, DB field: poszu.pme*
- **Factor:** Sales price factor of the processing price surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
  *Technical info: numeric field, DB field: poszu.vkfaktor*
- **SC:** Sales price surcharge for the processing in percent. The surcharge is charged on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is charged.
  *Technical info: numeric field, DB field: poszu.vktz*
- **ShpSrch:** Shape surcharge in percent.
  *Technical info: numeric field, DB field: poszu.vkmodzusch*
- **SalesPrc:** Sales price of the processing.
  *Technical info: numeric field, DB field: poszu.ppme*
- **Grp:** Number of the grouping. The processings can be grouped under a number.
  *Technical info: numeric field, DB field: poszu.masflag*

### Processing Prices (Purch) tab

Most of the columns are described for the Purchasing Prices (Sls) tab.
⇨ "Processing Prices (SIS) tab" on page D-310

In addition, the following columns are displayed:
- **PU Factor:** Purchasing price factor of the processing price surcharge in percent. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
  *Technical info: numeric field, DB field: poszu.ekfaktor*
- **PuSC:** Purchase price surcharge for the processing in percent. The surcharge is charged on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is charged.
  *Technical info: numeric field, DB field: poszu.ektz*
- **PuShSur:** Purchase price shape surcharge in percent.
  *Technical info: numeric field, DB field: poszu.ekmodzusch*
- **PU Price:** Purchasing price of the processing.
  *Technical info: numeric field, DB field: poszu.ppmeek*

### Processing Prices Detail View

Most of the fields in the detail view are described for the Purchasing Prices (Sls) tab.
⇨ "Processing Prices (SIS) tab" on page D-310

In addition, the following fields are displayed:

**Round Size** Dimension rounding per processing in quantity unit.
*Technical info: display field, DB field: poszu.massrund*

**Minim. Calculat.** Specification of the minimum calculated quantity unit of the processing.
*Technical info: display field, DB field: poszu.minber, poszu.minberek*

**Basic Price** Basic price of a price-relevant processing for sales and purchasing. The basic price for sales corresponds to the value in the SA Price field on the Processing Prices (Sls) tab, the basic price for purchasing to the value in the PU Price field on the Processing Prices (Purch) tab.
*Technical info: numeric fields, DB fields: poszu.ppme, poszu.ppmeek*

**Min. Price** Minimum price for the processing.
*Technical info: numeric field, DB field: poszu.minpreis*

### Footer

This area displays the description of the article and the code for the article's product group.

## Item Conditions – Muntin Prices

**Sales > Order Entry > Items tab > Price field of item article including muntins > <Shift> + <F9>**

This tab displays the price conditions for muntin prices of an item article. You can edit the price conditions.

The tab is only enabled if muntins are entered in the selected item. The values for sales and purchasing prices are displayed in two individual areas.

### Sales and Purchasing

**Muntin PCD** Muntin price code from the pre-defined price list for muntin calculation.
*Technical info: numeric field, DB field: pokospro.vkpkz, pokospro.ekpkz*

**Muntins Calcul. Type** Calculation type of the muntins. The muntin calculation types are described in detail elsewhere:
⇨ "Order Muntin Prices" on page D-273
*Technical info: numeric field, DB field: pokospro.vkberart, pokospro.ekberart*

**Muntins Factor** Factor for the muntin surcharge in percent. Using the factor, you can change the price calculation for the item without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
*Technical info: numeric field, DB field: pokospro.vkfaktor, pokospro.ekfaktor*

**Muntins SC** Muntin surcharge in percent. The surcharge is charged on the quantity unit price. If you enter the value 0 or a value <0, no surcharge is charged.
*Technical info: numeric field, DB field: pokospro.vktz, pokospro.ektz*

**Price per Field** Muntin price by number of fields if there are crossing points in the muntin pattern. If, for example, two vertical and two horizontal muntins divide the window into nine fields, the price is calculated nine times. The price is evaluated for the calculation types Fields, Field+LM, Field+E+C and Special.
*Technical info: numeric field, DB field: pokospro.vkfeld, pokospro.ekfeld*

**Price per Field 2** Muntin price by number of fields if there are no crossing points in the muntin pattern. If, for example, four vertical and no horizontal muntins divide the window into five fields, the price is calculated five times. The price is evaluated for the calculation types Fields, Field+LM, Field+E+C and Special.
*Technical info: numeric field, DB field: pokospro.vk2feld, pokospro.ek2feld*

**Price per Inch** Price per inch for the muntin. The price is evaluated for the calculation types LM, LM+C+E, LM+C, LM+E, field+LM, and Special.
*Technical info: numeric field, DB field: pokospro.vklaufm, pokospro.eklaufm*

**Price per Edge** Price per edge connection. The price is evaluated for the calculation types E, LM+C+E, LM+E, C+E, field+C+E, and Special.
*Technical info: numeric field, DB field: pokospro.vkrand, pokospro.ekrand*

**Price per Cross** Price per crossing point. The price is evaluated for the calculation types C, C+E, LM+C, LM+C+E, C or LM, field+C+R, and Special.
*Technical info: numeric field, DB field: pokospro.vkkreuz, pokospro.ekkreuz*

**Percent** Price as percentage on the price of the head article. The price is evaluated for the calculation type Percent.
*Technical info: numeric field, DB field: pokospro.vkprozent, pokospro.ekprozent*

**Price/Sqft** Price per square foot. The price is evaluated with the calculation type sqm price.
*Technical info: numeric field, DB field: pokospro.vkqmpreis, pokospro.ekqmpreis*

**Price/Pc.** Price per muntin pattern. The price is evaluated for the calculation type Piece.
*Technical info: numeric field, DB field: pokospro.vkstueckprs, pokospro.ekstueckprs*

**Min. Lin. Meter** Minimum length of the muntins in meters, which will be calculated for the price. If the muntin measures fewer linear meters than the minimum linear meters, then the price for the minimum linear meters will be calculated. The price is evaluated with the calculation type LM.
*Technical info: numeric field, DB field: pokospro.vkminlm, pokospro.ekminlm*

**Min. No. of Fields** Minimum number of muntin fields for which the price will be calculated. The price is evaluated with the calculation type Fields.
*Technical info: numeric field, DB field: pokospro.vkminfeld, pokospro.ekminfeld*

**Muntins Factor 2** Factor for the muntin surcharge in percent for the second muntin. Using the factor, you can change the price calculation for the article without having to adjust all prices, e.g. for price increases or discounts. Generally a discount is granted with a factor.
*Technical info: numeric field, DB field: pokospro.vkfaktor2, pokospro.ekfaktor2*

**Price per Field (2nd muntin)** Muntin price by number of fields for the second muntin if there are crossing points in the muntin pattern. The price is evaluated for the calculation types Fields, Field+LM, Field+E+C and Special.
*Technical info: numeric field, DB field: pokospro.vkfeld2, pokospro.ekfeld2*

**Price per Field 2 (2nd muntin)** Muntin price by number of fields for the second muntin if there are no crossing points in the muntin pattern. The price is evaluated for the calculation types Fields, Field+LM, Field+E+C and Special.
*Technical info: numeric field, DB field: pokospro.vk2feld2, pokospro.ek2feld2*

**Price per Inch (2nd muntin)** Price per inch for the second muntin. The price is evaluated for the calculation types LM, LM+C+E, LM+C, LM+E, field+LM, and Special.
*Technical info: numeric field, DB field: pokospro.vklaufm2, pokospro.eklaufm2*

**Price per Edge (2nd muntin)** Price per edge connection for the second muntin. The price is evaluated for the calculation types E, LM+C+E, LM+E, C+E, field+C+E, and Special.
*Technical info: numeric field, DB field: pokospro.vkrand2, pokospro.ekrand2*

**Min. Lin. Meter (2nd muntin)** Minimum length of the second muntin in meters, which will be calculated for the price. If the muntin measures fewer linear meters than the minimum linear meters, then the price for the minimum linear meters will be calculated. The price is evaluated with the calculation type LM.
*Technical info: numeric field, DB field: pokospro.vkminlm2, pokospro.ekminlm2*

### Footer

This area displays the description of the article and the code for the article's product group.

## Production Cost Calculation

**Sales > Order Entry > Items tab > Price field > <Ctrl> + <F10>**

This dialog displays the results of the cost calculation. You can edit some of the values.
In the document entry, first only the material costs are displayed. The machine and personnel costs are only displayed if the document has been scheduled in a production system.

This dialog offers the following tabs:
- "Production Cost Calculation – Overview" on page D-316
- "Production Cost Calculation - Details" on page D-318

### Production Cost Calculation – Overview

**Sales > Order Entry > Items tab > Price field > <Ctrl> + <F10> > Overview**

This tab displays the production costs for the selected item. You can edit the calculated quantity and unit price of the items.

If for a processing article machines or personnel costs are calculated, then the corresponding article number and description for the item article are displayed via the table in the tab heading.

Use `<F2>` to change to the detail view where you can edit additional data.

> **Calculation only after transfer to production**
> Depending on the system configuration, the production costs are only displayed if you have already transferred an order to production. If you have not yet transferred the order to production, only the material costs are displayed.

#### Overview

- **Cost type:** Display of the type of the production costs.
  - Material costs
  - Internal contribution margin
  - Assembly costs
  - Machinery costs
  - Personnel costs
  - Fixed Costs
  - Purchased
  *Technical info: display field, DB field: poskost.satztyp*
- **Article:** Display of the article number.
  *Technical info: display field, DB field: poskost.artnr*
- **Cost center:** Cost center name for statistical evaluations.
  *Technical info: alphanumeric field, DB field: poskost.kostenst*
- **Phys. Qty:** Display of the physical item quantity (actual quantity), e.g. glass area.
  *Technical info: display field, DB field: poskost.phymenge*
- **Calcul. Qty:** Display of the calculated item quantity, e.g. glass area + waste.
  *Technical info: display field, DB field: poskost.pme*
- **Price/QU:** Display of the price per quantity unit of the item.
  *Technical info: display field, DB field: poskost.ppme*
- **Price/pc.:** Price per piece of the item.
  *Technical info: numerical field, DB field: poskost.stprs*

#### Footer

Sums from the corresponding rate types. The following abbreviations are shown:
- **Mat.:** Material costs.
- **IntDB:** Internal contribution margin.
- **Assy.:** Assembly costs.
- **Mach.:** Machine costs.
- **Pers.:** Personnel costs.

### Production Cost Calculation – Details

**Sales > Order Entry > Items tab > Price field > <Ctrl> + <F10> > Details tab**

This tab displays the detail data for the production costs determined. You can edit the selected item and thus recalculate the production costs.

Use `<Page Up>` and `<Page Down>` to navigate between the individual costs of the current item.

If for a processing article machines or personnel costs are calculated, then the corresponding article number and description for the item article are displayed via the table in the tab heading.

#### Details

Depending on the cost type, different fields are displayed:

**Production Item** Production item number for production costs. For ordered processings, the corresponding item number for the order is displayed in which the subparts are ordered.
*Technical info: display field, DB field: poskost.plfdpos*

**Cost Type** Display of the type of the production costs.
*Technical info: display field, DB field: poskost.satztyp*

**Manual Modification** Specification whether the values were overwritten. If the production costs are changed, Manual will be displayed in the field. You cannot edit the content in the field.
*Technical info: display field, DB field: poskost.manuell*

**Type** Display of the type of the selected article. The value can only be edited for the record types Machine Costs and Personnel Costs.
- **None:** No type, e.g. for services.
- **P.O.:** Article has to be ordered from the supplier.
- **Stock:** Article will be taken from stock.
- **Production:** Article will be produced.
- **Acc.:** Article is delivered by the customer, e.g. for further processing.
- **not avail:** The article is not available.
*Technical info: toggle field, DB field: poskost.beschaffart*

**Quantity** Article quantity in the BOM of the item. For the production costs, the quantity is always 1. For machine costs, generally no quantity is displayed.
*Technical info: display field, DB field: poskost.menge*

**Article** Number of the article for which the costs are determined.
*Technical info: display field, DB field: postkost.artnr*

**Header Prod.** Article to which the selected article is attached as subpart. If the article is itself the header article, the field remains empty.
*Technical info: display field, DB field: poskost.refartnr*

**Machine no.** Number of the machine that is used for the calculation. This field is only displayed for the record type Machine Costs.
*Tecnical info: numeric field, DB field: poskost.bmnr*

**Production sub no.** Personnel number. You cannot edit the value. This field is only displayed for the record type Machine Costs.
*Technical info: numeric field, DB field: poskost.psbmnr*

**Process Class** Number of the process class for the production planning. Several work processes can be summarized in a process class. This field is only displayed for the record types Machine Costs and Personnel Costs.
*Technical info: numeric field, DB field: poskost.agknr*

**Work Process** Number of the work process for the production planning. This field is only displayed for the record types Machine Costs and Personnel Costs.
*Technical info: numeric field, DB field: poskost.agnr*

**Staff ID** Personnel class number. You cannot edit the value. This field is only displayed for record types Personnel Costs.
*Technical info: numeric field, DB field: poskost.pknr*

**Cost Center** Cost center name for statistical evaluations.
*Technical info: alphanumeric field, DB field: poskost.kostenst*

**Basic Unit of Qty** Basic quantity unit that was assigned to the article in the master data, e.g. square meter, piece. The value is used for calculation of the piece price for the record types Machine Costs and Personnel Costs. You cannot edit the value. This field is only displayed for the record types Machine Costs and Personnel Costs.
*Technical info: numeric field, DB field: poskost.lugme*

**Variant** Display of the variant number of the article.
*Technical info: numeric field, DB field: poskost.variante*

**Qty (Physical)** Physical quantity of the item (actual quantity), e.g. glass area, duration of work. The physical quantity is used as calculation basis for the calculational quantity and unit price. The field corresponds to the Phy. Qty column on the Overview tab.
*Technical info: numeric field, DB field: poskost.phymenge*

**Loss** Percentage loss of the item, e.g. material loss, time loss. The percentage of the loss is calculated on the calculated quantity. If you specify a negative loss, the calculated loss gets smaller.
*Technical info: numeric field, DB field: poskost.verlust*

**Quantity (Calculation)** Calculated quantity of the item, e.g. glass area + waste. The calculated quantity is calculated from the physical quantity including loss.
Physical quantity + loss/100xphysical quantity The field corresponds to the Calc. Qty column on the Overview tab.
*Technical info: numeric field, DB field: poskost.pme*

**Price/QU** Price per basic quantity unit of the item. The quantity unit price is used for calculation of the unit price. The field corresponds to the Qty Price column on the Overview tab.
*Technical info: numeric field, DB field: poskost.ppme*

**Price/Pc.** Price per unit of item. The unit price is calculated from the quantity unit price and the calculated quantities: Quantity unit price x calculated quantity. For the record types Machine Costs and Personnel Costs, the basic quantity unit is also used for calculation of the unit price.
Quantity unit price x calculated quantity / basic quantity unit
*Technical info: numeric field, DB field: poskost.stkprs*

**Date** Entry date of the item.
*Technical info: date field, DB field: poskost.datum*

**Price per quantity unit / Complet. report** Price per quantity unit with completion report.
*Technical info: numeric field, DB field: poskost.fppme*

**Price/Pc. / Completion report** Item price with completion report in own currency.
*Technical info: numeric field, DB field: poskost.fstprs*

**(Price/Pc.) in foreign currency** Price/Pc. in foreign currency.
*Technical info: numeric field, DB field: poskost.stkprsfw*

**(Price/Pc./Complet. Report in foreign currency)** Price/Pc. with completion report in foreign currency.
*Technical info: numeric field, DB field: poskost.fstprsfw*

#### Footer

The footer is described for the Overview tab:
⇨ "Footer" on page D-317

## Price Calculation

**Sales > Pricing**

Use this dialog to calculate the sales prices based on the defined conditions. The calculated price is only for your information and will not be saved.

The control elements are described for the Order Entry dialog:
⇨ "Order Entry" on page D-84

# Release

Depending on the system configuration, orders are not released during entry, e.g. if the operator does not have sufficient rights, the contribution margin is underrun or the company limit is exceeded. These orders have to be released manually for further processing in order to transfer them later to the system; that is, to production, purchasing, dispatch, and the warehouse.

The following dialogs are described in this section:
- "Order Release" on page D-323
- "Authorization" on page D-326

## Order Release

**Sales > Order Release > Release**

On these dialogs, you search for and release an order for further processing. You can only release an order if you have the appropriate rights. Depending on the reason for the order block, different rights are required for the order release.

On the **Order Release** search dialog, you can filter the search for release:
- **Enter search criteria > [Start]:**
  You can select department or operator and/or reason in the specified company. All orders are displayed that fulfill the criteria. If you don't enter any criteria, all orders not yet released are displayed in the hit list.
- **[Individual] > Enter reason > Specify company, operator > [OK]:**
  First you have to enter a reason and then you can select the company and/or the operator on the Release dialog.

On the order release dialog, all orders are displayed that fulfill the search criteria.
- Use `<Shift>+<F5>` to open the marked order in the order entry.
- Use `<Ctrl>+<F9>` to release all orders.
- Use `<Shift>+<F9>` to release all orders starting with the marked order.
- Use `<Shift>+<F12>` to open the Blockage reasons for unsuccessful release dialog. This dialog displays the reasons for the block of the order. The dialog is only displayed if an order is blocked for more than one reason.
- Use `<F3>` to release the selected orders.

### Header

This area displays the search criteria that you have specified. You cannot edit the search criteria after the fact. For a new search, you have to close the dialog and open it again.

### Overview

This area displays the orders that fulfill the search criteria and can be released. You can only edit the values in the **Free** and **LL** columns. The other columns are only for your information.

- **Order:** Number of the order that is not yet released.
  *Technical info: display field, DB field: kauf.auftrnr*
- **Free:** Information about releasing the order. If the field is grayed out, then the release is not possible for data-technical reasons or you do not have the appropriate rights for the release.
  - **NO:** order will not yet be released.
  - **YES:** order will now be released.
  - **NEVER:** order will never be released.
  - **SC:** transfer order to shipping control only.
  *Technical info: toggle field, DB field: kauf.tekap.kz*
- **Customer, Name:** Number and name of the customer in this order.
  *Technical info: display fields, DB fields: kauf.kunr, mp.name*
- **Req.On:** Planned delivery date.
  *Technical info: display field, DB field: kauf.Itideal*
- **Call:** The order will only be shipped on the customer's request.
  - **Y:** The order will only be shipped on the customer's request.
  - **N:** The order will be delivered by default.
  *Technical info: display field, DB field: kauf.abrufkz*
- **User, DptNo:** Number and department number of the order operator.
  *Technical info: display fields, DB fields: kauf.eusr, kauf.abtnr*
- **Entered:** Date on which the order was entered.
  *Technical info: display field, DB field: kauf.edat*
- **Site:** Site number that is assigned to the order.
  *Technical info: display field, DB field: kauf.hausnr*
- **LL:** Limit lock. Specification whether the order is locked. You can only release orders if you have the appropriate rights. You require special rights if you want to release orders that have exceeded the company limit or the general credit insurance limit.
  - **Y:** The limit lock is active. The **Free** field is locked and the value set automatically to **NO**.
  - **N:** The limit lock is disabled. The order can be released.
  *Technical info: toggle field, DB field: kauf.limsperre*
- **Remark:** Additional information on the order.
  *Technical info: display field, DB field: kauf.luspermodus*
- **Info:** Indication whether order information is stored. If an I appears in the column, information is stored for the order. Use `<F5>` to open the Remark dialog with the stored information.
  *Technical info: display field*

## Authorization

**Sales > Order Release > Authorization**

On this dialog, you can authorize an employee to release an order, even if this order exceeds the credit limit. You specify the maximum amount of the overage by specifying the new value accordingly or entering a value in the **Maximum Increase in Value** field.

The functions depend on the settings in the master data and the respective system configuration. For customer-specific adjustments, contact your contact person at A+W Software GmbH.

**Document** Number and type of the document. If you have specified a number, the document type is displayed in plain text.
*Technical info: mandatory field, numeric field, DB field: kauffrei.auftrnr*

**Serial Amendment No.** Number of the amendment process. The current amendment number is entered automatically. You can specify a smaller amendment number to view the corresponding amendment state.
*Technical info: numeric field, DB field: kauffrei.aendernr*

> **Increase the amendment number**
> You can only edit the last amendment state without increasing the amendment number. If you call up an amendment state that is farther back and edit it, the amendments are stored under a new amendment number.

**Customer** Customer name from the document. If you have specified the document number, the customer is displayed in plain text.
*Technical info: display field, DB field: kauf.kunr*

**Authorized Employee** Number and name of the employee for whom the authorization is created. If you have specified a number, the name of the employee is displayed in plain text.
*Technical info: numeric field, DB field: kauffrei.aendmanr*

**Old Value** Old net total value of the document. As value, the current net total value of the document is used.
*Technical info: numeric field*

**New Value** Upper limit for the new net total value of the document. The value has to be higher than the old net total value. The value depends on the **Maximum Increase in Value** field:
- If the **Maximum Increase in Value** field is empty and you specify a new net total value, the difference between the old and new net total value is displayed automatically in the **Maximum Increase in Value** field.
- If there is already a value in the **Maximum Increase in Value** field and you specify a new net total value, the value in the **Maximum Increase in Value** field is adjusted automatically to the new value.
*Technical info: numeric field*

**Maximum Increase in Value** Maximum increase of costs that exceed the old net total value of the order. The value depends on the **New Value** field:
- If the **New Value** field is empty and you specify a new maximum value, the difference between the old and new net total value is displayed automatically in the **New Value** field.
- If there is already a value in the **New Value** field and you specify a new maximum value, the value in the **New Value** field is adjusted automatically to the new value.
*Technical info: numeric field, DB field: kauffrei.maxpreisdiff*

### Footer

**Employee** Display of the name of the authorizing employee.
*Technical info: display field, DB field: kauffrei.automanr*

**Date** Display of the date on which the authorization was released. By default, the current date is displayed.
*Technical info: display field*

# Delivery

By default, delivery notes are entered and managed in the **Shipping Control** module because the bookings of packed and finished products from other modules and programs are forwarded automatically to the dispatch control. If the Shipping Control module is not configured, you can create delivery notes in the **Sales** module.

Depending on the configuration, you can create a delivery plan for an order. In the delivery plan, you can break up the order into partial deliveries. A delivery note is created for each (partial) delivery of an order. The delivery note serves as proof of the order processing for logistics and transportation and for the customer's information. Depending on the type of deliveries, the system distinguishes between complete and partial delivery notes. You can create and edit delivery notes automatically or manually.

The functions depend on the settings in the master data and the respective system configuration.
For customer-specific adjustments, contact your contact person at A+W Software GmbH.

The following dialogs are described in this section:
- "Deliv. Plan" on page D-329
- "Delivery Information - Delivery Details" on page D-331
- "Delivery Notes (automatic)" on page D-335
- "Delivery Notes (manual)" on page D-337
- "Delivery Notes Log" on page D-339

## Deliv. Plan

**Sales > Order Entry > Item level > <F4> > Delivery Plan**

On this dialog, you enter the delivery plan. You can specify several partial deliveries for an order. If you create a delivery note, the data is drawn from the delivery plan and evaluated. You can only create a delivery note for an order when the entry of the items is complete.

### Overview

- **Itm:** Number of the item from the order.
  *Technical info: display field, DB field: lieferplan.posnr*
- **Shipm.:** Number of the (partial) delivery.
  *Technical info: mandatory field, numeric field, DB field: liefplan.subnr*
- **Deliv. Date:** Estimated date for the (partial) delivery.
  *Technical info: date field, DB field: liefplan.Itplan*
- **ArrivalDay:** Estimated arrival date for the (partial) delivery.
  *Technical info: display field, DB field: liefplan.ankunft*
- **Article:** Name/description of the article.
  *Technical info: display field, DB field: liefplan.artbez1*
- **Route:** Number of the route for the (partial) delivery.
  *Technical info: mandatory field, numeric field, DB field: liefplan.route*
- **Total:** Total number of pieces of the ordered item from the order.
  *Technical item: numeric field, DB field: liefplan.geslief*
- **Deliv.:** Already delivered item of the order.
  *Technical item: numeric field, DB field: liefplan.geliefert*
- **Packed:** Quantity of packed items for the order.
  *Technical info: numeric field, DB field: liefplan.gespack*
- **Scheduled:** Scheduled number of pieces of the item that will be delivered in this (partial) delivery.
  *Technical info: mandatory field, numeric field, DB field: liefplan.zuliefern*

### Details

The Details tab is currently not used.

## Delivery Information – Delivery Details

**Sales > Order Entry > Item level > <F4> > Shipping Information**

On this dialog, the details of the delivery are displayed, e.g. the route and planned delivery date. The differing delivery information is especially important if there is a distinction between production and delivery site.

Some fields in the **Producing** and **Shipping Site** areas can only be pre-populated if you are working with internal site separation and the via site logic is active.

The fields on this dialog are pre-populated by the system. Generally you do not have to edit the fields.

### Producing Site

**Delivery Addr. Code** Code and name of the saved delivery address of the producting site.
*Technical info: alphanumeric fields, DB fields: kauf.lort, kauf.lort*

**Disp. Type** Number and description of the dispatch type. If a number is specified, the description of the dispatch type is displayed in plain text.
*Technical info: numeric field, display field, DB field: kauf.versandartvia*

**Sched. Delivery Date** Date of the planned delivery to the producing site. The date specifies the day on which the delivery will probably leave the producing site.
*Technical info: date field, DB field: kauf.ltplan*

**Route** Number of the route for delivery.
*Technical info: mandatory field, numeric field, DB field: kauf.routenr*

**Travel Time** Probable duration to the delivery site. If a route is specified for which a travel time is stored, the travel time is displayed in plain text. It can affect the delivery date.
*Technical info: display field*

**Route Days** Display of the days of the week on which the route is driven. If a route is specified, the associated days of the week are drawn from the master data and displayed in plain text.
*Technical info: display field*

**Area** Display of the dispatch region. Several delivery routes can be combined into a dispatch region if the system is configured appropriately. The dispatch region is drawn from the master data for the appropriate via route. The field is pre-populated if the regional routes module is configured and a dispatch region is assigned to the current route. In addition, you have to work with internal site separation and the via site logic must be active.
*Technical info: display field, DB field: route.region*

**Via Site** Number of the delivering site via which the delivery will be sent. You specify the via site in the header in the Route field with `<F5>`.
*Technical info: display field, DB field: kauf.vsvia*

**Site** Display of the site number (company number) in which the order is created.
*Technical info: display field, DB field: kauf.hausnr*

**Tonnage** Display of the load capacity of the vehicle in kilograms. This field can be configured at will.
*Technical info: display field*

**Calendar** Indication whether the calendar will be used for the delivery date determination. You can specify in the route master data for each route whether the calendar will be evaluated.
- The calendar will be used for the delivery date determination.
- The calendar will not be used for the delivery date determination.
*Technical info: checkbox*

### Delivery Site

This area is only displayed if you are working with internal site separation and the via site logic is active.

**Delivery Addr. Code, Delivery Addr. Name** Code and name of the delivery address of the delivery site.
*Technical info: alphanumeric fields, DB fields: kauf.lort, kauf.lort*

**Disp. Type** Number of the dispatch type, e.g. truck. If a number is selected, the description of the dispatch type is displayed in plain text.
*Technical info: display field, DB field: kauf.versandartvia*

**Arrival at Via Site** Date on which the delivery will probably reach the via site.
*Technical info: display field*

**Handling Time** Handling time for loading or unloading in the delivery site.
*Technical info: numeric field*

**Route** Number of the route via which delivery is made to the customer. The route has to be created in the master data as via route for the delivery site:
⇨ Stammdaten, "Routen" auf Seite J-193
*Technical info: mandatory field, numeric field, DB field: kauf.routenr*

**Travel Time** Display of the duration to the delivery site. If a route is specified for which a travel time is stored, the travel time is displayed in plain text.
*Technical info: display field*

**Route Days** Display of the days of the week on which the route is driven. If a route is specified, the associated days of the week are drawn from the master data and displayed in plain text.
*Technical info: display field*

**Area** Indication of the country code with naming of the dispatch region.
*Technical info: display field*

**Tonnage** Display of the load capacity of the vehicle in kilograms. This field can be configured at will.
*Technical info: display field*

**Requested Del. Date** Planned delivery date from the delivery site to the customer.
*Technical info: display field, DB field: kauf.ltplan*

### Customer

**Requested Del. Date** Date of delivery requested by the customer.
*Technical info: Date field, DB field: kauf.ltideal*

**Arrival Date** Date on which the delivery will probably reach the customer. The arrival date is calculated using the delivery date, the travel time, and the route days.
*Technical info: display field*

**Date Status** Status indicator whether the customer's requested date and the calculated arrival date of the delivery match.
*Technical info: display field*

| Symbol | Status indicator | Meaning |
| :--- | :--- | :--- |
| 🟢 | green | The probable delivery date corresponds precisely to the customer's requested date. |
| 🟡 | yellow | The probable delivery date is before the customer's requested date. |
| 🔴 | red | The probable delivery date is after the customer's requested date. |

### Calendar Section

The calendar section displays a section of three weeks around the customer's requested date. All dates, e.g. planned delivery date, customer's requested date, delivery date in the producing site, etc. that are in this period are displayed on the corresponding days. You can display information about the date in question as a tool tip.

## Delivery Notes (automatic)

**Sales > Delivery Notes > Automatic Release**

On this dialog, you generate delivery notes as accompanying documents for order delivery. On this dialog you can also generate invoices and complete documents.

If the Shipping Control module is configured in your system, you should only create delivery notes in the Shipping Control module. By default, the system is not configured to create delivery notes in the Sales module.

> **Inconsistencies with Shipping Control**
> Creating delivery notes in Sales can cause inconsistencies with Shipping Control since the status bookings, e.g. quantities packed or reported complete are only up-to-date in the Shipping Control. For customer-specific adjustment, please contact your partner at A+W Software GmbH.

- **Release:** Specification of the release type for the selected document.
  - **Delivery note:** A delivery note will be generated for the selected document.
  - **Invoice:** An invoice will be generated for the selected document. You can only generate an invoice for documents for which a delivery note exists.
  - **DN + Invoice:** A delivery note and invoice will be generated for the selected document.
  - **Complete document:** The selected document is completed. Changes to the document will no longer be forwarded to the system.
- **Site:** Site number.
- **Document:** Document number. For delivery note generation, you specify the number of the order, for invoice generation the number of the delivery note. The order and delivery note number are identical. For the delivery note, you can also specify the subnumber for partial deliveries.
- **SubNo:** Subnumber of the document, e.g. of the partial delivery note. The subnumber must be specified to generate a delivery note.
- **Grp:** Dispatch group. Delivery notes can be assigned to a dispatch group in the dispatch planning. The dispatch groups are stored in the system master data. The dispatch group serves as additional identifier for the route locking.
- **Deliv. Note:** Information as to whether a delivery note or partial delivery note exists. If there is already a delivery note, then this field will show **exists**.
- **Invoice:** Invoice number.
- **Cust. No.:** Customer number.
- **Cust.:** Customer name.
- **Date:** Date of the document entry.
- **Val.Date:** Period until the value date in days.
- **Cr.:** Create. Indication of whether the delivery notes and/or invoices should be generated.
  - ☑ Yes, generate.
  - ☐ Do not generate.

### Footer

Customer name and the total net amount are shown.
Use `<F2>` to display the following fields:
- **Amount:** Total net amount.
- **Emp.:** Employee number of the person who entered the document.
- **Entered by:** Name of the person who entered the document.
- **Document date:** Corresponds to the Date field.

## Delivery Notes (manual)

**Sales > Delivery Notes > Manual Delivery Notes**

Use this dialog to manually generate and edit delivery notes. You only generate delivery notes manually if you have to correct the order data, e.g. in case of a different delivery quantity.

If the Shipping Control module is configured in your system, you should only create delivery notes in the Shipping Control module. By default, the system is not configured to create delivery notes in the Sales module.

> **Inconsistencies with Shipping Control**
> Creating delivery notes in Sales can cause inconsistencies with Shipping Control since the status bookings, e.g. quantities packed or reported complete are only up-to-date in the Shipping Control. For customer-specific adjustment, please contact your partner at A+W Software GmbH.

The fields and tabs are described for the **Order Entry** dialog:
⇨ "Order Entry" on page D-84

In addition, the following fields are displayed.

### Header

**Order** Number of the order and subnumber. You assign subnumbers for partial delivery notes. Use `<TAB>` to assign the next free subnumber automatically. If delivery notes are already entered for an order, you can enter the subnumber and call up the already created delivery note.

### General tab

**Received** Item quantity that has already been delivered with the previous delivery note.

**Deliv.** Quantity of the article that are being delivered with the selected delivery note.

## Delivery Notes Log

**Sales > Delivery Notes > Log**

This dialog displays the delivery notes log. All documents for the delivery notes are noted with the specification of the date and the time.

If you are working with internal site separation, first a dialog opens where you can specify the site number. The log displays only the documents for the selected site.

> **Delivery note log for the current day**
> A delivery note log is generated for the current day. If the error message is displayed that the file is empty or cannot be read, then no delivery note has been generated on this day.

# Invoices

To account for customer orders, invoices are generated an sent to the financial accounting (FinAc).

You can create the invoices automatically or manually. An invoice can only be created if a delivery note exists.

The following dialogs are described in this section:
- "Invoices (automatic)" on page D-341
- "Item Info" on page D-344
- "Invoices (manual)" on page D-346
- "Cash Transaction" on page D-347
- "Booking of Invoices" on page D-348
- "Partial Invoice (automatic)" on page D-350
- "Partial Invoice (manual)" on page D-352
- "Final Invoices (automatic)" on page D-353
- "Final Invoices (manual)" on page D-354
- "Invoice Log" on page D-355

## Invoices (automatic)

**Sales > Invoices -> Automatic Release**

Use this dialog to create invoices for documents and send them to Financial Accounting. You can import the documents for which invoices can be generated or you can specify the document numbers manually.

Use `<Ctrl>+<F8>` to import the data for all documents for which an invoice can be generated. The data is imported via a freely configurable SQL query. The amount of data to be imported depends on the SQL query in question. You can use the query that is configured by A+W by default or specify a customer-specific SQL query for the data import.

For customer-specific adjustments, contact your contact person at A+W Software GmbH.

The footer displays the customer name and total amount from the order for which an invoice is being created.

If you have not yet booked an invoice. you can view additional information on the Invoices dialog and edit the invoice, e.g. to correct it.
⇨"Invoices (manual)" on page D-346

On this dialog, you can also generate the delivery note together with the invoice or complete the document.

Use `<F3>` to have the system generate the invoices for the selected orders.

### Information on Document tab

- **Release:** Specification of which documents you are releasing for the document that is specified in the Document field.
  - **Invoice:** An invoice will be generated for the document.
  - **DN + Invoice:** A delivery note and invoice will be generated for the document.
  - **Complete document:** The selected document will be completed, that is, it can no longer be edited.
  - **Delivery note:** A delivery note will be generated for the document.
  *Technical info: toggle field, DB field: kauf.vorgang*
- **Site:** Display of the site number.
  *Technical info: display field, DB field: kauf.hausnr*
- **Document:** Document number.
  *Technical info: mandatory field, numeric field, DB field: kauf.auftrnr*
- **SubNo:** Number of the partial delivery note. If the document is generated for a complete delivery, a 1 is displayed.
  *Technical info: numeric field, DB field: kauf.subnr*
- **Grp:** Dispatch group. Delivery notes can be assigned to a dispatch group in the dispatch planning. The dispatch groups are stored in the system master data. The dispatch group serves as additional identifier for the route locking.
  *Technical info: numeric field, DB field: lapool.vsgruppe*
- **Deliv. note:** Indication as to whether a delivery note or partial delivery note exists. If there is already a delivery note, then this field will show the entry **exists**.
  *Technical info: display field*
- **Invoice:** Number of the invoice if an invoice exists.
  *Technical info: display field*
- **Cust. No.:** Customer number.
  *Technical info: display field, DB field: kauf.kunr*
- **Cust.:** Display of the customer name.
  *Technical info: display field, DB field: mp.name*
- **Document date:** Date of the invoice creation or invoice booking. By default, the field is pre-populated with the current date. For invoices and delivery notes, you can change between document and booking date with `<Ctrl>+<B>`. Via the column header, it is indicated which date is currently displayed.
  *Technical info: mandatory field, date field, DB field: kauf.edat*
- **Val. Date:** Period until the value date in days up to a maximum of 99 days.
  *Technical info: display field, DB field: kauf.valuta*
- **Cr.:** Create. Indication of whether the selected documents should be generated.
  - ☑ Yes, generate.
  - ☐ Do not generate.
  *Technical info: checkbox*

Use `<F2>` to change to the **Information on Document** tab.

### Information on Document tab

The columns are described for the **Documents** tab:
⇨ "Information on Document tab" on page D-342

In addition, the following columns are displayed:
- **Amount:** Indication of the invoice amount.
  *Technical info: display field, DB field: kauf.nettototal*
- **rec., Operator:** Display of the operator number and name.
  *Technical info: display fields, DB fields: kauf.eust, mitarb.maname*

### Footer

The footer displays the customer name and invoice amount from the document.
Use `<F5>` to open the **Items** dialog on which additional details about the invoice items are displayed.
⇨ "Item Info” on page D-344

## Item Info

- **Sales > Invoices -> Automatic Release > Enter values > <F5>**
- **Sales > Invoices > Partial Invoice, Final Invoice > Automatic Release > Enter values > <F5>**
- **Sales > Credit Notes > Book Credit Notes > Enter values > <F5>**

This dialog displays the details of the individual items from the automatic invoice or credit creation.

### Item info I tab

- **Docum.:** Document number.
  *Technical info: numeric field, DB field: kauf.auftrnr*
- **Itm:** Number of the item in the document.
  *Technical info: numeric field, DB field: kpos.Ifdpos*
- **Article, Designation:** Number and description of the article.
  *Technical info: numeric field, alphanumeric field, DB fields: kpos.artnr, kpos.artbez1*
- **/:** Indication of whether the item has been invoiced.
  *Technical info: display field, DB field: kauf.fakturakz*
- **Qty:** Units of the item.
  *Technical info: numerical field, DB field: kpos.menge*
- **Width:** Width of the lite entered in the item in millimeters.
  *Technical info: numerical field, database field: kpos.laenge*
- **Height:** Height of the lite entered in the item in millimeters.
  *Technical info: numerical field, database field: kpos.breite*
- **Price/pc.:** Price per piece of the item.
  *Technical info: numeric field, DB field: kpos.nstpreis*
- **Item price:** Price of the complete item.
  *Technical info: numeric field, DB field: kpos.npospreis*

Use `<F2>` to change to the **Item Info II** tab.

### Item Info II tab

The columns are described for the **Item Info I** tab:
⇨ "Item info I tab" on page D-344

In addition, the following columns are displayed:
- **Shp:** Shape number for the item article.
  *Technical info: numeric field, DB field: kpos.modnr*
- **Deliv.:** Number of units that have already been delivered.
  *Technical info: numeric field, DB field: kpos.geslief*
- **(Field without description):** Indication of whether the item is invoiced.
  *Technical info: display field, DB field: kauf.fakturakz*
- **Invoiced:** Number of units that were already invoiced.
  *Technical info: numeric field, DB field: kpos.gesberech*
- **AIR1, AIR2:** Width of the airspace in millimeters. For multiple-lite insulated glass, the first airspace is displayed in AIR1 and the second in AIR2.
  *Technical info: numeric fields, DB fields: kpos.szr, kpos.szr2*

## Invoices (manual)

**Sales > Invoices > Manual Invoice**

On this dialog, you can edit or create invoices. Then you can transfer the invoices to the FinAc if the system is configured appropriately.

If you would like to create a manual partial or final invoice, you can select it directly using the appropriate menu element. In order to create a partial invoice manually, for example, select **Manual Invoice** in the menu path for partial invoices.

The fields are described for the **Order Entry** dialog:
⇨ "Order Entry" on page D-84

In addition, the following fields are displayed:

### Header

**Invoice No.** Invoice number. If you create an invoice, the system creates a temporary number for the invoice. After completion of invoicing, the system assigns a final invoice number. This way, the invoices are numbered sequentially. If you specify an existing invoice number, the corresponding invoice is opened.
The invoices are saved in the database table `kauf` under `vorgang` with the value `7` with their final invoice number.
*Technical info: numeric field, DB field: kauf.auftrnr*

> **Entering invoices with reference**
> Generally invoices are always entered with reference to a document, e.g. a delivery note or an order. You can enter the document number for which you want to issue the invoice in the **Ref.** field in the header area.

### General tab

**Itm** Item quantity that should be calculated. For a manual invoice, the field is pre-populated with the value Quantity from the document by default. You can reduce the value.
*Technical info: numeric field, DB field: kpos.berechnet*

### Footer

If an invoice has already been created for the reference document, then the invoice amount from all invoices already created is displayed in the **Net Total** field.

## Cash Transaction

**Sales > Invoices > Cash Transaction**

On this dialog, you handle cash transactions for customers who pick their goods up themselves and pay directly. For a cash transaction, you enter the order data the the invoice and delivery note are then created right away.
The fields are described for the **Order Entry** dialog:
⇨ "Order Entry" on page D-84

## Booking of Invoices

**Sales > Invoices -> Booking of Invoices**

Use this dialog to book invoices that have not yet been transferred to the FinAc. Generally invoices are booked automatically after generation.

In exceptional cases, the invoice can also be booked after the fact. In the invoice entry, depending on the configuration, when generating the invoice a query can be displayed asking whether the invoice should be booked. If you respond [No] to the query, you can import this unbooked invoice on the **Booking of Invoices** dialog and book it after the fact.

Use `<Ctrl>+<F8>` to import the data for all invoices that are generated in the specified period.

The footer displays the customer name and total amount from the order for which the invoice is booked.

Use `<F3>` to book the selected invoices.

### Sales Invoice tab

- **Invoice:** Invoice number. If you specify a number, the appropriate values are entered in the other columns.
  *Technical info: mandatory field, numeric field*
- **SubNo:** Display of the subnumber for partial invoices.
  *Technical info: display field, DB field: kauf.subnr*
- **External No.:** Display of the document number that is specified by the customer. For orders from another site, the order number of the sending site is in this field.
  *Technical info: display field, DB field: kauf.exaufnr*
- **Order:** Display of the order number.
  *Technical info: display field, DB field: kauf.auftrnr*
- **Doc. Date:** Display of the date of the invoice creation.
  *Technical info: display field, DB field: kauf.edat*
- **Book. Date:** Display of the invoice booking date. By default, the current date is entered. If you want to specify another booking date, you have to enter the new date in the field, confirm the entry, and enter the new data again. The date is only taken over into the field after the second entry.
  *Technical info: date field, DB field: kauf.bdat*
- **Bk.:** Specification whether the invoice should be booked.
  - ☑ The invoice will be booked.
  - ☐ The invoice will not be booked.
  *Technical info: checkbox*

### Information on Document tab

The **Information on Document** tab only appears on the **Invoices (automatic)** and **Delivery Notes (automatic)** dialogs:
⇨ "Invoices (automatic)" on page D-341
⇨ "Delivery Notes (automatic)" on page D-335

## Partial Invoice (automatic)

**Sales > Invoices > Partial Invoice > Automatic Release**

Use this dialog to create the partial invoices for orders using a corresponding payment plan. If there are orders for the current day for which there is a payment plan, then you can import these orders with `<Ctrl>+<F8>`. You can also enter the order numbers manually or search for orders with `<F9>`.

The footer displays the customer name and total amount from the order for which a partial invoice is being created.

Use `<F3>` to have the system generate the partial invoices for the selected orders.
- **Order:** Order number.
  *Technical info: mandatory field, numeric field, DB field: kauf.auftrnr*
- **Site:** Display of the site number.
  *Technical info: display field, DB field: kauf.hausnr*
- **Amount:** Partial amount from the payment plan.
  *Technical info: numeric field, DB field: zahlplan.betrag*
- **Deliv. Note:** Indicates if there is already a delivery note or partial invoice. If there is a delivery note, the entry **exists** is in this field.
  *Technical info: display field*
